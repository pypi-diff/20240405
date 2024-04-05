# Comparing `tmp/snowflakecli-0.3.1.tar.gz` & `tmp/snowflakecli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflakecli-0.3.1.tar", last modified: Fri Apr  5 13:52:02 2024, max compression
+gzip compressed data, was "snowflakecli-0.3.2.tar", last modified: Fri Apr  5 14:08:58 2024, max compression
```

## Comparing `snowflakecli-0.3.1.tar` & `snowflakecli-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 13:52:02.662218 snowflakecli-0.3.1/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-05 13:52:02.662017 snowflakecli-0.3.1/PKG-INFO
--rw-r--r--   0 jacobthomas   (501) staff       (20)       15 2024-03-29 15:52:39.000000 snowflakecli-0.3.1/README.md
--rw-r--r--   0 jacobthomas   (501) staff       (20)      475 2024-04-05 13:51:56.000000 snowflakecli-0.3.1/pyproject.toml
--rw-r--r--   0 jacobthomas   (501) staff       (20)       38 2024-04-05 13:52:02.662252 snowflakecli-0.3.1/setup.cfg
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 13:52:02.659370 snowflakecli-0.3.1/src/
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 13:52:02.659413 snowflakecli-0.3.1/src/snowflakecli/
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 13:52:02.661658 snowflakecli-0.3.1/src/snowflakecli/cli/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      250 2024-04-04 02:12:07.000000 snowflakecli-0.3.1/src/snowflakecli/cli/account.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      155 2024-04-04 01:55:51.000000 snowflakecli-0.3.1/src/snowflakecli/cli/ask.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      107 2024-04-05 13:44:20.000000 snowflakecli-0.3.1/src/snowflakecli/cli/configure.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      388 2024-04-04 02:03:43.000000 snowflakecli-0.3.1/src/snowflakecli/cli/database.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      809 2024-04-05 13:49:56.000000 snowflakecli-0.3.1/src/snowflakecli/cli/main.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:47.000000 snowflakecli-0.3.1/src/snowflakecli/cli/schema.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      479 2024-04-05 13:41:24.000000 snowflakecli-0.3.1/src/snowflakecli/cli/scrape.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:55.000000 snowflakecli-0.3.1/src/snowflakecli/cli/table.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      404 2024-04-04 01:52:20.000000 snowflakecli-0.3.1/src/snowflakecli/cli/warehouse.py
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 13:52:02.661833 snowflakecli-0.3.1/src/snowflakecli.egg-info/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-05 13:52:02.000000 snowflakecli-0.3.1/src/snowflakecli.egg-info/PKG-INFO
--rw-r--r--   0 jacobthomas   (501) staff       (20)      548 2024-04-05 13:52:02.000000 snowflakecli-0.3.1/src/snowflakecli.egg-info/SOURCES.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)        1 2024-04-05 13:52:02.000000 snowflakecli-0.3.1/src/snowflakecli.egg-info/dependency_links.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       41 2024-04-05 13:52:02.000000 snowflakecli-0.3.1/src/snowflakecli.egg-info/entry_points.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       82 2024-04-05 13:52:02.000000 snowflakecli-0.3.1/src/snowflakecli.egg-info/requires.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       13 2024-04-05 13:52:02.000000 snowflakecli-0.3.1/src/snowflakecli.egg-info/top_level.txt
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:08:58.679548 snowflakecli-0.3.2/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-05 14:08:58.679335 snowflakecli-0.3.2/PKG-INFO
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       15 2024-03-29 15:52:39.000000 snowflakecli-0.3.2/README.md
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      530 2024-04-05 14:04:31.000000 snowflakecli-0.3.2/pyproject.toml
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       38 2024-04-05 14:08:58.679580 snowflakecli-0.3.2/setup.cfg
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:08:58.676682 snowflakecli-0.3.2/src/
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:08:58.676723 snowflakecli-0.3.2/src/snowflakecli/
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:08:58.678975 snowflakecli-0.3.2/src/snowflakecli/cli/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      250 2024-04-04 02:12:07.000000 snowflakecli-0.3.2/src/snowflakecli/cli/account.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      155 2024-04-04 01:55:51.000000 snowflakecli-0.3.2/src/snowflakecli/cli/ask.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      107 2024-04-05 13:44:20.000000 snowflakecli-0.3.2/src/snowflakecli/cli/configure.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      388 2024-04-04 02:03:43.000000 snowflakecli-0.3.2/src/snowflakecli/cli/database.py
+-rwxr-xr-x   0 jacobthomas   (501) staff       (20)      827 2024-04-05 14:07:58.000000 snowflakecli-0.3.2/src/snowflakecli/cli/main.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:47.000000 snowflakecli-0.3.2/src/snowflakecli/cli/schema.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      479 2024-04-05 13:41:24.000000 snowflakecli-0.3.2/src/snowflakecli/cli/scrape.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:55.000000 snowflakecli-0.3.2/src/snowflakecli/cli/table.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      404 2024-04-04 01:52:20.000000 snowflakecli-0.3.2/src/snowflakecli/cli/warehouse.py
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:08:58.679145 snowflakecli-0.3.2/src/snowflakecli.egg-info/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-05 14:08:58.000000 snowflakecli-0.3.2/src/snowflakecli.egg-info/PKG-INFO
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      548 2024-04-05 14:08:58.000000 snowflakecli-0.3.2/src/snowflakecli.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        1 2024-04-05 14:08:58.000000 snowflakecli-0.3.2/src/snowflakecli.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       95 2024-04-05 14:08:58.000000 snowflakecli-0.3.2/src/snowflakecli.egg-info/entry_points.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       82 2024-04-05 14:08:58.000000 snowflakecli-0.3.2/src/snowflakecli.egg-info/requires.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       13 2024-04-05 14:08:58.000000 snowflakecli-0.3.2/src/snowflakecli.egg-info/top_level.txt
```

### Comparing `snowflakecli-0.3.1/src/snowflakecli.egg-info/SOURCES.txt` & `snowflakecli-0.3.2/src/snowflakecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

