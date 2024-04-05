# Comparing `tmp/galatasaray-0.1.7.tar.gz` & `tmp/galatasaray-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galatasaray-0.1.7.tar", max compression
+gzip compressed data, was "galatasaray-0.1.8.tar", max compression
```

## Comparing `galatasaray-0.1.7.tar` & `galatasaray-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2024-02-18 22:37:17.410602 galatasaray-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0      346 2024-02-18 22:37:17.410602 galatasaray-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-02-18 22:37:17.418602 galatasaray-0.1.7/galatasaray/__init__.py
--rw-r--r--   0        0        0      126 2024-02-18 22:37:17.418602 galatasaray-0.1.7/galatasaray/__main__.py
--rw-r--r--   0        0        0      253 2024-02-18 22:37:17.418602 galatasaray-0.1.7/galatasaray/cli.py
--rw-r--r--   0        0        0     3509 2024-02-18 22:37:17.418602 galatasaray-0.1.7/galatasaray/scrapper.py
--rw-r--r--   0        0        0     6189 2024-02-18 22:37:17.418602 galatasaray-0.1.7/galatasaray/screen.py
--rw-r--r--   0        0        0     1789 2024-02-18 22:37:17.418602 galatasaray-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 galatasaray-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-05 14:40:49.963051 galatasaray-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0      356 2024-04-05 14:40:49.963051 galatasaray-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 14:40:49.967051 galatasaray-0.1.8/galatasaray/__init__.py
+-rw-r--r--   0        0        0      129 2024-04-05 14:40:49.967051 galatasaray-0.1.8/galatasaray/__main__.py
+-rw-r--r--   0        0        0      620 2024-04-05 14:40:49.967051 galatasaray-0.1.8/galatasaray/cli.py
+-rw-r--r--   0        0        0     4719 2024-04-05 14:40:49.967051 galatasaray-0.1.8/galatasaray/scrapper.py
+-rw-r--r--   0        0        0     6368 2024-04-05 14:40:49.967051 galatasaray-0.1.8/galatasaray/screen.py
+-rw-r--r--   0        0        0     1789 2024-04-05 14:40:49.967051 galatasaray-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 galatasaray-0.1.8/PKG-INFO
```

### Comparing `galatasaray-0.1.7/LICENSE.txt` & `galatasaray-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galatasaray-0.1.7/galatasaray/screen.py` & `galatasaray-0.1.8/galatasaray/screen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from importlib import metadata
 from time import sleep
 
 from rich import box
 from rich.align import Align
 from rich.console import Group
 from rich.layout import Layout
 from rich.live import Live
@@ -10,19 +11,18 @@
 from rich.table import Table
 from rich.text import Text
 
 from galatasaray.scrapper import Scraper
 
 
 class Application:
-    """
-    Main application class
-    """
-
     def __init__(self):
+        """
+        Initialize the application
+        """
         self.scrapper = Scraper()
         self.layout = Layout(name="root")
         self.layout.split(
             Layout(name="header", ratio=3),
             Layout(name="main", ratio=12),
             Layout(name="footer", ratio=1),
         )
@@ -151,14 +151,20 @@
                 title="[cyan][b]GÜNCEL SÖYLENTİLER[/b][/cyan]"
             ),
             box=box.SIMPLE
         )
 
     @staticmethod
     def get_footer():
-        table = Table.grid()
-        table.add_column()
+        table = Table.grid(expand=True)
         table.add_column()
-        table.add_column()
-        table.add_row("quit", ": ", "CTRL + C")
-        table.add_row("credit", ": ", Text("@ozcanyarimdunya", style="link https://yarimdunya.com"))
+        table.add_row(
+            Align.center(
+                Text("ozcanyarimdunya", style="link https://yarimdunya.com") + " @ {}".format(datetime.today().year)
+            )
+        )
+        table.add_row(
+            Align.center(
+                "v{}".format(metadata.version("galatasaray"))
+            )
+        )
         return Panel(table, box=box.SIMPLE)
```

### Comparing `galatasaray-0.1.7/pyproject.toml` & `galatasaray-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galatasaray"
-version = "0.1.7"
+version = "0.1.8"
 description = "Everything about the Galatasaray from cli!"
 authors = ["Ozcan Yarimdunya <ozcanyd@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/ozcanyarimdunya/galatasaray"
 homepage = "https://github.com/ozcanyarimdunya/galatasaray"
 readme = "README.md"
 keywords = ["galatasaray"]
@@ -29,15 +29,15 @@
 packages = [
     { include = "galatasaray" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
-rich = "^13.7.0"
+rich = "^13.7.1"
 beautifulsoup4 = "^4.12.3"
 
 [tool.poetry.group.dev.dependencies]
 portray = "^1.8.0"
 
 [tool.poetry.scripts]
 galatasaray = "galatasaray.cli:main"
```

### Comparing `galatasaray-0.1.7/PKG-INFO` & `galatasaray-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galatasaray
-Version: 0.1.7
+Version: 0.1.8
 Summary: Everything about the Galatasaray from cli!
 Home-page: https://github.com/ozcanyarimdunya/galatasaray
 License: MIT
 Keywords: galatasaray
 Author: Ozcan Yarimdunya
 Author-email: ozcanyd@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -21,28 +21,28 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Project-URL: Repository, https://github.com/ozcanyarimdunya/galatasaray
 Description-Content-Type: text/markdown
 
 # Galatasaray
 
 Everything about the Galatasaray from cli!
 
 ## Installation & Usage on Local
 
 Open your terminal and run:
 
 ```shell
-pip install galatasaray
+pip install --upgrade galatasaray
 ```
 
 ```shell
 galatasaray
 ```
 
 ## Install & Usage with Docker
```

