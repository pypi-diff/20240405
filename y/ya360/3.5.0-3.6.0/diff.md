# Comparing `tmp/ya360-3.5.0.tar.gz` & `tmp/ya360-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ya360-3.5.0.tar", last modified: Thu Apr  4 07:10:36 2024, max compression
+gzip compressed data, was "ya360-3.6.0.tar", last modified: Fri Apr  5 07:28:42 2024, max compression
```

## Comparing `ya360-3.5.0.tar` & `ya360-3.6.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.706895 ya360-3.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.698895 ya360-3.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.698895 ya360-3.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-04 07:10:31.000000 ya360-3.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 07:10:31.000000 ya360-3.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-04 07:10:31.000000 ya360-3.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.698895 ya360-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-04 07:10:31.000000 ya360-3.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-04 07:10:31.000000 ya360-3.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-04 07:10:31.000000 ya360-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-04 07:10:31.000000 ya360-3.5.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.698895 ya360-3.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 07:10:31.000000 ya360-3.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-04 07:10:31.000000 ya360-3.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 07:10:31.000000 ya360-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 07:10:31.000000 ya360-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-04 07:10:36.706895 ya360-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-04 07:10:31.000000 ya360-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-04 07:10:31.000000 ya360-3.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-04 07:10:31.000000 ya360-3.5.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.702895 ya360-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.702895 ya360-3.5.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.702895 ya360-3.5.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    38353 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/_static/fig1.png
--rw-r--r--   0 runner    (1001) docker     (127)   127538 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/_static/fig2.png
--rw-r--r--   0 runner    (1001) docker     (127)    36447 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/_static/fig3.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/_static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/befo.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/cmd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/lic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/routing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-04 07:10:31.000000 ya360-3.5.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-04 07:10:31.000000 ya360-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:10:36.706895 ya360-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 07:10:31.000000 ya360-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.706895 ya360-3.5.0/ya360/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 07:10:36.000000 ya360-3.5.0/ya360/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/antispam.py
--rw-r--r--   0 runner    (1001) docker     (127)    28749 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/departments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/tid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-04 07:10:31.000000 ya360-3.5.0/ya360/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:10:36.706895 ya360-3.5.0/ya360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-04 07:10:36.000000 ya360-3.5.0/ya360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-04 07:10:36.000000 ya360-3.5.0/ya360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:10:36.000000 ya360-3.5.0/ya360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 07:10:36.000000 ya360-3.5.0/ya360.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:10:36.000000 ya360-3.5.0/ya360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 07:10:36.000000 ya360-3.5.0/ya360.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.860254 ya360-3.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-05 07:28:37.000000 ya360-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-05 07:28:37.000000 ya360-3.6.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 07:28:37.000000 ya360-3.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-05 07:28:37.000000 ya360-3.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 07:28:37.000000 ya360-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 07:28:37.000000 ya360-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-05 07:28:42.860254 ya360-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-05 07:28:37.000000 ya360-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-05 07:28:37.000000 ya360-3.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-05 07:28:37.000000 ya360-3.6.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.856254 ya360-3.6.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.856254 ya360-3.6.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    38353 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/_static/fig1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127538 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/_static/fig2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36447 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/_static/fig3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/_static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/befo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/cmd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/lic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-05 07:28:37.000000 ya360-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:28:42.860254 ya360-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 07:28:37.000000 ya360-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.856254 ya360-3.6.0/ya360/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/antispam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31096 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/departments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/tid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.860254 ya360-3.6.0/ya360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/top_level.txt
```

### Comparing `ya360-3.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ya360-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `ya360-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/.github/workflows/codeql-analysis.yml` & `ya360-3.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/.github/workflows/python-publish.yml` & `ya360-3.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/.gitignore` & `ya360-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/.readthedocs.yaml` & `ya360-3.6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/CODE_OF_CONDUCT.md` & `ya360-3.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/LICENSE` & `ya360-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/PKG-INFO` & `ya360-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya360
-Version: 3.5.0
+Version: 3.6.0
 Summary: Утилита командной строки для Yandex 360
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Homepage, https://ya360.uh.net.ru
 Project-URL: Bug Tracker, https://github.com/imercury13/ya360/issues
 Project-URL: Documentation, https://ya360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/ya360
```

