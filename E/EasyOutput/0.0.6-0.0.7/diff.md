# Comparing `tmp/EasyOutput-0.0.6.tar.gz` & `tmp/easyoutput-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyOutput-0.0.6.tar", last modified: Tue Apr  2 03:16:16 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `EasyOutput-0.0.6.tar` & `easyoutput-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 03:16:16.873241 EasyOutput-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-02 03:16:16.871240 EasyOutput-0.0.6/EasyOutput.egg-info/
--rw-rw-rw-   0        0        0     2468 2024-04-02 03:16:16.000000 EasyOutput-0.0.6/EasyOutput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-02 03:16:16.000000 EasyOutput-0.0.6/EasyOutput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 03:16:16.000000 EasyOutput-0.0.6/EasyOutput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 03:16:16.000000 EasyOutput-0.0.6/EasyOutput.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 03:16:16.000000 EasyOutput-0.0.6/EasyOutput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-04-02 02:23:26.000000 EasyOutput-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2468 2024-04-02 03:16:16.872242 EasyOutput-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 03:16:16.869241 EasyOutput-0.0.6/easyoutput/
--rw-rw-rw-   0        0        0     2481 2024-04-02 02:11:20.000000 EasyOutput-0.0.6/easyoutput/EasyOutput.py
--rw-rw-rw-   0        0        0        0 2024-04-02 02:14:53.000000 EasyOutput-0.0.6/easyoutput/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-02 03:16:16.873241 EasyOutput-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1171 2024-04-02 03:15:51.000000 EasyOutput-0.0.6/setup.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.0.7/.github/ISSUE_TEMPLATE/🐞-bug-report.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.0.7/.github/ISSUE_TEMPLATE/🚀feature-request.md
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 easyoutput-0.0.7/src/EasyOutput/EasyOutput.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyoutput-0.0.7/src/EasyOutput/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 easyoutput-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 easyoutput-0.0.7/README.md
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 easyoutput-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 easyoutput-0.0.7/PKG-INFO
```

### Comparing `EasyOutput-0.0.6/easyoutput/EasyOutput.py` & `easyoutput-0.0.7/src/EasyOutput/EasyOutput.py`

 * *Files identical despite different names*

