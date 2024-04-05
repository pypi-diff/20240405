# Comparing `tmp/blackneedles-0.1.2.tar.gz` & `tmp/blackneedles-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackneedles-0.1.2.tar", max compression
+gzip compressed data, was "blackneedles-0.1.3.tar", max compression
```

## Comparing `blackneedles-0.1.2.tar` & `blackneedles-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1648 2024-04-04 22:12:45.991319 blackneedles-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/__init__.py
--rw-r--r--   0        0        0     1017 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/__main__.py
--rw-r--r--   0        0        0        0 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/commands/__init__.py
--rw-r--r--   0        0        0     2016 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/commands/service.py
--rw-r--r--   0        0        0     1982 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/connection.py
--rw-r--r--   0        0        0     1301 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/console.py
--rw-r--r--   0        0        0        0 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/models/__init__.py
--rw-r--r--   0        0        0     3258 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/models/service.py
--rw-r--r--   0        0        0     1371 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/procedures/monitoring_procedures.sql
--rw-r--r--   0        0        0      691 2024-04-04 22:12:46.491322 blackneedles-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 blackneedles-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1639 2024-04-04 22:59:26.980475 blackneedles-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/__init__.py
+-rw-r--r--   0        0        0     2534 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/commands/__init__.py
+-rw-r--r--   0        0        0     2258 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/commands/service.py
+-rw-r--r--   0        0        0     2069 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/connection.py
+-rw-r--r--   0        0        0     1301 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/console.py
+-rw-r--r--   0        0        0        0 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/models/__init__.py
+-rw-r--r--   0        0        0     3258 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/models/service.py
+-rw-r--r--   0        0        0      431 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/procedures/grant_permissions.sql
+-rw-r--r--   0        0        0     1644 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/procedures/monitoring_procedures.sql
+-rw-r--r--   0        0        0       47 2024-04-04 22:59:26.980475 blackneedles-0.1.3/blackneedles/procedures/uninstall.sql
+-rw-r--r--   0        0        0      711 2024-04-04 22:59:27.464474 blackneedles-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.3/PKG-INFO
```

### Comparing `blackneedles-0.1.2/README.md` & `blackneedles-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Blackneedles
 
 Blackneedles a simple and easy to use python library and command line tool to manage and bring observability to Snowflake Snowpark Container Services and Snowflake Native Apps.
 
-The name comes from the Black Needles Peak (Pico das Agulhas Negras), the highest mountain in the state of Rio de Janeiro, Brazil, and only place in the state where one can see snow flakes falling.
+The name comes from the Black Needles Peak (Pico das Agulhas Negras), the highest mountain in the state of Rio de Janeiro, Brazil, and only place in the state where one can see snowflakes.
 
 ## Installation
 
 ```bash
 pip install blackneedles
 ```
```

### Comparing `blackneedles-0.1.2/blackneedles/commands/service.py` & `blackneedles-0.1.3/blackneedles/commands/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Annotated, List, Optional
 import typer
 
 from blackneedles.console import print_table
 from blackneedles.models.service import Service
 
-app = typer.Typer()
+app = typer.Typer(short_help="Manage services in Snowpark Container Services.")
 
 
 @app.command("list")
 def list_all_services(
     ctx: typer.Context,
     schema: Annotated[
         Optional[str], typer.Option(help="The schema to list services from")
     ] = None,
     compute_pool: Annotated[
         Optional[str],
         typer.Option("--compute-pool", help="The compute pool to list services from"),
     ] = None,
 ):
+    """Gives the list of services and its current status"""
     services = Service.objects.from_namespace(
         {
             "schema_name": schema,
             "compute_pool": compute_pool,
         }
     )
     services = list(services)
@@ -46,14 +47,15 @@
 @app.command("describe")
 def describe_service(
     ctx: typer.Context,
     service_names: Annotated[
         List[str], typer.Argument(..., help="The name of the service to describe")
     ],
 ):
