# Comparing `tmp/tdmd-0.0.1.tar.gz` & `tmp/tdmd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdmd-0.0.1.tar", last modified: Fri Apr  5 21:43:40 2024, max compression
+gzip compressed data, was "tdmd-0.0.2.tar", last modified: Fri Apr  5 21:53:14 2024, max compression
```

## Comparing `tdmd-0.0.1.tar` & `tdmd-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-04-05 21:43:40.809020 tdmd-0.0.1/
--rw-r--r--   0 alex      (1000) alex      (1000)     1501 2023-11-11 18:20:34.000000 tdmd-0.0.1/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      740 2024-04-05 21:43:40.808020 tdmd-0.0.1/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      454 2024-04-05 21:31:07.000000 tdmd-0.0.1/README.md
--rw-r--r--   0 alex      (1000) alex      (1000)      356 2024-04-05 21:42:57.000000 tdmd-0.0.1/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2024-04-05 21:43:40.809020 tdmd-0.0.1/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-04-05 21:43:40.808020 tdmd-0.0.1/tdmd.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      740 2024-04-05 21:43:40.000000 tdmd-0.0.1/tdmd.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      209 2024-04-05 21:43:40.000000 tdmd-0.0.1/tdmd.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-04-05 21:43:40.000000 tdmd-0.0.1/tdmd.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        5 2024-04-05 21:43:40.000000 tdmd-0.0.1/tdmd.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        7 2024-04-05 21:43:40.000000 tdmd-0.0.1/tdmd.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-04-05 21:43:40.807021 tdmd-0.0.1/todomd/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2024-04-01 05:32:20.000000 tdmd-0.0.1/todomd/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      272 2024-04-05 21:34:44.000000 tdmd-0.0.1/todomd/__main__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-04-05 21:53:14.050496 tdmd-0.0.2/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1501 2023-11-11 18:20:34.000000 tdmd-0.0.2/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      776 2024-04-05 21:53:14.050496 tdmd-0.0.2/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      454 2024-04-05 21:46:42.000000 tdmd-0.0.2/README.md
+-rw-r--r--   0 alex      (1000) alex      (1000)      392 2024-04-05 21:52:59.000000 tdmd-0.0.2/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2024-04-05 21:53:14.050496 tdmd-0.0.2/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-04-05 21:53:14.049496 tdmd-0.0.2/tdmd.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      776 2024-04-05 21:53:14.000000 tdmd-0.0.2/tdmd.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      209 2024-04-05 21:53:14.000000 tdmd-0.0.2/tdmd.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-04-05 21:53:14.000000 tdmd-0.0.2/tdmd.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        5 2024-04-05 21:53:14.000000 tdmd-0.0.2/tdmd.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        7 2024-04-05 21:53:14.000000 tdmd-0.0.2/tdmd.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-04-05 21:53:14.049496 tdmd-0.0.2/todomd/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2024-04-01 05:32:20.000000 tdmd-0.0.2/todomd/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      272 2024-04-05 21:34:44.000000 tdmd-0.0.2/todomd/__main__.py
```

### Comparing `tdmd-0.0.1/LICENSE` & `tdmd-0.0.2/LICENSE`

 * *Files identical despite different names*

