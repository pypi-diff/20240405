# Comparing `tmp/sigiq-0.2.6.1.tar.gz` & `tmp/sigiq-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigiq-0.2.6.1.tar", last modified: Wed Mar  6 02:34:26 2024, max compression
+gzip compressed data, was "sigiq-0.3.tar", last modified: Fri Apr  5 02:13:35 2024, max compression
```

## Comparing `sigiq-0.2.6.1.tar` & `sigiq-0.3.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-03-06 02:34:26.929550 sigiq-0.2.6.1/
--rw-r--r--   0 kevinshi   (501) staff       (20)      138 2024-03-06 02:34:26.929352 sigiq-0.2.6.1/PKG-INFO
--rw-r--r--   0 kevinshi   (501) staff       (20)       38 2024-03-06 02:34:26.929611 sigiq-0.2.6.1/setup.cfg
--rw-r--r--   0 kevinshi   (501) staff       (20)      231 2024-03-06 02:32:58.000000 sigiq-0.2.6.1/setup.py
-drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-03-06 02:34:26.927642 sigiq-0.2.6.1/sigiq/
--rw-r--r--   0 kevinshi   (501) staff       (20)      252 2024-03-06 01:45:01.000000 sigiq-0.2.6.1/sigiq/__init__.py
--rw-r--r--   0 kevinshi   (501) staff       (20)     7688 2024-03-02 21:20:19.000000 sigiq-0.2.6.1/sigiq/classes.py
-drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-03-06 02:34:26.928523 sigiq-0.2.6.1/sigiq/decorators/
--rw-r--r--   0 kevinshi   (501) staff       (20)        0 2024-03-06 02:33:49.000000 sigiq-0.2.6.1/sigiq/decorators/__init__.py
-drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-03-06 02:34:26.928742 sigiq-0.2.6.1/sigiq/decorators/li_token_tracking/
--rw-r--r--   0 kevinshi   (501) staff       (20)        0 2024-03-06 02:29:46.000000 sigiq-0.2.6.1/sigiq/decorators/li_token_tracking/__init__.py
--rw-r--r--   0 kevinshi   (501) staff       (20)     5224 2024-03-06 01:45:01.000000 sigiq-0.2.6.1/sigiq/decorators/li_token_tracking/token_tracking.py
--rw-r--r--   0 kevinshi   (501) staff       (20)     1250 2024-03-06 02:19:22.000000 sigiq-0.2.6.1/sigiq/functions.py
--rw-r--r--   0 kevinshi   (501) staff       (20)      464 2023-12-12 19:09:21.000000 sigiq-0.2.6.1/sigiq/login.py
--rw-r--r--   0 kevinshi   (501) staff       (20)      521 2023-12-12 19:24:31.000000 sigiq-0.2.6.1/sigiq/utils.py
-drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-03-06 02:34:26.929144 sigiq-0.2.6.1/sigiq.egg-info/
--rw-r--r--   0 kevinshi   (501) staff       (20)      138 2024-03-06 02:34:26.000000 sigiq-0.2.6.1/sigiq.egg-info/PKG-INFO
--rw-r--r--   0 kevinshi   (501) staff       (20)      365 2024-03-06 02:34:26.000000 sigiq-0.2.6.1/sigiq.egg-info/SOURCES.txt
--rw-r--r--   0 kevinshi   (501) staff       (20)        1 2024-03-06 02:34:26.000000 sigiq-0.2.6.1/sigiq.egg-info/dependency_links.txt
--rw-r--r--   0 kevinshi   (501) staff       (20)       42 2024-03-06 02:34:26.000000 sigiq-0.2.6.1/sigiq.egg-info/requires.txt
--rw-r--r--   0 kevinshi   (501) staff       (20)        6 2024-03-06 02:34:26.000000 sigiq-0.2.6.1/sigiq.egg-info/top_level.txt
+drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-04-05 02:13:35.026468 sigiq-0.3/
+-rw-r--r--   0 kevinshi   (501) staff       (20)      134 2024-04-05 02:13:35.026255 sigiq-0.3/PKG-INFO
+-rw-r--r--   0 kevinshi   (501) staff       (20)       38 2024-04-05 02:13:35.026534 sigiq-0.3/setup.cfg
+-rw-r--r--   0 kevinshi   (501) staff       (20)      227 2024-04-05 02:11:44.000000 sigiq-0.3/setup.py
+drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-04-05 02:13:35.024267 sigiq-0.3/sigiq/
+-rw-r--r--   0 kevinshi   (501) staff       (20)      115 2024-04-05 02:09:41.000000 sigiq-0.3/sigiq/__init__.py
+drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-04-05 02:13:35.025238 sigiq-0.3/sigiq/decorators/
+-rw-r--r--   0 kevinshi   (501) staff       (20)        0 2024-03-21 17:45:06.000000 sigiq-0.3/sigiq/decorators/__init__.py
+drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-04-05 02:13:35.025473 sigiq-0.3/sigiq/decorators/li_token_tracking/
+-rw-r--r--   0 kevinshi   (501) staff       (20)        0 2024-03-21 17:45:06.000000 sigiq-0.3/sigiq/decorators/li_token_tracking/__init__.py
+-rw-r--r--   0 kevinshi   (501) staff       (20)     5224 2024-03-21 17:45:06.000000 sigiq-0.3/sigiq/decorators/li_token_tracking/token_tracking.py
+-rw-r--r--   0 kevinshi   (501) staff       (20)      928 2024-04-05 02:11:48.000000 sigiq-0.3/sigiq/functions.py
+drwxr-xr-x   0 kevinshi   (501) staff       (20)        0 2024-04-05 02:13:35.025972 sigiq-0.3/sigiq.egg-info/
+-rw-r--r--   0 kevinshi   (501) staff       (20)      134 2024-04-05 02:13:35.000000 sigiq-0.3/sigiq.egg-info/PKG-INFO
+-rw-r--r--   0 kevinshi   (501) staff       (20)      318 2024-04-05 02:13:35.000000 sigiq-0.3/sigiq.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinshi   (501) staff       (20)        1 2024-04-05 02:13:35.000000 sigiq-0.3/sigiq.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinshi   (501) staff       (20)       42 2024-04-05 02:13:35.000000 sigiq-0.3/sigiq.egg-info/requires.txt
+-rw-r--r--   0 kevinshi   (501) staff       (20)        6 2024-04-05 02:13:35.000000 sigiq-0.3/sigiq.egg-info/top_level.txt
```

### Comparing `sigiq-0.2.6.1/sigiq/decorators/li_token_tracking/token_tracking.py` & `sigiq-0.3/sigiq/decorators/li_token_tracking/token_tracking.py`

 * *Files identical despite different names*

