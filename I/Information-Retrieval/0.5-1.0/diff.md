# Comparing `tmp/Information_Retrieval-0.5.tar.gz` & `tmp/Information_Retrieval-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Information_Retrieval-0.5.tar", last modified: Sat Mar 30 15:32:36 2024, max compression
+gzip compressed data, was "Information_Retrieval-1.0.tar", last modified: Sat Mar 30 15:56:17 2024, max compression
```

## Comparing `Information_Retrieval-0.5.tar` & `Information_Retrieval-1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:32:36.473287 Information_Retrieval-0.5/
-drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:32:36.472226 Information_Retrieval-0.5/Information_Retrieval/
--rw-r--r--   0 kushpai    (501) staff       (20)      175 2024-03-30 15:32:09.000000 Information_Retrieval-0.5/Information_Retrieval/__init__.py
--rw-r--r--   0 kushpai    (501) staff       (20)     3859 2024-03-30 15:25:01.000000 Information_Retrieval-0.5/Information_Retrieval/main.py
-drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:32:36.472955 Information_Retrieval-0.5/Information_Retrieval.egg-info/
--rw-r--r--   0 kushpai    (501) staff       (20)      144 2024-03-30 15:32:36.000000 Information_Retrieval-0.5/Information_Retrieval.egg-info/PKG-INFO
--rw-r--r--   0 kushpai    (501) staff       (20)      300 2024-03-30 15:32:36.000000 Information_Retrieval-0.5/Information_Retrieval.egg-info/SOURCES.txt
--rw-r--r--   0 kushpai    (501) staff       (20)        1 2024-03-30 15:32:36.000000 Information_Retrieval-0.5/Information_Retrieval.egg-info/dependency_links.txt
--rw-r--r--   0 kushpai    (501) staff       (20)       55 2024-03-30 15:32:36.000000 Information_Retrieval-0.5/Information_Retrieval.egg-info/entry_points.txt
--rw-r--r--   0 kushpai    (501) staff       (20)       22 2024-03-30 15:32:36.000000 Information_Retrieval-0.5/Information_Retrieval.egg-info/top_level.txt
--rw-r--r--   0 kushpai    (501) staff       (20)      144 2024-03-30 15:32:36.473113 Information_Retrieval-0.5/PKG-INFO
--rw-r--r--   0 kushpai    (501) staff       (20)       38 2024-03-30 15:32:36.473342 Information_Retrieval-0.5/setup.cfg
--rw-r--r--   0 kushpai    (501) staff       (20)      317 2024-03-30 15:32:32.000000 Information_Retrieval-0.5/setup.py
+drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:56:17.646221 Information_Retrieval-1.0/
+drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:56:17.645159 Information_Retrieval-1.0/Information_Retrieval/
+-rw-r--r--   0 kushpai    (501) staff       (20)      500 2024-03-30 15:55:33.000000 Information_Retrieval-1.0/Information_Retrieval/__init__.py
+-rw-r--r--   0 kushpai    (501) staff       (20)    10502 2024-03-30 15:55:26.000000 Information_Retrieval-1.0/Information_Retrieval/main.py
+drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:56:17.645885 Information_Retrieval-1.0/Information_Retrieval.egg-info/
+-rw-r--r--   0 kushpai    (501) staff       (20)      144 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/PKG-INFO
+-rw-r--r--   0 kushpai    (501) staff       (20)      300 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 kushpai    (501) staff       (20)        1 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 kushpai    (501) staff       (20)       55 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/entry_points.txt
+-rw-r--r--   0 kushpai    (501) staff       (20)       22 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/top_level.txt
+-rw-r--r--   0 kushpai    (501) staff       (20)      144 2024-03-30 15:56:17.646050 Information_Retrieval-1.0/PKG-INFO
+-rw-r--r--   0 kushpai    (501) staff       (20)       38 2024-03-30 15:56:17.646281 Information_Retrieval-1.0/setup.cfg
+-rw-r--r--   0 kushpai    (501) staff       (20)      317 2024-03-30 15:55:38.000000 Information_Retrieval-1.0/setup.py
```

