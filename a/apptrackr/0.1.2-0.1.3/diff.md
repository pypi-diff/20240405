# Comparing `tmp/apptrackr-0.1.2.tar.gz` & `tmp/apptrackr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.2.tar", max compression
+gzip compressed data, was "apptrackr-0.1.3.tar", max compression
```

## Comparing `apptrackr-0.1.2.tar` & `apptrackr-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.2/README.md
--rw-r--r--   0        0        0     5452 2024-04-05 12:02:44.413755 apptrackr-0.1.2/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.2/apptrackr/model/__init__.py
--rw-r--r--   0        0        0      654 2024-04-05 12:09:54.199285 apptrackr-0.1.2/apptrackr/model/model.py
--rw-r--r--   0        0        0      414 2024-04-05 12:10:26.037098 apptrackr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.3/README.md
+-rw-r--r--   0        0        0     5633 2024-04-05 14:44:34.320401 apptrackr-0.1.3/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.3/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-05 14:43:11.847544 apptrackr-0.1.3/apptrackr/model/model.py
+-rw-r--r--   0        0        0      414 2024-04-05 14:45:06.671574 apptrackr-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.3/PKG-INFO
```

### Comparing `apptrackr-0.1.2/apptrackr/main.py` & `apptrackr-0.1.3/apptrackr/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 
 @tracker.command()
 def add_application(
     name: Annotated[str, typer.Argument(help="Job application name")],
     status: Annotated[str, typer.Argument(help="Job status")],
     apply_link: Annotated[str, typer.Argument(help="Application link")],
+    applied_through: Annotated[
+        str, typer.Argument(help="Email Id sent with application")
+    ],
     location: Annotated[
         Optional[str], typer.Argument(help="Optional Job location")
     ] = None,
     date: Annotated[
         Optional[str], typer.Argument(help="Optional Application date")
     ] = None,
 ) -> None:
@@ -57,15 +60,20 @@
     Raises:
         typer.Exit: For invalid arguments
     """
     if status not in ("active", "rejected", "accepted"):
         typer.echo("Invalid status argument!")
         raise typer.Exit(-1)
 
-    application_details = {"name": name, "status": status, "apply_link": apply_link}
+    application_details = {
+        "name": name,
+        "status": status,
+        "apply_link": apply_link,
+        "applied_through": applied_through,
+    }
 
     if location:
         application_details["location"] = location
 
     if date:
         application_details["date"] = date
```

### Comparing `apptrackr-0.1.2/apptrackr/model/model.py` & `apptrackr-0.1.3/apptrackr/model/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 class Applications(Model):
     application_id = AutoField()
     name = CharField(max_length=100)
     status = CharField()
     location = CharField(default="uk")
     date = DateTimeField(formats="%d/%m/%y %H:%M:%S.%f", default=datetime.now)
     apply_link = CharField(max_length=150)
+    applied_through = CharField()
 
     class Meta:
         database = database
 
 
 if not Applications.table_exists():
     print("Creating Application Table...")
```

