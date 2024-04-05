# Comparing `tmp/ibuilder-3.5.0.tar.gz` & `tmp/ibuilder-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibuilder-3.5.0.tar", max compression
+gzip compressed data, was "ibuilder-3.6.0.tar", max compression
```

## Comparing `ibuilder-3.5.0.tar` & `ibuilder-3.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    32471 2022-05-11 12:07:56.761894 ibuilder-3.5.0/LICENSE
--rw-r--r--   0        0        0     5015 2024-01-06 11:58:15.600892 ibuilder-3.5.0/README.md
--rw-r--r--   0        0        0        0 2024-01-06 11:55:51.913157 ibuilder-3.5.0/ibuilder/__init__.py
--rw-r--r--   0        0        0       43 2024-01-06 11:55:51.916490 ibuilder-3.5.0/ibuilder/__main__.py
--rw-r--r--   0        0        0     4231 2024-01-06 11:55:51.919824 ibuilder-3.5.0/ibuilder/config/config.py
--rw-r--r--   0        0        0     2124 2024-01-06 11:55:51.919824 ibuilder-3.5.0/ibuilder/config/models.py
--rwxr-xr-x   0        0        0     5297 2024-01-06 11:55:51.923157 ibuilder-3.5.0/ibuilder/history.py
--rwxr-xr-x   0        0        0     3748 2024-01-06 12:03:11.386576 ibuilder-3.5.0/ibuilder/images.py
--rwxr-xr-x   0        0        0    14135 2024-01-06 12:00:12.107783 ibuilder-3.5.0/ibuilder/main.py
--rw-r--r--   0        0        0     1590 2024-01-06 11:55:51.916490 ibuilder-3.5.0/ibuilder/models.py
--rw-r--r--   0        0        0    15058 2024-01-06 11:55:51.909823 ibuilder-3.5.0/ibuilder/utils.py
--rw-r--r--   0        0        0      891 2024-01-06 11:48:21.879200 ibuilder-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 ibuilder-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2022-05-11 12:07:56.761894 ibuilder-3.6.0/LICENSE
+-rw-r--r--   0        0        0     5130 2024-04-05 09:24:54.705266 ibuilder-3.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-01-06 11:55:51.913157 ibuilder-3.6.0/ibuilder/__init__.py
+-rw-r--r--   0        0        0       43 2024-01-06 11:55:51.916490 ibuilder-3.6.0/ibuilder/__main__.py
+-rw-r--r--   0        0        0     4231 2024-01-06 11:55:51.919824 ibuilder-3.6.0/ibuilder/config/config.py
+-rw-r--r--   0        0        0     2124 2024-04-04 20:37:02.132422 ibuilder-3.6.0/ibuilder/config/models.py
+-rwxr-xr-x   0        0        0     5877 2024-04-05 09:16:29.587532 ibuilder-3.6.0/ibuilder/history.py
+-rwxr-xr-x   0        0        0     3748 2024-01-06 12:03:11.386576 ibuilder-3.6.0/ibuilder/images.py
+-rwxr-xr-x   0        0        0    14079 2024-04-05 09:19:24.556372 ibuilder-3.6.0/ibuilder/main.py
+-rw-r--r--   0        0        0     1564 2024-04-05 09:15:56.066470 ibuilder-3.6.0/ibuilder/models.py
+-rw-r--r--   0        0        0    15058 2024-01-06 11:55:51.909823 ibuilder-3.6.0/ibuilder/utils.py
+-rw-r--r--   0        0        0      890 2024-04-04 18:58:11.184246 ibuilder-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6365 1970-01-01 00:00:00.000000 ibuilder-3.6.0/PKG-INFO
```

### Comparing `ibuilder-3.5.0/LICENSE` & `ibuilder-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibuilder-3.5.0/README.md` & `ibuilder-3.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # README
 
 ibuilder is a [cli](https://en.wikipedia.org/wiki/Command-line_interface) based builder of [docker](https://hub.docker.com/) images. It provides an interface for building and pushing the image, signing images, as well as for tagging source code after build with a build version and other common image tasks.
 
 
 ### Latest Changes
 
-- replaced black, flake8, isort with ruff
-- upgraded packages: idna, pygments, rich, types-python-dateutil, typing-extensions, urllib3, websocket-client
-- add modified [date] to --version & standardize version metadata
+- upgrade to pydantic 2x
+- upgraded packages: docker, packaging, pydantic, rich, typer
+- changed --version to use importlib.metadata
+- removed capturing of sign_logs
+- turned off pretty_exceptions (typer/rich)
 
 
 ### NOTICES
 
-- this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
+- __Next Release Will Require Python 3.11 or Newer__ as we would like to move away from tomllib to address the following:
+  + this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
 
 
 ### Features
 
 - build: build docker images
 - push: push images to any container registry
 - sign: sign images for container signing and verification
```

### Comparing `ibuilder-3.5.0/ibuilder/config/config.py` & `ibuilder-3.6.0/ibuilder/config/config.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.5.0/ibuilder/config/models.py` & `ibuilder-3.6.0/ibuilder/config/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,18 +52,18 @@
 
 
 class PushRegistry(BaseModel):
     """
     Push registry components such as url, username, etc.
     """
 
-    url: str = None
-    username: str = None
-    password: str = None
-    email: str = None
+    url: str | None
+    username: str | None
+    password: str | None
+    email: str | None
 
 
 class Push(BaseModel):
     """
     Push components such as the image, registry, and docker config path.
     """
```

### Comparing `ibuilder-3.5.0/ibuilder/history.py` & `ibuilder-3.6.0/ibuilder/history.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
 #  Copyright 2023 drad <sa@adercon.com>
 
 from pprint import pformat
 
 import arrow
+import logging
 import typer
 from rich import box
 from rich.console import Console
 from rich.table import Table
 from tinydb import where
 
 from ibuilder.config.config import get_db
 from ibuilder.models import HistoryOnDB, ResultStatus
 
+logger_base = logging.getLogger("default")
+logger = logging.LoggerAdapter(logging.getLogger("default"))
+
 app = typer.Typer(help="Interact with build history.")
 
 
 def completed(item):
     return "✓" if item else "✗"
 
 
@@ -39,15 +43,21 @@
     table.add_column("Calling Params")
     table.add_column("B/L/S/P")
     table.add_column("Version")
 
     history = db.table("history").all()
     if history:
         for r in history:
-            h = HistoryOnDB(doc_id=r.doc_id, **r)
+            r['doc_id'] = str(r.doc_id)
+            r['build_logs'] = '' if not 'build_logs' in r else r['build_logs']
+            r['tag_source_logs'] = '' if not 'tag_source_logs' in r else r['tag_source_logs']
+            r['tag_source_push_logs'] = '' if not 'tag_source_push_logs' in r else r['tag_source_push_logs']
+            r['image_push_logs'] = '' if not 'image_push_logs' in r else r['image_push_logs']
+            r['image_push_latest_logs'] = '' if not 'image_push_latest_logs' in r else r['image_push_latest_logs']
+            h = HistoryOnDB(**r)
             blsp = []
             ver = ""
             if h.run_params:
                 blsp.append(completed(h.run_params["build"]["image"]))
                 blsp.append(completed(h.run_params["build"]["tag_image_latest"]))
                 blsp.append(completed(h.run_params["source"]["tag"]))
                 blsp.append(completed(h.run_params["push"]["image"]))
@@ -67,15 +77,16 @@
     return False
 
 
 def history_detail(db, id):
     """Show history detail (all info for a specific history item)."""
 
     r = db.table("history").get(doc_id=id)
-    h = HistoryOnDB(doc_id=r.doc_id, **r)
+    r['doc_id'] = str(id)
+    h = HistoryOnDB(**r)
 
     brief = Table(
         title="History Detail",
         show_header=True,
         show_edge=True,
         show_lines=True,
         header_style="bold magenta",
@@ -122,16 +133,14 @@
         table.add_row("Source Tag", h.tag_source_logs)
     if h.tag_source_push_logs:
         table.add_row("Source Tag Push", h.tag_source_push_logs)
     if h.image_push_logs:
         table.add_row("Push", h.image_push_logs)
     if h.image_push_latest_logs:
         table.add_row("Push Latest", h.image_push_latest_logs)
-    if h.sign_logs:
-        table.add_row("Sign", h.sign_logs)
 
     return brief, table
 
 
 def history_prune(db, result):
     """Remove data from history file by result value."""
```

### Comparing `ibuilder-3.5.0/ibuilder/images.py` & `ibuilder-3.6.0/ibuilder/images.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.5.0/ibuilder/main.py` & `ibuilder-3.6.0/ibuilder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 logger_base = logging.getLogger("default")
 logger_base.setLevel(logging.getLevelName(getenv("LOG_LEVEL", "INFO")))
 logger_base.addHandler(logging.StreamHandler())
 logger = logging.LoggerAdapter(logging.getLogger("default"))
 
 app = typer.Typer(
+    pretty_exceptions_enable=False,
     help="build, tag, and push images\n\nNOTE: set LOG_LEVEL environment variable to adjust logging (e.g. $ LOG_LEVEL=DEBUG ib build -i minor)"
 )
 app.add_typer(ibuilder.history.app, name="history")
 app.add_typer(ibuilder.images.app, name="images")
 
 _prj = None
 _db = None
@@ -252,15 +253,15 @@
         # create and write the history record.
         h = History(
             created=RUNDTS,
             runtime=runtime,
             result=result_status,
             task_status=task_status,
             calling_params=CALLING_PARAMS,
-            run_params=_prj,
+            run_params=vars(_prj),
             build_logs="\n".join(_image_build) if _image_build else "",
             tag_source_logs=_tag_source_logs.stdout
             if _tag_source_logs and _tag_source_logs.stdout
             else "",
             tag_source_push_logs=_tag_source_push_logs.stdout
             if _tag_source_push_logs and _tag_source_push_logs.stdout
             else "",
@@ -339,24 +340,21 @@
 
 def version_callback(value: bool):
     """
     Show version.
     NOTICE: we load the pyproject.toml here (rather than a config) so its not loaded on normal app usage as it is not needed then.
     """
 
-    if value:
-        with open("pyproject.toml", "rb") as f:
-            _meta = tomli.load(f)
-
-        _name = _meta["tool"]["poetry"]["name"]
-        _version = _meta["tool"]["poetry"]["version"]
-        _modified = _meta["internal"]["modified"]
-
-        typer.echo(f"{_name} {_version} ({_modified})")
+    import importlib.metadata
 
+    if value:
+        _meta = importlib.metadata.metadata('ibuilder')
+        _name = _meta["Name"]
+        _version = _meta["Version"]
+        typer.echo(f"{_name} {_version}")
         raise typer.Exit()
 
 
 @app.callback()
 def main(
     version: Optional[bool] = typer.Option(
         None,
```

### Comparing `ibuilder-3.5.0/ibuilder/models.py` & `ibuilder-3.6.0/ibuilder/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,26 +43,25 @@
 
 
 class History(BaseModel):
     """
     History
     """
 
-    created: str = None
-    runtime: float = None
-    result: ResultStatus = None
+    created: str | None
+    runtime: float | None
+    result: ResultStatus | None
     task_status: List[TaskStatus] = []
-    calling_params: str = None
-    run_params: dict = None
-    build_logs: str = None
-    tag_source_logs: str = None
-    tag_source_push_logs: str = None
-    image_push_logs: str = None
-    image_push_latest_logs: str = None
-    sign_logs: str = None
+    calling_params: str | None
+    run_params: dict | None
+    build_logs: str | None
+    tag_source_logs: str | None
+    tag_source_push_logs: str | None
+    image_push_logs: str | None
+    image_push_latest_logs: str | None
     last: bool = False
 
 
 class HistoryOnDB(History):
     """
     Extended History
     """
```

### Comparing `ibuilder-3.5.0/ibuilder/utils.py` & `ibuilder-3.6.0/ibuilder/utils.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.5.0/pyproject.toml` & `ibuilder-3.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [internal]
 created = 2019-06-15
 modified = 2024-01-06
 
 [tool.poetry]
 name = "ibuilder"
-version = "3.5.0"
+version = "3.6.0"
 description = "build, tag, push, and sign docker images"
 authors = ["drad <sa@adercon.com>"]
 maintainers = ["drad <sa@adercon.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://gitlab.com/drad/ibuilder"
 repository = "https://gitlab.com/drad/ibuilder"
@@ -17,21 +17,21 @@
 [tool.poetry.scripts]
 ib = "ibuilder.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 arrow = "^1.3.0"
 click = "^8.1.7"
-docker = "^6.1.3"
-packaging = "^23.2"
-pydantic = "^1.10.13"
+docker = "^7.0.0"
+packaging = "^24.0"
+pydantic = "^2.6.4"
 requests = "^2.31.0"
-rich = "^13.6.0"
+rich = "^13.7.1"
 tinydb = "^4.8.0"
 tomli = "^2.0.1"
-typer = "^0.9.0"
+typer = "^0.12.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ibuilder-3.5.0/PKG-INFO` & `ibuilder-3.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibuilder
-Version: 3.5.0
+Version: 3.6.0
 Summary: build, tag, push, and sign docker images
 Home-page: https://gitlab.com/drad/ibuilder
 License: GPL-3.0-only
 Keywords: cli,docker,containers,build,ci,cd,image,tag,git,push,sign,cosign
 Author: drad
 Author-email: sa@adercon.com
 Maintainer: drad
@@ -15,40 +15,43 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: arrow (>=1.3.0,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: docker (>=6.1.3,<7.0.0)
-Requires-Dist: packaging (>=23.2,<24.0)
-Requires-Dist: pydantic (>=1.10.13,<2.0.0)
+Requires-Dist: docker (>=7.0.0,<8.0.0)
+Requires-Dist: packaging (>=24.0,<25.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.6.0,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.12.0,<0.13.0)
 Project-URL: Repository, https://gitlab.com/drad/ibuilder
 Description-Content-Type: text/markdown
 
 # README
 
 ibuilder is a [cli](https://en.wikipedia.org/wiki/Command-line_interface) based builder of [docker](https://hub.docker.com/) images. It provides an interface for building and pushing the image, signing images, as well as for tagging source code after build with a build version and other common image tasks.
 
 
 ### Latest Changes
 
-- replaced black, flake8, isort with ruff
-- upgraded packages: idna, pygments, rich, types-python-dateutil, typing-extensions, urllib3, websocket-client
-- add modified [date] to --version & standardize version metadata
+- upgrade to pydantic 2x
+- upgraded packages: docker, packaging, pydantic, rich, typer
+- changed --version to use importlib.metadata
+- removed capturing of sign_logs
+- turned off pretty_exceptions (typer/rich)
 
 
 ### NOTICES
 
-- this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
+- __Next Release Will Require Python 3.11 or Newer__ as we would like to move away from tomllib to address the following:
+  + this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
 
 
 ### Features
 
 - build: build docker images
 - push: push images to any container registry
 - sign: sign images for container signing and verification
```

