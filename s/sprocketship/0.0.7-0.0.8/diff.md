# Comparing `tmp/sprocketship-0.0.7.tar.gz` & `tmp/sprocketship-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.0.7.tar", last modified: Fri Apr  5 17:33:53 2024, max compression
+gzip compressed data, was "sprocketship-0.0.8.tar", last modified: Fri Apr  5 17:38:30 2024, max compression
```

## Comparing `sprocketship-0.0.7.tar` & `sprocketship-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:53.758884 sprocketship-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 17:33:45.000000 sprocketship-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-05 17:33:53.758884 sprocketship-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 17:33:45.000000 sprocketship-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 17:33:45.000000 sprocketship-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:33:53.758884 sprocketship-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:53.758884 sprocketship-0.0.7/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-05 17:33:45.000000 sprocketship-0.0.7/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:53.758884 sprocketship-0.0.7/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:38:30.583635 sprocketship-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 17:38:26.000000 sprocketship-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-05 17:38:30.583635 sprocketship-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 17:38:26.000000 sprocketship-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 17:38:26.000000 sprocketship-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:38:30.583635 sprocketship-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:38:30.583635 sprocketship-0.0.8/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-05 17:38:26.000000 sprocketship-0.0.8/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:38:30.583635 sprocketship-0.0.8/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.0.7/LICENSE` & `sprocketship-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.7/PKG-INFO` & `sprocketship-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.7
+Version: 0.0.8
+Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.7 Author-email: Nicklaus
-Roacb
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.8 Summary: Better stored
+procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
```

### Comparing `sprocketship-0.0.7/README.md` & `sprocketship-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.7/pyproject.toml` & `sprocketship-0.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
+description = "Better stored procedure management"
 dependencies = [
     "click",
     "snowflake",
     "ABSQL",
     "ruamel.yaml",
     "jinja2"
 ]
```

### Comparing `sprocketship-0.0.7/sprocketship/cli.py` & `sprocketship-0.0.8/sprocketship/cli.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.7/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.0.8/sprocketship.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.7
+Version: 0.0.8
+Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.7 Author-email: Nicklaus
-Roacb
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.8 Summary: Better stored
+procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
```