### Comparing `ya360-3.5.0/README.md` & `ya360-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/README.rst` & `ya360-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/Makefile` & `ya360-3.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/make.bat` & `ya360-3.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/_static/fig1.png` & `ya360-3.6.0/docs/source/_static/fig1.png`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/_static/fig2.png` & `ya360-3.6.0/docs/source/_static/fig2.png`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/_static/fig3.png` & `ya360-3.6.0/docs/source/_static/fig3.png`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/befo.rst` & `ya360-3.6.0/docs/source/befo.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/cmd.rst` & `ya360-3.6.0/docs/source/cmd.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/conf.py` & `ya360-3.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/index.rst` & `ya360-3.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/lic.rst` & `ya360-3.6.0/docs/source/lic.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/docs/source/usage.rst` & `ya360-3.6.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/pyproject.toml` & `ya360-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/antispam.py` & `ya360-3.6.0/ya360/antispam.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/cmd.py` & `ya360-3.6.0/ya360/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from .departments import create_department, update_department, add_alias_department, delete_alias_department, delete_department, show_department, show_departments
 from .users import show_users, show_user, update_user, create_user, add_alias_user, delete_alias_user, delete_user, upload_avatar_user
 from .groups import create_group, delete_group, update_group, add_member_group, delete_member_group, show_group, show_groups
 from .mail import (edit_access_mailbox, delete_access_mailbox, show_status_access_mailbox,
     show_access_mailbox_user, show_users_access_mailbox,show_main_address,
     show_signs, edit_main_address, save_sign_to_file,
     edit_sign_param, add_sign, delete_sign,
-    edit_sign_position)
+    edit_sign_position, show_rules_user, add_rule_autoreplies,
+    add_rule_forwards, delete_rule)
 from .whois import whois
 from .logs import show_mail_log, show_disk_log
 from .configure import make_config
 from .antispam import show_whitelist, add_in_whitelist, remove_from_whitelist, delete_whitelist
 from .routing import add_in_routing, show_routing, remove_from_routing
 
 
@@ -227,14 +228,32 @@
     parser_signs_comm.add_argument('--emails', type=str, help='Список адресов для ассоциирования')
     parser_signs_comm.add_argument('--lang', type=str, help='Язык')
     parser_signs_comm.add_argument('--filename', type=str, help='Имя файла с текстом подписи')
     parser_signs_comm = subparser_signs.add_parser('delete', help='Удалить подпись')
     parser_signs_comm.add_argument('nickname', type=str, help='Login пользователя почтового ящика')
     parser_signs_comm.add_argument('num', type=int, help='Номер подписи')
 
+    parser_rules = subparser_sender_mailbox.add_parser('rules', help='Управление правилами автоответа и переадресации')
+    subparser_rules = parser_rules.add_subparsers(dest='sub_com_rules')
+    parser_rules_comm =  subparser_rules.add_parser('show', help='Список правил')
+    parser_rules_comm.add_argument('nickname', type=str, help='Login пользователя почтового ящика')
+    parser_rules_comm =  subparser_rules.add_parser('add-autoreplies', help='Добавить правило автоответа')
+    parser_rules_comm.add_argument('nickname', type=str, help='Login пользователя почтового ящика')
+    parser_rules_comm.add_argument('ruleName', type=str, help='Наименование правила')
+    parser_rules_comm.add_argument('text', type=str, help='Текст автоответа')
+    parser_rules_comm =  subparser_rules.add_parser('add-forwards', help='Добавить правило пересылки')
+    parser_rules_comm.add_argument('nickname', type=str, help='Login пользователя почтового ящика')
+    parser_rules_comm.add_argument('ruleName', type=str, help='Наименование правила')
+    parser_rules_comm.add_argument('address', type=str, help='Адрес получателя')
+    parser_rules_comm.add_argument('copy', type=str, choices=['True','False'], help='Сохранять копию письма')
+    parser_rules_comm =  subparser_rules.add_parser('delete', help='Удалить правило')
+    parser_rules_comm.add_argument('nickname', type=str, help='Login пользователя почтового ящика')
+    parser_rules_comm.add_argument('ruleId', type=int, help='Номер правила')
+
+
 
     parser_logs = subparsers.add_parser('logs', help='Аудит-лог событий в организации')
     subparser_logs = parser_logs.add_subparsers(dest='sub_com_logs')
 
     parser_logs_comm = subparser_logs.add_parser('mail',help='Аудит-лог почты')
     parser_logs_comm.add_argument('--beforeDate', type=str, help='Верхняя граница периода выборки в формате ISO 8601')
     parser_logs_comm.add_argument('--afterDate', type=str, help='Нижняя граница периода выборки в формате ISO 8601')
@@ -372,14 +391,24 @@
                     edit_sign_param(args)
                 if args.sub_com_signs == 'add':
                     add_sign(args)
                 if args.sub_com_signs == 'delete':
                     delete_sign(args)
             if args.sub_com_sender_mailbox == 'sign-position':
                 edit_sign_position(args)
+            if args.sub_com_sender_mailbox == 'rules':
+                if args.sub_com_rules == 'show':
+                    show_rules_user(args)
+                if args.sub_com_rules == 'add-autoreplies':
+                    add_rule_autoreplies(args)
+                if args.sub_com_rules == 'add-forwards':
+                    add_rule_forwards(args)
+                if args.sub_com_rules == 'delete':
+                    delete_rule(args)
+                
 
     if args.sub_com == 'logs':
         if args.sub_com_logs == 'mail':
             show_mail_log(args)
         if args.sub_com_logs == 'disk':
             show_disk_log(args)
