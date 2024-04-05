# Comparing `tmp/nrp-invenio-client-0.1.0.tar.gz` & `tmp/nrp-invenio-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrp-invenio-client-0.1.0.tar", last modified: Thu Mar 14 20:05:32 2024, max compression
+gzip compressed data, was "nrp-invenio-client-0.2.0.tar", last modified: Fri Apr  5 05:42:46 2024, max compression
```

## Comparing `nrp-invenio-client-0.1.0.tar` & `nrp-invenio-client-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:05:32.265423 nrp-invenio-client-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-14 20:05:32.265423 nrp-invenio-client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 20:05:32.265423 nrp-invenio-client-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:05:32.257423 nrp-invenio-client-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:05:32.261423 nrp-invenio-client-0.1.0/src/nrp_invenio_client/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:05:32.261423 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:05:32.265423 nrp-invenio-client-0.1.0/src/nrp_invenio_client/config/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/config/repository_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-14 20:04:29.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:05:32.265423 nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-14 20:05:32.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-14 20:05:32.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 20:05:32.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-14 20:05:32.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-14 20:05:32.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 20:05:32.000000 nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:46.568403 nrp-invenio-client-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 05:42:46.568403 nrp-invenio-client-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 05:42:46.568403 nrp-invenio-client-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:46.560403 nrp-invenio-client-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:46.564403 nrp-invenio-client-0.2.0/src/nrp_invenio_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:46.568403 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:46.568403 nrp-invenio-client-0.2.0/src/nrp_invenio_client/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/config/repository_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-05 05:41:48.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:46.568403 nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 05:42:46.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-05 05:42:46.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 05:42:46.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 05:42:46.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 05:42:46.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 05:42:46.000000 nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/top_level.txt
```

### Comparing `nrp-invenio-client-0.1.0/PKG-INFO` & `nrp-invenio-client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrp-invenio-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python and commandline client for NRP Invenio API
 Author-email: Mirek Simek <miroslav.simek@cesnet.cz>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: click>=8.1.7
 Requires-Dist: dacite>=1.8.1
```

### Comparing `nrp-invenio-client-0.1.0/README.md` & `nrp-invenio-client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nrp-invenio-client-0.1.0/pyproject.toml` & `nrp-invenio-client-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nrp-invenio-client"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python and commandline client for NRP Invenio API"
 authors = [
     {name = "Mirek Simek", email = "miroslav.simek@cesnet.cz"},
 ]
 dependencies = [
     "click>=8.1.7",
     "dacite>=1.8.1",
@@ -18,11 +18,12 @@
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "MIT"}
 
 [tool.pdm.dev-dependencies]
 dev = [
     "nuitka>=2.0",
+    "pydoc-markdown>=4.8.2",
 ]
 
 [project.scripts]
 nrp-cmd = "nrp_invenio_client.cli:nrp_command"
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/base.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     NRPInvenioClientInvalidContentTypeError,
     NRPInvenioClientNotFoundError,
     NRPInvenioClientServerBusyError,
 )
 from nrp_invenio_client.info import NRPInfoApi
 from nrp_invenio_client.records import NRPRecordsApi
 from nrp_invenio_client.search import NRPSearchRequest, NRPSearchResponse
-from nrp_invenio_client.tokens import NRPTokensApi
 
 JSON: TypeAlias = dict[str, "JSON"] | list["JSON"] | str | int | float | bool | None
 
 
 class ResponseFormat(Enum):
     JSON = "json"
     "The response is expected to be JSON"
@@ -124,15 +123,15 @@
             ),
             retry_interval=int(
                 os.environ.get(
                     "NRP_INVENIO_CLIENT_RETRY_INTERVAL",
                     repository_config.retry_interval,
                 )
             ),
-            repository_config = repository_config
+            repository_config=repository_config,
         )
 
     @property
     def repository_config(self):
         return self._repository_config
 
     #
@@ -142,18 +141,14 @@
     def info(self) -> NRPInfoApi:
         return NRPInfoApi(self)
 
     @cached_property
     def records(self) -> NRPRecordsApi:
         return NRPRecordsApi(self)
 
-    @cached_property
-    def tokens(self) -> NRPTokensApi:
-        return NRPTokensApi(self)
-
     def search_request(
         self,
         models=None,
         page=None,
         size=None,
         order_by=None,
         fields=None,
@@ -308,14 +303,15 @@
                     full_url,
                     f"Server is too busy at url {full_url}, retry after {retry_after} seconds",
                     retry_after,
                 )
             raise
         except:
             import traceback
+
             traceback.print_exc()
             raise
 
     def _decode_response(self, response: httpx.Response, format: ResponseFormat):
         if response.status_code == 204:
             return {}
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/alias.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/alias.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,18 @@
 import urllib.parse
 
 import click
 
 from nrp_invenio_client.config import NRPConfig
 from nrp_invenio_client.config.repository_config import RepositoryConfig
 
-from .base import (
-    add_group,
-    list_group,
-    remove_group,
-    select_group,
-    with_config,
-    with_output_format,
-)
+from .base import with_config, with_output_format
 from .output import print_output
 
 
-@list_group.command(name="aliases")
 @with_output_format()
 @with_config()
 def list_aliases(config: NRPConfig, output_format):
     """
     List known repositories
     """
     click.secho("")
@@ -33,15 +25,14 @@
             "url": repo.url,
         }
         for repo in config.repositories
     ]
     print_output(data, output_format)
 
 
