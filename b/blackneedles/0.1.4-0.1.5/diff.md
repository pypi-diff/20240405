# Comparing `tmp/blackneedles-0.1.4.tar.gz` & `tmp/blackneedles-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackneedles-0.1.4.tar", max compression
+gzip compressed data, was "blackneedles-0.1.5.tar", max compression
```

## Comparing `blackneedles-0.1.4.tar` & `blackneedles-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1639 2024-04-05 15:32:43.416303 blackneedles-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/__init__.py
--rw-r--r--   0        0        0     2601 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/__main__.py
--rw-r--r--   0        0        0        0 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/commands/__init__.py
--rw-r--r--   0        0        0      964 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/commands/compute_pool.py
--rw-r--r--   0        0        0     2258 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/commands/service.py
--rw-r--r--   0        0        0     2069 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/connection.py
--rw-r--r--   0        0        0     1301 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/console.py
--rw-r--r--   0        0        0        0 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/models/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/models/compute_pool.py
--rw-r--r--   0        0        0     3258 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/models/service.py
--rw-r--r--   0        0        0      431 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/procedures/grant_permissions.sql
--rw-r--r--   0        0        0     1644 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/procedures/monitoring_procedures.sql
--rw-r--r--   0        0        0       47 2024-04-05 15:32:43.416303 blackneedles-0.1.4/blackneedles/procedures/uninstall.sql
--rw-r--r--   0        0        0      711 2024-04-05 15:32:43.928303 blackneedles-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1639 2024-04-05 16:39:13.952380 blackneedles-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/__init__.py
+-rw-r--r--   0        0        0     2601 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/commands/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/commands/compute_pool.py
+-rw-r--r--   0        0        0     3237 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/commands/service.py
+-rw-r--r--   0        0        0     2069 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/connection.py
+-rw-r--r--   0        0        0     1301 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/console.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/models/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/models/compute_pool.py
+-rw-r--r--   0        0        0     3568 2024-04-05 16:39:13.952380 blackneedles-0.1.5/blackneedles/models/service.py
+-rw-r--r--   0        0        0      455 2024-04-05 16:39:13.956380 blackneedles-0.1.5/blackneedles/procedures/grant_permissions.sql
+-rw-r--r--   0        0        0     1749 2024-04-05 16:39:13.956380 blackneedles-0.1.5/blackneedles/procedures/monitoring_procedures.sql
+-rw-r--r--   0        0        0       47 2024-04-05 16:39:13.956380 blackneedles-0.1.5/blackneedles/procedures/uninstall.sql
+-rw-r--r--   0        0        0      711 2024-04-05 16:39:14.524380 blackneedles-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.5/PKG-INFO
```

### Comparing `blackneedles-0.1.4/README.md` & `blackneedles-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.4/blackneedles/__main__.py` & `blackneedles-0.1.5/blackneedles/__main__.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.4/blackneedles/commands/compute_pool.py` & `blackneedles-0.1.5/blackneedles/commands/compute_pool.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.4/blackneedles/commands/service.py` & `blackneedles-0.1.5/blackneedles/commands/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+from time import sleep
 from typing import Annotated, List, Optional
 import typer
 
 from blackneedles.console import print_table
 from blackneedles.models.service import Service
 
 app = typer.Typer(short_help="Manage services in Snowpark Container Services.")
@@ -66,14 +68,48 @@
             "ID",
             "Compute pool" "Status",
             "spec",
         ],
     )
 
 
+@app.command("logs")
+def get_service_logs(
+    ctx: typer.Context,
+    service_name: Annotated[
+        str, typer.Argument(..., help="The name of the service to describe")
+    ],
+    instance_id: Annotated[
+        str,
+        typer.Argument(
+            ..., help="The service instance id to get logs from. If unsure, try '0'"
+        ),
+    ],
+    container_name: Annotated[
+        str, typer.Argument(..., help="The name of the container in the service")
+    ],
+    follow: Annotated[bool, typer.Option("-f")] = False,
+):
+    """
+    Shows logs from the given service.
+
+    If -f is passed, it will follow the logs.
+    """
+    service = Service.objects.get(service_name)
+    log = service.get_logs(instance_id, container_name)
+    if not follow:
+        print(log)
+        sys.exit(0)
+    while True:
+        if log:
+            print(log)
+        sleep(0.5)
+        log = service.get_logs(instance_id, container_name).replace(log, "")
+
+
 @app.command("alter")
 def alter_status(
     ctx: typer.Context,
     service_name: Annotated[
         str, typer.Argument(..., help="The name of the service to describe")
     ],
     action: Annotated[
```

### Comparing `blackneedles-0.1.4/blackneedles/connection.py` & `blackneedles-0.1.5/blackneedles/connection.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.4/blackneedles/console.py` & `blackneedles-0.1.5/blackneedles/console.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.4/blackneedles/models/compute_pool.py` & `blackneedles-0.1.5/blackneedles/models/compute_pool.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.4/blackneedles/models/service.py` & `blackneedles-0.1.5/blackneedles/models/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,14 +61,22 @@
             raise ValueError(
                 f"Invalid status: {status}. Should be one of {valid_status}"
             )
         Database.get_instance().get_rows(
             "CALL __blackneedles__.alter_service(?, ?)", (self.full_path, status)
         )
 
+    def get_logs(self, instance_id, container_name: str) -> str:
+        return list(
+            Database.get_instance().get_rows(
+                "CALL __blackneedles__.get_service_logs(?, ?, ?)",
+                (self.full_path, instance_id, container_name),
+            )
+        )[0]["GET_SERVICE_LOGS"]
+
     class objects:
         @classmethod
         def get(cls, service_name: str) -> "Service":
             db = Database.get_instance()
             return list(
                 db.query(
                     Service,
```

### Comparing `blackneedles-0.1.4/blackneedles/procedures/monitoring_procedures.sql` & `blackneedles-0.1.5/blackneedles/procedures/monitoring_procedures.sql`

 * *Files 16% similar despite different names*

```diff
@@ -51,21 +51,17 @@
     LET alter_service_statement string := 'ALTER SERVICE ' || service_name || ' ' || action || ' ;';
     EXECUTE IMMEDIATE alter_service_statement;
     RETURN alter_service_statement;
 END;
 $$
 ;
 
-
--- CALL __blackneedles__.list_compute_pool(database_name)
-CREATE OR REPLACE PROCEDURE __blackneedles__.list_compute_pool ()
-    RETURNS TABLE ()
+-- CALL __blackneedles__.get_service_logs('service_name', 'container_name'))
+CREATE OR REPLACE PROCEDURE __blackneedles__.get_service_logs (service_name varchar, service_instance varchar, container_name varchar)
+    RETURNS string
     LANGUAGE sql
     as $$
-DECLARE
-    res RESULTSET;
 BEGIN
-    res := (SHOW COMPUTE POOLS);
-    RETURN TABLE(res);
+    RETURN (SELECT SYSTEM$GET_SERVICE_LOGS(:service_name, :service_instance, :container_name) AS log);
 END;
 $$
 ;
```

### Comparing `blackneedles-0.1.4/pyproject.toml` & `blackneedles-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackneedles"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Thiago F Pappacena <pappacena@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 # Note: snowflake-snowpark-python requires <3.12. Fix this once they support 3.12
 python = "^3.8,<3.12"
```

### Comparing `blackneedles-0.1.4/PKG-INFO` & `blackneedles-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackneedles
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Thiago F Pappacena
 Author-email: pappacena@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

