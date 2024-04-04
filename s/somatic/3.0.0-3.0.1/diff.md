# Comparing `tmp/somatic-3.0.0.tar.gz` & `tmp/somatic-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somatic-3.0.0.tar", last modified: Thu Apr  4 23:17:36 2024, max compression
+gzip compressed data, was "somatic-3.0.1.tar", last modified: Thu Apr  4 23:19:36 2024, max compression
```

## Comparing `somatic-3.0.0.tar` & `somatic-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.202466 somatic-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-04 23:17:36.202466 somatic-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1719 2024-04-04 23:16:29.000000 somatic-3.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     3316 2024-04-04 23:16:39.000000 somatic-3.0.0/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 23:17:36.202466 somatic-3.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/somatic/
--rw-r--r--   0 root         (0) root         (0)      368 2024-04-04 22:59:35.000000 somatic-3.0.0/venues/stages/somatic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/somatic/__license/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/somatic/__license/licenses/
--rw-r--r--   0 root         (0) root         (0)    37279 2023-12-01 20:51:04.000000 somatic-3.0.0/venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html
--rw-r--r--   0 root         (0) root         (0)     2645 2024-04-04 23:16:16.000000 somatic-3.0.0/venues/stages/somatic/_clique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/somatic/_controls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/somatic/_controls/flask/
--rw-rw-r--   0 root         (0) root         (0)     2040 2024-04-04 22:08:21.000000 somatic-3.0.0/venues/stages/somatic/_controls/flask/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/somatic/_controls/sanic/
--rw-rw-r--   0 root         (0) root         (0)     2848 2024-04-04 22:41:36.000000 somatic-3.0.0/venues/stages/somatic/_controls/sanic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/somatic/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.198466 somatic-3.0.0/venues/stages/somatic/_status/checks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.202466 somatic-3.0.0/venues/stages/somatic/_status/checks/1/
--rw-r--r--   0 root         (0) root         (0)      659 2024-04-04 20:52:44.000000 somatic-3.0.0/venues/stages/somatic/_status/checks/1/status_1.py
--rw-r--r--   0 root         (0) root         (0)     1205 2024-04-04 22:05:34.000000 somatic-3.0.0/venues/stages/somatic/_status/status.proc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.202466 somatic-3.0.0/venues/stages/somatic/climate/
--rw-rw-r--   0 root         (0) root         (0)      220 2024-02-14 04:20:52.000000 somatic-3.0.0/venues/stages/somatic/climate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.202466 somatic-3.0.0/venues/stages/somatic/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.202466 somatic-3.0.0/venues/stages/somatic/modules/HTML/
--rw-rw-r--   0 root         (0) root         (0)     3550 2024-04-04 21:54:29.000000 somatic-3.0.0/venues/stages/somatic/modules/HTML/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      553 2024-04-04 20:53:54.000000 somatic-3.0.0/venues/stages/somatic/modules/add_glob_to_paths.py
--rw-rw-r--   0 root         (0) root         (0)      806 2024-02-14 04:20:52.000000 somatic-3.0.0/venues/stages/somatic/modules/parse_extensions.py
--rw-rw-r--   0 root         (0) root         (0)      270 2024-04-04 22:07:22.000000 somatic-3.0.0/venues/stages/somatic/modules/port_in_use.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.202466 somatic-3.0.0/venues/stages/somatic/moves/
--rw-rw-r--   0 root         (0) root         (0)     2761 2024-04-04 23:13:56.000000 somatic-3.0.0/venues/stages/somatic/moves/start.py
--rw-rw-r--   0 root         (0) root         (0)      452 2024-02-14 04:20:52.000000 somatic-3.0.0/venues/stages/somatic/start.proc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:17:36.202466 somatic-3.0.0/venues/stages/somatic.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-04 23:17:36.000000 somatic-3.0.0/venues/stages/somatic.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      932 2024-04-04 23:17:36.000000 somatic-3.0.0/venues/stages/somatic.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-04 23:17:36.000000 somatic-3.0.0/venues/stages/somatic.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       43 2024-04-04 23:17:36.000000 somatic-3.0.0/venues/stages/somatic.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       69 2024-04-04 23:17:36.000000 somatic-3.0.0/venues/stages/somatic.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        8 2024-04-04 23:17:36.000000 somatic-3.0.0/venues/stages/somatic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.597034 somatic-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-04-04 23:19:36.597034 somatic-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1729 2024-04-04 23:19:05.000000 somatic-3.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     3316 2024-04-04 23:16:39.000000 somatic-3.0.1/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 23:19:36.597034 somatic-3.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/stages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/___itinerary/
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-04 23:15:15.000000 somatic-3.0.1/venues/stages/somatic/___itinerary/itinerary.S.HTML
+-rw-rw-r--   0 root         (0) root         (0)      977 2024-04-04 21:52:53.000000 somatic-3.0.1/venues/stages/somatic/___itinerary/possibilities.S.HTML
+-rw-r--r--   0 root         (0) root         (0)      368 2024-04-04 22:59:35.000000 somatic-3.0.1/venues/stages/somatic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/__license/
+-rw-r--r--   0 root         (0) root         (0)      362 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/__license/license.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/__license/licenses/
+-rw-r--r--   0 root         (0) root         (0)    37279 2023-12-01 20:51:04.000000 somatic-3.0.1/venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html
+-rw-r--r--   0 root         (0) root         (0)     2645 2024-04-04 23:16:16.000000 somatic-3.0.1/venues/stages/somatic/_clique.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/stages/somatic/_controls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_controls/flask/
+-rw-rw-r--   0 root         (0) root         (0)     2040 2024-04-04 22:08:21.000000 somatic-3.0.1/venues/stages/somatic/_controls/flask/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_controls/sanic/
+-rw-rw-r--   0 root         (0) root         (0)     2848 2024-04-04 22:41:36.000000 somatic-3.0.1/venues/stages/somatic/_controls/sanic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/stages/somatic/_status/checks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_status/checks/1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_status/checks/1/shares/
+-rw-r--r--   0 root         (0) root         (0)       25 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/_status/checks/1/shares/shares 1.s.HTML
+-rw-r--r--   0 root         (0) root         (0)       25 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/_status/checks/1/shares/shares 2.s.HTML
+-rw-r--r--   0 root         (0) root         (0)      659 2024-04-04 20:52:44.000000 somatic-3.0.1/venues/stages/somatic/_status/checks/1/status_1.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2024-04-04 22:05:34.000000 somatic-3.0.1/venues/stages/somatic/_status/status.proc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/climate/
+-rw-rw-r--   0 root         (0) root         (0)      220 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/climate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2024-03-15 01:31:11.000000 somatic-3.0.1/venues/stages/somatic/module.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/modules/HTML/
+-rw-rw-r--   0 root         (0) root         (0)     3550 2024-04-04 21:54:29.000000 somatic-3.0.1/venues/stages/somatic/modules/HTML/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      553 2024-04-04 20:53:54.000000 somatic-3.0.1/venues/stages/somatic/modules/add_glob_to_paths.py
+-rw-rw-r--   0 root         (0) root         (0)      806 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/modules/parse_extensions.py
+-rw-rw-r--   0 root         (0) root         (0)      270 2024-04-04 22:07:22.000000 somatic-3.0.1/venues/stages/somatic/modules/port_in_use.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/stages/somatic/modules_ES/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/modules_ES/address/
+-rw-r--r--   0 root         (0) root         (0)      524 2024-01-31 20:00:34.000000 somatic-3.0.1/venues/stages/somatic/modules_ES/address/address.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/moves/
+-rw-rw-r--   0 root         (0) root         (0)     2761 2024-04-04 23:13:56.000000 somatic-3.0.1/venues/stages/somatic/moves/start.py
+-rw-rw-r--   0 root         (0) root         (0)      452 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/start.proc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1303 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       43 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)       69 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        8 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/top_level.txt
```

### Comparing `somatic-3.0.0/PKG-INFO` & `somatic-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somatic
-Version: 3.0.0
+Version: 3.0.1
 Summary: The best documentation framework every created.
 License: GPL 3.0
 Project-URL: GitLab, https://gitlab.com/offline-money/squash-1/somatic
 Keywords: documentation
 Description-Content-Type: text/markdown
 Requires-Dist: volts
 Requires-Dist: law_dictionary
