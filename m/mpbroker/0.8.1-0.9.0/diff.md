# Comparing `tmp/mpbroker-0.8.1.tar.gz` & `tmp/mpbroker-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpbroker-0.8.1.tar", max compression
+gzip compressed data, was "mpbroker-0.9.0.tar", max compression
```

## Comparing `mpbroker-0.8.1.tar` & `mpbroker-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35067 2022-04-21 09:47:13.597689 mpbroker-0.8.1/LICENSE
--rw-r--r--   0        0        0     5315 2022-05-07 11:11:29.175437 mpbroker-0.8.1/README.md
--rw-r--r--   0        0        0       22 2022-04-29 18:06:03.791139 mpbroker-0.8.1/mpbroker/__init__.py
--rw-r--r--   0        0        0       44 2022-04-29 18:06:03.791139 mpbroker-0.8.1/mpbroker/__main__.py
--rw-r--r--   0        0        0        0 2022-04-26 10:06:01.180041 mpbroker-0.8.1/mpbroker/config/__init__.py
--rw-r--r--   0        0        0     2008 2022-05-03 10:04:47.659519 mpbroker-0.8.1/mpbroker/config/config.py
--rw-r--r--   0        0        0     1511 2022-05-05 21:47:20.154898 mpbroker-0.8.1/mpbroker/config/db_init_design_docs.py
--rw-r--r--   0        0        0      814 2022-05-07 11:07:35.023774 mpbroker-0.8.1/mpbroker/config/models.py
--rw-r--r--   0        0        0     1017 2022-05-07 11:06:44.183416 mpbroker-0.8.1/mpbroker/example/user_config.toml
--rw-r--r--   0        0        0    15722 2022-05-09 10:40:51.286638 mpbroker-0.8.1/mpbroker/main.py
--rw-r--r--   0        0        0        0 2022-04-21 11:50:22.897600 mpbroker-0.8.1/mpbroker/models/__init__.py
--rw-r--r--   0        0        0     1708 2022-05-04 10:57:19.337941 mpbroker-0.8.1/mpbroker/models/injest.py
--rw-r--r--   0        0        0     3429 2022-05-05 10:41:17.732115 mpbroker-0.8.1/mpbroker/models/media.py
--rw-r--r--   0        0        0     4795 2022-05-05 10:29:54.722619 mpbroker-0.8.1/mpbroker/tools.py
--rw-r--r--   0        0        0     3291 2022-05-04 10:57:36.678323 mpbroker-0.8.1/mpbroker/utils.py
--rw-r--r--   0        0        0     1124 2022-05-09 10:40:26.103130 mpbroker-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     6435 2022-05-09 10:41:05.219558 mpbroker-0.8.1/setup.py
--rw-r--r--   0        0        0     6458 2022-05-09 10:41:05.220206 mpbroker-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35067 2022-04-21 09:47:13.597689 mpbroker-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5315 2022-05-07 11:11:29.175437 mpbroker-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2022-04-29 18:06:03.791139 mpbroker-0.9.0/mpbroker/__init__.py
+-rw-r--r--   0        0        0       44 2022-04-29 18:06:03.791139 mpbroker-0.9.0/mpbroker/__main__.py
+-rw-r--r--   0        0        0        0 2022-04-26 10:06:01.180041 mpbroker-0.9.0/mpbroker/config/__init__.py
+-rw-r--r--   0        0        0     2008 2022-05-03 10:04:47.659519 mpbroker-0.9.0/mpbroker/config/config.py
+-rw-r--r--   0        0        0     1511 2022-05-05 21:47:20.154898 mpbroker-0.9.0/mpbroker/config/db_init_design_docs.py
+-rw-r--r--   0        0        0      814 2022-05-07 11:07:35.023774 mpbroker-0.9.0/mpbroker/config/models.py
+-rw-r--r--   0        0        0     1017 2022-05-07 11:06:44.183416 mpbroker-0.9.0/mpbroker/example/user_config.toml
+-rw-r--r--   0        0        0    17031 2022-05-10 13:38:40.197327 mpbroker-0.9.0/mpbroker/main.py
+-rw-r--r--   0        0        0        0 2022-04-21 11:50:22.897600 mpbroker-0.9.0/mpbroker/models/__init__.py
+-rw-r--r--   0        0        0     1708 2022-05-04 10:57:19.337941 mpbroker-0.9.0/mpbroker/models/injest.py
+-rw-r--r--   0        0        0     3429 2022-05-05 10:41:17.732115 mpbroker-0.9.0/mpbroker/models/media.py
+-rw-r--r--   0        0        0     4662 2022-05-10 13:15:38.748487 mpbroker-0.9.0/mpbroker/tools.py
+-rw-r--r--   0        0        0     5907 2022-05-10 13:37:53.920369 mpbroker-0.9.0/mpbroker/utils.py
+-rw-r--r--   0        0        0     1124 2022-05-10 12:21:08.088333 mpbroker-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6435 2022-05-10 13:39:06.990675 mpbroker-0.9.0/setup.py
+-rw-r--r--   0        0        0     6458 2022-05-10 13:39:06.991325 mpbroker-0.9.0/PKG-INFO
```

### Comparing `mpbroker-0.8.1/LICENSE` & `mpbroker-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpbroker-0.8.1/README.md` & `mpbroker-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mpbroker-0.8.1/mpbroker/config/config.py` & `mpbroker-0.9.0/mpbroker/config/config.py`

 * *Files identical despite different names*

### Comparing `mpbroker-0.8.1/mpbroker/config/db_init_design_docs.py` & `mpbroker-0.9.0/mpbroker/config/db_init_design_docs.py`

 * *Files identical despite different names*

### Comparing `mpbroker-0.8.1/mpbroker/config/models.py` & `mpbroker-0.9.0/mpbroker/config/models.py`

 * *Files identical despite different names*

### Comparing `mpbroker-0.8.1/mpbroker/example/user_config.toml` & `mpbroker-0.9.0/mpbroker/example/user_config.toml`

 * *Files identical despite different names*

### Comparing `mpbroker-0.8.1/mpbroker/main.py` & `mpbroker-0.9.0/mpbroker/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,26 +13,34 @@
 
 import arrow
 import click
 import pycouchdb
 import requests
 import typer
 import urllib3
