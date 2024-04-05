# Comparing `tmp/blackneedles-0.1.3.tar.gz` & `tmp/blackneedles-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackneedles-0.1.3.tar", max compression
+gzip compressed data, was "blackneedles-0.1.4.tar", max compression
```

## Comparing `blackneedles-0.1.3.tar` & `blackneedles-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1639 2024-04-04 22:59:26.980475 blackneedles-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/__init__.py
--rw-r--r--   0        0        0     2534 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/__main__.py
--rw-r--r--   0        0        0        0 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/commands/__init__.py
--rw-r--r--   0        0        0     2258 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/commands/service.py
--rw-r--r--   0        0        0     2069 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/connection.py
--rw-r--r--   0        0        0     1301 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/console.py
--rw-r--r--   0        0        0        0 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/models/__init__.py
--rw-r--r--   0        0        0     3258 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/models/service.py
--rw-r--r--   0        0        0      431 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/procedures/grant_permissions.sql
--rw-r--r--   0        0        0     1644 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/procedures/monitoring_procedures.sql
--rw-r--r--   0        0        0       47 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/procedures/uninstall.sql
--rw-r--r--   0        0        0      711 2024-04-04 22:59:27.464474 blackneedles-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1639 2024-04-05 15:32:43.416303 blackneedles-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/__init__.py
+-rw-r--r--   0        0        0     2601 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/commands/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/commands/compute_pool.py
+-rw-r--r--   0        0        0     2258 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/commands/service.py
+-rw-r--r--   0        0        0     2069 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/connection.py
+-rw-r--r--   0        0        0     1301 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/console.py
+-rw-r--r--   0        0        0        0 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/models/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/models/compute_pool.py
+-rw-r--r--   0        0        0     3258 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/models/service.py
+-rw-r--r--   0        0        0      431 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/procedures/grant_permissions.sql
+-rw-r--r--   0        0        0     1644 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/procedures/monitoring_procedures.sql
+-rw-r--r--   0        0        0       47 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/procedures/uninstall.sql
+-rw-r--r--   0        0        0      711 2024-04-05 15:32:43.928303 blackneedles-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.4/PKG-INFO
```

### Comparing `blackneedles-0.1.3/README.md` & `blackneedles-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.3/blackneedles/__main__.py` & `blackneedles-0.1.4/blackneedles/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from dataclasses import dataclass
 import os
 from typing import Annotated, Literal, Optional
 import typer
 import sqlparse  # type: ignore
 
-from blackneedles.commands import service
+from blackneedles.commands import compute_pool, service
 from blackneedles.connection import Database
 
 
 @dataclass
 class GlobalParams:
     table_style: Literal["rich", "plain"]
 
 
 app = typer.Typer()
 app.add_typer(service.app, name="service")
+app.add_typer(compute_pool.app, name="compute-pool")
 
 
 @app.command("install")
 def install_procedures(
     ctx: typer.Context,
     grant_target: Annotated[
         Optional[str], typer.Option(help="To whom should we grant permission?")
```

### Comparing `blackneedles-0.1.3/blackneedles/commands/service.py` & `blackneedles-0.1.4/blackneedles/commands/service.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.3/blackneedles/connection.py` & `blackneedles-0.1.4/blackneedles/connection.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.3/blackneedles/console.py` & `blackneedles-0.1.4/blackneedles/console.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.3/blackneedles/models/service.py` & `blackneedles-0.1.4/blackneedles/models/service.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.3/blackneedles/procedures/monitoring_procedures.sql` & `blackneedles-0.1.4/blackneedles/procedures/monitoring_procedures.sql`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.3/pyproject.toml` & `blackneedles-0.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackneedles"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Thiago F Pappacena <pappacena@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 # Note: snowflake-snowpark-python requires <3.12. Fix this once they support 3.12
 python = "^3.8,<3.12"
```

### Comparing `blackneedles-0.1.3/PKG-INFO` & `blackneedles-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackneedles
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Thiago F Pappacena
 Author-email: pappacena@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

