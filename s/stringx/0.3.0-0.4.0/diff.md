# Comparing `tmp/stringx-0.3.0.tar.gz` & `tmp/stringx-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringx-0.3.0.tar", last modified: Mon Apr  1 00:12:51 2024, max compression
+gzip compressed data, was "stringx-0.4.0.tar", last modified: Fri Apr  5 12:49:33 2024, max compression
```

## Comparing `stringx-0.3.0.tar` & `stringx-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-03-31 00:59:04.811433 stringx-0.3.0/LICENSE
--rw-r--r--   0        0        0     2022 2024-04-01 00:11:07.190775 stringx-0.3.0/README.md
--rw-r--r--   0        0        0      638 2024-04-01 00:12:51.550404 stringx-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      696 2024-04-01 00:12:27.338473 stringx-0.3.0/src/stringx/__init__.py
--rw-r--r--   0        0        0     2484 2024-03-31 23:11:05.391418 stringx-0.3.0/src/stringx/client.py
--rw-r--r--   0        0        0        0 2024-03-31 00:59:04.811433 stringx-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3365 2024-03-31 23:07:27.274958 stringx-0.3.0/tests/test_client.py
--rw-r--r--   0        0        0     1750 2024-03-31 23:04:56.310374 stringx-0.3.0/tests/test_stringx.py
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 stringx-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-18 00:39:05.484210 stringx-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3218 2024-04-04 00:16:00.373070 stringx-0.4.0/README.md
+-rw-r--r--   0        0        0     1783 2024-04-05 12:49:33.259956 stringx-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2006 2024-04-05 12:44:27.699955 stringx-0.4.0/src/stringx/__init__.py
+-rw-r--r--   0        0        0     2923 2024-04-05 12:48:49.719956 stringx-0.4.0/src/stringx/client.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:27:23.943070 stringx-0.4.0/src/stringx/py.typed
+-rw-r--r--   0        0        0        0 2024-03-18 00:39:05.504210 stringx-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-04 00:02:15.343066 stringx-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     5002 2024-04-04 23:44:22.050896 stringx-0.4.0/tests/test_client.py
+-rw-r--r--   0        0        0     1353 2024-04-05 12:40:11.419953 stringx-0.4.0/tests/test_stringx.py
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 stringx-0.4.0/PKG-INFO
```

### Comparing `stringx-0.3.0/LICENSE` & `stringx-0.4.0/LICENSE`

 * *Files identical despite different names*