-@add_group.command(name="alias")
 @click.argument("servername")
 @click.argument("alias", required=False)
 @click.option(
     "--default", is_flag=True, default=False, help="Set this repository as the default"
 )
 @click.option(
     "--token",
@@ -109,18 +100,17 @@
     )
     if default:
         config.default_repository = alias
     click.secho(f"Added repository {alias} -> {url}", fg="green")
     config.save()
 
 
-@select_group.command(name="alias")
 @click.argument("alias")
 @with_config()
-def select_repository(config, alias):
+def select_alias(config, alias):
     """
     Select a default repository
     """
     if config.default_repository == alias:
         click.secho(f"Repository {alias} is already selected", fg="yellow")
         return
 
@@ -129,15 +119,14 @@
         return
 
     config.default_repository = alias
     config.save()
     click.secho(f"Repository {alias} selected", fg="green")
 
 
-@remove_group.command(name="alias")
 @click.argument("alias")
 @with_config()
 def remove_alias(config, alias):
     """
     Remove an alias to a repository
     """
     if not any(repo.alias == alias for repo in config.repositories):
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/describe.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/describe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import click
 
-from .base import describe_group, with_config, with_output_format, with_repository
+from .base import with_config, with_output_format, with_repository
 from .output import print_output, print_output_list
 
 
-@describe_group.command(name="repository")
 @with_output_format()
 @with_config()
 @with_repository()
 def describe_repository(*, client, output_format, **kwargs):
     """
     Show information about a repository
     """
     repository_info = client.info.repository
 
     print_output(repository_info.to_dict(), output_format, order={"description": 10})
 
 
