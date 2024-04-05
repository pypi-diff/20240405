# Comparing `tmp/cozo_migrate-0.2.3.tar.gz` & `tmp/cozo_migrate-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cozo_migrate-0.2.3.tar", max compression
+gzip compressed data, was "cozo_migrate-0.2.4.tar", max compression
```

## Comparing `cozo_migrate-0.2.3.tar` & `cozo_migrate-0.2.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1065 2024-01-07 13:33:12.365368 cozo_migrate-0.2.3/LICENSE
--rw-r--r--   0        0        0    10252 2024-01-10 05:40:45.096558 cozo_migrate-0.2.3/README.md
--rw-r--r--   0        0        0       46 2024-01-08 10:26:55.521771 cozo_migrate-0.2.3/cozo_migrate/__init__.py
--rw-r--r--   0        0        0       64 2024-01-09 09:52:34.471830 cozo_migrate-0.2.3/cozo_migrate/__main__.py
--rw-r--r--   0        0        0      144 2024-01-09 09:55:01.612126 cozo_migrate-0.2.3/cozo_migrate/api/__init__.py
--rw-r--r--   0        0        0     1735 2024-01-09 10:32:02.806824 cozo_migrate-0.2.3/cozo_migrate/api/apply.py
--rw-r--r--   0        0        0     1232 2024-01-09 10:17:19.678766 cozo_migrate-0.2.3/cozo_migrate/api/create.py
--rw-r--r--   0        0        0      228 2024-01-09 10:03:41.137291 cozo_migrate-0.2.3/cozo_migrate/api/history.py
--rw-r--r--   0        0        0      270 2024-01-09 10:09:19.444935 cozo_migrate-0.2.3/cozo_migrate/api/init.py
--rw-r--r--   0        0        0      391 2024-01-09 10:00:50.747806 cozo_migrate-0.2.3/cozo_migrate/api/status.py
--rw-r--r--   0        0        0      173 2024-01-08 13:25:23.457943 cozo_migrate-0.2.3/cozo_migrate/cli/__init__.py
--rw-r--r--   0        0        0     2570 2024-01-09 10:36:34.265894 cozo_migrate-0.2.3/cozo_migrate/cli/apply.py
--rw-r--r--   0        0        0     1812 2024-01-08 13:51:11.869212 cozo_migrate-0.2.3/cozo_migrate/cli/create.py
--rw-r--r--   0        0        0      485 2024-01-08 14:22:47.904793 cozo_migrate-0.2.3/cozo_migrate/cli/history.py
--rw-r--r--   0        0        0      521 2024-01-09 10:10:39.614511 cozo_migrate-0.2.3/cozo_migrate/cli/init.py
--rw-r--r--   0        0        0     1809 2024-01-09 09:20:40.361541 cozo_migrate-0.2.3/cozo_migrate/cli/main.py
--rw-r--r--   0        0        0      579 2024-01-09 09:49:56.842260 cozo_migrate-0.2.3/cozo_migrate/cli/status.py
--rw-r--r--   0        0        0      220 2024-01-08 13:23:26.360172 cozo_migrate-0.2.3/cozo_migrate/cli/version.py
--rw-r--r--   0        0        0     1774 2024-01-09 09:19:37.572173 cozo_migrate-0.2.3/cozo_migrate/context.py
--rw-r--r--   0        0        0      800 2024-01-06 20:04:23.042497 cozo_migrate-0.2.3/cozo_migrate/files.py
--rw-r--r--   0        0        0     2205 2024-01-09 09:48:28.914513 cozo_migrate-0.2.3/cozo_migrate/modules.py
--rw-r--r--   0        0        0     2862 2024-01-10 08:18:45.650157 cozo_migrate-0.2.3/cozo_migrate/ops.py
--rw-r--r--   0        0        0     2005 2024-01-09 10:13:32.021031 cozo_migrate-0.2.3/cozo_migrate/queries.py
--rw-r--r--   0        0        0      654 2024-01-09 10:37:24.875701 cozo_migrate-0.2.3/cozo_migrate/schema.py
--rw-r--r--   0        0        0      189 2024-01-06 17:44:47.984105 cozo_migrate-0.2.3/cozo_migrate/template.py
--rw-r--r--   0        0        0     1586 2024-01-09 09:43:16.149374 cozo_migrate-0.2.3/cozo_migrate/types.py
--rw-r--r--   0        0        0       23 2024-01-06 14:52:42.904170 cozo_migrate-0.2.3/cozo_migrate/utils/__init__.py
--rw-r--r--   0        0        0      193 2024-01-08 13:25:06.335130 cozo_migrate-0.2.3/cozo_migrate/utils/client.py
--rw-r--r--   0        0        0      736 2024-01-09 10:28:01.352153 cozo_migrate-0.2.3/cozo_migrate/utils/console.py
--rw-r--r--   0        0        0      334 2024-01-08 14:12:37.736561 cozo_migrate-0.2.3/cozo_migrate/utils/datetime.py
--rw-r--r--   0        0        0      757 2024-01-09 09:40:33.657527 cozo_migrate-0.2.3/cozo_migrate/utils/fn.py
--rw-r--r--   0        0        0     2142 2024-01-08 10:07:18.232941 cozo_migrate-0.2.3/cozo_migrate/utils/rich.py
--rw-r--r--   0        0        0     1368 2024-02-28 15:07:10.702160 cozo_migrate-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    11030 1970-01-01 00:00:00.000000 cozo_migrate-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-07 13:33:12.365368 cozo_migrate-0.2.4/LICENSE
+-rw-r--r--   0        0        0    10665 2024-04-05 08:38:40.077649 cozo_migrate-0.2.4/README.md
+-rw-r--r--   0        0        0       46 2024-01-08 10:26:55.521771 cozo_migrate-0.2.4/cozo_migrate/__init__.py
+-rw-r--r--   0        0        0       64 2024-01-09 09:52:34.471830 cozo_migrate-0.2.4/cozo_migrate/__main__.py
+-rw-r--r--   0        0        0      144 2024-01-09 09:55:01.612126 cozo_migrate-0.2.4/cozo_migrate/api/__init__.py
+-rw-r--r--   0        0        0     1735 2024-01-09 10:32:02.806824 cozo_migrate-0.2.4/cozo_migrate/api/apply.py
+-rw-r--r--   0        0        0     1232 2024-01-09 10:17:19.678766 cozo_migrate-0.2.4/cozo_migrate/api/create.py
+-rw-r--r--   0        0        0      228 2024-01-09 10:03:41.137291 cozo_migrate-0.2.4/cozo_migrate/api/history.py
+-rw-r--r--   0        0        0      270 2024-01-09 10:09:19.444935 cozo_migrate-0.2.4/cozo_migrate/api/init.py
+-rw-r--r--   0        0        0      391 2024-01-09 10:00:50.747806 cozo_migrate-0.2.4/cozo_migrate/api/status.py
+-rw-r--r--   0        0        0      196 2024-04-05 08:15:47.137817 cozo_migrate-0.2.4/cozo_migrate/cli/__init__.py
+-rw-r--r--   0        0        0     2731 2024-04-05 06:57:03.087336 cozo_migrate-0.2.4/cozo_migrate/cli/apply.py
+-rw-r--r--   0        0        0     1812 2024-01-08 13:51:11.869212 cozo_migrate-0.2.4/cozo_migrate/cli/create.py
+-rw-r--r--   0        0        0      485 2024-01-08 14:22:47.904793 cozo_migrate-0.2.4/cozo_migrate/cli/history.py
+-rw-r--r--   0        0        0      521 2024-01-09 10:10:39.614511 cozo_migrate-0.2.4/cozo_migrate/cli/init.py
+-rw-r--r--   0        0        0     1809 2024-01-09 09:20:40.361541 cozo_migrate-0.2.4/cozo_migrate/cli/main.py
+-rw-r--r--   0        0        0      629 2024-04-05 08:34:06.052587 cozo_migrate-0.2.4/cozo_migrate/cli/show.py
+-rw-r--r--   0        0        0      579 2024-01-09 09:49:56.842260 cozo_migrate-0.2.4/cozo_migrate/cli/status.py
+-rw-r--r--   0        0        0      220 2024-01-08 13:23:26.360172 cozo_migrate-0.2.4/cozo_migrate/cli/version.py
+-rw-r--r--   0        0        0     1774 2024-01-09 09:19:37.572173 cozo_migrate-0.2.4/cozo_migrate/context.py
+-rw-r--r--   0        0        0      800 2024-01-06 20:04:23.042497 cozo_migrate-0.2.4/cozo_migrate/files.py
+-rw-r--r--   0        0        0     2205 2024-01-09 09:48:28.914513 cozo_migrate-0.2.4/cozo_migrate/modules.py
+-rw-r--r--   0        0        0     2862 2024-01-10 08:18:45.650157 cozo_migrate-0.2.4/cozo_migrate/ops.py
+-rw-r--r--   0        0        0     2465 2024-04-05 08:36:47.882846 cozo_migrate-0.2.4/cozo_migrate/queries.py
+-rw-r--r--   0        0        0      654 2024-01-09 10:37:24.875701 cozo_migrate-0.2.4/cozo_migrate/schema.py
+-rw-r--r--   0        0        0      189 2024-01-06 17:44:47.984105 cozo_migrate-0.2.4/cozo_migrate/template.py
+-rw-r--r--   0        0        0     1586 2024-01-09 09:43:16.149374 cozo_migrate-0.2.4/cozo_migrate/types.py
+-rw-r--r--   0        0        0       23 2024-01-06 14:52:42.904170 cozo_migrate-0.2.4/cozo_migrate/utils/__init__.py
+-rw-r--r--   0        0        0      193 2024-01-08 13:25:06.335130 cozo_migrate-0.2.4/cozo_migrate/utils/client.py
+-rw-r--r--   0        0        0      736 2024-01-09 10:28:01.352153 cozo_migrate-0.2.4/cozo_migrate/utils/console.py
+-rw-r--r--   0        0        0      334 2024-01-08 14:12:37.736561 cozo_migrate-0.2.4/cozo_migrate/utils/datetime.py
+-rw-r--r--   0        0        0      757 2024-01-09 09:40:33.657527 cozo_migrate-0.2.4/cozo_migrate/utils/fn.py
+-rw-r--r--   0        0        0     2142 2024-01-08 10:07:18.232941 cozo_migrate-0.2.4/cozo_migrate/utils/rich.py
+-rw-r--r--   0        0        0     1424 2024-04-05 08:37:35.846333 cozo_migrate-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    11494 1970-01-01 00:00:00.000000 cozo_migrate-0.2.4/PKG-INFO
```

### Comparing `cozo_migrate-0.2.3/LICENSE` & `cozo_migrate-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/README.md` & `cozo_migrate-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 $ # Let's create a migration
 $ cozo-migrate -e http -d ./migrations create demo
   Writing 'migrations/migrate_1704803704_demo.py' Confirm? [y/N]: y
   ✔ Created migration at: migrations/migrate_1704803704_demo.py
 
 $ cat migrations/migrate_1704803704_demo.py
   #/usr/bin/env python3
