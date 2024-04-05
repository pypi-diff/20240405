# Comparing `tmp/litestar_users-1.2.2.tar.gz` & `tmp/litestar_users-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar_users-1.2.2.tar", max compression
+gzip compressed data, was "litestar_users-1.2.3.tar", max compression
```

## Comparing `litestar_users-1.2.2.tar` & `litestar_users-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2024-02-13 11:20:28.360218 litestar_users-1.2.2/LICENSE
--rw-r--r--   0        0        0      702 2024-02-13 11:20:28.360218 litestar_users-1.2.2/README.md
--rw-r--r--   0        0        0      136 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/__init__.py
--rw-r--r--   0        0        0     1218 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/adapter/abc.py
--rw-r--r--   0        0        0        0 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/adapter/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1076 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/adapter/sqlalchemy/mixins.py
--rw-r--r--   0        0        0     1292 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/adapter/sqlalchemy/protocols.py
--rw-r--r--   0        0        0     2609 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/adapter/sqlalchemy/repository.py
--rw-r--r--   0        0        0     6261 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/cli.py
--rw-r--r--   0        0        0    13614 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/config.py
--rw-r--r--   0        0        0     1891 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/dependencies.py
--rw-r--r--   0        0        0     2510 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/exceptions.py
--rw-r--r--   0        0        0     1559 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/guards.py
--rw-r--r--   0        0        0     9606 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/main.py
--rw-r--r--   0        0        0     1191 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/password.py
--rw-r--r--   0        0        0     1046 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/protocols.py
--rw-r--r--   0        0        0        0 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/py.typed
--rw-r--r--   0        0        0    15115 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/route_handlers.py
--rw-r--r--   0        0        0      599 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/schema.py
--rw-r--r--   0        0        0    17135 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/service.py
--rw-r--r--   0        0        0     3486 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/user_handlers.py
--rw-r--r--   0        0        0     2601 2024-02-13 11:20:28.360218 litestar_users-1.2.2/litestar_users/utils.py
--rw-r--r--   0        0        0     4552 2024-02-13 11:20:28.364218 litestar_users-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1511 1970-01-01 00:00:00.000000 litestar_users-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-05 12:07:31.045598 litestar_users-1.2.3/LICENSE
+-rw-r--r--   0        0        0      702 2024-04-05 12:07:31.045598 litestar_users-1.2.3/README.md
+-rw-r--r--   0        0        0      136 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/__init__.py
+-rw-r--r--   0        0        0     1218 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/adapter/abc.py
+-rw-r--r--   0        0        0        0 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/adapter/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/adapter/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0     1292 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/adapter/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0     2609 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/adapter/sqlalchemy/repository.py
+-rw-r--r--   0        0        0     6261 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/cli.py
+-rw-r--r--   0        0        0    13614 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/config.py
+-rw-r--r--   0        0        0     1891 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/dependencies.py
+-rw-r--r--   0        0        0     2510 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/exceptions.py
+-rw-r--r--   0        0        0     1559 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/guards.py
+-rw-r--r--   0        0        0     9606 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/main.py
+-rw-r--r--   0        0        0     1191 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/password.py
+-rw-r--r--   0        0        0     1046 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/protocols.py
+-rw-r--r--   0        0        0        0 2024-04-05 12:07:31.045598 litestar_users-1.2.3/litestar_users/py.typed
+-rw-r--r--   0        0        0    15115 2024-04-05 12:07:31.049598 litestar_users-1.2.3/litestar_users/route_handlers.py
+-rw-r--r--   0        0        0      599 2024-04-05 12:07:31.049598 litestar_users-1.2.3/litestar_users/schema.py
+-rw-r--r--   0        0        0    17135 2024-04-05 12:07:31.049598 litestar_users-1.2.3/litestar_users/service.py
+-rw-r--r--   0        0        0     3635 2024-04-05 12:07:31.049598 litestar_users-1.2.3/litestar_users/user_handlers.py
+-rw-r--r--   0        0        0     2601 2024-04-05 12:07:31.049598 litestar_users-1.2.3/litestar_users/utils.py
+-rw-r--r--   0        0        0     4552 2024-04-05 12:07:31.049598 litestar_users-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1511 1970-01-01 00:00:00.000000 litestar_users-1.2.3/PKG-INFO
```

### Comparing `litestar_users-1.2.2/LICENSE` & `litestar_users-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/README.md` & `litestar_users-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/adapter/abc.py` & `litestar_users-1.2.3/litestar_users/adapter/abc.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/adapter/sqlalchemy/mixins.py` & `litestar_users-1.2.3/litestar_users/adapter/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/adapter/sqlalchemy/protocols.py` & `litestar_users-1.2.3/litestar_users/adapter/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/adapter/sqlalchemy/repository.py` & `litestar_users-1.2.3/litestar_users/adapter/sqlalchemy/repository.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/cli.py` & `litestar_users-1.2.3/litestar_users/cli.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/config.py` & `litestar_users-1.2.3/litestar_users/config.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/dependencies.py` & `litestar_users-1.2.3/litestar_users/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/exceptions.py` & `litestar_users-1.2.3/litestar_users/exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/guards.py` & `litestar_users-1.2.3/litestar_users/guards.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/main.py` & `litestar_users-1.2.3/litestar_users/main.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/password.py` & `litestar_users-1.2.3/litestar_users/password.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/protocols.py` & `litestar_users-1.2.3/litestar_users/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/route_handlers.py` & `litestar_users-1.2.3/litestar_users/route_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/schema.py` & `litestar_users-1.2.3/litestar_users/schema.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/service.py` & `litestar_users-1.2.3/litestar_users/service.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/litestar_users/user_handlers.py` & `litestar_users-1.2.3/litestar_users/user_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,13 +74,18 @@
         token: Encoded JWT.
         connection: The ASGI connection.
     """
     repository = _get_user_repository(connection)
     try:
         # undocumented relationship loading api
         statement = _check_update_statement(connection, repository.statement)
-        user = await repository.get(UUID(token.sub), statement=statement)
+        user_id: UUID | int | None = None
+        try:
+            user_id = UUID(token.sub)
+        except ValueError:
+            user_id = int(token.sub)
+        user = await repository.get(user_id, statement=statement)
         if user.is_active and user.is_verified:
             return user  # type: ignore[no-any-return]
     except NotFoundError:
         pass
     return None
```

### Comparing `litestar_users-1.2.2/litestar_users/utils.py` & `litestar_users-1.2.3/litestar_users/utils.py`

 * *Files identical despite different names*

### Comparing `litestar_users-1.2.2/pyproject.toml` & `litestar_users-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar-users"
-version = "1.2.2"
+version = "1.2.3"
 description = "Authentication and user management for Litestar"
 authors = ["Michael Bosch <michael@lonelyviking.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "litestar_users"}]
 
 [tool.poetry.dependencies]
```

### Comparing `litestar_users-1.2.2/PKG-INFO` & `litestar_users-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar-users
-Version: 1.2.2
+Version: 1.2.3
 Summary: Authentication and user management for Litestar
 License: MIT
 Author: Michael Bosch
 Author-email: michael@lonelyviking.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

