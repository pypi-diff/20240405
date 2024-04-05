# Comparing `tmp/markdown-up-1.7.4.tar.gz` & `tmp/markdown-up-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-up-1.7.4.tar", last modified: Mon Feb 12 20:02:03 2024, max compression
+gzip compressed data, was "markdown-up-1.7.5.tar", last modified: Fri Apr  5 18:18:34 2024, max compression
```

## Comparing `markdown-up-1.7.4.tar` & `markdown-up-1.7.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-02-12 20:02:03.569258 markdown-up-1.7.4/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-02-10 00:56:42.000000 markdown-up-1.7.4/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     2232 2024-02-12 20:02:03.569196 markdown-up-1.7.4/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     1386 2024-02-10 00:56:42.000000 markdown-up-1.7.4/README.md
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-02-10 00:56:42.000000 markdown-up-1.7.4/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)      935 2024-02-12 20:02:03.569498 markdown-up-1.7.4/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-02-12 20:02:03.567214 markdown-up-1.7.4/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-02-12 20:02:03.568175 markdown-up-1.7.4/src/markdown_up/
--rw-r--r--   0 craighobbs   (501) staff       (20)       99 2024-02-10 00:56:42.000000 markdown-up-1.7.4/src/markdown_up/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)      245 2024-02-10 00:56:42.000000 markdown-up-1.7.4/src/markdown_up/__main__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     9347 2024-02-10 18:50:39.000000 markdown-up-1.7.4/src/markdown_up/app.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     2889 2024-02-12 19:56:17.000000 markdown-up-1.7.4/src/markdown_up/main.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-02-12 20:02:03.568988 markdown-up-1.7.4/src/markdown_up.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     2232 2024-02-12 20:02:03.000000 markdown-up-1.7.4/src/markdown_up.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      381 2024-02-12 20:02:03.000000 markdown-up-1.7.4/src/markdown_up.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-02-12 20:02:03.000000 markdown-up-1.7.4/src/markdown_up.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-02-12 20:02:03.000000 markdown-up-1.7.4/src/markdown_up.egg-info/entry_points.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       28 2024-02-12 20:02:03.000000 markdown-up-1.7.4/src/markdown_up.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-02-12 20:02:03.000000 markdown-up-1.7.4/src/markdown_up.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-05 18:18:34.550319 markdown-up-1.7.5/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-04-02 16:27:18.000000 markdown-up-1.7.5/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2232 2024-04-05 18:18:34.550244 markdown-up-1.7.5/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1386 2024-04-02 16:27:18.000000 markdown-up-1.7.5/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-04-02 16:27:18.000000 markdown-up-1.7.5/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)      935 2024-04-05 18:18:34.550643 markdown-up-1.7.5/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-05 18:18:34.548190 markdown-up-1.7.5/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-05 18:18:34.549197 markdown-up-1.7.5/src/markdown_up/
+-rw-r--r--   0 craighobbs   (501) staff       (20)       99 2024-04-02 16:27:18.000000 markdown-up-1.7.5/src/markdown_up/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)      245 2024-04-02 16:27:18.000000 markdown-up-1.7.5/src/markdown_up/__main__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     9591 2024-04-05 18:15:19.000000 markdown-up-1.7.5/src/markdown_up/app.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2889 2024-04-02 16:27:18.000000 markdown-up-1.7.5/src/markdown_up/main.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-05 18:18:34.550025 markdown-up-1.7.5/src/markdown_up.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2232 2024-04-05 18:18:34.000000 markdown-up-1.7.5/src/markdown_up.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      381 2024-04-05 18:18:34.000000 markdown-up-1.7.5/src/markdown_up.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-04-05 18:18:34.000000 markdown-up-1.7.5/src/markdown_up.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-04-05 18:18:34.000000 markdown-up-1.7.5/src/markdown_up.egg-info/entry_points.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       28 2024-04-05 18:18:34.000000 markdown-up-1.7.5/src/markdown_up.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-04-05 18:18:34.000000 markdown-up-1.7.5/src/markdown_up.egg-info/top_level.txt
```

### Comparing `markdown-up-1.7.4/LICENSE` & `markdown-up-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-up-1.7.4/PKG-INFO` & `markdown-up-1.7.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-up
-Version: 1.7.4
+Version: 1.7.5
 Summary: The MarkdownUp launcher
 Home-page: https://github.com/craigahobbs/markdown-up-py
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: Markdown,viewer
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `markdown-up-1.7.4/README.md` & `markdown-up-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `markdown-up-1.7.4/setup.cfg` & `markdown-up-1.7.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = markdown-up
-version = 1.7.4
+version = 1.7.5
 url = https://github.com/craigahobbs/markdown-up-py
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = The MarkdownUp launcher
 long_description = file:README.md
 long_description_content_type = text/markdown
```

### Comparing `markdown-up-1.7.4/src/markdown_up/app.py` & `markdown-up-1.7.5/src/markdown_up/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,17 +117,19 @@
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <link rel="stylesheet" href="https://craigahobbs.github.io/markdown-up/app.css">
 
         <!-- Preloads -->
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/bare-script/lib/data.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/bare-script/lib/library.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/bare-script/lib/model.js" as="script">
+        <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/bare-script/lib/options.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/bare-script/lib/parser.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/bare-script/lib/runtime.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/bare-script/lib/runtimeAsync.js" as="script">
+        <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/bare-script/lib/value.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/element-model/lib/elementModel.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/lib/app.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/lib/dataTable.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/lib/dataUtil.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/lib/lineChart.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/lib/script.js" as="script">
         <link rel="modulepreload" href="https://craigahobbs.github.io/markdown-up/lib/scriptLibrary.js" as="script">
```

### Comparing `markdown-up-1.7.4/src/markdown_up/main.py` & `markdown-up-1.7.5/src/markdown_up/main.py`

 * *Files identical despite different names*

### Comparing `markdown-up-1.7.4/src/markdown_up.egg-info/PKG-INFO` & `markdown-up-1.7.5/src/markdown_up.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-up
-Version: 1.7.4
+Version: 1.7.5
 Summary: The MarkdownUp launcher
 Home-page: https://github.com/craigahobbs/markdown-up-py
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: Markdown,viewer
 Classifier: Development Status :: 5 - Production/Stable
```