-  
+
   MIGRATION_ID = "demo"
   CREATED_AT = 1704803704.762879
-  
+
   def up(client):
       pass
-  
+
   def down(client):
       pass
 
 $ # Edit the migration to add schema change queries and then apply!
 $ cozo-migrate -e http -d ./migrations apply -a
   • Migrate path: [NONE] → demo
   Are you sure you want to apply these migrations? [y/N]: y
@@ -114,14 +114,26 @@
 │ --down                                         │
 │ --all   -a                                     │
 │ --yes   -y                                     │
 │ --help            Show this message and exit.  │
 ╰────────────────────────────────────────────────╯
 ```
 
+#### Show
+
+```bash
+ Usage: cozo-migrate show
+
+ Show the current schema in the database.
+
+╭─ Options ────────────────────────────────────╮
+│ --help          Show this message and exit.  │
+╰──────────────────────────────────────────────╯
+```
+
 #### Status
 
 ```bash
  Usage: cozo-migrate status [OPTIONS]
 
  Display the current migration status.
```

### Comparing `cozo_migrate-0.2.3/cozo_migrate/api/apply.py` & `cozo_migrate-0.2.4/cozo_migrate/api/apply.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/api/create.py` & `cozo_migrate-0.2.4/cozo_migrate/api/create.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/cli/apply.py` & `cozo_migrate-0.2.4/cozo_migrate/cli/apply.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @app.command()
 def apply(
     ctx: typer.Context,
     steps: Annotated[int, typer.Argument()] = 1,
     down: Annotated[bool, typer.Option("--down")] = False,
     all_: Annotated[bool, typer.Option("--all", "-a")] = False,
     confirm: Annotated[bool, typer.Option("--yes", "-y")] = False,
+    compact: Annotated[bool, typer.Option("--compact")] = False,
 ):
     """
     Apply migrations to the database.
     You can specify the number of steps to apply and the direction.
     """
 
     # Validate client
