# Comparing `tmp/sprocketship-0.0.1.tar.gz` & `tmp/sprocketship-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.0.1.tar", last modified: Fri Apr  5 15:28:57 2024, max compression
+gzip compressed data, was "sprocketship-0.0.2.tar", last modified: Fri Apr  5 15:33:29 2024, max compression
```

## Comparing `sprocketship-0.0.1.tar` & `sprocketship-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:57.672615 sprocketship-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 15:28:51.000000 sprocketship-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-05 15:28:57.672615 sprocketship-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-05 15:28:51.000000 sprocketship-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 15:28:51.000000 sprocketship-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:28:57.672615 sprocketship-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:57.672615 sprocketship-0.0.1/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-05 15:28:51.000000 sprocketship-0.0.1/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:57.672615 sprocketship-0.0.1/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-05 15:28:57.000000 sprocketship-0.0.1/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 15:28:57.000000 sprocketship-0.0.1/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:28:57.000000 sprocketship-0.0.1/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 15:28:57.000000 sprocketship-0.0.1/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 15:28:57.000000 sprocketship-0.0.1/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 15:28:57.000000 sprocketship-0.0.1/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:29.385696 sprocketship-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 15:33:24.000000 sprocketship-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8626 2024-04-05 15:33:29.385696 sprocketship-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-05 15:33:24.000000 sprocketship-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 15:33:24.000000 sprocketship-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:33:29.385696 sprocketship-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:29.385696 sprocketship-0.0.2/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-05 15:33:24.000000 sprocketship-0.0.2/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:29.385696 sprocketship-0.0.2/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8626 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.0.1/LICENSE` & `sprocketship-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.1/PKG-INFO` & `sprocketship-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: snowflake
 Requires-Dist: ABSQL
-Requires-Dist: ruamel
+Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.1 Author-email: Nicklaus
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.2 Author-email: Nicklaus
 Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel
+click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
 url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
```

### Comparing `sprocketship-0.0.1/README.md` & `sprocketship-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.1/pyproject.toml` & `sprocketship-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
     "click",
     "snowflake",
     "ABSQL",
-    "ruamel",
+    "ruamel.yaml",
     "jinja2"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sprocketship-0.0.1/sprocketship/cli.py` & `sprocketship-0.0.2/sprocketship/cli.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.1/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.0.2/sprocketship.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: snowflake
 Requires-Dist: ABSQL
-Requires-Dist: ruamel
+Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.1 Author-email: Nicklaus
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.2 Author-email: Nicklaus
 Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel
+click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
 url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
```