+    """Describe a given service name."""
     services = [Service.objects.get(name) for name in service_names]
     print_table(
         ctx,
         services,
         [
             "full_path",
             "compute_pool",
@@ -70,12 +72,15 @@
 
 @app.command("alter")
 def alter_status(
     ctx: typer.Context,
     service_name: Annotated[
         str, typer.Argument(..., help="The name of the service to describe")
     ],
-    action: Annotated[str, typer.Argument(..., help="Service state to change")],
+    action: Annotated[
+        str, typer.Argument(..., help="Service state to change [SUSPEND, RESUME]")
+    ],
 ):
+    """Changes the status of a given service."""
     service = Service.objects.get(service_name)
     service.alter_status(action)
     typer.echo(f"Service {service_name} is now {action}")
```

### Comparing `blackneedles-0.1.2/blackneedles/connection.py` & `blackneedles-0.1.3/blackneedles/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             or config["connections"]["password"],
             warehouse=os.getenv("SNOWFLAKE_WAREHOUSE")
             or config["connections"].get("warehousename"),
             database=os.getenv("SNOWFLAKE_DATABASE")
             or config["connections"].get("dbname"),
             schema=os.getenv("SNOWFLAKE_SCHEMA")
             or config["connections"].get("schemaname"),
+            role=os.getenv("SNOWFLAKE_ROLE") or config["connections"].get("rolename"),
         )
         session_builder = Session.builder.config("connection_name", "default")
         session_builder.configs(self.config)
         self.session = session_builder.create()
 
     @classmethod
     def get_instance(self) -> "Database":
```

### Comparing `blackneedles-0.1.2/blackneedles/console.py` & `blackneedles-0.1.3/blackneedles/console.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.2/blackneedles/models/service.py` & `blackneedles-0.1.3/blackneedles/models/service.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.2/blackneedles/procedures/monitoring_procedures.sql` & `blackneedles-0.1.3/blackneedles/procedures/monitoring_procedures.sql`

 * *Files 13% similar despite different names*

```diff
@@ -50,7 +50,22 @@
 BEGIN
     LET alter_service_statement string := 'ALTER SERVICE ' || service_name || ' ' || action || ' ;';
     EXECUTE IMMEDIATE alter_service_statement;
     RETURN alter_service_statement;
 END;
 $$
 ;
+
+
+-- CALL __blackneedles__.list_compute_pool(database_name)
+CREATE OR REPLACE PROCEDURE __blackneedles__.list_compute_pool ()
+    RETURNS TABLE ()
+    LANGUAGE sql
+    as $$
+DECLARE
+    res RESULTSET;
+BEGIN
+    res := (SHOW COMPUTE POOLS);
+    RETURN TABLE(res);
+END;
+$$
+;
```

### Comparing `blackneedles-0.1.2/pyproject.toml` & `blackneedles-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "blackneedles"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Thiago F Pappacena <pappacena@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 # Note: snowflake-snowpark-python requires <3.12. Fix this once they support 3.12
 python = "^3.8,<3.12"
 typer = "^0.11.0"
 snowflake-connector-python = "^3.7.1"
 snowflake-snowpark-python = "^1.14.0"
 pydantic = "^2.6.4"
 ipython = "^8.0.0"
 rich = "^13.7.1"
+sqlparse = "^0.4.4"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.4"
 pytest = "^8.1.1"
 pre-commit = "^3.0.0"
 mypy = "^1.9.0"
```

### Comparing `blackneedles-0.1.2/PKG-INFO` & `blackneedles-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: blackneedles
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Thiago F Pappacena
 Author-email: pappacena@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipython (>=8.0.0,<9.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: snowflake-connector-python (>=3.7.1,<4.0.0)
 Requires-Dist: snowflake-snowpark-python (>=1.14.0,<2.0.0)
+Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
 Requires-Dist: typer (>=0.11.0,<0.12.0)
 Description-Content-Type: text/markdown
 
 # Blackneedles
 
 Blackneedles a simple and easy to use python library and command line tool to manage and bring observability to Snowflake Snowpark Container Services and Snowflake Native Apps.
 
-The name comes from the Black Needles Peak (Pico das Agulhas Negras), the highest mountain in the state of Rio de Janeiro, Brazil, and only place in the state where one can see snow flakes falling.
+The name comes from the Black Needles Peak (Pico das Agulhas Negras), the highest mountain in the state of Rio de Janeiro, Brazil, and only place in the state where one can see snowflakes.
 
 ## Installation
 
 ```bash
 pip install blackneedles
 ```
```