+from rich.console import Console
 
 import mpbroker.tools
 from mpbroker.config.config import APP_NAME, APP_VERSION, user_cfg
 from mpbroker.models.injest import InjestLog, InjestLogReason, InjestLogStatus
 from mpbroker.models.media import (
     Media,
     MediaPlay,
     MediaPlayHistory,
     MediaPlayRating,
     MediaPlayStatus,
 )
-from mpbroker.utils import extract_metadata, get_sources_paths, make_doc
+from mpbroker.utils import (
+    db_not_available,
+    extract_metadata,
+    get_sources_paths,
+    make_doc,
+    results_by_name,
+    results_to_table,
+)
 
 # disable InsecureRequestWarnings which come up if you are proxying couchdb through haproxy with ssl termination.
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 server = pycouchdb.Server(user_cfg.database.db_uri)
 app = typer.Typer()
 app.add_typer(mpbroker.tools.app, name="tools")
@@ -132,16 +140,15 @@
         )
         if notes:
             _doc["play"]["notes"] = notes
 
         db.save(_doc)
 
     except requests.exceptions.ConnectionError:
-        typer.echo("Database unavailable, is it up?")
-        raise typer.Exit()
+        db_not_available()
     except pycouchdb.exceptions.NotFound:
         typer.secho(
             f"Media item {name} not found for user {user}.",
             fg=typer.colors.RED,
             bold=True,
         )
         raise typer.Exit()
@@ -156,88 +163,132 @@
         help="user to use for listing",
     ),
 ):
     """
     List media by name.
     """
 
-    from operator import itemgetter
+    table = results_to_table(
+        results_by_name(name=name, user=user), name=name, user=user
+    )
 
-    from natsort import natsorted
-    from rich import box
-    from rich.console import Console
-    from rich.table import Table
+    console = Console()
+    if user_cfg.use_pager:
+        with console.pager(styles=True):
+            console.print(table)
+    else:
+        console.print(table)
 
