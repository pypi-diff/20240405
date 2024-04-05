# Comparing `tmp/chisel-1.2.6.tar.gz` & `tmp/chisel-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chisel-1.2.6.tar", last modified: Wed Apr  3 20:48:15 2024, max compression
+gzip compressed data, was "chisel-1.2.7.tar", last modified: Fri Apr  5 18:09:54 2024, max compression
```

## Comparing `chisel-1.2.6.tar` & `chisel-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 20:48:15.674208 chisel-1.2.6/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-04-02 16:27:20.000000 chisel-1.2.6/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     4155 2024-04-03 20:48:15.674147 chisel-1.2.6/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     3096 2024-04-03 20:25:13.000000 chisel-1.2.6/README.md
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-04-02 16:27:20.000000 chisel-1.2.6/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)     1056 2024-04-03 20:48:15.674508 chisel-1.2.6/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 20:48:15.671950 chisel-1.2.6/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 20:48:15.673120 chisel-1.2.6/src/chisel/
--rw-r--r--   0 craighobbs   (501) staff       (20)      502 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    13926 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/action.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    22354 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/app.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     9936 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/doc.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     8147 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/request.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 20:48:15.673912 chisel-1.2.6/src/chisel.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     4155 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      313 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       23 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        7 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-05 18:09:54.018664 chisel-1.2.7/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-04-02 16:27:20.000000 chisel-1.2.7/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     4155 2024-04-05 18:09:54.018598 chisel-1.2.7/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3096 2024-04-03 20:25:13.000000 chisel-1.2.7/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-04-02 16:27:20.000000 chisel-1.2.7/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1056 2024-04-05 18:09:54.019033 chisel-1.2.7/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-05 18:09:54.012036 chisel-1.2.7/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-05 18:09:54.016401 chisel-1.2.7/src/chisel/
+-rw-r--r--   0 craighobbs   (501) staff       (20)      502 2024-04-02 16:27:20.000000 chisel-1.2.7/src/chisel/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    13926 2024-04-02 16:27:20.000000 chisel-1.2.7/src/chisel/action.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    22354 2024-04-02 16:27:20.000000 chisel-1.2.7/src/chisel/app.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    10180 2024-04-05 18:07:36.000000 chisel-1.2.7/src/chisel/doc.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     8147 2024-04-02 16:27:20.000000 chisel-1.2.7/src/chisel/request.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-05 18:09:54.018316 chisel-1.2.7/src/chisel.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     4155 2024-04-05 18:09:53.000000 chisel-1.2.7/src/chisel.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      313 2024-04-05 18:09:53.000000 chisel-1.2.7/src/chisel.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-04-05 18:09:53.000000 chisel-1.2.7/src/chisel.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       23 2024-04-05 18:09:53.000000 chisel-1.2.7/src/chisel.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        7 2024-04-05 18:09:53.000000 chisel-1.2.7/src/chisel.egg-info/top_level.txt
```

### Comparing `chisel-1.2.6/LICENSE` & `chisel-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chisel-1.2.6/PKG-INFO` & `chisel-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chisel
-Version: 1.2.6
+Version: 1.2.7
 Summary: Lightweight WSGI application framework, schema-validated JSON APIs, and API documentation
 Home-page: https://github.com/craigahobbs/chisel
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: api,json,framework,schema,wsgi
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chisel-1.2.6/README.md` & `chisel-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `chisel-1.2.6/setup.cfg` & `chisel-1.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chisel
-version = 1.2.6
+version = 1.2.7
 url = https://github.com/craigahobbs/chisel
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = Lightweight WSGI application framework, schema-validated JSON APIs, and API documentation
 long_description = file:README.md
 long_description_content_type = text/markdown
```

### Comparing `chisel-1.2.6/src/chisel/action.py` & `chisel-1.2.7/src/chisel/action.py`

 * *Files identical despite different names*

### Comparing `chisel-1.2.6/src/chisel/app.py` & `chisel-1.2.7/src/chisel/app.py`

 * *Files identical despite different names*

### Comparing `chisel-1.2.6/src/chisel/doc.py` & `chisel-1.2.7/src/chisel/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,19 @@
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

### Comparing `chisel-1.2.6/src/chisel/request.py` & `chisel-1.2.7/src/chisel/request.py`

 * *Files identical despite different names*

### Comparing `chisel-1.2.6/src/chisel.egg-info/PKG-INFO` & `chisel-1.2.7/src/chisel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chisel
-Version: 1.2.6
+Version: 1.2.7
 Summary: Lightweight WSGI application framework, schema-validated JSON APIs, and API documentation
 Home-page: https://github.com/craigahobbs/chisel
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: api,json,framework,schema,wsgi
 Classifier: Development Status :: 5 - Production/Stable
```