@@ -71,11 +72,15 @@
             raise typer.Abort()
 
     info("Migrating the database...")
     applied_successfully, migration_error = apply_migrations(
         client, migrations, down=down, verbose=verbose, from_cli=True
     )
 
+    if compact:
+        client.run("::compact")
+        info("Database compaction initiated.")
+
     if applied_successfully:
         success("Database migrated.")
     else:
         fail("Migration failed.", error=migration_error)
```

### Comparing `cozo_migrate-0.2.3/cozo_migrate/cli/create.py` & `cozo_migrate-0.2.4/cozo_migrate/cli/create.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/cli/init.py` & `cozo_migrate-0.2.4/cozo_migrate/cli/init.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/cli/main.py` & `cozo_migrate-0.2.4/cozo_migrate/cli/main.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/cli/status.py` & `cozo_migrate-0.2.4/cozo_migrate/cli/status.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/context.py` & `cozo_migrate-0.2.4/cozo_migrate/context.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/files.py` & `cozo_migrate-0.2.4/cozo_migrate/files.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/modules.py` & `cozo_migrate-0.2.4/cozo_migrate/modules.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/ops.py` & `cozo_migrate-0.2.4/cozo_migrate/ops.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/queries.py` & `cozo_migrate-0.2.4/cozo_migrate/queries.py`

 * *Files 20% similar despite different names*

```diff
@@ -95,7 +95,22 @@
     migration = Migration.get_first(client.run(get_latest_query))
     return migration
 
 
 def get_first_migration(client: Client) -> Optional[Migration]:
     migration = Migration.get_first(client.run(get_first_query))
     return migration