-    try:
-        db = server.database("media")
 
-        results = db.query(
-            "filters/names",
-            # ~ group='true',
-            # ~ keys=[name],
-            startkey=f"{user}:{name}",
-            endkey=f"{user}:{name}\ufff0",
-            as_list=True,
-            # ~ flat="key"
-        )
+@app.command()
+def update(
+    name: str,
+    user: str = typer.Option(
+        user_cfg.defaults.user,
+        "--user",
+        help="user to use for listing",
+    ),
+):
+    """
+    Update media by name.
+    """
 
-        if results:
-            typer.echo("\n\n")
-            # ~ typer.echo(f"- results: {results}")
-            table = Table(
-                title=f"Results for: '{name}'",
-                title_justify="center",
-                box=box.ROUNDED,
-                show_lines=False,
-                caption=f"Results for: '{name}'",
-                collapse_padding=True,
-                pad_edge=False,
-                padding=0,
-                show_edge=True,
-                leading=0,
-                header_style="bold magenta",
+    try:
+        results = results_by_name(name=name, user=user)
+        table = results_to_table(results, name=name, user=user)
+        console = Console()
+        # NOTE: no pagination for update display.
+        console.print(table)
+
+        typer.confirm("Do you want to continue?", abort=True)
+        _rating_list = [str(i) for i in MediaPlayRating._value2member_map_]
+        _rating_list.append("")
+        _status = None
+
+        if typer.confirm("  Update Status?"):
+            _status = typer.prompt(
+                "    New Status",
+                default=MediaPlayStatus.new,
+                type=click.Choice([str(i) for i in MediaPlayStatus._value2member_map_]),
             )
-            table.add_column("Item", style="cyan", no_wrap=True)
-            table.add_column("Status", justify="center", style="magenta")
-            table.add_column("Rating")
-            table.add_column("Notes")
-            table.add_column("Sources", justify="right", style="yellow")
-            table.add_column("Length")
-
-            # typer.echo(f"- results: {results}")
-            for item in natsorted(results, key=itemgetter(*["id"])):
-                _status = item["value"][1]
-                _rating = f"{item['value'][2]}" if item["value"][2] else ""
-                _rating = (
-                    f"{_rating} {item['value'][3]}" if item["value"][3] else _rating
-                )
-                _notes = f"{item['value'][4]}" if item["value"][4] else ""
-                _duration = f"{item['value'][6]}" if item["value"][6] else ""
-                # ~ typer.echo(f" - {item['value'][0]}/{item['key']} | {_status} {_rating}")
-                _user = f"{user}:"
-                table.add_row(
-                    f"{item['value'][0]}/{item['key'].replace(_user, '')}",
-                    _status,
-                    _rating,
-                    _notes,
-                    f"{', '.join(item['value'][5])}",
-                    _duration,
-                )
-
-            console = Console()
-            if user_cfg.use_pager:
-                with console.pager(styles=True):
-                    console.print(table)
-            else:
-                console.print(table)
-        else:
-            typer.echo("No results found")
+        _update_rating = typer.confirm("  Update Rating?")
+        if _update_rating:
+            _rating = typer.prompt(
+                "    New Rating (blank to clear)",
+                default="",
+                type=click.Choice(_rating_list),
+            )
+        _update_rating_notes = typer.confirm("  Update Rating Notes?")
+        if _update_rating_notes:
+            _rating_notes = typer.prompt(
+                "  New Rating Notes (blank to clear)",
+                default="",
+                show_default=False,
+            )
+        _update_notes = typer.confirm("  Update Notes?")
+        if _update_notes:
+            _notes = typer.prompt(
+                "    New Notes (blank to clear)",
+                default="",
+                show_default=False,
+            )
+        _extract_metadata = typer.confirm("  Extract Metadata for item?")
+        # iterate over docs and update accordingly.
+        _updated = 0
+        db = server.database("media")
+        with typer.progressbar(results) as progress:
+            for item in progress:
+                _doc = db.get(item["id"])
+                _dirty = False
+                if _status:
+                    _doc["play"]["status"] = _status
+                    _dirty = True
+                if _update_rating:
+                    if _rating:
+                        _doc["play"]["rating"] = int(_rating)
+                    else:
+                        _doc["play"]["rating"] = None
+                    _dirty = True
+                if _update_rating_notes:
+                    if _rating_notes:
+                        _doc["play"]["rating_notes"] = _rating_notes
+                    else:
+                        _doc["play"]["rating_notes"] = None
+                    _dirty = True
+                if _update_notes:
+                    if _notes:
+                        _doc["play"]["notes"] = _notes
+                    else:
+                        _doc["play"]["notes"] = None
+                    _dirty = True
+                if _extract_metadata:
+                    _filepath = f"{_doc['base']}{_doc['directory']}/{_doc['name']}"
+                    # ~ typer.echo(f"    ::> {_filepath}")
+                    metadata, error = extract_metadata(_filepath)
+                    _doc["metadata"] = json.loads(metadata.json())
+                    _dirty = True
+                if _dirty:
+                    _updated += 1
+                    _doc["updated"] = datetime.timestamp(datetime.now())
+                    _doc["updator"] = user
+                    db.save(_doc)
+        typer.secho(
+            f"Updated {_updated} Library items!",
+            fg=typer.colors.MAGENTA,
+            bold=True,
+        )
 
     except requests.exceptions.ConnectionError:
-        typer.echo("Database unavailable, is it up?")
+        db_not_available()
+    except pycouchdb.exceptions.NotFound:
+        typer.secho(
+            f"Media item {name} not found for user {user}.",
+            fg=typer.colors.RED,
+            bold=True,
+        )
         raise typer.Exit()
 
 
 @app.command()
 def injest(
     base: str = typer.Option(
         ..., "--base", help="the base path to search for media items to injest"
@@ -317,16 +368,15 @@
         )
         # typer.echo(f"injest_logs info: {_il_status}")
         _rr = []
         for row in _il_status:
             _rr.append(f"\n\t- {row['key'][1]} ({row['key'][2]}): {row['value']}")
 
     except requests.exceptions.ConnectionError:
-        typer.echo("Database unavailable, is it up?")
-        raise typer.Exit()
+        db_not_available()
 
     typer.echo(
         f"""
 ---------- Injest Summary ----------
 Details
 \t- location:        {_base.as_posix()}
 \t- user:            {_user}
@@ -398,16 +448,15 @@
     try:
         db = server.database("media")
         db.save(
             dts
         )  # note: dont use .json() here as it serializes to a string which wont work!
 
     except requests.exceptions.ConnectionError:
-        typer.echo("Database unavailable, is it up?")
-        raise typer.Exit()
+        db_not_available()
     except pycouchdb.exceptions.Conflict:
         _doc = db.get(m.doc_id)
         # set source and check if current matches, if not add.
         if source not in _doc["sources"]:
             _doc["sources"].append(source)
             db.save(_doc)
             # il.status = InjestLogStatus.ok
@@ -421,16 +470,15 @@
     try:
         db = server.database("injest_logs")
         db.save(
             # stopped here, need to get an _id on the il doc somewhere and go...
             make_doc(doc=il, rename_doc_id=False)
         )
     except requests.exceptions.ConnectionError:
-        typer.echo("Database unavailable, is it up?")
-        raise typer.Exit()
+        db_not_available()
 
 
 @app.command()
 def info():
     """
     Show info such as config summary and library stats.
     """
@@ -490,16 +538,15 @@
 \t- Played:  {_played[0]['value'] if _played else 0}
 \t- Watched: {_watched[0]['value'] if _watched else 0}
 \t- Sources: {''.join(_sources_list)}
 """
         )
 
     except requests.exceptions.ConnectionError:
-        typer.echo("Database unavailable, is it up?")
-        raise typer.Exit()
+        db_not_available()
 
 
 def version_callback(value: bool):
     if value:
         typer.echo(f"{APP_NAME} {APP_VERSION}")
 
         raise typer.Exit()
```

### Comparing `mpbroker-0.8.1/mpbroker/models/injest.py` & `mpbroker-0.9.0/mpbroker/models/injest.py`

 * *Files identical despite different names*

### Comparing `mpbroker-0.8.1/mpbroker/models/media.py` & `mpbroker-0.9.0/mpbroker/models/media.py`

 * *Files identical despite different names*

### Comparing `mpbroker-0.8.1/mpbroker/tools.py` & `mpbroker-0.9.0/mpbroker/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 
 import pycouchdb
 import requests
 import typer
 
 from mpbroker.config.config import DATABASES, user_cfg
+from mpbroker.utils import db_not_available
 
 server = pycouchdb.Server(user_cfg.database.db_uri)
 
 app = typer.Typer(help="[Somewhat] useful tools!")
 
 
 @app.command()
@@ -25,16 +26,15 @@
     for db in DATABASES:
         try:
             server.create(db)
             typer.secho(f" ✓ {db} - created", fg=typer.colors.GREEN)
         except pycouchdb.exceptions.Conflict:
             typer.secho(f" ✗ {db} - skipped (already exists)", fg=typer.colors.WHITE)
         except requests.exceptions.ConnectionError:
-            typer.echo("Database unavailable, is it up?")
-            raise typer.Exit()
+            db_not_available()
         except Exception as e:
             typer.secho(
                 f"Other error occurred during create databases: {e}",
                 fg=typer.colors.RED,
                 bold=True,
                 err=True,
             )
@@ -46,18 +46,15 @@
             db = server.database(view[0])
             db.save(view[1])
             typer.secho(
                 f" ✓ {view[0]}/{view[1]['_id']} - created", fg=typer.colors.GREEN
             )
 
     except requests.exceptions.ConnectionError:
-        typer.secho(
-            "Database unavailable, is it up?", fg=typer.colors.RED, bold=True, err=True
-        )
-        raise typer.Exit()
+        db_not_available()
     except pycouchdb.exceptions.Conflict:
         typer.secho(
             f" ✗ {view[0]}/{view[1]['_id']} - skipped (already exists)",
             fg=typer.colors.WHITE,
         )
     except Exception as e:
         typer.secho(
```

### Comparing `mpbroker-0.8.1/pyproject.toml` & `mpbroker-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [internal]
 created = 2022-04-21
 
 [tool.poetry]
 name = "mpbroker"
-version = "0.8.1"
+version = "0.9.0"
 description = "Media Player Broker"
 license = "GPL-3.0-only"
 authors = ["David Rader <sa@adercon.com>"]
 maintainers = ["David Rader <sa@adercon.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/drad/mpbroker"
 repository = "https://gitlab.com/drad/mpbroker"
```

### Comparing `mpbroker-0.8.1/setup.py` & `mpbroker-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'typer[all]>=0.4.1,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['mpb = mpbroker.main:app']}
 
 setup_kwargs = {
     'name': 'mpbroker',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Media Player Broker',
     'long_description': "# README\n\nMedia Player Broker (mpb) is an application that helps you play and track media you have watched over disparet locations. mpb keeps track of what you have played at Location A so when you are at Location B you can see what you have watched from either location to avoid digging through history command output over SSH.\n\nmpb is not a player itself but it can be configured to launch your player of choice to view media.\n\n\n### The Need\n\nRather than living in the cloud I have my videos duplicated at various locations. I needed something that remembers what episode of MacGyver I had watched in one location so when I was in another location I could continue watching the next episode without digging through `history` output or keeping track of what was played where.\n\nmpb consists of a CLI application (the client) and a database (couchdb). From the client you `injest` your media metadata. This extracts the file names from file paths and stores the data in the database. After injesting, you can `list` your media which shows you the media Item, whether it has been watched or not along with a Rating, Notes, and the Sources the item is available at. You can then use the `play` command along with the Item to watch the Item. After playback is completed you are prompted to mark the item as played/watched, Rate it and add Notes - all of which are used in the `list` command to show what you have already watched and what is new.\n\nmpb can also be used by multiple 'users' - you can share a 'user' so your wife can see what you have watched or you can keep separate users so your wife sees what she has watched and you know what you have watched.\n\n\n### Install\n\nWe recommend using [pipx](https://github.com/pypa/pipx) to install mpbroker: `pipx install mpbroker`. You can also install via pip: `pip install --user mpbroker`.\n\nmpbroker uses a config file to store your setup. This file contains information such as your media player, the database url, and types of data to injest. You can grab the sample config file from  [mpbroker/example/user_config.toml](https://gitlab.com/drad/mpbroker/-/blob/master/mpbroker/example/user_config.toml) and place it in a config location. mpbroker searches the following locations for the config file (in order of precedence):\n\n- $MPB_CONFIG_HOME: set this environment variable to any path you like and place the mpbroker `user_config.toml` file in this location\n- $XDG_CONFIG_HOME/mpbroker\n- $APPDATA/mpbroker\n- $HOME/.config/mpbroker\n\n\n### Configure\n\n#### Notices\n- an example `user_config.toml` file can be found in the [project example directory](https://gitlab.com/drad/mpbroker/-/tree/master/mpbroker/example)\n- if you do not want to use the standard locations and do not want to set a `MPB_CONFIG_HOME` envvar you can set `MPB_CONFIG_HOME` on the command line before calling mpb such as `MPB_CONFIG_HOME=/opt/tmp mpb list 'The_Matrix'`\n\nTo set up MPB you need to:\n- create your `user_config.toml` file (see above for locations of this file)\n- configure your user_config.toml file (at a minimum you will need to set/change the `database.db_uri` value)\n- ensure your mpb database is available\n  + use the `db-init` command to initialize your db if it is a new instance!\n\nIf you are testing mpb or do not have a database you can use docker-compose to start a local database with `docker-compose up` from the [project's docker-compose.yml file](https://gitlab.com/drad/mpbroker). If you use the local database your `database.db_uri` would be: `http://admin:couchdb@localhost:5984`\n\n\n### Using MPB\n\nmpb has built in help (`mpb --help`) which should give you enough info to get going.\n\nA Quick Start:\n\n- you will likely want to `injest` some media\n- next you can use `list` to view/find an item to play\n- finally you can `play` an item\n\n#### Paging Output\n\nmpb has pager support, to enable it set the 'use_pager' config option in the user_config.toml file. By default this is not enabled as most pagers drop color support. If you would like pager support and want color to remain in the output you can set the following in your `~/.bashrc` (or equivalent) file:\n\n```\nexport LESS='--RAW-CONTROL-CHARS'\n```\n\nTip: using a pager allows showing one 'page' (screen) of results at a time; however, most pagers (less) also allow searching within the results easily and quickly. We recommend setting the `--RAW-CONTROL-CHARS` and using `less` with mpbroker.\n\n\n### Injestion\n\nInjestion is the process of loading media metadata into your mpbroker database.\n\n#### Extract Metadata\n\nExtracting metadata on injestion increases the injestion time but adds the following data to each injested media item:\n\n    file_size: # filesize in human readable format (569 MiB, 1.1 GiB)\n    file_type: # file type (video/H265)\n    file_format: # file format (Matroska)\n    encoding: # encoding (x265)\n    duration: # duration in human readable format (1 h 52 min, 2 h 48 min)\n    resolution: # resulution in width x height format (720 x 480)\n    aspect_ratio: # display aspect ratio (16:9)\n    audio_format:  audio format (AAC)\n    audio_sampling: audio sample rate (48000)\n\n#### Injestion Time Details\n\n- ~500 videos\n    + with metadata extraction: 6.05s\n    + without metadata extraction: 99.05s\n- 2785 videos\n    + with metadata extraction: 596.53s\n    + without metadata extraction: 72.75s\n",
     'author': 'David Rader',
     'author_email': 'sa@adercon.com',
     'maintainer': 'David Rader',
     'maintainer_email': 'sa@adercon.com',
     'url': 'https://gitlab.com/drad/mpbroker',
```

### Comparing `mpbroker-0.8.1/PKG-INFO` & `mpbroker-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbroker
-Version: 0.8.1
+Version: 0.9.0
 Summary: Media Player Broker
 Home-page: https://gitlab.com/drad/mpbroker
 License: GPL-3.0-only
 Keywords: media player,broker,player,video,smplayer,vlc,couchdb,cli
 Author: David Rader
 Author-email: sa@adercon.com
 Maintainer: David Rader
```

