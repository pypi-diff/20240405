# Comparing `tmp/snowflakecli-0.3.5.tar.gz` & `tmp/snowflakecli-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflakecli-0.3.5.tar", last modified: Fri Apr  5 14:25:06 2024, max compression
+gzip compressed data, was "snowflakecli-0.3.6.tar", last modified: Fri Apr  5 14:25:49 2024, max compression
```

## Comparing `snowflakecli-0.3.5.tar` & `snowflakecli-0.3.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:06.274950 snowflakecli-0.3.5/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      450 2024-04-05 14:25:06.274765 snowflakecli-0.3.5/PKG-INFO
--rw-r--r--   0 jacobthomas   (501) staff       (20)       15 2024-03-29 15:52:39.000000 snowflakecli-0.3.5/README.md
--rw-r--r--   0 jacobthomas   (501) staff       (20)      572 2024-04-05 14:24:51.000000 snowflakecli-0.3.5/pyproject.toml
--rw-r--r--   0 jacobthomas   (501) staff       (20)       38 2024-04-05 14:25:06.274984 snowflakecli-0.3.5/setup.cfg
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:06.271994 snowflakecli-0.3.5/src/
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:06.272043 snowflakecli-0.3.5/src/snowflakecli/
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:06.274341 snowflakecli-0.3.5/src/snowflakecli/cli/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      424 2024-04-05 14:22:07.000000 snowflakecli-0.3.5/src/snowflakecli/cli/account.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      155 2024-04-04 01:55:51.000000 snowflakecli-0.3.5/src/snowflakecli/cli/ask.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      185 2024-04-05 14:22:44.000000 snowflakecli-0.3.5/src/snowflakecli/cli/configure.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      388 2024-04-04 02:03:43.000000 snowflakecli-0.3.5/src/snowflakecli/cli/database.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      225 2024-04-05 14:24:07.000000 snowflakecli-0.3.5/src/snowflakecli/cli/debug.py
--rwxr-xr-x   0 jacobthomas   (501) staff       (20)     1121 2024-04-05 14:19:22.000000 snowflakecli-0.3.5/src/snowflakecli/cli/main.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:47.000000 snowflakecli-0.3.5/src/snowflakecli/cli/schema.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      479 2024-04-05 13:41:24.000000 snowflakecli-0.3.5/src/snowflakecli/cli/scrape.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:55.000000 snowflakecli-0.3.5/src/snowflakecli/cli/table.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      404 2024-04-04 01:52:20.000000 snowflakecli-0.3.5/src/snowflakecli/cli/warehouse.py
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:06.274569 snowflakecli-0.3.5/src/snowflakecli.egg-info/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      450 2024-04-05 14:25:06.000000 snowflakecli-0.3.5/src/snowflakecli.egg-info/PKG-INFO
--rw-r--r--   0 jacobthomas   (501) staff       (20)      578 2024-04-05 14:25:06.000000 snowflakecli-0.3.5/src/snowflakecli.egg-info/SOURCES.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)        1 2024-04-05 14:25:06.000000 snowflakecli-0.3.5/src/snowflakecli.egg-info/dependency_links.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       95 2024-04-05 14:25:06.000000 snowflakecli-0.3.5/src/snowflakecli.egg-info/entry_points.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       82 2024-04-05 14:25:06.000000 snowflakecli-0.3.5/src/snowflakecli.egg-info/requires.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       13 2024-04-05 14:25:06.000000 snowflakecli-0.3.5/src/snowflakecli.egg-info/top_level.txt
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:49.239729 snowflakecli-0.3.6/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      465 2024-04-05 14:25:49.239559 snowflakecli-0.3.6/PKG-INFO
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       15 2024-03-29 15:52:39.000000 snowflakecli-0.3.6/README.md
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      587 2024-04-05 14:25:40.000000 snowflakecli-0.3.6/pyproject.toml
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       38 2024-04-05 14:25:49.239772 snowflakecli-0.3.6/setup.cfg
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:49.236971 snowflakecli-0.3.6/src/
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:49.237018 snowflakecli-0.3.6/src/snowflakecli/
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:49.239236 snowflakecli-0.3.6/src/snowflakecli/cli/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      424 2024-04-05 14:22:07.000000 snowflakecli-0.3.6/src/snowflakecli/cli/account.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      155 2024-04-04 01:55:51.000000 snowflakecli-0.3.6/src/snowflakecli/cli/ask.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      185 2024-04-05 14:22:44.000000 snowflakecli-0.3.6/src/snowflakecli/cli/configure.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      388 2024-04-04 02:03:43.000000 snowflakecli-0.3.6/src/snowflakecli/cli/database.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      225 2024-04-05 14:24:07.000000 snowflakecli-0.3.6/src/snowflakecli/cli/debug.py
+-rwxr-xr-x   0 jacobthomas   (501) staff       (20)     1121 2024-04-05 14:19:22.000000 snowflakecli-0.3.6/src/snowflakecli/cli/main.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:47.000000 snowflakecli-0.3.6/src/snowflakecli/cli/schema.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      479 2024-04-05 13:41:24.000000 snowflakecli-0.3.6/src/snowflakecli/cli/scrape.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:55.000000 snowflakecli-0.3.6/src/snowflakecli/cli/table.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      404 2024-04-04 01:52:20.000000 snowflakecli-0.3.6/src/snowflakecli/cli/warehouse.py
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:25:49.239388 snowflakecli-0.3.6/src/snowflakecli.egg-info/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      465 2024-04-05 14:25:49.000000 snowflakecli-0.3.6/src/snowflakecli.egg-info/PKG-INFO
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      578 2024-04-05 14:25:49.000000 snowflakecli-0.3.6/src/snowflakecli.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        1 2024-04-05 14:25:49.000000 snowflakecli-0.3.6/src/snowflakecli.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       95 2024-04-05 14:25:49.000000 snowflakecli-0.3.6/src/snowflakecli.egg-info/entry_points.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       82 2024-04-05 14:25:49.000000 snowflakecli-0.3.6/src/snowflakecli.egg-info/requires.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       13 2024-04-05 14:25:49.000000 snowflakecli-0.3.6/src/snowflakecli.egg-info/top_level.txt
```

### Comparing `snowflakecli-0.3.5/src/snowflakecli/cli/main.py` & `snowflakecli-0.3.6/src/snowflakecli/cli/main.py`

 * *Files identical despite different names*

### Comparing `snowflakecli-0.3.5/src/snowflakecli.egg-info/SOURCES.txt` & `snowflakecli-0.3.6/src/snowflakecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