+
+
+def get_current_schema(client: Client) -> pd.DataFrame:
+    all_relations = client.run("::relations")
+    normal_relations = all_relations[all_relations["access_level"] != "index"][
+        ["name", "description"]
+    ]
+
+    relation_wise_columns = {
+        relation: client.run(f"::columns {relation}").drop("index", axis=1)
+        for relation in normal_relations["name"]
+        if relation != MANAGER_TABLE_NAME
+    }
+
+    return relation_wise_columns
```

### Comparing `cozo_migrate-0.2.3/cozo_migrate/schema.py` & `cozo_migrate-0.2.4/cozo_migrate/schema.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/types.py` & `cozo_migrate-0.2.4/cozo_migrate/types.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/utils/console.py` & `cozo_migrate-0.2.4/cozo_migrate/utils/console.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/utils/fn.py` & `cozo_migrate-0.2.4/cozo_migrate/utils/fn.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/cozo_migrate/utils/rich.py` & `cozo_migrate-0.2.4/cozo_migrate/utils/rich.py`

 * *Files identical despite different names*

### Comparing `cozo_migrate-0.2.3/pyproject.toml` & `cozo_migrate-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cozo-migrate"
-version = "0.2.3"
+version = "0.2.4"
 description = "A simple utility for migrations for cozo db"
 authors = ["Diwank Singh Tomer <diwank.singh@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -44,13 +44,14 @@
     "lint",
     "typecheck",
 ]
 
 test = [
     { cmd = "cozo-migrate -f cozo.db init" },
     { cmd = "cozo-migrate -d dummy/migrations create hello -y" },
-    { cmd = "cozo-migrate -f cozo.db -d test/migrations apply -y" },
+    { cmd = "cozo-migrate -f cozo.db -d test/migrations apply -y --compact" },
     { cmd = "cozo-migrate -f cozo.db status" },
+    { cmd = "cozo-migrate -f cozo.db show" },
     { cmd = "cozo-migrate -f cozo.db -d test/migrations apply -ay --down" },
     { cmd = "cozo-migrate -f cozo.db history" },
     { cmd = "rm -rf cozo.db dummy/migrations" },
 ]
```

### Comparing `cozo_migrate-0.2.3/PKG-INFO` & `cozo_migrate-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: cozo-migrate
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple utility for migrations for cozo db
 License: MIT
 Author: Diwank Singh Tomer
 Author-email: diwank.singh@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.0,<0.6.0)
 Requires-Dist: cozo-embedded (>=0.7.6,<0.8.0)
 Requires-Dist: pandas (>=2.0.0,<2.5.0)
 Requires-Dist: pycozo (>=0.7.6,<0.8.0)
 Requires-Dist: requests (>=2.0.0,<3.0.0)
 Requires-Dist: rich (>=13.0.0,<14.0.0)
 Requires-Dist: shellingham (>=1.4.0,<2.0.0)
@@ -45,21 +46,21 @@
 $ # Let's create a migration
 $ cozo-migrate -e http -d ./migrations create demo
   Writing 'migrations/migrate_1704803704_demo.py' Confirm? [y/N]: y
   ✔ Created migration at: migrations/migrate_1704803704_demo.py
 
 $ cat migrations/migrate_1704803704_demo.py
   #/usr/bin/env python3
-  
+
   MIGRATION_ID = "demo"
   CREATED_AT = 1704803704.762879
-  
+
   def up(client):
       pass
-  
+
   def down(client):
       pass
 
 $ # Edit the migration to add schema change queries and then apply!
 $ cozo-migrate -e http -d ./migrations apply -a
   • Migrate path: [NONE] → demo
   Are you sure you want to apply these migrations? [y/N]: y
@@ -136,14 +137,26 @@
 │ --down                                         │
 │ --all   -a                                     │
 │ --yes   -y                                     │
 │ --help            Show this message and exit.  │
 ╰────────────────────────────────────────────────╯
 ```
 
+#### Show
+
+```bash
+ Usage: cozo-migrate show
+
+ Show the current schema in the database.
+
+╭─ Options ────────────────────────────────────╮
+│ --help          Show this message and exit.  │
+╰──────────────────────────────────────────────╯
+```
+
 #### Status
 
 ```bash
  Usage: cozo-migrate status [OPTIONS]
 
  Display the current migration status.
```