-@describe_group.command(name="models")
 @with_output_format()
 @with_config()
 @with_repository()
 @click.argument("alias", required=False)
 def describe_models(*, client, output_format, **kwargs):
     """
     Show information about models within the repository
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/files.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/files.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,214 +1,226 @@
-import re
 import shutil
 import sys
 from pathlib import Path
 
 import click
 from deepmerge import always_merger
 
 from nrp_invenio_client import NRPInvenioClient
-from nrp_invenio_client.cli.base import with_config, with_repository, upload_group, with_output_format, list_group, \
-    download_group, update_group, replace_group, delete_group
-from nrp_invenio_client.cli.output import print_output, print_list_output, print_output_list
+from nrp_invenio_client.cli.base import with_config, with_output_format, with_repository
+from nrp_invenio_client.cli.output import print_output, print_output_list
+from nrp_invenio_client.cli.utils import format_filename
 from nrp_invenio_client.config import NRPConfig
-from nrp_invenio_client.files import NRPFile
 from nrp_invenio_client.records import record_getter
 from nrp_invenio_client.utils import read_input_file
 
 
-@upload_group.command(name="file")
 @click.argument("record_id", required=True)
 @click.argument("filename", required=True)
 @click.argument("metadata", required=False)
 @click.option("--key", help="Key of the file")
 @with_config()
 @with_output_format()
 @with_repository()
 def upload_file(
-    config: NRPConfig, client: NRPInvenioClient, *, record_id, output_format, filename, key, metadata, **kwargs
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    record_id,
+    output_format,
+    filename,
+    key,
+    metadata,
+    **kwargs,
 ):
     record_id = _resolve_record_id(client, record_id)
 
-    rec = record_getter(
-        config, record_id, include_files=True, client=client
-    )
+    rec = record_getter(config, record_id, include_files=True, client=client)
 
     if not key:
-        if filename == '-':
+        if filename == "-":
             click.secho("--key is required when uploading from stdin", fg="red")
             sys.exit(1)
 
         key = Path(filename).name
 
     if key in rec.files:
-        click.secho(f"File with key '{key}' already exists in record '{record_id}'", fg="red")
+        click.secho(
+            f"File with key '{key}' already exists in record '{record_id}'", fg="red"
+        )
         sys.exit(1)
 
     metadata = read_input_file(metadata, "json")
 
-    if filename == '-':
+    if filename == "-":
         stream = click.get_binary_stream("stdin")
     else:
         stream = open(filename, "rb")
     try:
         created_file = rec.files.create(key, metadata, stream)
         print_output(created_file.data, output_format or "yaml")
     finally:
-        if filename != '-':
+        if filename != "-":
             stream.close()
 
 
 def _resolve_record_id(client, record_id):
-    if record_id.startswith('@'):
+    if record_id.startswith("@"):
         record_id = client.repository_config.record_aliases[record_id]
         if isinstance(record_id, list):
-            raise ValueError(f"Alias points to multiple records '{record_id}', please specify the record id directly")
+            raise ValueError(
+                f"Alias points to multiple records '{record_id}', please specify the record id directly"
+            )
     return record_id
 
 
-@list_group.command(name="files")
 @click.argument("record_id", required=True)
 @with_output_format()
 @with_config()
 @with_repository()
 def list_files(
     config: NRPConfig, client: NRPInvenioClient, *, record_id, output_format, **kwargs
 ):
     record_id = _resolve_record_id(client, record_id)
 
-    rec = record_getter(
-        config, record_id, include_files=True, client=client
-    )
+    rec = record_getter(config, record_id, include_files=True, client=client)
     data = [x.to_dict() for x in rec.files.values()]
     print_output_list(data, output_format or "yaml")
 
-@download_group.command(name="file")
+
 @click.argument("record_id", required=True)
 @click.argument("filenames", required=True, nargs=-1)
-@click.option('-o', '--output', help="Output file", default='{key}')
+@click.option("-o", "--output", help="Output file", default="{key}")
 @with_config()
 @with_repository()
-def list_files(
-    config: NRPConfig, client: NRPInvenioClient, *, record_id, filenames, output, **kwargs
+def download_file(
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    record_id,
+    filenames,
+    output,
+    **kwargs,
 ):
     record_id = _resolve_record_id(client, record_id)
 
-    rec = record_getter(
-        config, record_id, include_files=True, client=client
-    )
+    rec = record_getter(config, record_id, include_files=True, client=client)
 
     transformed_filenames = {}
     for filename in filenames:
-        if filename == '*':
+        if filename == "*":
             for file in rec.files.values():
-                transformed_filenames[file.key] = format_filename(output, file)
+                transformed_filenames[file.key] = format_filename(
+                    output, file.to_dict()
+                )
         else:
             file = rec.files.get(filename)
-            transformed_filenames[file.key] = format_filename(output, file)
+            transformed_filenames[file.key] = format_filename(output, file.to_dict())
 
     for k, v in transformed_filenames.items():
         file = rec.files.get(k)
-        if v != '-':
+        if v != "-":
             pth = Path(v)
             pth.parent.mkdir(parents=True, exist_ok=True)
 
         with file.open() as s:
-            if v == '-':
+            if v == "-":
                 shutil.copyfileobj(s, sys.stdout.buffer)
             else:
-                with open(v, 'wb') as f:
+                with open(v, "wb") as f:
                     shutil.copyfileobj(s, f)
 
 
-def format_filename(fmt, f: NRPFile):
-    def sanitize(x):
-        x = str(x)
-        ret = x.replace('/', '_').replace('\\', '_')
-        return re.sub(r'^[./\\]+', '', ret)
-
-    replacements = {
-        k: sanitize(v) for k, v in f.metadata.items()
-    }
-    for k, v in f.metadata.get('metadata', {}).items():
-        replacements[k] = sanitize(v)
-
-    return fmt.format(**replacements)
-
-@update_group.command(name="file")
 @click.argument("record_id", required=True)
 @click.argument("key", required=True)
 @click.argument("metadata", required=False)
-@click.option("--replace", is_flag=True, help="Do not merge in the provided metadata, "
-                                              "replace the metadata")
+@click.option(
+    "--replace",
+    is_flag=True,
+    help="Do not merge in the provided metadata, " "replace the metadata",
+)
 @with_config()
 @with_output_format()
 @with_repository()
 def update_file_metadata(
-    config: NRPConfig, client: NRPInvenioClient, *, record_id, output_format, replace, key, metadata, **kwargs
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    record_id,
+    output_format,
+    replace,
+    key,
+    metadata,
+    **kwargs,
 ):
     record_id = _resolve_record_id(client, record_id)
 
-    rec = record_getter(
-        config, record_id, include_files=True, client=client
-    )
+    rec = record_getter(config, record_id, include_files=True, client=client)
     f = rec.files.get(key)
     if not f:
-        click.secho(f"File with key '{key}' does not exist in record '{record_id}'", fg="red")
+        click.secho(
+            f"File with key '{key}' does not exist in record '{record_id}'", fg="red"
+        )
         sys.exit(1)
 
     metadata = read_input_file(metadata, "json")
     if replace:
         f.metadata.clear()
 
     f.metadata.update(always_merger.merge(f.metadata, metadata))
 
     f.save()
 
     print_output(f.data, output_format or "yaml")
 
 
-@replace_group.command(name="file")
 @click.argument("record_id", required=True)
 @click.argument("key", required=True)
 @click.argument("filename", required=True)
 @with_config()
 @with_output_format()
 @with_repository()
 def replace_file(
-    config: NRPConfig, client: NRPInvenioClient, *, record_id, filename, key, output_format, **kwargs
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    record_id,
+    filename,
+    key,
+    output_format,
+    **kwargs,
 ):
     record_id = _resolve_record_id(client, record_id)
 
-    rec = record_getter(
-        config, record_id, include_files=True, client=client
-    )
+    rec = record_getter(config, record_id, include_files=True, client=client)
 
     f = rec.files.get(key)
     if not f:
-        click.secho(f"File with key '{key}' does not exist in record '{record_id}'", fg="red")
+        click.secho(
+            f"File with key '{key}' does not exist in record '{record_id}'", fg="red"
+        )
         sys.exit(1)
 
     with open(filename, "rb") as stream:
         f.replace(stream)
 
     print_output(f.data, output_format or "yaml")
 
-@delete_group.command(name="file")
+
 @click.argument("record_id", required=True)
 @click.argument("key", required=True)
 @with_config()
 @with_repository()
 def delete_file(
     config: NRPConfig, client: NRPInvenioClient, *, record_id, key, **kwargs
 ):
     record_id = _resolve_record_id(client, record_id)
 
-    rec = record_getter(
-        config, record_id, include_files=True, client=client
-    )
+    rec = record_getter(config, record_id, include_files=True, client=client)
 
     f = rec.files.get(key)
     if not f:
-        click.secho(f"File with key '{key}' does not exist in record '{record_id}'", fg="red")
+        click.secho(
+            f"File with key '{key}' does not exist in record '{record_id}'", fg="red"
+        )
         sys.exit(1)
-    f.delete()
+    f.delete()
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/output.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import json
-from typing import Dict, Iterable, List, Generator, Any
+import sys
+from typing import Any, Dict, Generator, Iterable, List
 
 import yaml
 from tabulate import tabulate
 
 
+# taken from https://stackoverflow.com/a/66853182
+class NoAliasDumper(yaml.SafeDumper):
+    def ignore_aliases(self, data):
+        return True
+
+
 def print_output(
     data: List[Dict] | Dict, output_format="table", order: Dict[str, int] = None
 ):
     if not output_format:
         output_format = "table"
     if isinstance(data, list):
         print_list_output(data, output_format, order or {})
@@ -20,39 +27,57 @@
 
 def print_list_output(
     data: List[Dict], output_format="table", order: Dict[str, int] = None
 ):
     if not output_format:
         output_format = "table"
     if output_format == "json":
-        print(json.dumps(sorted_data(data), indent=4))
+        print(json.dumps(sorted_data(data), indent=4, ensure_ascii=False))
     elif output_format == "yaml":
-        print(yaml.dump(sorted_data(data), sort_keys=False))
+        print(
+            yaml.dump(
+                sorted_data(data),
+                sort_keys=False,
+                Dumper=NoAliasDumper,
+                allow_unicode=True,
+            )
+        )
     elif output_format == "table":
         formatted_table = format_list_to_table(data, order)
         print(formatted_table)
     else:
         raise ValueError(f"Unknown output format: {output_format}")
 
 
 def print_dict_output(
-    data: Dict, output_format: str = "table", order: Dict[str, int] = None
+    data: Dict,
+    output_format: str = "table",
+    order: Dict[str, int] = None,
+    file=sys.stdout,
 ):
     if not output_format:
         output_format = "table"
     if output_format == "json":
-        print(json.dumps(sorted_data(data), indent=4))
+        print(json.dumps(sorted_data(data), indent=4, ensure_ascii=False), file=file)
     elif output_format == "yaml":
-        print(yaml.dump(sorted_data(data), sort_keys=False))
+        print(
+            yaml.dump(
+                sorted_data(data),
+                sort_keys=False,
+                Dumper=NoAliasDumper,
+                allow_unicode=True,
+            ),
+            file=file,
+        )
     elif output_format == "table":
         formatted_table = format_dict_to_table(data, order)
-        print(formatted_table)
+        print(formatted_table, file=file)
     elif output_format == "long":
         formatted_table = format_dict_to_long_table(data, order)
-        print(formatted_table)
+        print(formatted_table, file=file)
     else:
         raise ValueError(f"Unknown output format: {output_format}")
 
 
 def format_dict_to_table(data, order):
     header = list(data.keys())
     sort_header(header, order)
@@ -86,15 +111,17 @@
 def sort_header(header, order):
     if order:
         sort_mapping = {x: order.get(x, idx) for idx, x in enumerate(header)}
 
         header.sort()
 
 
-def print_output_list(data: Iterable[Dict]|Generator[Dict, Any, None], output_format: str):
+def print_output_list(
+    data: Iterable[Dict] | Generator[Dict, Any, None], output_format: str
+):
     if not output_format:
         output_format = "table"
     if output_format == "json":
         print("[")
     for idx, item in enumerate(data):
         if idx > 0:
             if output_format == "json":
@@ -110,8 +137,9 @@
     def key(x):
         return (
             {"mid": 0, "id": 1, "metadata": 100}.get(  # keep the metadata last
                 x[0], 10
             ),
             x[0],
         )
+
     return dict(sorted(data.items(), key=key))
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/search.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import functools
-from typing import Iterator, Any, Generator
+from typing import Any, Generator
 
 import click
 
-from .base import (
-    arg_split,
-    list_group,
-    search_group,
-    with_config,
-    with_output_format,
-    with_repository,
-)
-from .output import print_output, print_output_list
-from .utils import extract_alias
 from ..config import NRPConfig
 from ..records import NRPRecord
+from .base import arg_split, with_config, with_output_format, with_repository
+from .output import print_output, print_output_list
+from .utils import extract_alias
 
 
 def search_decorator(f):
     @with_config()
     @with_output_format()
     @with_repository()
     @click.option(
@@ -61,26 +54,24 @@
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
         return f(*args, **kwargs)
 
     return wrapper
 
 
-@search_group.command(name="records")
 @search_decorator
 def search_records(**kwargs):
     """
     Searches within records. You can either specify just a search query or
     restrict to models of certain type, status (published or draft) or records belonging
     to you.
     """
     internal_search(**kwargs)
 
 
-@list_group.command(name="records")
 @search_decorator
 def list_records(**kwargs):
     """
     Lists records. You can also specify search query or
     restrict the listing to models of certain type,
     status (published or draft) or records belonging to you.
     """
@@ -101,15 +92,17 @@
     published,
     query,
     **kwargs,
 ):
     query, save_to_alias = extract_alias(query)
     if save_to_alias:
         if not client.repository_config:
-            raise click.ClickException("A repository alias must be specified to save the results to an alias.")
+            raise click.ClickException(
+                "A repository alias must be specified to save the results to an alias."
+            )
 
     request = client.search_request(models)
 
     if page is not None:
         request.page(page)
     if size is not None:
         request.size(size)
@@ -120,14 +113,15 @@
     if drafts:
         request.drafts()
     if query is not None:
         request.query(query)
 
     record_aliases = []
     if all_records:
+
         def alias_saver(results: Generator[NRPRecord, Any, None]):
             for res in results:
                 if save_to_alias:
                     record_aliases.append(res.record_id)
                 yield res.to_dict()
 
         with request.scan() as results:
@@ -145,9 +139,7 @@
         )
         if save_to_alias:
             record_aliases.extend(rec.record_id for rec in results)
 
     if save_to_alias:
         client.repository_config.record_aliases[save_to_alias] = record_aliases
     config.save()
-
-
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/cli/set.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,52 @@
 import click
 
 from nrp_invenio_client import NRPInvenioClient
-from nrp_invenio_client.cli.base import with_repository, with_config, set_group, get_group, list_group, \
-    with_output_format, delete_group, remove_group
-from nrp_invenio_client.cli.output import print_output_list, print_output
+from nrp_invenio_client.cli.base import with_config, with_output_format, with_repository
+from nrp_invenio_client.cli.output import print_output
 from nrp_invenio_client.config import NRPConfig
 
 
-@set_group.command(name="variable")
 @click.argument("variable")
 @click.argument("value")
 @with_config()
 @with_repository()
 def set_variable(
     config: NRPConfig, client: NRPInvenioClient, *, variable, value, **kwargs
 ):
     client.repository_config.record_aliases[f"@{variable}"] = value
     config.save()
 
-@get_group.command(name="variable")
+
 @click.argument("variable")
 @click.argument("value")
 @with_config()
 @with_repository()
 def get_variable(
     config: NRPConfig, client: NRPInvenioClient, *, variable, value, **kwargs
 ):
     print(client.repository_config.record_aliases[f"@{variable}"])
 
 
-@list_group.command(name="variables")
 @with_output_format()
 @with_config()
 @with_repository()
 def list_variables(
     config: NRPConfig, client: NRPInvenioClient, *, output_format, **kwargs
 ):
-    if output_format in ('yaml', 'json'):
-        ret = {k[1:]:v for k, v in client.repository_config.record_aliases.items()}
+    if output_format in ("yaml", "json"):
+        ret = {k[1:]: v for k, v in client.repository_config.record_aliases.items()}
         print_output(ret, output_format)
     else:
-        ret = [{
-            'name': k[1:],
-            'value': v
-        } for k, v in client.repository_config.record_aliases.items()]
+        ret = [
+            {"name": k[1:], "value": v}
+            for k, v in client.repository_config.record_aliases.items()
+        ]
         print_output(ret, output_format)
 
 
-@remove_group.command(name="variable")
 @click.argument("variable")
 @with_config()
 @with_repository()
-def delete_variable(
-    config: NRPConfig, client: NRPInvenioClient, *, variable, **kwargs
-):
+def remove_variable(config: NRPConfig, client: NRPInvenioClient, *, variable, **kwargs):
     client.repository_config.record_aliases.pop(f"@{variable}", None)
     config.save()
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/config/config.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/config/config.py`

 * *Files identical despite different names*

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/errors.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/errors.py`

 * *Files identical despite different names*

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/info.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/info.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,86 +2,145 @@
 from functools import cached_property
 
 if typing.TYPE_CHECKING:
     from nrp_invenio_client.base import NRPInvenioClient
 
 
 class NRPModelInfo:
+    """
+    Information about a model in the repository.
+    """
+
     def __init__(self, data: dict):
         self._data = data
 
     @property
     def name(self):
+        """
+        Model name, used in all record's related calls
+        """
         return self._data.get("name")
 
     @property
     def schemas(self):
+        """
+        A list of json schema identifiers that model's records must conform to.
+        """
         return self._data.get("schemas")
 
     @property
     def links(self):
+        """
+        Links to the model's records, etc.
+        """
         return self._data.get("links")
 
     @property
     def description(self):
+        """
+        Human description of the model
+        """
         return self._data.get("description")
 
     @property
     def version(self):
+        """
+        Current model schema version
+        """
         return self._data.get("version")
 
     @property
     def features(self):
+        """
+        A list of features implemented in the model (such as drafts, requests, ...)
+        """
         return self._data.get("features")
 
     @property
     def url(self):
+        """
+        URL of model records
+        """
         return self._data.get("links", {}).get("self")
 
     @property
     def user_url(self):
+        """
+        URL of model records belonging to the logged-in user (the user bearing the token)
+        """
         return self._data.get("links", {}).get("user")
 
     def to_dict(self):
+        """
+        Get a json representation of the model
+        """
         return self._data
 
 
 class NRPRepositoryInfo:
+    """
+    Information about the repository.
+    """
+
     def __init__(self, data: dict):
         self._data = data
 
     @property
     def name(self):
+        """
+        Repository name
+        """
         return self._data.get("name")
 
     @property
     def description(self):
+        """
+        Repository description
+        """
         return self._data.get("description")
 
     @property
     def version(self):
+        """
+        Version of the software of the repository
+        """
         return self._data.get("version")
 
     @property
     def invenio_version(self):
+        """
+        Version of invenio libraries as aggregated in the `oarepo` package.
+        """
         return self._data.get("invenio_version")
 
     @property
     def links(self):
+        """
+        Links to models, ...
+        """
         return self._data.get("links")
 
     @property
     def features(self):
+        """
+        Features of the repository
+        """
         return self._data.get("features")
 
     @property
     def transfers(self):
+        """
+        Enabled binary data transfer types
+        """
         return self._data.get("transfers")
 
     def to_dict(self):
+        """
+        Get a json representation of the repository
+        """
         return self._data
 
 
 class NRPInfoApi:
     """
     Client API for invenio-based NRP repositories.
 