```

### Comparing `ya360-3.5.0/ya360/configure.py` & `ya360-3.6.0/ya360/configure.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/departments.py` & `ya360-3.6.0/ya360/departments.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/groups.py` & `ya360-3.6.0/ya360/groups.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/logs.py` & `ya360-3.6.0/ya360/logs.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/mail.py` & `ya360-3.6.0/ya360/mail.py`

 * *Files 12% similar despite different names*

```diff
@@ -321,7 +321,95 @@
     body = check_request(mail.show_sender_info(__token__, __orgid__, uid))
 
     body['signPosition'] = args.position
 
     res = check_request(mail.edit_sender_info(__token__,__orgid__,uid,body))
 
     return None
+
+def show_rules_user(args):
+    """Функция просмотра правила автоответа и пересылки писем
+	
+	:param args: словарь аргументов командной строки
+	:type args: dict
+	"""
+
+    __token__ = load_token()
+    __orgid__ = load_orgid()
+
+    uid = check_request(tools.get_id_user_by_nickname(args.nickname, __token__, __orgid__))['id']
+
+    body = check_request(mail.show_user_rules(__token__, __orgid__, uid))
+
+    print('Автоответы:')
+    print(f'{"ID":<10} {"Название":<25} {"Текст"}')
+    for rule in body['autoreplies']:
+        print(f'{rule["ruleId"]:>10} {rule["ruleName"]:<25} {rule["text"]}')
+    print('Переадресации:')
+    print(f'{"ID":<10} {"Название":<25} {"Адрес":<25} {"Копия"}')
+    for rule in body['forwards']:
+        print(f'{rule["ruleId"]:>10} {rule["ruleName"]:<25} {rule["address"]:<25} {rule["withStore"]}')
+    
+    return None
+
+def add_rule_autoreplies(args):
+    """Функция добавления правила автоответа
+	
+	:param args: словарь аргументов командной строки
+	:type args: dict
+	"""
+
+    __token__ = load_token()
+    __orgid__ = load_orgid()
+
+    uid = check_request(tools.get_id_user_by_nickname(args.nickname, __token__, __orgid__))['id']
+
+    body = {
+        "autoreply":{
+            "ruleName":args.ruleName,
+            "text":args.text
+        }
+    }
+
+    body = check_request(mail.edit_user_rules(__token__, __orgid__, uid, body))
+
+    return None
+
+def add_rule_forwards(args):
+    """Функция добавления правила пересылки
+	
+	:param args: словарь аргументов командной строки
+	:type args: dict
+	"""
+
+    __token__ = load_token()
+    __orgid__ = load_orgid()
+
+    uid = check_request(tools.get_id_user_by_nickname(args.nickname, __token__, __orgid__))['id']
+
+    body = {
+        "forward":{
+            "ruleName":args.ruleName,
+            "address":args.address,
+            "withStore":args.copy
+        }
+    }
+
+    res = check_request(mail.edit_user_rules(__token__, __orgid__, uid, body))
+
+    return None
+
+def delete_rule(args):
+    """Функция удаления правила
+	
+	:param args: словарь аргументов командной строки
+	:type args: dict
+	"""
+
+    __token__ = load_token()
+    __orgid__ = load_orgid()
+
+    uid = check_request(tools.get_id_user_by_nickname(args.nickname, __token__, __orgid__))['id']
+
+    check_request(mail.delete_user_rules(__token__, __orgid__, uid, args.ruleId))
+
+    return None
```

### Comparing `ya360-3.5.0/ya360/routing.py` & `ya360-3.6.0/ya360/routing.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/tid.py` & `ya360-3.6.0/ya360/tid.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/tools.py` & `ya360-3.6.0/ya360/tools.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/users.py` & `ya360-3.6.0/ya360/users.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360/whois.py` & `ya360-3.6.0/ya360/whois.py`

 * *Files identical despite different names*

### Comparing `ya360-3.5.0/ya360.egg-info/PKG-INFO` & `ya360-3.6.0/ya360.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya360
-Version: 3.5.0
+Version: 3.6.0
 Summary: Утилита командной строки для Yandex 360
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Homepage, https://ya360.uh.net.ru
 Project-URL: Bug Tracker, https://github.com/imercury13/ya360/issues
 Project-URL: Documentation, https://ya360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/ya360
```

### Comparing `ya360-3.5.0/ya360.egg-info/SOURCES.txt` & `ya360-3.6.0/ya360.egg-info/SOURCES.txt`

 * *Files identical despite different names*

