# Comparing `tmp/razorbill-0.2.7.tar.gz` & `tmp/razorbill-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "razorbill-0.2.7.tar", max compression
+gzip compressed data, was "razorbill-0.2.9.tar", max compression
```

## Comparing `razorbill-0.2.7.tar` & `razorbill-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-10-15 15:36:12.158598 razorbill-0.2.7/LICENSE
--rw-r--r--   0        0        0      108 2023-08-21 10:16:19.500131 razorbill-0.2.7/README.md
--rw-r--r--   0        0        0      716 2024-02-05 07:47:03.701916 razorbill-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-21 10:14:54.840160 razorbill-0.2.7/razorbill/__init__.py
--rw-r--r--   0        0        0      197 2023-08-21 10:16:19.500131 razorbill-0.2.7/razorbill/_types.py
--rw-r--r--   0        0        0     1526 2023-10-19 21:20:16.533077 razorbill-0.2.7/razorbill/builder.py
--rw-r--r--   0        0        0        0 2023-08-10 04:39:52.673740 razorbill-0.2.7/razorbill/connectors/__init__.py
--rw-r--r--   0        0        0        0 2023-09-04 07:03:29.929457 razorbill-0.2.7/razorbill/connectors/alchemy/__init__.py
--rw-r--r--   0        0        0      133 2023-10-19 21:16:19.873139 razorbill-0.2.7/razorbill/connectors/alchemy/_types.py
--rw-r--r--   0        0        0     7037 2024-02-05 07:47:03.701916 razorbill-0.2.7/razorbill/connectors/alchemy/connector.py
--rw-r--r--   0        0        0     1720 2023-10-22 17:51:25.653301 razorbill-0.2.7/razorbill/connectors/alchemy/converter.py
--rw-r--r--   0        0        0      132 2023-10-20 06:06:10.991426 razorbill-0.2.7/razorbill/connectors/alchemy/exceptions.py
--rw-r--r--   0        0        0     1361 2023-10-22 20:53:01.129874 razorbill-0.2.7/razorbill/connectors/alchemy/select.py
--rw-r--r--   0        0        0      213 2023-10-26 16:49:57.526474 razorbill-0.2.7/razorbill/connectors/alchemy/utils.py
--rw-r--r--   0        0        0     1224 2023-10-22 19:57:48.180913 razorbill-0.2.7/razorbill/connectors/base.py
--rw-r--r--   0        0        0     5945 2023-08-30 11:52:59.380888 razorbill-0.2.7/razorbill/connectors/memory.py
--rw-r--r--   0        0        0        0 2023-09-15 10:00:48.672369 razorbill-0.2.7/razorbill/connectors/mongo/__init__.py
--rw-r--r--   0        0        0     7299 2023-09-18 11:28:25.519511 razorbill-0.2.7/razorbill/connectors/mongo/mongo.py
--rw-r--r--   0        0        0     2485 2023-10-15 16:20:13.318330 razorbill-0.2.7/razorbill/connectors/mongo/utils.py
--rw-r--r--   0        0        0     6771 2023-12-01 09:51:08.661398 razorbill-0.2.7/razorbill/crud.py
--rw-r--r--   0        0        0     3145 2023-11-28 12:35:17.754067 razorbill-0.2.7/razorbill/deps.py
--rw-r--r--   0        0        0      605 2023-10-19 17:38:55.506673 razorbill-0.2.7/razorbill/exceptions.py
--rw-r--r--   0        0        0    13161 2023-11-28 12:35:17.754067 razorbill-0.2.7/razorbill/router.py
--rw-r--r--   0        0        0     1565 2023-10-22 21:10:18.059549 razorbill-0.2.7/razorbill/schema.py
--rw-r--r--   0        0        0      999 2023-11-28 12:35:17.754067 razorbill-0.2.7/razorbill/utils.py
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 razorbill-0.2.7/setup.py
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 razorbill-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-10-15 15:36:12.158598 razorbill-0.2.9/LICENSE
+-rw-r--r--   0        0        0      108 2023-08-21 10:16:19.500131 razorbill-0.2.9/README.md
+-rw-r--r--   0        0        0      716 2024-04-05 07:06:18.028708 razorbill-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-21 10:14:54.840160 razorbill-0.2.9/razorbill/__init__.py
+-rw-r--r--   0        0        0      197 2023-08-21 10:16:19.500131 razorbill-0.2.9/razorbill/_types.py
+-rw-r--r--   0        0        0     1526 2023-10-19 21:20:16.533077 razorbill-0.2.9/razorbill/builder.py
+-rw-r--r--   0        0        0        0 2023-08-10 04:39:52.673740 razorbill-0.2.9/razorbill/connectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-04 07:03:29.929457 razorbill-0.2.9/razorbill/connectors/alchemy/__init__.py
+-rw-r--r--   0        0        0      133 2023-10-19 21:16:19.873139 razorbill-0.2.9/razorbill/connectors/alchemy/_types.py
+-rw-r--r--   0        0        0     7198 2024-04-05 07:06:18.028708 razorbill-0.2.9/razorbill/connectors/alchemy/connector.py
+-rw-r--r--   0        0        0     1720 2023-10-22 17:51:25.653301 razorbill-0.2.9/razorbill/connectors/alchemy/converter.py
+-rw-r--r--   0        0        0      132 2023-10-20 06:06:10.991426 razorbill-0.2.9/razorbill/connectors/alchemy/exceptions.py
+-rw-r--r--   0        0        0     1361 2023-10-22 20:53:01.129874 razorbill-0.2.9/razorbill/connectors/alchemy/select.py
+-rw-r--r--   0        0        0      213 2023-10-26 16:49:57.526474 razorbill-0.2.9/razorbill/connectors/alchemy/utils.py
+-rw-r--r--   0        0        0     1224 2023-10-22 19:57:48.180913 razorbill-0.2.9/razorbill/connectors/base.py
+-rw-r--r--   0        0        0     5945 2023-08-30 11:52:59.380888 razorbill-0.2.9/razorbill/connectors/memory.py
+-rw-r--r--   0        0        0        0 2023-09-15 10:00:48.672369 razorbill-0.2.9/razorbill/connectors/mongo/__init__.py
+-rw-r--r--   0        0        0     7299 2023-09-18 11:28:25.519511 razorbill-0.2.9/razorbill/connectors/mongo/mongo.py
+-rw-r--r--   0        0        0     2485 2023-10-15 16:20:13.318330 razorbill-0.2.9/razorbill/connectors/mongo/utils.py
+-rw-r--r--   0        0        0     6771 2023-12-01 09:51:08.661398 razorbill-0.2.9/razorbill/crud.py
+-rw-r--r--   0        0        0     3145 2023-11-28 12:35:17.754067 razorbill-0.2.9/razorbill/deps.py
+-rw-r--r--   0        0        0      605 2023-10-19 17:38:55.506673 razorbill-0.2.9/razorbill/exceptions.py
+-rw-r--r--   0        0        0    13161 2023-11-28 12:35:17.754067 razorbill-0.2.9/razorbill/router.py
+-rw-r--r--   0        0        0     1565 2023-10-22 21:10:18.059549 razorbill-0.2.9/razorbill/schema.py
+-rw-r--r--   0        0        0      999 2023-11-28 12:35:17.754067 razorbill-0.2.9/razorbill/utils.py
+-rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 razorbill-0.2.9/setup.py
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 razorbill-0.2.9/PKG-INFO
```

### Comparing `razorbill-0.2.7/LICENSE` & `razorbill-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/pyproject.toml` & `razorbill-0.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "razorbill"
-version = "0.2.7"
+version = "0.2.9"
 description = "Razorbill is a framework for quickly creating API applications using only the description of the data model."
 authors = ["Nikita Irgashev <nik.irg@yandex.ru>", "Vladislav Vavilov <vladvav94@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-fastapi = "^0.103.0"
+fastapi = "^0.110.1"
 sqlalchemy = "^2.0.17"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 loguru = "^0.7.0"
 psycopg2-binary = "^2.9.7"
 asyncpg = "^0.28.0"
 asyncpgsa = "^0.27.1"
```

### Comparing `razorbill-0.2.7/razorbill/builder.py` & `razorbill-0.2.9/razorbill/builder.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/connectors/alchemy/connector.py` & `razorbill-0.2.9/razorbill/connectors/alchemy/connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,15 +105,18 @@
         
         async with self.session_maker.begin() as session:
             result = await session.execute(statement)
             items = result.scalars().all()
             return [object_to_dict(item) for item in items]
 
     async def get_one(self, obj_id: int, populate: list[str]|None = None) -> dict[str, Any]|None:
-        filters = {self._pk_name: int(obj_id)}
+        try:
+            filters = {self._pk_name: int(obj_id)}
+        except ValueError:
+            return None
         
         statement = build_select_statement(
             self.model, 
             limit=1, 
             filters=filters, 
             populate=populate
         )
@@ -121,19 +124,24 @@
         async with self.session_maker.begin() as session:
             query = await session.execute(statement)
             item = query.scalars().one_or_none()
             return object_to_dict(item) if item else None
 
     async def update_one(self, obj_id: int, obj: dict[str, Any]) -> dict[str, Any] | None:
         pk_column = getattr(self.model, self._pk_name)
+        try:
+            obj_id = int(obj_id)
+        except ValueError:
+            return None
+
         # TODO сделать через один запрос и проверить что update session работает и variable_values нормально сохраняется
         statement = (
             update(self.model)
             .values(obj)
-            .where(self.model.id == int(obj_id))
+            .where(self.model.id == obj_id)
             .execution_options(synchronize_session="fetch")
         )
         try:
             async with self.session_maker.begin() as session:
                 await session.execute(statement)
                 await session.commit()
                 updated_obj = await self.get_one(obj_id)
```

### Comparing `razorbill-0.2.7/razorbill/connectors/alchemy/converter.py` & `razorbill-0.2.9/razorbill/connectors/alchemy/converter.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/connectors/alchemy/select.py` & `razorbill-0.2.9/razorbill/connectors/alchemy/select.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/connectors/base.py` & `razorbill-0.2.9/razorbill/connectors/base.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/connectors/memory.py` & `razorbill-0.2.9/razorbill/connectors/memory.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/connectors/mongo/mongo.py` & `razorbill-0.2.9/razorbill/connectors/mongo/mongo.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/connectors/mongo/utils.py` & `razorbill-0.2.9/razorbill/connectors/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/crud.py` & `razorbill-0.2.9/razorbill/crud.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/deps.py` & `razorbill-0.2.9/razorbill/deps.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/exceptions.py` & `razorbill-0.2.9/razorbill/exceptions.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/router.py` & `razorbill-0.2.9/razorbill/router.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/schema.py` & `razorbill-0.2.9/razorbill/schema.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/razorbill/utils.py` & `razorbill-0.2.9/razorbill/utils.py`

 * *Files identical despite different names*

### Comparing `razorbill-0.2.7/setup.py` & `razorbill-0.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 
 install_requires = \
 ['aiosqlite>=0.19.0,<0.20.0',
  'alembic>=1.12.0,<2.0.0',
  'asyncpg>=0.28.0,<0.29.0',
  'asyncpgsa>=0.27.1,<0.28.0',
  'beanie>=1.21.0,<2.0.0',
- 'fastapi>=0.103.0,<0.104.0',
+ 'fastapi>=0.110.1,<0.111.0',
  'greenlet>=2.0.2,<3.0.0',
  'loguru>=0.7.0,<0.8.0',
  'motor>=3.3.1,<4.0.0',
  'psycopg2-binary>=2.9.7,<3.0.0',
  'pytest-asyncio>=0.21.1,<0.22.0',
  'pytest>=7.4.0,<8.0.0',
  'sqlalchemy>=2.0.17,<3.0.0',
  'uvicorn>=0.23.2,<0.24.0']
 
 setup_kwargs = {
     'name': 'razorbill',
-    'version': '0.2.7',
+    'version': '0.2.9',
     'description': 'Razorbill is a framework for quickly creating API applications using only the description of the data model.',
     'long_description': 'Razorbill is a framework for quickly creating API applications using only the description of the data model.',
     'author': 'Nikita Irgashev',
     'author_email': 'nik.irg@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `razorbill-0.2.7/PKG-INFO` & `razorbill-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: razorbill
-Version: 0.2.7
+Version: 0.2.9
 Summary: Razorbill is a framework for quickly creating API applications using only the description of the data model.
 Author: Nikita Irgashev
 Author-email: nik.irg@yandex.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: alembic (>=1.12.0,<2.0.0)
 Requires-Dist: asyncpg (>=0.28.0,<0.29.0)
 Requires-Dist: asyncpgsa (>=0.27.1,<0.28.0)
 Requires-Dist: beanie (>=1.21.0,<2.0.0)
-Requires-Dist: fastapi (>=0.103.0,<0.104.0)
+Requires-Dist: fastapi (>=0.110.1,<0.111.0)
 Requires-Dist: greenlet (>=2.0.2,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: motor (>=3.3.1,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.7,<3.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0)
 Requires-Dist: sqlalchemy (>=2.0.17,<3.0.0)
```

