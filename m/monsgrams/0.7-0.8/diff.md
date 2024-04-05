# Comparing `tmp/monsgrams-0.7.tar.gz` & `tmp/monsgrams-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.7.tar", last modified: Thu Apr  4 20:00:29 2024, max compression
+gzip compressed data, was "monsgrams-0.8.tar", last modified: Fri Apr  5 03:11:34 2024, max compression
```

## Comparing `monsgrams-0.7.tar` & `monsgrams-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 20:00:28.996426 monsgrams-0.7/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      759 2024-04-04 20:00:28.996426 monsgrams-0.7/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      523 2024-04-04 20:00:03.000000 monsgrams-0.7/README.md
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 20:00:28.984426 monsgrams-0.7/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       82 2024-04-04 19:58:17.000000 monsgrams-0.7/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      778 2024-04-04 19:50:47.000000 monsgrams-0.7/monsgrams/api.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      210 2024-04-04 19:58:09.000000 monsgrams-0.7/monsgrams/context.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     1463 2024-04-04 19:58:55.000000 monsgrams-0.7/monsgrams/main.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 20:00:28.992426 monsgrams-0.7/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      759 2024-04-04 20:00:28.000000 monsgrams-0.7/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      228 2024-04-04 20:00:28.000000 monsgrams-0.7/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 20:00:28.000000 monsgrams-0.7/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 20:00:28.000000 monsgrams-0.7/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 20:00:29.000426 monsgrams-0.7/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      387 2024-04-04 19:28:18.000000 monsgrams-0.7/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:11:34.514729 monsgrams-0.8/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      759 2024-04-05 03:11:34.510729 monsgrams-0.8/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      523 2024-04-04 20:00:03.000000 monsgrams-0.8/README.md
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:11:34.498729 monsgrams-0.8/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       52 2024-04-04 23:18:54.000000 monsgrams-0.8/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     1639 2024-04-05 02:49:12.000000 monsgrams-0.8/monsgrams/api.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     2175 2024-04-05 03:11:01.000000 monsgrams-0.8/monsgrams/bot.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      395 2024-04-04 22:54:44.000000 monsgrams-0.8/monsgrams/context.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:11:34.510729 monsgrams-0.8/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      759 2024-04-05 03:11:34.000000 monsgrams-0.8/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      227 2024-04-05 03:11:34.000000 monsgrams-0.8/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-05 03:11:34.000000 monsgrams-0.8/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-05 03:11:34.000000 monsgrams-0.8/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-05 03:11:34.514729 monsgrams-0.8/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      387 2024-04-05 03:11:27.000000 monsgrams-0.8/setup.py
```

### Comparing `monsgrams-0.7/PKG-INFO` & `monsgrams-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monsgrams
-Version: 0.7
+Version: 0.8
 Summary: A simple Python library for creating telegram bot.
 Home-page: https://github.com/tech-voyager/monsgrams/
 Author: grubx64
 License: MIT
 Description-Content-Type: text/markdown
 
 **This library provides interesting opportunities for creating telegram bots.
```

### Comparing `monsgrams-0.7/README.md` & `monsgrams-0.8/README.md`

 * *Files identical despite different names*

### Comparing `monsgrams-0.7/monsgrams.egg-info/PKG-INFO` & `monsgrams-0.8/monsgrams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monsgrams
-Version: 0.7
+Version: 0.8
 Summary: A simple Python library for creating telegram bot.
 Home-page: https://github.com/tech-voyager/monsgrams/
 Author: grubx64
 License: MIT
 Description-Content-Type: text/markdown
 
 **This library provides interesting opportunities for creating telegram bots.
```