@@ -102,20 +161,27 @@
         """
         Get information about the repository
         """
         return NRPRepositoryInfo(self._api.get(path="/.well-known/repository"))
 
     @cached_property
     def models(self) -> typing.List[NRPModelInfo]:
+        """
+        Get information about the models in the repository
+        """
         return [
             NRPModelInfo(v)
             for v in self._api.get(path="/.well-known/repository/models")
         ]
 
     def get_model(self, model_name: str):
+        """
+        Get information about a specific model in the repository
+        :param model_name: name of the model
+        """
         model_info = next(
             (model for model in self.models if model.name == model_name), None
         )
         if not model_info:
             model_names = ", ".join(model.name for model in self.models)
             raise KeyError(f"Model {model_name} not found, got {model_names}")
         return model_info
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client/records.py` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client/cli/record.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,267 @@
-import typing
-from urllib.parse import urljoin
+import sys
+from pathlib import Path
 
-from nrp_invenio_client.config import NRPConfig
-from nrp_invenio_client.files import NRPFile, NRPRecordFiles
-from nrp_invenio_client.utils import (
-    get_mid,
-    is_doi,
-    is_mid,
-    is_url,
-    resolve_record_doi,
-    resolve_repository_url,
-)
+import click
+from deepmerge import always_merger
 
-if typing.TYPE_CHECKING:
-    from nrp_invenio_client.base import NRPInvenioClient
+from nrp_invenio_client import NRPInvenioClient
+from nrp_invenio_client.cli.base import (
+    handle_http_exceptions,
+    with_config,
+    with_input_format,
+    with_output_format,
+    with_repository,
+)
+from nrp_invenio_client.cli.output import (
+    print_dict_output,
+    print_output,
+    print_output_list,
+)
+from nrp_invenio_client.cli.utils import format_filename
+from nrp_invenio_client.config import NRPConfig
+from nrp_invenio_client.records import record_getter
+from nrp_invenio_client.utils import read_input_file
 
 
-class NRPRecord:
-    def __init__(
-        self,
-        *,
-        client: "NRPInvenioClient",
-        model: str,
-        record_id: typing.Optional[str] = None,
-        data: typing.Optional[dict] = None,
-        files: typing.Optional[dict] = None,
-        requests: typing.Optional[dict] = None,
-    ):
-        self._client = client
-        self._model = model
-        self._record_id = record_id
-        self._data = data
-        self._files = NRPRecordFiles(
-            self,
-            **{
-                metadata["key"]: NRPFile(
-                    record=self, key=metadata["key"], data=metadata
-                )
-                for metadata in (files or [])
-            },
-        )
-        self._requests = requests
-
-    @property
-    def data(self):
-        return self._data
-
-    def to_dict(self):
-        ret = {
-            "mid": self.record_id,
-            **self._data,
-        }
-        if self._files:
-            ret["files"] = self._files.to_dict()
-        if self._requests:
-            ret["requests"] = self._requests
-        return ret
-
-    @property
-    def metadata(self):
-        if not self.data:
-            return {}
-        return self._data.get("metadata", None) or self._data
-
-    @property
-    def files(self):
-        return self._files
-
-    @property
-    def requests(self):
-        return self._requests
-
-    @property
-    def links(self):
-        return self._data["links"]
-
-    @property
-    def record_id(self):
-        if self.links.get('self') == self.links.get('draft'):
-            return f"draft/{self._model}/{self._record_id}"
+@click.option("-o", "--output-file", help="Output file, might use placeholders")
+@click.option(
+    "--files/--no-files",
+    "include_files",
+    help="Add a list of files associated with the record to the output",
+)
+@click.option(
+    "--requests/--no-requests",
+    "include_requests",
+    help="Add a list of requests associated with the record to the output",
+)
+@click.argument("records_ids", nargs=-1, required=True)
+@with_config()
+@with_output_format()
+@with_repository()
+@handle_http_exceptions()
+def get_record(
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    records_ids,
+    output_file,
+    include_files,
+    include_requests,
+    output_format,
+    **kwargs,
+):
+    """
+    Retrieve a single record or a list of records given by id. The id can be of the following form:
+
+    * mid (model/id within model)
+    * id without model together with --model option (or without if there is just a single model inside the repository)
+    * full url (API or HTML)
+    * doi of the record
+    """
+
+    expanded_record_ids = []
+    for record_id in records_ids:
+        if record_id.startswith("@"):
+            record_id_or_ids = client.repository_config.record_aliases[record_id]
+            if isinstance(record_id_or_ids, str):
+                expanded_record_ids.append(record_id_or_ids)
+            else:
+                expanded_record_ids.extend(record_id_or_ids)
         else:
-            return f"{self._model}/{self._record_id}"
+            expanded_record_ids.append(record_id)
+    records_ids = expanded_record_ids
 
-    def clear_data(self):
-        for k in list(self._data.keys()):
-            if k not in ('links', 'parent', 'revision_id', 'id'):
-                del self._data[k]
-
-    def save(self):
-        ret = self._client.put(
-            self.links["self"], data=self.to_dict(),
-            headers={"Content-Type": "application/json",
-                     "If-Match": str(self._data["revision_id"])}
-        )
-        self._data = ret
-
-    def delete(self):
-        return self._client.delete(
-            self.links["self"],
-            headers={}
-        )
-
-    def publish(self):
-        raise NotImplementedError()
-
-    def edit(self):
-        raise NotImplementedError()
-
-    def __str__(self):
-        return f"NRPRecord[{self._model}/{self._record_id}]"
-
-
-class NRPRecordsApi:
-    def __init__(self, api: "NRPInvenioClient"):
-        self._api = api
-
-    def get(
-        self,
-        mid: str | typing.Tuple[str, str],
-        include_files=False,
-        include_requests=False,
-    ) -> NRPRecord:
-        """
-        Returns a record by its id
-
-        :param mid: Either a string mid "model/id within model" or a tuple (model, id within model).
-                    For drafts, the mid is "draft/model/id within model" or tuple
-                    ("draft", model, id within model)
-        :return: The JSON data of the record
-        """
-        if isinstance(mid, str):
-            mid = mid.split("/")
-        elif not isinstance(mid, (tuple, list)):
-            raise ValueError(f"Invalid mid {mid}. Must be either a string or a tuple")
-
-        match len(mid):
-            case 2:
-                prefix = None
-                model, record_id = mid
-            case 3:
-                prefix, model, record_id = mid
-            case _:
-                raise ValueError(
-                    f'Invalid mid tuple {mid}. Must be either (model, id) or ("draft", model, id)'
-                )
-
-        model_info = self._api.info.get_model(model)
-
-        match prefix:
-            case "draft":
-                url = urljoin(model_info.links["api"], f"{record_id}/draft")
-            case None:
-                url = urljoin(model_info.links["api"], record_id)
-            case _:
-                raise ValueError(
-                    f"Invalid prefix {prefix} in \"mid\". Must be either 'draft' or not used at all"
-                )
-
-        metadata = self._api.get(url)
-
-        files = {}
-        if include_files and "files" in metadata["links"]:
-            files = self._api.get(metadata["links"]["files"])["entries"]
-
-        requests = {}
-        if include_requests and "requests" in metadata["links"]:
-            requests = self._api.get(
-                metadata["links"]["requests"], params={"size": 10000}
-            )["hits"]["hits"]
-
-        return NRPRecord(
-            client=self._api,
-            model=model,
-            record_id=record_id,
-            data=metadata,
-            files=files,
-            requests=requests,
-        )
-
-    def create(self, model, metadata):
-        response = self._api.post(
-            self._api.info.get_model(model).links["api"], data=metadata
-        )
-        return NRPRecord(
-            client=self._api, model=model, record_id=response["id"], data=response
-        )
-
-
-def _fetch_by_path(client, api_path, add_files, add_requests) -> NRPRecord:
-    ret = client.get(api_path)
-    files = None
-    requests = None
-    if add_files and "files" in ret["links"]:
-        files = client.get(ret["links"]["files"])["entries"]
-    if add_requests and "requests" in ret["links"]:
-        requests = client.get(ret["links"]["requests"])["hits"]["hits"]
-    model, id = get_mid(client.info.models, ret)
-    return NRPRecord(
-        client=client,
-        model=model,
-        record_id=id,
-        data=ret,
-        files=files,
-        requests=requests,
-    )
-
-
-def record_getter(
-    config: NRPConfig, record_id, include_files=False, include_requests=False, client=None
-) -> NRPRecord:
-    if is_doi(record_id):
-        client_from_doi, api_path = resolve_record_doi(config, record_id)
-        return _fetch_by_path(
-            client_from_doi, api_path, include_files, include_requests
-        )
-    elif is_url(record_id):
-        client_from_url, api_path = resolve_repository_url(config, record_id)
-        return _fetch_by_path(
-            client_from_url, api_path, include_files, include_requests
-        )
-    elif is_mid(record_id):
-        if client is None:
-            client = config.default_repository
-        return client.records.get(
-            mid=record_id,
-            include_files=include_files,
-            include_requests=include_requests,
-        )
-    else:
-        raise ValueError(
-            f"Unknown record id format for '{record_id}'. "
-            "Pass either <model>/<id>, draft/<model>/<id>, API url, UI url or DOI"
-        )
+    for record_id in records_ids:
+        try:
+            rec = record_getter(
+                config, record_id, include_files, include_requests, client=client
+            )
+            if output_file:
+                save_record_to_output_file(rec, output_file, output_format)
+            else:
+                print_output(rec.to_dict(), output_format or "yaml")
+        except ValueError as e:
+            click.secho(str(e), fg="red")
+            raise click.Abort()
+
+
+def save_record_to_output_file(rec, output_file, output_format, saved_data=None):
+    data = rec.to_dict()
+    output_file = format_filename(output_file, data)
+    Path(output_file).parent.mkdir(parents=True, exist_ok=True)
+    with open(output_file, "w") as f:
+        if not output_format:
+            if output_file.endswith(".yaml"):
+                output_format = "yaml"
+            elif output_file.endswith(".json"):
+                output_format = "json"
+            else:
+                output_format = "json"
+        print_dict_output(saved_data or data, output_format, file=f)
+
+
+@click.argument("model")
+@click.argument("data")
+@click.argument("save_to_alias", required=False)
+@with_config()
+@with_input_format()
+@with_repository()
+@handle_http_exceptions()
+def create_record(
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    model,
+    data,
+    input_format,
+    save_to_alias,
+    **kwargs,
+):
+
+    data = read_input_file(data, input_format)
+    rec = client.records.create(model, data)
+    print_output(rec.to_dict(), input_format or "yaml")
+
+    if save_to_alias:
+        client.repository_config.record_aliases[save_to_alias] = rec.record_id
+        config.save()
+
+
+@click.argument("record_id", required=True)
+@click.argument("data", required=True)
+@click.option(
+    "--replace",
+    is_flag=True,
+    help="Do not merge in the provided data, replace the record",
+)
+@with_config()
+@with_input_format()
+@with_repository()
+@handle_http_exceptions()
+def update_record(
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    record_id,
+    data,
+    input_format,
+    replace,
+    **kwargs,
+):
+    data = read_input_file(data, input_format)
+    if record_id.startswith("@"):
+        record_id = client.repository_config.record_aliases[record_id]
+        if isinstance(record_id, list):
+            raise ValueError(
+                f"Alias points to multiple records '{record_id}', please specify the record id directly"
+            )
+
+    rec = record_getter(config, record_id, False, False, client=client)
+    if replace:
+        rec.clear_data()
+
+    rec.data.update(always_merger.merge(rec.data, data))
+    rec.save()
+
+    print_output(rec.to_dict(), input_format or "yaml")
+
+
+@click.argument("record_id", required=True)
+@with_config()
+@with_repository()
+@with_output_format()
+@handle_http_exceptions()
+def validate_record(
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    record_id,
+    output_format,
+    **kwargs,
+):
+    if record_id.startswith("@"):
+        record_id = client.repository_config.record_aliases[record_id]
+        if isinstance(record_id, list):
+            raise ValueError(
+                f"Alias points to multiple records '{record_id}', please specify the record id directly"
+            )
+
+    rec = record_getter(config, record_id, False, False, client=client)
+    rec.save()
+    if rec.errors:
+        print_output_list(rec.errors, output_format or "table")
+        sys.exit(1)
+
+
+@click.argument("record_id", required=True)
+@with_config()
+@with_repository()
+@handle_http_exceptions()
+def delete_record(config: NRPConfig, client: NRPInvenioClient, *, record_id, **kwargs):
+    if record_id.startswith("@"):
+        record_id = client.repository_config.record_aliases[record_id]
+        if isinstance(record_id, list):
+            raise ValueError(
+                f"Alias points to multiple records '{record_id}', please specify the record id directly"
+            )
+
+    rec = record_getter(config, record_id, False, False, client=client)
+    response = rec.delete()
+    print_output(response, "yaml")
+
+
+@click.argument("record_id", required=True)
+@click.argument("version", required=False)
+@with_config()
+@with_repository()
+@with_output_format()
+@handle_http_exceptions()
+def publish_record(
+    config: NRPConfig,
+    client: NRPInvenioClient,
+    *,
+    record_id,
+    version,
+    output_format,
+    **kwargs,
+):
+    variable = None
+    if record_id.startswith("@"):
+        variable = record_id
+        record_id = client.repository_config.record_aliases[record_id]
+        if isinstance(record_id, list):
+            raise ValueError(
+                f"Alias points to multiple records '{record_id}', please specify the record id directly"
+            )
+
+    rec = record_getter(config, record_id, False, False, client=client)
+    published_rec = rec.publish(version=version)
+    if variable:
+        client.repository_config.record_aliases[variable] = published_rec.record_id
+        config.save()
+    print_output(published_rec.to_dict(), output_format or "yaml")
+
+
+@click.argument("record_id", required=True)
+@with_config()
+@with_repository()
+@with_output_format()
+@handle_http_exceptions()
+def edit_record(
+    config: NRPConfig, client: NRPInvenioClient, *, record_id, output_format, **kwargs
+):
+    variable = None
+    if record_id.startswith("@"):
+        variable = record_id
+        record_id = client.repository_config.record_aliases[record_id]
+        if isinstance(record_id, list):
+            raise ValueError(
+                f"Alias points to multiple records '{record_id}', please specify the record id directly"
+            )
+
+    rec = record_getter(config, record_id, False, False, client=client)
+    draft_rec = rec.edit()
+    if variable:
+        client.repository_config.record_aliases[variable] = draft_rec.record_id
+        config.save()
+    print_output(draft_rec.to_dict(), output_format or "yaml")
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/PKG-INFO` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrp-invenio-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python and commandline client for NRP Invenio API
 Author-email: Mirek Simek <miroslav.simek@cesnet.cz>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: click>=8.1.7
 Requires-Dist: dacite>=1.8.1
