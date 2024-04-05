# Comparing `tmp/padmy-0.8.2.tar.gz` & `tmp/padmy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "padmy-0.8.2.tar", max compression
+gzip compressed data, was "padmy-0.9.0.tar", max compression
```

## Comparing `padmy-0.8.2.tar` & `padmy-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/__init__.py
--rw-r--r--   0        0        0       36 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/anonymize/__init__.py
--rw-r--r--   0        0        0     3407 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/anonymize/anonymize.py
--rw-r--r--   0        0        0     1232 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/compare.py
--rw-r--r--   0        0        0     2854 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/config.py
--rw-r--r--   0        0        0    13291 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/db.py
--rw-r--r--   0        0        0      557 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/env.py
--rw-r--r--   0        0        0      306 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/logs.py
--rw-r--r--   0        0        0      195 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/migration/__init__.py
--rw-r--r--   0        0        0      632 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/migration/config.py
--rw-r--r--   0        0        0     1842 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/migration/create_files.py
--rw-r--r--   0        0        0      697 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/migration/db.sql
--rw-r--r--   0        0        0     7796 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/migration/migration.py
--rw-r--r--   0        0        0     1085 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/migration/new_sql.py
--rw-r--r--   0        0        0     4882 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/migration/run.py
--rw-r--r--   0        0        0     3862 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/migration/utils.py
--rw-r--r--   0        0        0       53 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/sampling/__init__.py
--rw-r--r--   0        0        0      876 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/sampling/network.py
--rw-r--r--   0        0        0    11487 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/sampling/sampling.py
--rw-r--r--   0        0        0     4181 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/sampling/viz.py
--rw-r--r--   0        0        0    12257 2024-03-29 13:49:17.417580 padmy-0.8.2/padmy/utils.py
--rw-r--r--   0        0        0     1767 2024-03-29 13:49:36.969621 padmy-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 padmy-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/__init__.py
+-rw-r--r--   0        0        0       36 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/anonymize/__init__.py
+-rw-r--r--   0        0        0     3407 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/anonymize/anonymize.py
+-rw-r--r--   0        0        0     1232 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/compare.py
+-rw-r--r--   0        0        0     2854 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/config.py
+-rw-r--r--   0        0        0    13291 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/db.py
+-rw-r--r--   0        0        0      557 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/env.py
+-rw-r--r--   0        0        0      306 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/logs.py
+-rw-r--r--   0        0        0      195 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/migration/__init__.py
+-rw-r--r--   0        0        0      632 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/migration/config.py
+-rw-r--r--   0        0        0     1842 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/migration/create_files.py
+-rw-r--r--   0        0        0      768 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/migration/db.sql
+-rw-r--r--   0        0        0     8008 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/migration/migration.py
+-rw-r--r--   0        0        0     1085 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/migration/new_sql.py
+-rw-r--r--   0        0        0     4882 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/migration/run.py
+-rw-r--r--   0        0        0     3862 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/migration/utils.py
+-rw-r--r--   0        0        0       53 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/sampling/__init__.py
+-rw-r--r--   0        0        0      876 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/sampling/network.py
+-rw-r--r--   0        0        0    11487 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/sampling/sampling.py
+-rw-r--r--   0        0        0     4181 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/sampling/viz.py
+-rw-r--r--   0        0        0    12257 2024-03-29 14:09:54.218954 padmy-0.9.0/padmy/utils.py
+-rw-r--r--   0        0        0     1767 2024-03-29 14:10:13.339130 padmy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 padmy-0.9.0/PKG-INFO
```

### Comparing `padmy-0.8.2/padmy/anonymize/anonymize.py` & `padmy-0.9.0/padmy/anonymize/anonymize.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/compare.py` & `padmy-0.9.0/padmy/compare.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/config.py` & `padmy-0.9.0/padmy/config.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/db.py` & `padmy-0.9.0/padmy/db.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/env.py` & `padmy-0.9.0/padmy/env.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/migration/config.py` & `padmy-0.9.0/padmy/migration/config.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/migration/create_files.py` & `padmy-0.9.0/padmy/migration/create_files.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/migration/db.sql` & `padmy-0.9.0/padmy/migration/db.sql`

 * *Files 8% similar despite different names*

```diff
@@ -20,7 +20,10 @@
     id             serial PRIMARY KEY NOT NULL,
     applied_at     timestamp          NOT NULL DEFAULT now(),
     migration_type MIGRATION_TYPE     NOT NULL,
     file_name      text               NOT NULL,
     file_ts        TIMESTAMP          NOT NULL,
     file_id        varchar(10)        NOT NULL
 );
