# Comparing `tmp/rewire-sqlmodel-0.0.5.tar.gz` & `tmp/rewire-sqlmodel-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire-sqlmodel-0.0.5.tar", last modified: Thu Apr  4 20:12:02 2024, max compression
+gzip compressed data, was "rewire-sqlmodel-0.1.0.tar", last modified: Fri Apr  5 21:10:22 2024, max compression
```

## Comparing `rewire-sqlmodel-0.0.5.tar` & `rewire-sqlmodel-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.130680 rewire-sqlmodel-0.0.5/
--rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2131 2024-04-04 20:12:02.130680 rewire-sqlmodel-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.0.5/README.md
--rw-rw-rw-   0        0        0      812 2024-04-04 20:11:07.000000 rewire-sqlmodel-0.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.110632 rewire-sqlmodel-0.0.5/rewire_sqlmodel/
--rw-rw-rw-   0        0        0    14947 2024-04-04 20:10:45.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.127170 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/
--rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_merge_dev.py
--rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_migrations.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.127170 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/
--rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/env.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.128675 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/versions/
--rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
--rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/fastapi.py
--rw-rw-rw-   0        0        0     2485 2024-02-04 08:52:32.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/tests.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.129682 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/
--rw-rw-rw-   0        0        0     2131 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 20:12:02.130680 rewire-sqlmodel-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.022064 rewire-sqlmodel-0.1.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2131 2024-04-05 21:10:22.022064 rewire-sqlmodel-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.1.0/README.md
+-rw-rw-rw-   0        0        0      812 2024-04-05 20:57:56.000000 rewire-sqlmodel-0.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.010847 rewire-sqlmodel-0.1.0/rewire_sqlmodel/
+-rw-rw-rw-   0        0        0    15704 2024-04-05 21:08:47.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.018063 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/
+-rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_merge_dev.py
+-rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_migrations.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.019062 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/
+-rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/env.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.020062 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/versions/
+-rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
+-rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/fastapi.py
+-rw-rw-rw-   0        0        0     2485 2024-02-04 08:52:32.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.021062 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-04-05 21:10:21.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-05 21:10:22.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 21:10:21.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-05 21:10:21.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-05 21:10:21.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 21:10:22.022064 rewire-sqlmodel-0.1.0/setup.cfg
```

### Comparing `rewire-sqlmodel-0.0.5/LICENSE` & `rewire-sqlmodel-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.5/PKG-INFO` & `rewire-sqlmodel-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.0.5
+Version: 0.1.0
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire-sqlmodel-0.0.5/pyproject.toml` & `rewire-sqlmodel-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire-sqlmodel"
-version = "0.0.5"
+version = "0.1.0"
 description = "Integration of rewire and sqlmodel"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire-sqlmodel-0.0.5/rewire_sqlmodel/__init__.py` & `rewire-sqlmodel-0.1.0/rewire_sqlmodel/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -220,75 +220,98 @@
 
 
 tx_lock = anyio.Lock()
 
 session_context = Context[AsyncSession]()
 
 
-class LazySession:
-    ctx = CTX()
+class ContextSession:
     session: AsyncSession | None = None
-
-    async def start(self):
-        if self.session:
-            return self.session
-        logger.trace("lazy session started")
-        self.session = DependenciesModule.get().resolve(AsyncSessionmaker)()
-        await self.session.__aenter__()
-        return self.session
+    commit_hooks: list[Callable[[], Awaitable]]
+    rollback_hooks: list[Callable[[], Awaitable]]
 
     async def __aenter__(self):
-        if self.ctx.get(None) is not None:
+        if self.session is not None:
+            self.context = session_context.use(self.session)
+            self.context.__enter__()
+            return self
+        lazy = LazySession.ctx.get(None)
+        if lazy is not None:
             self.context = None
-            return
-        self.context = use_context_value(self.ctx, self)
+            session = await lazy.start()
+            return session
+        await self.start()
+        assert self.session is not None
+        self.context = session_context.use(self.session)
         self.context.__enter__()
         return self
 
+    async def start(self):
+        self.session = Dependencies.ctx.get().resolve(AsyncSessionmaker)()
+        self.commit_hooks = []
+        self.rollback_hooks = []
+
     async def __aexit__(self, exc_type, exc_value, trace):
         if not self.context:
             return
         self.context.__exit__(exc_type, exc_value, trace)
-        if not self.session:
+        if self.session is None:
             return
+
         if not exc_type:
-            await self.session.commit()
+            try:
+                await self.session.commit()
+            finally:
+                await self.session.__aexit__(exc_type, exc_value, trace)
+            for hook in self.commit_hooks:
+                await hook()
         else:
-            await self.session.rollback()
+            try:
+                await self.session.rollback()
+            finally:
+                await self.session.__aexit__(exc_type, exc_value, trace)
+            for hook in self.rollback_hooks:
+                await hook()
+
+    async def commit(self):
+        assert self.session is not None
+        await self.session.commit()
+
+    async def rollback(self):
+        assert self.session is not None
+        await self.session.rollback()
 
-        await self.session.__aexit__(exc_type, exc_value, trace)
 
+class LazySession:
+    ctx = CTX()
+    session: ContextSession | None = None
 
-class ContextSession:
-    session: AsyncSession | None = None
+    async def start(self):
+        if self.session:
+            return self.session
+        logger.trace("lazy session started")
+        self.session = ContextSession()
+        await self.session.start()
+        await self.session.__aenter__()
+        return self.session
 
     async def __aenter__(self):
-        lazy = LazySession.ctx.get(None)
-        if lazy is not None:
+        if self.ctx.get(None) is not None:
             self.context = None
-            session = await lazy.start()
-            self.context = session_context.use(session)
-            self.context.__enter__()
             return
-        self.session = Dependencies.ctx.get().resolve(AsyncSessionmaker)()
-        self.context = session_context.use(self.session)
+        self.context = use_context_value(self.ctx, self)
         self.context.__enter__()
         return self
 
     async def __aexit__(self, exc_type, exc_value, trace):
         if not self.context:
             return
         self.context.__exit__(exc_type, exc_value, trace)
-        if self.session is None:
+        if not self.session:
             return
-        if not exc_type:
-            await self.session.commit()
-        else:
-            await self.session.rollback()
-
         await self.session.__aexit__(exc_type, exc_value, trace)
 
 
 class SelectOfScalarExtended[TM](SelectOfScalar[TM]):
     inherit_cache = True
 
     def __await__(self):
```

### Comparing `rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_merge_dev.py` & `rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_merge_dev.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_migrations.py` & `rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_migrations.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/env.py` & `rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/env.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/fastapi.py` & `rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.5/rewire_sqlmodel/tests.py` & `rewire-sqlmodel-0.1.0/rewire_sqlmodel/tests.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/PKG-INFO` & `rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.0.5
+Version: 0.1.0
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

