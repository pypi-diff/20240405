# Comparing `tmp/fleks-2024.4.4.13.29.tar.gz` & `tmp/fleks-2024.4.5.9.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleks-2024.4.4.13.29.tar", last modified: Thu Apr  4 13:29:37 2024, max compression
+gzip compressed data, was "fleks-2024.4.5.9.29.tar", last modified: Fri Apr  5 09:29:16 2024, max compression
```

## Comparing `fleks-2024.4.4.13.29.tar` & `fleks-2024.4.5.9.29.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:29:37.632601 fleks-2024.4.4.13.29/
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-04 13:29:37.632601 fleks-2024.4.4.13.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 13:29:37.632601 fleks-2024.4.4.13.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:29:37.624601 fleks-2024.4.4.13.29/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:29:37.628601 fleks-2024.4.4.13.29/src/fleks/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 13:29:35.000000 fleks-2024.4.4.13.29/src/fleks/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:29:37.628601 fleks-2024.4.4.13.29/src/fleks/app/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:29:37.628601 fleks-2024.4.4.13.29/src/fleks/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-04 13:29:00.000000 fleks-2024.4.4.13.29/src/fleks/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/cli/root_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:29:37.632601 fleks-2024.4.4.13.29/src/fleks/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/meta/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-04 13:29:00.000000 fleks-2024.4.4.13.29/src/fleks/meta/oop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:29:37.632601 fleks-2024.4.4.13.29/src/fleks/util/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/util/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-04 13:29:00.000000 fleks-2024.4.4.13.29/src/fleks/util/lme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-04 13:28:25.000000 fleks-2024.4.4.13.29/src/fleks/util/tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-04 13:29:00.000000 fleks-2024.4.4.13.29/src/fleks/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:29:37.632601 fleks-2024.4.4.13.29/src/fleks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-04 13:29:37.000000 fleks-2024.4.4.13.29/src/fleks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-04 13:29:37.000000 fleks-2024.4.4.13.29/src/fleks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:29:37.000000 fleks-2024.4.4.13.29/src/fleks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:29:37.000000 fleks-2024.4.4.13.29/src/fleks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-04 13:29:37.000000 fleks-2024.4.4.13.29/src/fleks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 13:29:37.000000 fleks-2024.4.4.13.29/src/fleks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.712915 fleks-2024.4.5.9.29/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.716915 fleks-2024.4.5.9.29/src/fleks/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 09:29:14.000000 fleks-2024.4.5.9.29/src/fleks/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.716915 fleks-2024.4.5.9.29/src/fleks/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.716915 fleks-2024.4.5.9.29/src/fleks/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-05 09:28:39.000000 fleks-2024.4.5.9.29/src/fleks/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/cli/root_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/src/fleks/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/meta/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-05 09:28:39.000000 fleks-2024.4.5.9.29/src/fleks/meta/oop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/src/fleks/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-05 09:28:39.000000 fleks-2024.4.5.9.29/src/fleks/util/lme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/util/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-05 09:28:39.000000 fleks-2024.4.5.9.29/src/fleks/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/src/fleks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/top_level.txt
```

### Comparing `fleks-2024.4.4.13.29/PKG-INFO` & `fleks-2024.4.5.9.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleks
-Version: 2024.4.4.13.29
+Version: 2024.4.5.9.29
 Summary: Python application framework
 Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/fleks/
 Project-URL: Source, https://github.com/elo-enterprises/fleks/
 Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fleks Version: 2024.4.4.13.29 Summary: Python
+Metadata-Version: 2.1 Name: fleks Version: 2024.4.5.9.29 Summary: Python
 application framework Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/fleks/ Project-URL: Source, https://github.com/elo-enterprises/
 fleks/ Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
 Platform: any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown Requires-Dist: pydash==7.0.1 Requires-
 Dist: memoized-property==1.0.3 Requires-Dist: pydantic==1.10.11 Requires-Dist:
```

### Comparing `fleks-2024.4.4.13.29/README.md` & `fleks-2024.4.5.9.29/README.md`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/setup.cfg` & `fleks-2024.4.5.9.29/setup.cfg`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/setup.py` & `fleks-2024.4.5.9.29/setup.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/cli/click.py` & `fleks-2024.4.5.9.29/src/fleks/cli/click.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/cli/options.py` & `fleks-2024.4.5.9.29/src/fleks/cli/options.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/cli/root_group.py` & `fleks-2024.4.5.9.29/src/fleks/cli/root_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,15 +71,21 @@
                 ordering = []
                 for o in order:
                     for subc, subh in toplevel["core"]:
                         if subc == o:
                             ordering.append((subc, subh))
                             toplevel["core"].remove((subc, subh))
                 toplevel["core"] = ordering + toplevel["core"]
-                with formatter.section(_(click.style("Core Subcommands", bold=True))):
+                with formatter.section(_(click.style("Top-level", bold=True))):
+                    formatter.write_text(
+                        click.style(
+                            "Core functionality (these names are forbid to plugins)",
+                            dim=True,
+                        )
+                    )
                     formatter.write_dl(toplevel["core"])
             for label in toplevel["plugins"]:
                 cli_description = toplevel["meta"][label]["description"]
                 with formatter.section(_(click.style(f"{label.title()}", bold=True))):
                     if cli_description:
                         formatter.write_text(
                             click.style(f"{cli_description.lstrip()}", dim=True)
```

### Comparing `fleks-2024.4.4.13.29/src/fleks/config.py` & `fleks-2024.4.5.9.29/src/fleks/config.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/meta/namespace.py` & `fleks-2024.4.5.9.29/src/fleks/meta/namespace.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/meta/oop.py` & `fleks-2024.4.5.9.29/src/fleks/meta/oop.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/models.py` & `fleks-2024.4.5.9.29/src/fleks/models.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/plugin.py` & `fleks-2024.4.5.9.29/src/fleks/plugin.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/util/click.py` & `fleks-2024.4.5.9.29/src/fleks/util/click.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/util/lme.py` & `fleks-2024.4.5.9.29/src/fleks/util/lme.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/util/tagging.py` & `fleks-2024.4.5.9.29/src/fleks/util/tagging.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks/util/typing.py` & `fleks-2024.4.5.9.29/src/fleks/util/typing.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.4.13.29/src/fleks.egg-info/PKG-INFO` & `fleks-2024.4.5.9.29/src/fleks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleks
-Version: 2024.4.4.13.29
+Version: 2024.4.5.9.29
 Summary: Python application framework
 Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/fleks/
 Project-URL: Source, https://github.com/elo-enterprises/fleks/
 Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fleks Version: 2024.4.4.13.29 Summary: Python
+Metadata-Version: 2.1 Name: fleks Version: 2024.4.5.9.29 Summary: Python
 application framework Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/fleks/ Project-URL: Source, https://github.com/elo-enterprises/
 fleks/ Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
 Platform: any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown Requires-Dist: pydash==7.0.1 Requires-
 Dist: memoized-property==1.0.3 Requires-Dist: pydantic==1.10.11 Requires-Dist:
```

### Comparing `fleks-2024.4.4.13.29/src/fleks.egg-info/SOURCES.txt` & `fleks-2024.4.5.9.29/src/fleks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

