# Comparing `tmp/snowflakecli-0.3.3.tar.gz` & `tmp/snowflakecli-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflakecli-0.3.3.tar", last modified: Fri Apr  5 14:11:36 2024, max compression
+gzip compressed data, was "snowflakecli-0.3.4.tar", last modified: Fri Apr  5 14:13:13 2024, max compression
```

## Comparing `snowflakecli-0.3.3.tar` & `snowflakecli-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:11:36.327452 snowflakecli-0.3.3/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-05 14:11:36.327267 snowflakecli-0.3.3/PKG-INFO
--rw-r--r--   0 jacobthomas   (501) staff       (20)       15 2024-03-29 15:52:39.000000 snowflakecli-0.3.3/README.md
--rw-r--r--   0 jacobthomas   (501) staff       (20)      530 2024-04-05 14:11:29.000000 snowflakecli-0.3.3/pyproject.toml
--rw-r--r--   0 jacobthomas   (501) staff       (20)       38 2024-04-05 14:11:36.327488 snowflakecli-0.3.3/setup.cfg
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:11:36.324978 snowflakecli-0.3.3/src/
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:11:36.325020 snowflakecli-0.3.3/src/snowflakecli/
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:11:36.326924 snowflakecli-0.3.3/src/snowflakecli/cli/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      250 2024-04-04 02:12:07.000000 snowflakecli-0.3.3/src/snowflakecli/cli/account.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      155 2024-04-04 01:55:51.000000 snowflakecli-0.3.3/src/snowflakecli/cli/ask.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      107 2024-04-05 13:44:20.000000 snowflakecli-0.3.3/src/snowflakecli/cli/configure.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      388 2024-04-04 02:03:43.000000 snowflakecli-0.3.3/src/snowflakecli/cli/database.py
--rwxr-xr-x   0 jacobthomas   (501) staff       (20)      929 2024-04-05 14:10:49.000000 snowflakecli-0.3.3/src/snowflakecli/cli/main.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:47.000000 snowflakecli-0.3.3/src/snowflakecli/cli/schema.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      479 2024-04-05 13:41:24.000000 snowflakecli-0.3.3/src/snowflakecli/cli/scrape.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:55.000000 snowflakecli-0.3.3/src/snowflakecli/cli/table.py
--rw-r--r--   0 jacobthomas   (501) staff       (20)      404 2024-04-04 01:52:20.000000 snowflakecli-0.3.3/src/snowflakecli/cli/warehouse.py
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:11:36.327074 snowflakecli-0.3.3/src/snowflakecli.egg-info/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-05 14:11:36.000000 snowflakecli-0.3.3/src/snowflakecli.egg-info/PKG-INFO
--rw-r--r--   0 jacobthomas   (501) staff       (20)      548 2024-04-05 14:11:36.000000 snowflakecli-0.3.3/src/snowflakecli.egg-info/SOURCES.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)        1 2024-04-05 14:11:36.000000 snowflakecli-0.3.3/src/snowflakecli.egg-info/dependency_links.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       95 2024-04-05 14:11:36.000000 snowflakecli-0.3.3/src/snowflakecli.egg-info/entry_points.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       82 2024-04-05 14:11:36.000000 snowflakecli-0.3.3/src/snowflakecli.egg-info/requires.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       13 2024-04-05 14:11:36.000000 snowflakecli-0.3.3/src/snowflakecli.egg-info/top_level.txt
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:13:13.957704 snowflakecli-0.3.4/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-05 14:13:13.957490 snowflakecli-0.3.4/PKG-INFO
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       15 2024-03-29 15:52:39.000000 snowflakecli-0.3.4/README.md
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      530 2024-04-05 14:13:06.000000 snowflakecli-0.3.4/pyproject.toml
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       38 2024-04-05 14:13:13.957738 snowflakecli-0.3.4/setup.cfg
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:13:13.954692 snowflakecli-0.3.4/src/
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:13:13.954744 snowflakecli-0.3.4/src/snowflakecli/
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:13:13.956956 snowflakecli-0.3.4/src/snowflakecli/cli/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      250 2024-04-04 02:12:07.000000 snowflakecli-0.3.4/src/snowflakecli/cli/account.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      155 2024-04-04 01:55:51.000000 snowflakecli-0.3.4/src/snowflakecli/cli/ask.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      107 2024-04-05 13:44:20.000000 snowflakecli-0.3.4/src/snowflakecli/cli/configure.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      388 2024-04-04 02:03:43.000000 snowflakecli-0.3.4/src/snowflakecli/cli/database.py
+-rwxr-xr-x   0 jacobthomas   (501) staff       (20)      995 2024-04-05 14:12:40.000000 snowflakecli-0.3.4/src/snowflakecli/cli/main.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:47.000000 snowflakecli-0.3.4/src/snowflakecli/cli/schema.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      479 2024-04-05 13:41:24.000000 snowflakecli-0.3.4/src/snowflakecli/cli/scrape.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:55.000000 snowflakecli-0.3.4/src/snowflakecli/cli/table.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      404 2024-04-04 01:52:20.000000 snowflakecli-0.3.4/src/snowflakecli/cli/warehouse.py
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-05 14:13:13.957160 snowflakecli-0.3.4/src/snowflakecli.egg-info/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-05 14:13:13.000000 snowflakecli-0.3.4/src/snowflakecli.egg-info/PKG-INFO
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      548 2024-04-05 14:13:13.000000 snowflakecli-0.3.4/src/snowflakecli.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        1 2024-04-05 14:13:13.000000 snowflakecli-0.3.4/src/snowflakecli.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       95 2024-04-05 14:13:13.000000 snowflakecli-0.3.4/src/snowflakecli.egg-info/entry_points.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       82 2024-04-05 14:13:13.000000 snowflakecli-0.3.4/src/snowflakecli.egg-info/requires.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       13 2024-04-05 14:13:13.000000 snowflakecli-0.3.4/src/snowflakecli.egg-info/top_level.txt
```

### Comparing `snowflakecli-0.3.3/pyproject.toml` & `snowflakecli-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "snowflakecli"
-version = "0.3.3"
+version = "0.3.4"
 description = "A DuckDB-powered, AI-augmented command line interface to Snowflake."
 authors = [{ name = "jake", email = "jake@bostata.com" }]
 dependencies = [
     "duckdb>=0.10.1",
     "snowflake-connector-python>=3.7.1",
     "typer>=0.12.0",
     "datafusion>=36.0.0",
```

### Comparing `snowflakecli-0.3.3/src/snowflakecli/cli/main.py` & `snowflakecli-0.3.4/src/snowflakecli/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 import typer
-import snowflakecli.cli.ask
-import snowflakecli.cli.configure
-import snowflakecli.cli.scrape
-import snowflakecli.cli.account
-import snowflakecli.cli.database
-import snowflakecli.cli.warehouse
+import snowflakecli.cli.ask as ask
+import snowflakecli.cli.configure as configure
+import snowflakecli.cli.scrape as scrape
+import snowflakecli.cli.account as account
+import snowflakecli.cli.database as database
+import snowflakecli.cli.warehouse as warehouse
 
 app = typer.Typer()
 
 
 app.add_typer(
     ask.app,
     name="ask",
```

### Comparing `snowflakecli-0.3.3/src/snowflakecli.egg-info/SOURCES.txt` & `snowflakecli-0.3.4/src/snowflakecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

