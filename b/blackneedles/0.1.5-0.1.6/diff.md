# Comparing `tmp/blackneedles-0.1.5.tar.gz` & `tmp/blackneedles-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackneedles-0.1.5.tar", max compression
+gzip compressed data, was "blackneedles-0.1.6.tar", max compression
```

## Comparing `blackneedles-0.1.5.tar` & `blackneedles-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1639 2024-04-05 16:39:13.952380 blackneedles-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/__init__.py
--rw-r--r--   0        0        0     2601 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/__main__.py
--rw-r--r--   0        0        0        0 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/commands/__init__.py
--rw-r--r--   0        0        0      964 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/commands/compute_pool.py
--rw-r--r--   0        0        0     3237 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/commands/service.py
--rw-r--r--   0        0        0     2069 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/connection.py
--rw-r--r--   0        0        0     1301 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/console.py
--rw-r--r--   0        0        0        0 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/models/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/models/compute_pool.py
--rw-r--r--   0        0        0     3568 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/models/service.py
--rw-r--r--   0        0        0      455 2024-04-05 16:39:13.956380 blackneedles-0.1.5/blackneedles/procedures/grant_permissions.sql
--rw-r--r--   0        0        0     1749 2024-04-05 16:39:13.956380 blackneedles-0.1.5/blackneedles/procedures/monitoring_procedures.sql
--rw-r--r--   0        0        0       47 2024-04-05 16:39:13.956380 blackneedles-0.1.5/blackneedles/procedures/uninstall.sql
--rw-r--r--   0        0        0      711 2024-04-05 16:39:14.524380 blackneedles-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1639 2024-04-05 21:40:25.442183 blackneedles-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/__init__.py
+-rw-r--r--   0        0        0     2601 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/commands/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/commands/compute_pool.py
+-rw-r--r--   0        0        0     3459 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/commands/service.py
+-rw-r--r--   0        0        0     2069 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/connection.py
+-rw-r--r--   0        0        0     1301 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/console.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/models/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/models/compute_pool.py
+-rw-r--r--   0        0        0     3568 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/models/service.py
+-rw-r--r--   0        0        0      455 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/procedures/grant_permissions.sql
+-rw-r--r--   0        0        0     1749 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/procedures/monitoring_procedures.sql
+-rw-r--r--   0        0        0       47 2024-04-05 21:40:25.442183 blackneedles-0.1.6/blackneedles/procedures/uninstall.sql
+-rw-r--r--   0        0        0      711 2024-04-05 21:40:25.942189 blackneedles-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.6/PKG-INFO
```

### Comparing `blackneedles-0.1.5/README.md` & `blackneedles-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.5/blackneedles/__main__.py` & `blackneedles-0.1.6/blackneedles/__main__.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.5/blackneedles/commands/compute_pool.py` & `blackneedles-0.1.6/blackneedles/commands/compute_pool.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.5/blackneedles/commands/service.py` & `blackneedles-0.1.6/blackneedles/commands/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 from time import sleep
 from typing import Annotated, List, Optional
 import typer
 
 from blackneedles.console import print_table
 from blackneedles.models.service import Service
+from utils.logs import replace_repeated_lines
 
 app = typer.Typer(short_help="Manage services in Snowpark Container Services.")
 
 
 @app.command("list")
 def list_all_services(
     ctx: typer.Context,
@@ -90,24 +91,33 @@
     follow: Annotated[bool, typer.Option("-f")] = False,
 ):
     """
     Shows logs from the given service.
 
     If -f is passed, it will follow the logs.
     """
+
+    def get_log_lines():
+        return service.get_logs(instance_id, container_name).split("\n")
+
+    def print_lines(lines):
+        if not lines:
+            return
+        print("\n".join(lines), end="")
+
     service = Service.objects.get(service_name)
-    log = service.get_logs(instance_id, container_name)
+    log = get_log_lines()
+    print_lines(log)
     if not follow:
-        print(log)
         sys.exit(0)
     while True:
-        if log:
-            print(log)
         sleep(0.5)
-        log = service.get_logs(instance_id, container_name).replace(log, "")
+        old_log = log
+        log = get_log_lines()
+        print_lines(replace_repeated_lines(log, old_log))
 
 
 @app.command("alter")
 def alter_status(
     ctx: typer.Context,
     service_name: Annotated[
         str, typer.Argument(..., help="The name of the service to describe")
```

### Comparing `blackneedles-0.1.5/blackneedles/connection.py` & `blackneedles-0.1.6/blackneedles/connection.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.5/blackneedles/console.py` & `blackneedles-0.1.6/blackneedles/console.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.5/blackneedles/models/compute_pool.py` & `blackneedles-0.1.6/blackneedles/models/compute_pool.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.5/blackneedles/models/service.py` & `blackneedles-0.1.6/blackneedles/models/service.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.5/blackneedles/procedures/monitoring_procedures.sql` & `blackneedles-0.1.6/blackneedles/procedures/monitoring_procedures.sql`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.5/pyproject.toml` & `blackneedles-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackneedles"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Thiago F Pappacena <pappacena@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 # Note: snowflake-snowpark-python requires <3.12. Fix this once they support 3.12
 python = "^3.8,<3.12"
```

### Comparing `blackneedles-0.1.5/PKG-INFO` & `blackneedles-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackneedles
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Thiago F Pappacena
 Author-email: pappacena@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

