# Comparing `tmp/vlite-0.1.8.tar.gz` & `tmp/vlite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.1.8.tar", last modified: Tue Aug  8 21:44:27 2023, max compression
+gzip compressed data, was "vlite-0.2.0.tar", last modified: Fri Apr  5 11:56:22 2024, max compression
```

## Comparing `vlite-0.1.8.tar` & `vlite-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-08-08 21:44:27.954951 vlite-0.1.8/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-08-08 21:44:27.954815 vlite-0.1.8/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)     1605 2023-07-07 07:20:20.000000 vlite-0.1.8/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2023-08-08 21:44:27.954997 vlite-0.1.8/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)      410 2023-08-08 21:43:28.000000 vlite-0.1.8/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-08-08 21:44:27.953975 vlite-0.1.8/vlite/
--rw-r--r--   0 sdan       (501) staff       (20)       23 2023-07-04 08:27:33.000000 vlite-0.1.8/vlite/__init__.py
--rw-r--r--   0 sdan       (501) staff       (20)     2760 2023-07-09 11:01:10.000000 vlite-0.1.8/vlite/main.py
--rw-r--r--   0 sdan       (501) staff       (20)     3278 2023-07-06 23:49:16.000000 vlite-0.1.8/vlite/model.py
--rw-r--r--   0 sdan       (501) staff       (20)     3066 2023-07-07 07:20:20.000000 vlite-0.1.8/vlite/utils.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-08-08 21:44:27.954627 vlite-0.1.8/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      224 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)       43 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        6 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-05 11:56:22.415560 vlite-0.2.0/
+-rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.0/LICENSE
+-rw-r--r--   0 sdan       (501) staff       (20)      218 2024-04-05 11:56:22.415428 vlite-0.2.0/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)     2635 2024-04-05 11:47:06.000000 vlite-0.2.0/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-05 11:56:22.415604 vlite-0.2.0/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)      558 2024-04-05 11:54:26.000000 vlite-0.2.0/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-05 11:56:22.414493 vlite-0.2.0/vlite/
+-rw-r--r--   0 sdan       (501) staff       (20)       80 2024-04-05 11:37:40.000000 vlite-0.2.0/vlite/__init__.py
+-rw-r--r--   0 sdan       (501) staff       (20)     8527 2024-04-05 10:47:15.000000 vlite-0.2.0/vlite/main.py
+-rw-r--r--   0 sdan       (501) staff       (20)     1799 2024-04-05 11:37:40.000000 vlite-0.2.0/vlite/model.py
+-rw-r--r--   0 sdan       (501) staff       (20)     6650 2024-04-05 10:43:40.000000 vlite-0.2.0/vlite/omom.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7747 2024-04-03 19:37:27.000000 vlite-0.2.0/vlite/server.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7687 2024-04-05 11:37:40.000000 vlite-0.2.0/vlite/utils.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-05 11:56:22.415262 vlite-0.2.0/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      218 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      262 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)      118 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/top_level.txt
```

