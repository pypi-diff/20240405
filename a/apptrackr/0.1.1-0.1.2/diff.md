# Comparing `tmp/apptrackr-0.1.1.tar.gz` & `tmp/apptrackr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.1.tar", max compression
+gzip compressed data, was "apptrackr-0.1.2.tar", max compression
```

## Comparing `apptrackr-0.1.1.tar` & `apptrackr-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.1/README.md
--rw-r--r--   0        0        0     4772 2024-04-05 11:41:48.188446 apptrackr-0.1.1/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.1/apptrackr/model/__init__.py
--rw-r--r--   0        0        0      598 2024-04-04 18:12:10.777458 apptrackr-0.1.1/apptrackr/model/model.py
--rw-r--r--   0        0        0      414 2024-04-05 11:46:28.424294 apptrackr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.2/README.md
+-rw-r--r--   0        0        0     5452 2024-04-05 12:02:44.413755 apptrackr-0.1.2/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.2/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-05 12:09:54.199285 apptrackr-0.1.2/apptrackr/model/model.py
+-rw-r--r--   0        0        0      414 2024-04-05 12:10:26.037098 apptrackr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.2/PKG-INFO
```

### Comparing `apptrackr-0.1.1/apptrackr/main.py` & `apptrackr-0.1.2/apptrackr/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from typing import Optional
 
 import typer
-from .model import Applications
 from typing_extensions import Annotated
 
+from .model import Applications
+
 tracker = typer.Typer()
 
 
 @tracker.command()
 def count(
     active: Annotated[
         bool,
         typer.Option(
             help="Get only active application",
         ),
     ] = False
 ) -> None:
-    """Get count of application"""
+    """
+    Fetch counts of applications.
+
+    Args:
+        active (Annotated[ bool, typer.Option, optional): Fetch only active applications.)]=False.
+    """
     if active:
         count = Applications.select().where(Applications.status == "active").count()
     else:
         count = Applications.select().count()
 
     typer.echo(
         typer.style(f"Application Count: {count}", fg=typer.colors.BRIGHT_WHITE),
@@ -35,14 +41,26 @@
     location: Annotated[
         Optional[str], typer.Argument(help="Optional Job location")
     ] = None,
     date: Annotated[
         Optional[str], typer.Argument(help="Optional Application date")
     ] = None,
 ) -> None:
+    """Add new application to the database.
+
+    Args:
+        name (Annotated[str, typer.Argument, optional): Job application name)].
+        status (Annotated[str, typer.Argument, optional): Job status)].
+        apply_link (Annotated[str, typer.Argument, optional): Application link)].
+        location (Annotated[ Optional[str], typer.Argument, optional): Optional Job location)]=None.
+        date (Annotated[ Optional[str], typer.Argument, optional): Optional Application date)]=None.
+
+    Raises:
+        typer.Exit: For invalid arguments
+    """
     if status not in ("active", "rejected", "accepted"):
         typer.echo("Invalid status argument!")
         raise typer.Exit(-1)
 
     application_details = {"name": name, "status": status, "apply_link": apply_link}
 
     if location:
```

### Comparing `apptrackr-0.1.1/apptrackr/model/model.py` & `apptrackr-0.1.2/apptrackr/model/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import os
 from datetime import datetime
 
 from peewee import AutoField, CharField, DateTimeField, Model, SqliteDatabase
 
-database = SqliteDatabase("applications.db")
+database = SqliteDatabase(
+    os.path.join(os.path.expanduser("~"), "applications.db"),
+)
 
 
 class Applications(Model):
     application_id = AutoField()
     name = CharField(max_length=100)
     status = CharField()
     location = CharField(default="uk")
```