+
+ALTER TABLE public.migration
+    ADD COLUMN IF NOT EXISTS meta JSONB;
```

### Comparing `padmy-0.8.2/padmy/migration/migration.py` & `padmy-0.9.0/padmy/migration/migration.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 
 
 async def migrate_up(
     conn: Connection,
     folder: Path,
     *,
     nb_migrations: int = -1,
+    metadata: dict | None = None,
 ):
     """Migrate from the latest migration applied available in the database
     to the latest one in the `folder` dir.
     """
     latest_migration = await _get_latest_migration(conn)
     logs.info(f"Latest timestamp: {latest_migration.timestamp}" if latest_migration else "No previous migration found")
     migration_files = get_files(folder)
@@ -200,24 +201,27 @@
                 raise e
             commit_data = {
                 "file_ts": _migration.ts,
                 "file_id": _migration.file_id,
                 "migration_type": "up",
                 "file_name": _migration.path.name,
             }
+            if metadata:
+                commit_data["meta"] = metadata
             await insert_many(conn, "public.migration", [commit_data])
 
     logs.info("Done!")
 
 
 async def migrate_down(
     conn: Connection,
     folder: Path,
     *,
     nb_migrations: int = -1,
+    metadata: dict | None = None,
     # migration_id: str = None
 ):
     """
     Rollback `nb_migrations` back (default -1 for all available)
     """
     latest_migration = await _get_latest_migration(conn)
 
@@ -250,10 +254,12 @@
 
             commit_data = {
                 "file_ts": _rollback.ts,
                 "file_id": _rollback.file_id,
                 "migration_type": "down",
                 "file_name": _rollback.path.name,
             }
+            if metadata:
+                commit_data["meta"] = metadata
             await insert_many(conn, "public.migration", [commit_data])
 
     logs.info("Done!")
```

### Comparing `padmy-0.8.2/padmy/migration/new_sql.py` & `padmy-0.9.0/padmy/migration/new_sql.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/migration/run.py` & `padmy-0.9.0/padmy/migration/run.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/migration/utils.py` & `padmy-0.9.0/padmy/migration/utils.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/sampling/network.py` & `padmy-0.9.0/padmy/sampling/network.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/sampling/sampling.py` & `padmy-0.9.0/padmy/sampling/sampling.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/sampling/viz.py` & `padmy-0.9.0/padmy/sampling/viz.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/padmy/utils.py` & `padmy-0.9.0/padmy/utils.py`

 * *Files identical despite different names*

### Comparing `padmy-0.8.2/pyproject.toml` & `padmy-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "padmy"
-version = "0.8.2"
+version = "0.9.0"
 description = ""
 authors = ["andarius <julien.brayere@tracktor.fr>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 piou = ">=0.13.4,<1.0.0"
 asyncpg = ">=0.28.0"
@@ -51,15 +51,15 @@
 
 [tool.poetry.scripts]
 cli = 'run:run'
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.2"
+version = "0.9.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "release $current_version → $new_version [skip ci]"
```

### Comparing `padmy-0.8.2/PKG-INFO` & `padmy-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: padmy
-Version: 0.8.2
+Version: 0.9.0
 Summary: 
 Author: andarius
 Author-email: julien.brayere@tracktor.fr
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

