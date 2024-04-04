# Comparing `tmp/blackneedles-0.1.1.tar.gz` & `tmp/blackneedles-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackneedles-0.1.1.tar", max compression
+gzip compressed data, was "blackneedles-0.1.2.tar", max compression
```

## Comparing `blackneedles-0.1.1.tar` & `blackneedles-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1648 2024-03-28 23:18:34.656333 blackneedles-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/__init__.py
--rw-r--r--   0        0        0     1017 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/__main__.py
--rw-r--r--   0        0        0        0 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/commands/__init__.py
--rw-r--r--   0        0        0     1994 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/commands/service.py
--rw-r--r--   0        0        0     1952 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/connection.py
--rw-r--r--   0        0        0     1270 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/console.py
--rw-r--r--   0        0        0        0 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/models/__init__.py
--rw-r--r--   0        0        0     3221 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/models/service.py
--rw-r--r--   0        0        0     1371 2024-03-28 23:18:34.656333 blackneedles-0.1.1/blackneedles/procedures/monitoring_procedures.sql
--rw-r--r--   0        0        0      690 2024-03-28 23:18:35.140334 blackneedles-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 blackneedles-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1648 2024-04-04 22:12:45.991319 blackneedles-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/commands/__init__.py
+-rw-r--r--   0        0        0     2016 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/commands/service.py
+-rw-r--r--   0        0        0     1982 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/connection.py
+-rw-r--r--   0        0        0     1301 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/console.py
+-rw-r--r--   0        0        0        0 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/models/__init__.py
+-rw-r--r--   0        0        0     3258 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/models/service.py
+-rw-r--r--   0        0        0     1371 2024-04-04 22:12:45.991319 blackneedles-0.1.2/blackneedles/procedures/monitoring_procedures.sql
+-rw-r--r--   0        0        0      691 2024-04-04 22:12:46.491322 blackneedles-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 blackneedles-0.1.2/PKG-INFO
```

### Comparing `blackneedles-0.1.1/README.md` & `blackneedles-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.1/blackneedles/__main__.py` & `blackneedles-0.1.2/blackneedles/__main__.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.1/blackneedles/commands/service.py` & `blackneedles-0.1.2/blackneedles/commands/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Annotated
+from typing import Annotated, List, Optional
 import typer
 
 from blackneedles.console import print_table
 from blackneedles.models.service import Service
 
 app = typer.Typer()
 
 
 @app.command("list")
 def list_all_services(
     ctx: typer.Context,
     schema: Annotated[
-        str | None, typer.Option(help="The schema to list services from")
+        Optional[str], typer.Option(help="The schema to list services from")
     ] = None,
     compute_pool: Annotated[
-        str | None,
+        Optional[str],
         typer.Option("--compute-pool", help="The compute pool to list services from"),
     ] = None,
 ):
     services = Service.objects.from_namespace(
         {
             "schema_name": schema,
             "compute_pool": compute_pool,
@@ -43,15 +43,15 @@
     )
 
 
 @app.command("describe")
 def describe_service(
     ctx: typer.Context,
     service_names: Annotated[
-        list[str], typer.Argument(..., help="The name of the service to describe")
+        List[str], typer.Argument(..., help="The name of the service to describe")
     ],
 ):
     services = [Service.objects.get(name) for name in service_names]
     print_table(
         ctx,
         services,
         [
```

### Comparing `blackneedles-0.1.1/blackneedles/connection.py` & `blackneedles-0.1.2/blackneedles/connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import configparser
 import os
-from typing import Any, Iterator, Sequence, Type, TypeVar
+from typing import Any, Iterator, Optional, Sequence, Type, TypeVar
 
 from pydantic import BaseModel
 from snowflake.snowpark.row import Row
 from snowflake.snowpark import Session
 from threading import local
 
 threadlocal_data = local()
@@ -36,18 +36,20 @@
 
     @classmethod
     def get_instance(self) -> "Database":
         if not hasattr(threadlocal_data, "database_instance"):
             threadlocal_data.database_instance = Database()
         return threadlocal_data.database_instance
 
-    def get_rows(self, sql: str, params: Sequence[Any] | None = None) -> Iterator[Row]:
+    def get_rows(
+        self, sql: str, params: Optional[Sequence[Any]] = None
+    ) -> Iterator[Row]:
         return self.session.sql(sql, params).collect()
 
     def query(
         self,
         model: Type[AnyModel],
         sql: str,
-        params: Sequence[Any] | None = None,
+        params: Optional[Sequence[Any]] = None,
     ) -> Iterator[AnyModel]:
         for row in self.session.sql(sql, params).collect():
             yield model.model_validate(row.as_dict())
```

### Comparing `blackneedles-0.1.1/blackneedles/console.py` & `blackneedles-0.1.2/blackneedles/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Callable, List
+from typing import Callable, List, Optional, Union
 import typer
 
 from rich.console import Console
 from rich.progress import Progress
 from rich.table import Table
 
 from blackneedles.connection import AnyModel
 
 
 def print_table(
     ctx: typer.Context,
     data: List[AnyModel],
-    attributes: List[str | Callable[[AnyModel], str]],
+    attributes: List[Union[str, Callable[[AnyModel], str], str]],
     headers: List[str],
-    title: str | None = None,
+    title: Optional[str] = None,
 ) -> None:
     with Progress() as progress:
         if ctx.obj.table_style == "rich":
             table = Table(title=title)
             task = progress.add_task("Loading...", total=len(data))
         else:
             table = Table(
```

### Comparing `blackneedles-0.1.1/blackneedles/models/service.py` & `blackneedles-0.1.2/blackneedles/models/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import datetime
 from functools import cached_property
 import json
-from typing import Any, Callable, Iterable
+from typing import Any, Callable, Iterable, Optional
 from pydantic import BaseModel
 
 from blackneedles.connection import Database
 
 
 class Service(BaseModel):
     name: str
     database_name: str
     schema_name: str
     owner: str
     compute_pool: str
-    dns_name: str | None
+    dns_name: Optional[str]
     min_instances: int
     max_instances: int
     auto_resume: bool
     created_on: datetime.datetime
-    updated_on: datetime.datetime | None
-    resumed_on: datetime.datetime | None
-    comment: str | None
-    owner_role_type: str | None
-    query_warehouse: str | None
+    updated_on: Optional[datetime.datetime]
+    resumed_on: Optional[datetime.datetime]
+    comment: Optional[str]
+    owner_role_type: Optional[str]
+    query_warehouse: Optional[str]
     is_job: bool = False
-    spec: str | None = None
+    spec: Optional[str] = None
 
     class Config:
         frozen = True
 
     @property
     def full_name(self):
         return f"{self.schema_name}.{self.name}"
@@ -43,19 +43,19 @@
 
     @full_path.setter
     def full_path(self, value: str):
         self.database_name, self.schema_name, self.name = value.split(".")
 
     @cached_property
     def status(self) -> str:
-        result = next(
+        result = list(
             Database.get_instance().get_rows(
                 "CALL __blackneedles__.check_statuS(?)", (self.full_path,)
             )
-        )
+        )[0]
         return json.loads(result.CHECK_STATUS)[0]["status"]
 
     def alter_status(self, status: str) -> None:
         status = status.upper()
         valid_status = ["SUSPEND", "RESUME"]
         if status not in valid_status:
             raise ValueError(
@@ -65,21 +65,21 @@
             "CALL __blackneedles__.alter_service(?, ?)", (self.full_path, status)
         )
 
     class objects:
         @classmethod
         def get(cls, service_name: str) -> "Service":
             db = Database.get_instance()
-            return next(
+            return list(
                 db.query(
                     Service,
                     "CALL __blackneedles__.describe_service(?);",
                     (service_name,),
                 )
-            )
+            )[0]
 
         @classmethod
         def from_namespace(
             cls,
             filters: dict[str, Any],
         ) -> Iterable["Service"]:
             return cls.filter(
```

### Comparing `blackneedles-0.1.1/blackneedles/procedures/monitoring_procedures.sql` & `blackneedles-0.1.2/blackneedles/procedures/monitoring_procedures.sql`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.1/pyproject.toml` & `blackneedles-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackneedles"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Thiago F Pappacena <pappacena@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 # Note: snowflake-snowpark-python requires <3.12. Fix this once they support 3.12
 python = "^3.8,<3.12"
@@ -23,8 +23,8 @@
 mypy = "^1.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-blackneedles = "blackneedles.__main__:app"
+blackneedles = "blackneedles.__main__:app"
```

### Comparing `blackneedles-0.1.1/PKG-INFO` & `blackneedles-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackneedles
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Thiago F Pappacena
 Author-email: pappacena@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

