# Comparing `tmp/louvre-0.1.0.tar.gz` & `tmp/louvre-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "louvre-0.1.0.tar", max compression
+gzip compressed data, was "louvre-1.0.0.tar", max compression
```

## Comparing `louvre-0.1.0.tar` & `louvre-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0      114 2024-02-28 18:16:21.325533 louvre-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-02-28 18:09:35.941787 louvre-0.1.0/louvre/__init__.py
--rw-r--r--   0        0        0      331 2024-02-28 18:14:12.617637 louvre-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 louvre-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      201 2024-04-05 18:27:19.551775 louvre-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 18:27:19.551948 louvre-1.0.0/louvre/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-05 18:27:19.552276 louvre-1.0.0/louvre/coingecko/__init__.py
+-rw-r--r--   0        0        0      664 2024-04-05 18:27:19.552467 louvre-1.0.0/louvre/coingecko/client.py
+-rw-r--r--   0        0        0      333 2024-04-05 18:27:19.552649 louvre-1.0.0/louvre/coingecko/format.py
+-rw-r--r--   0        0        0      433 2024-04-05 18:33:33.833201 louvre-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 louvre-1.0.0/PKG-INFO
```

