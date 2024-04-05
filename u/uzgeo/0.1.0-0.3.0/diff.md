# Comparing `tmp/uzgeo-0.1.0.tar.gz` & `tmp/uzgeo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uzgeo-0.1.0.tar", last modified: Tue Mar 26 04:29:50 2024, max compression
+gzip compressed data, was "uzgeo-0.3.0.tar", last modified: Fri Apr  5 19:51:05 2024, max compression
```

## Comparing `uzgeo-0.1.0.tar` & `uzgeo-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.767784 uzgeo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.755784 uzgeo-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.759784 uzgeo-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.759784 uzgeo-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-26 04:29:38.000000 uzgeo-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 04:29:38.000000 uzgeo-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-26 04:29:38.000000 uzgeo-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-26 04:29:50.763784 uzgeo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-26 04:29:38.000000 uzgeo-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.759784 uzgeo-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.763784 uzgeo-0.1.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/cats.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/dogs.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/guest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/guest_book.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/introfunction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/ipyleaflet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    43796 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/lab5.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/learning_python.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/mean.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/examples/programming_reasons.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.763784 uzgeo-0.1.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 04:29:38.000000 uzgeo-0.1.0/docs/uzgeo.md
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-26 04:29:38.000000 uzgeo-0.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-26 04:29:38.000000 uzgeo-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 04:29:38.000000 uzgeo-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-26 04:29:38.000000 uzgeo-0.1.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 04:29:50.767784 uzgeo-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.763784 uzgeo-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-26 04:29:38.000000 uzgeo-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-26 04:29:38.000000 uzgeo-0.1.0/tests/test_uzgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.763784 uzgeo-0.1.0/uzgeo/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-26 04:29:38.000000 uzgeo-0.1.0/uzgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 04:29:38.000000 uzgeo-0.1.0/uzgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-26 04:29:38.000000 uzgeo-0.1.0/uzgeo/uzgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 04:29:50.763784 uzgeo-0.1.0/uzgeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-26 04:29:50.000000 uzgeo-0.1.0/uzgeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-26 04:29:50.000000 uzgeo-0.1.0/uzgeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 04:29:50.000000 uzgeo-0.1.0/uzgeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 04:29:50.000000 uzgeo-0.1.0/uzgeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 04:29:50.000000 uzgeo-0.1.0/uzgeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 04:29:50.000000 uzgeo-0.1.0/uzgeo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.774156 uzgeo-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.762156 uzgeo-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.766156 uzgeo-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.766156 uzgeo-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-05 19:50:54.000000 uzgeo-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:50:54.000000 uzgeo-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 19:50:54.000000 uzgeo-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-05 19:51:05.774156 uzgeo-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 19:50:54.000000 uzgeo-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.766156 uzgeo-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.770156 uzgeo-0.3.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/cats.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/dogs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/guest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/guest_book.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/introfunction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    43796 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/learning_python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/mean.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/examples/programming_reasons.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.770156 uzgeo-0.3.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 19:50:54.000000 uzgeo-0.3.0/docs/uzgeo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-05 19:50:54.000000 uzgeo-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-05 19:50:54.000000 uzgeo-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 19:50:54.000000 uzgeo-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-05 19:50:54.000000 uzgeo-0.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:51:05.774156 uzgeo-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.770156 uzgeo-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 19:50:54.000000 uzgeo-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-05 19:50:54.000000 uzgeo-0.3.0/tests/test_uzgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.770156 uzgeo-0.3.0/uzgeo/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 19:50:54.000000 uzgeo-0.3.0/uzgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-05 19:50:54.000000 uzgeo-0.3.0/uzgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-05 19:50:54.000000 uzgeo-0.3.0/uzgeo/uzgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:05.774156 uzgeo-0.3.0/uzgeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-05 19:51:05.000000 uzgeo-0.3.0/uzgeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-05 19:51:05.000000 uzgeo-0.3.0/uzgeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:51:05.000000 uzgeo-0.3.0/uzgeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 19:51:05.000000 uzgeo-0.3.0/uzgeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 19:51:05.000000 uzgeo-0.3.0/uzgeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 19:51:05.000000 uzgeo-0.3.0/uzgeo.egg-info/top_level.txt
```

### Comparing `uzgeo-0.1.0/.github/workflows/docs-build.yml` & `uzgeo-0.3.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/.github/workflows/docs.yml` & `uzgeo-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/.github/workflows/installation.yml` & `uzgeo-0.3.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/.github/workflows/macos.yml` & `uzgeo-0.3.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/.github/workflows/pypi.yml` & `uzgeo-0.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/.github/workflows/ubuntu.yml` & `uzgeo-0.3.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/.github/workflows/windows.yml` & `uzgeo-0.3.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/.gitignore` & `uzgeo-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/PKG-INFO` & `uzgeo-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uzgeo
-Version: 0.1.0
+Version: 0.3.0
 Summary: A python package for geospatial analysis
 Author-email: Yuze Li <yli190@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/Younguz/uzgeo
 Keywords: uzgeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uzgeo-0.1.0/docs/contributing.md` & `uzgeo-0.3.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/docs/examples/introfunction.ipynb` & `uzgeo-0.3.0/docs/examples/ipyleaflet.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.90171875%*

 * *Differences: {"'cells'": "{0: {'source': ['import uzgeo\\n']}, 1: {'outputs': {0: {'output_type': "*

 * *            "'display_data', 'data': OrderedDict([('application/vnd.jupyter.widget-view+json', "*

 * *            "OrderedDict([('model_id', 'e8b480c90c33424f953416df814c31c5'), ('version_major', 2), "*

 * *            '(\'version_minor\', 0)])), (\'text/plain\', ["Map(center=[20, 0], '*

 * *            "controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', "*

 * *            '\'zoom_out_text…"])]), \'metadata\': Ordere […]*

```diff
@@ -1,87 +1,41 @@
 {
     "cells": [
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Younguz/uzgeo/blob/main/docs/examples/introfunction.ipynb)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Introduction\n",
-                "\n",
-                "When you want to use a package, use import to load it."
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import uzgeo"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Print function\n",
-                "\n",
-                "When you need to use the print function, use it in this way."
+                "import uzgeo\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "what you want to print\n"
-                    ]
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "e8b480c90c33424f953416df814c31c5",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Map(center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text\u2026"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "print(\"what you want to print\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "When you are trying to find the mean of a number sequence, check the example/Mean. You can know that how to use the function."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "\n",
-                "\n",
-                "\n",
-                "\n",
-                "\n",
-                "\n",
-                "This package can help you quickly create previewable maps and focus on anywhere in the world. Check the usage of map class in the example."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Conclusion\n",
-                "\n",
-                "This package can help you quickly import some practical functions and solve some troublesome mathematical and geographical problems."
+                "m=uzgeo.Map()\n",
+                "m"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "UZVB",
             "language": "python",
```

### Comparing `uzgeo-0.1.0/docs/examples/ipyleaflet.ipynb` & `uzgeo-0.3.0/docs/examples/mean.ipynb`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.963125%*

 * *Differences: {"'cells'": "{0: {'execution_count': 2, 'outputs': [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['Mean of the numbers: 4.8\\n'])])], 'source': "*

 * *            "['numbers = [1, 5, 5, 6, 7]\\n', '\\n', 'mean = sum(numbers) / len(numbers)\\n', "*

 * *            '\'\\n\', \'print("Mean of the numbers:", mean)\']}, 1: {\'execution_count\': 3, '*

 * *            "'outputs': {0: {'output_type': 'stream', 'name': 'stdout', 'text': ['Mean: 4.8\\n'], "*

 * *            "delete: ['data', 'metad […]*

```diff
@@ -1,41 +1,49 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Mean of the numbers: 4.8\n"
+                    ]
+                }
+            ],
             "source": [
-                "import uzgeo\n"
+                "numbers = [1, 5, 5, 6, 7]\n",
+                "\n",
+                "mean = sum(numbers) / len(numbers)\n",
+                "\n",
+                "print(\"Mean of the numbers:\", mean)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "e8b480c90c33424f953416df814c31c5",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "Map(center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text\u2026"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Mean: 4.8\n"
+                    ]
                 }
             ],
             "source": [
-                "m=uzgeo.Map()\n",
-                "m"
+                "from uzgeo.common import calculate_average\n",
+                "\n",
+                "mean_value = calculate_average(numbers)\n",
+                "\n",
+                "print(\"Mean:\", mean_value)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "UZVB",
             "language": "python",
```

### Comparing `uzgeo-0.1.0/docs/examples/lab4.ipynb` & `uzgeo-0.3.0/docs/examples/lab4.ipynb`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/docs/examples/lab5.ipynb` & `uzgeo-0.3.0/docs/examples/lab5.ipynb`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/docs/installation.md` & `uzgeo-0.3.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/mkdocs.yml` & `uzgeo-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/pyproject.toml` & `uzgeo-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "uzgeo"
-version = "0.1.0"
+version = "0.3.0"
 dynamic = [
     "dependencies",
 ]
 description = "A python package for geospatial analysis"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.1.0"
+current_version = "0.3.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `uzgeo-0.1.0/uzgeo/common.py` & `uzgeo-0.3.0/uzgeo/common.py`

 * *Files identical despite different names*

### Comparing `uzgeo-0.1.0/uzgeo.egg-info/PKG-INFO` & `uzgeo-0.3.0/uzgeo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uzgeo
-Version: 0.1.0
+Version: 0.3.0
 Summary: A python package for geospatial analysis
 Author-email: Yuze Li <yli190@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/Younguz/uzgeo
 Keywords: uzgeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uzgeo-0.1.0/uzgeo.egg-info/SOURCES.txt` & `uzgeo-0.3.0/uzgeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