```

### Comparing `nrp-invenio-client-0.1.0/src/nrp_invenio_client.egg-info/SOURCES.txt` & `nrp-invenio-client-0.2.0/src/nrp_invenio_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 pyproject.toml
 src/nrp_invenio_client/__init__.py
 src/nrp_invenio_client/base.py
 src/nrp_invenio_client/errors.py
 src/nrp_invenio_client/files.py
 src/nrp_invenio_client/info.py
 src/nrp_invenio_client/records.py
+src/nrp_invenio_client/requests.py
 src/nrp_invenio_client/search.py
-src/nrp_invenio_client/tokens.py
 src/nrp_invenio_client/utils.py
 src/nrp_invenio_client.egg-info/PKG-INFO
 src/nrp_invenio_client.egg-info/SOURCES.txt
 src/nrp_invenio_client.egg-info/dependency_links.txt
 src/nrp_invenio_client.egg-info/entry_points.txt
 src/nrp_invenio_client.egg-info/requires.txt
 src/nrp_invenio_client.egg-info/top_level.txt
 src/nrp_invenio_client/cli/__init__.py
 src/nrp_invenio_client/cli/alias.py
 src/nrp_invenio_client/cli/base.py
+src/nrp_invenio_client/cli/commands.py
 src/nrp_invenio_client/cli/describe.py
 src/nrp_invenio_client/cli/files.py
 src/nrp_invenio_client/cli/output.py
 src/nrp_invenio_client/cli/record.py
+src/nrp_invenio_client/cli/requests.py
 src/nrp_invenio_client/cli/search.py
 src/nrp_invenio_client/cli/set.py
 src/nrp_invenio_client/cli/utils.py
 src/nrp_invenio_client/config/__init__.py
 src/nrp_invenio_client/config/config.py
 src/nrp_invenio_client/config/repository_config.py
```

