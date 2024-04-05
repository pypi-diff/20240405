# Comparing `tmp/monsgrams-0.8.tar.gz` & `tmp/monsgrams-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.8.tar", last modified: Fri Apr  5 03:11:34 2024, max compression
+gzip compressed data, was "monsgrams-0.9.tar", last modified: Fri Apr  5 03:31:11 2024, max compression
```

## Comparing `monsgrams-0.8.tar` & `monsgrams-0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:11:34.514729 monsgrams-0.8/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      759 2024-04-05 03:11:34.510729 monsgrams-0.8/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      523 2024-04-04 20:00:03.000000 monsgrams-0.8/README.md
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:11:34.498729 monsgrams-0.8/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       52 2024-04-04 23:18:54.000000 monsgrams-0.8/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     1639 2024-04-05 02:49:12.000000 monsgrams-0.8/monsgrams/api.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     2175 2024-04-05 03:11:01.000000 monsgrams-0.8/monsgrams/bot.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      395 2024-04-04 22:54:44.000000 monsgrams-0.8/monsgrams/context.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:11:34.510729 monsgrams-0.8/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      759 2024-04-05 03:11:34.000000 monsgrams-0.8/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      227 2024-04-05 03:11:34.000000 monsgrams-0.8/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-05 03:11:34.000000 monsgrams-0.8/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-05 03:11:34.000000 monsgrams-0.8/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-05 03:11:34.514729 monsgrams-0.8/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      387 2024-04-05 03:11:27.000000 monsgrams-0.8/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:31:11.462729 monsgrams-0.9/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      789 2024-04-05 03:31:11.462729 monsgrams-0.9/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      523 2024-04-04 20:00:03.000000 monsgrams-0.9/README.md
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:31:11.450729 monsgrams-0.9/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       52 2024-04-04 23:18:54.000000 monsgrams-0.9/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      167 2024-04-05 03:30:56.000000 monsgrams-0.9/monsgrams/api.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     2175 2024-04-05 03:11:01.000000 monsgrams-0.9/monsgrams/bot.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      395 2024-04-04 22:54:44.000000 monsgrams-0.9/monsgrams/context.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:31:11.458729 monsgrams-0.9/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      789 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      259 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       15 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/requires.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-05 03:31:11.466729 monsgrams-0.9/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      443 2024-04-05 03:29:33.000000 monsgrams-0.9/setup.py
```

### Comparing `monsgrams-0.8/README.md` & `monsgrams-0.9/README.md`

 * *Files identical despite different names*

### Comparing `monsgrams-0.8/monsgrams/bot.py` & `monsgrams-0.9/monsgrams/bot.py`

 * *Files identical despite different names*

