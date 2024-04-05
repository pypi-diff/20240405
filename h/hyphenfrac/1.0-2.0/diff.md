# Comparing `tmp/hyphenfrac-1.0.tar.gz` & `tmp/hyphenfrac-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyphenfrac-1.0.tar", last modified: Tue Feb 27 06:17:48 2024, max compression
+gzip compressed data, was "hyphenfrac-2.0.tar", last modified: Fri Apr  5 11:57:50 2024, max compression
```

## Comparing `hyphenfrac-1.0.tar` & `hyphenfrac-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-02-27 06:17:48.925013 hyphenfrac-1.0/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      706 2024-02-27 06:17:48.925013 hyphenfrac-1.0/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      378 2024-02-27 05:39:51.000000 hyphenfrac-1.0/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-02-27 06:17:48.924013 hyphenfrac-1.0/hyphenfrac/
--rw-r--r--   0 xyz       (1000) xyz       (1000)       55 2024-02-27 05:46:28.000000 hyphenfrac-1.0/hyphenfrac/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1715 2024-02-27 05:45:51.000000 hyphenfrac-1.0/hyphenfrac/main.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-02-27 06:17:48.925013 hyphenfrac-1.0/hyphenfrac.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      706 2024-02-27 06:17:48.000000 hyphenfrac-1.0/hyphenfrac.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      196 2024-02-27 06:17:48.000000 hyphenfrac-1.0/hyphenfrac.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-02-27 06:17:48.000000 hyphenfrac-1.0/hyphenfrac.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-02-27 06:17:48.000000 hyphenfrac-1.0/hyphenfrac.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-02-27 06:17:48.925013 hyphenfrac-1.0/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)      523 2024-02-27 06:07:34.000000 hyphenfrac-1.0/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 11:57:50.015260 hyphenfrac-2.0/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1062 2024-02-27 06:30:18.000000 hyphenfrac-2.0/LICENSE
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2033 2024-04-05 11:57:50.015260 hyphenfrac-2.0/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1259 2024-04-05 11:44:33.000000 hyphenfrac-2.0/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 11:57:50.015260 hyphenfrac-2.0/hyphenfrac/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3337 2024-04-05 11:56:40.000000 hyphenfrac-2.0/hyphenfrac/__init__.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 11:57:50.015260 hyphenfrac-2.0/hyphenfrac.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2033 2024-04-05 11:57:50.000000 hyphenfrac-2.0/hyphenfrac.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      185 2024-04-05 11:57:50.000000 hyphenfrac-2.0/hyphenfrac.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-05 11:57:50.000000 hyphenfrac-2.0/hyphenfrac.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-04-05 11:57:50.000000 hyphenfrac-2.0/hyphenfrac.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-05 11:57:50.015260 hyphenfrac-2.0/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      951 2024-04-05 11:00:43.000000 hyphenfrac-2.0/setup.py
```

