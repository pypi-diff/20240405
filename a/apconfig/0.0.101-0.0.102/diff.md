# Comparing `tmp/apconfig-0.0.101.tar.gz` & `tmp/apconfig-0.0.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apconfig-0.0.101.tar", max compression
+gzip compressed data, was "apconfig-0.0.102.tar", max compression
```

## Comparing `apconfig-0.0.101.tar` & `apconfig-0.0.102.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.101/README.md
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 apconfig-0.0.101/apconfig/__init__.py
--rw-r--r--   0        0        0      305 2024-03-27 10:48:26.036377 apconfig-0.0.101/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.101/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.102/README.md
+-rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 apconfig-0.0.102/apconfig/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-05 06:25:39.273690 apconfig-0.0.102/apconfig/utilities.py
+-rw-r--r--   0        0        0      305 2024-04-05 06:25:49.645785 apconfig-0.0.102/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.102/PKG-INFO
```

### Comparing `apconfig-0.0.101/apconfig/__init__.py` & `apconfig-0.0.102/apconfig/__init__.py`

 * *Files identical despite different names*

