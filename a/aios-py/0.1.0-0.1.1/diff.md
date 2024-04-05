# Comparing `tmp/aios_py-0.1.0.tar.gz` & `tmp/aios_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aios_py-0.1.0.tar", max compression
+gzip compressed data, was "aios_py-0.1.1.tar", max compression
```

## Comparing `aios_py-0.1.0.tar` & `aios_py-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-03 15:30:46.945829 aios_py-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-03 15:30:46.945789 aios_py-0.1.0/aios_py/__init__.py
--rw-r--r--   0        0        0      260 2024-04-03 15:30:46.946670 aios_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      279 1970-01-01 00:00:00.000000 aios_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-05 15:39:31.328883 aios_py-0.1.1/README.md
+-rw-r--r--   0        0        0       28 2024-04-05 15:48:18.986663 aios_py-0.1.1/aios_py/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-05 15:47:01.928638 aios_py-0.1.1/aios_py/utils.py
+-rw-r--r--   0        0        0      319 2024-04-05 15:50:25.110076 aios_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 aios_py-0.1.1/PKG-INFO
```