```

### Comparing `somatic-3.0.0/pyproject.toml` & `somatic-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "somatic"
-version = "3.0.0"
+version = "3.0.1"
 dependencies = [
 	"volts",
 	"law_dictionary",
 	
 	"clique",
 	"esprima",
 	"flask",
@@ -80,12 +80,12 @@
 [tool.setuptools.packages.find]
 where = [ "venues/stages" ]
 
 #
 #	https://setuptools.pypa.io/en/latest/userguide/datafiles.html
 #
 [tool.setuptools.package-data]
-"*" = [ "*.html" ]
+"*" = [ "*.html", "*.HTML" ]
```

### Comparing `somatic-3.0.0/readme.md` & `somatic-3.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html` & `somatic-3.0.1/venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/_clique.py` & `somatic-3.0.1/venues/stages/somatic/_clique.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/_controls/flask/__init__.py` & `somatic-3.0.1/venues/stages/somatic/_controls/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/_controls/sanic/__init__.py` & `somatic-3.0.1/venues/stages/somatic/_controls/sanic/__init__.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/_status/checks/1/status_1.py` & `somatic-3.0.1/venues/stages/somatic/_status/checks/1/status_1.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/_status/status.proc.py` & `somatic-3.0.1/venues/stages/somatic/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/modules/HTML/__init__.py` & `somatic-3.0.1/venues/stages/somatic/modules/HTML/__init__.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/modules/add_glob_to_paths.py` & `somatic-3.0.1/venues/stages/somatic/modules/add_glob_to_paths.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/modules/parse_extensions.py` & `somatic-3.0.1/venues/stages/somatic/modules/parse_extensions.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic/moves/start.py` & `somatic-3.0.1/venues/stages/somatic/moves/start.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.0/venues/stages/somatic.egg-info/PKG-INFO` & `somatic-3.0.1/venues/stages/somatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somatic
-Version: 3.0.0
+Version: 3.0.1
 Summary: The best documentation framework every created.
 License: GPL 3.0
 Project-URL: GitLab, https://gitlab.com/offline-money/squash-1/somatic
 Keywords: documentation
 Description-Content-Type: text/markdown
 Requires-Dist: volts
 Requires-Dist: law_dictionary
```

### Comparing `somatic-3.0.0/venues/stages/somatic.egg-info/SOURCES.txt` & `somatic-3.0.1/venues/stages/somatic.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 pyproject.toml
 readme.md
 venues/stages/somatic/__init__.py
 venues/stages/somatic/_clique.py
+venues/stages/somatic/module.s.HTML
 venues/stages/somatic/start.proc.py
 venues/stages/somatic.egg-info/PKG-INFO
 venues/stages/somatic.egg-info/SOURCES.txt
 venues/stages/somatic.egg-info/dependency_links.txt
 venues/stages/somatic.egg-info/entry_points.txt
 venues/stages/somatic.egg-info/requires.txt
 venues/stages/somatic.egg-info/top_level.txt
+venues/stages/somatic/___itinerary/itinerary.S.HTML
+venues/stages/somatic/___itinerary/possibilities.S.HTML
+venues/stages/somatic/__license/license.s.HTML
 venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html
 venues/stages/somatic/_controls/flask/__init__.py
 venues/stages/somatic/_controls/sanic/__init__.py
 venues/stages/somatic/_status/status.proc.py
 venues/stages/somatic/_status/checks/1/status_1.py
+venues/stages/somatic/_status/checks/1/shares/shares 1.s.HTML
+venues/stages/somatic/_status/checks/1/shares/shares 2.s.HTML
 venues/stages/somatic/climate/__init__.py
 venues/stages/somatic/modules/add_glob_to_paths.py
 venues/stages/somatic/modules/parse_extensions.py
 venues/stages/somatic/modules/port_in_use.py
 venues/stages/somatic/modules/HTML/__init__.py
+venues/stages/somatic/modules_ES/address/address.s.HTML
 venues/stages/somatic/moves/start.py
```

