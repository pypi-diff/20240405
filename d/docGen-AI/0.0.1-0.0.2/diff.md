# Comparing `tmp/docGen-AI-0.0.1.tar.gz` & `tmp/docGen-AI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docGen-AI-0.0.1.tar", last modified: Fri Apr  5 18:51:21 2024, max compression
+gzip compressed data, was "docGen-AI-0.0.2.tar", last modified: Fri Apr  5 19:00:57 2024, max compression
```

## Comparing `docGen-AI-0.0.1.tar` & `docGen-AI-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 18:51:21.254113 docGen-AI-0.0.1/
--rw-rw-rw-   0        0        0     1088 2024-03-20 14:29:16.000000 docGen-AI-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1737 2024-04-05 18:51:21.250114 docGen-AI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1158 2024-04-05 18:33:42.000000 docGen-AI-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 18:51:21.248110 docGen-AI-0.0.1/docGen_AI.egg-info/
--rw-rw-rw-   0        0        0     1737 2024-04-05 18:51:20.000000 docGen-AI-0.0.1/docGen_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-04-05 18:51:20.000000 docGen-AI-0.0.1/docGen_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:51:20.000000 docGen-AI-0.0.1/docGen_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:51:20.000000 docGen-AI-0.0.1/docGen_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      601 2024-04-05 18:50:51.000000 docGen-AI-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 18:51:21.255141 docGen-AI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      196 2024-03-31 05:39:46.000000 docGen-AI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:00:57.616422 docGen-AI-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-03-20 14:29:16.000000 docGen-AI-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1737 2024-04-05 19:00:57.596420 docGen-AI-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1158 2024-04-05 18:33:42.000000 docGen-AI-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 19:00:57.592423 docGen-AI-0.0.2/docGen_AI.egg-info/
+-rw-rw-rw-   0        0        0     1737 2024-04-05 19:00:57.000000 docGen-AI-0.0.2/docGen_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-04-05 19:00:57.000000 docGen-AI-0.0.2/docGen_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:00:57.000000 docGen-AI-0.0.2/docGen_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:00:57.000000 docGen-AI-0.0.2/docGen_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2024-04-05 19:00:43.000000 docGen-AI-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 19:00:57.616422 docGen-AI-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      196 2024-03-31 05:39:46.000000 docGen-AI-0.0.2/setup.py
```

### Comparing `docGen-AI-0.0.1/LICENSE` & `docGen-AI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docGen-AI-0.0.1/PKG-INFO` & `docGen-AI-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: docGen-AI
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for generating Docstring for python.
-Author-email: Amal <amal76735@gmail.com>, Rijin <rijin@gmail.com>, yadhu <yadhu2309@gmail.com>
+Author-email: Rijin <rijin@gmail.com>, Amal <amal76735@gmail.com>, yadhu <yadhu2309@gmail.com>
 Project-URL: Homepage, https://github.com/RijinRaju/DocGen-AI
 Project-URL: Issues, https://github.com/RijinRaju/DocGen-AI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `docGen-AI-0.0.1/README.md` & `docGen-AI-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `docGen-AI-0.0.1/docGen_AI.egg-info/PKG-INFO` & `docGen-AI-0.0.2/docGen_AI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: docGen-AI
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for generating Docstring for python.
-Author-email: Amal <amal76735@gmail.com>, Rijin <rijin@gmail.com>, yadhu <yadhu2309@gmail.com>
+Author-email: Rijin <rijin@gmail.com>, Amal <amal76735@gmail.com>, yadhu <yadhu2309@gmail.com>
 Project-URL: Homepage, https://github.com/RijinRaju/DocGen-AI
 Project-URL: Issues, https://github.com/RijinRaju/DocGen-AI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `docGen-AI-0.0.1/pyproject.toml` & `docGen-AI-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "docGen-AI"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
+    { name="Rijin", email="rijin@gmail.com"},
   { name="Amal", email="amal76735@gmail.com"},
-  { name="Rijin", email="rijin@gmail.com"},
   { name="yadhu", email="yadhu2309@gmail.com"}
 ]
 description = "A package for generating Docstring for python."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

