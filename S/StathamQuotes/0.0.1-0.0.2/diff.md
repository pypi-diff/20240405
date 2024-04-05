# Comparing `tmp/StathamQuotes-0.0.1.tar.gz` & `tmp/StathamQuotes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StathamQuotes-0.0.1.tar", last modified: Fri Apr  5 19:11:06 2024, max compression
+gzip compressed data, was "StathamQuotes-0.0.2.tar", last modified: Fri Apr  5 19:21:53 2024, max compression
```

## Comparing `StathamQuotes-0.0.1.tar` & `StathamQuotes-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-05 19:11:06.106830 StathamQuotes-0.0.1/
--rw-r--r--   0 apple      (501) staff       (20)      152 2024-04-05 19:11:06.106592 StathamQuotes-0.0.1/PKG-INFO
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-05 19:11:06.099147 StathamQuotes-0.0.1/StathamQuotes/
--rw-r--r--   0 apple      (501) staff       (20)       19 2024-04-05 19:07:27.000000 StathamQuotes-0.0.1/StathamQuotes/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      803 2024-04-05 19:09:20.000000 StathamQuotes-0.0.1/StathamQuotes/main.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-05 19:11:06.105676 StathamQuotes-0.0.1/StathamQuotes.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)      152 2024-04-05 19:11:06.000000 StathamQuotes-0.0.1/StathamQuotes.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      250 2024-04-05 19:11:06.000000 StathamQuotes-0.0.1/StathamQuotes.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2024-04-05 19:11:06.000000 StathamQuotes-0.0.1/StathamQuotes.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        7 2024-04-05 19:11:06.000000 StathamQuotes-0.0.1/StathamQuotes.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)       14 2024-04-05 19:11:06.000000 StathamQuotes-0.0.1/StathamQuotes.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)       38 2024-04-05 19:11:06.107636 StathamQuotes-0.0.1/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      318 2024-04-05 19:10:55.000000 StathamQuotes-0.0.1/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-05 19:21:53.149021 StathamQuotes-0.0.2/
+-rw-r--r--   0 apple      (501) staff       (20)      130 2024-04-05 19:21:53.148859 StathamQuotes-0.0.2/PKG-INFO
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-05 19:21:53.144932 StathamQuotes-0.0.2/StathamQuotes/
+-rw-r--r--   0 apple      (501) staff       (20)       19 2024-04-05 19:07:27.000000 StathamQuotes-0.0.2/StathamQuotes/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)      803 2024-04-05 19:09:20.000000 StathamQuotes-0.0.2/StathamQuotes/main.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-04-05 19:21:53.148156 StathamQuotes-0.0.2/StathamQuotes.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)      130 2024-04-05 19:21:53.000000 StathamQuotes-0.0.2/StathamQuotes.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      214 2024-04-05 19:21:53.000000 StathamQuotes-0.0.2/StathamQuotes.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-04-05 19:21:53.000000 StathamQuotes-0.0.2/StathamQuotes.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       14 2024-04-05 19:21:53.000000 StathamQuotes-0.0.2/StathamQuotes.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)       38 2024-04-05 19:21:53.149527 StathamQuotes-0.0.2/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      314 2024-04-05 19:21:43.000000 StathamQuotes-0.0.2/setup.py
```

### Comparing `StathamQuotes-0.0.1/StathamQuotes/main.py` & `StathamQuotes-0.0.2/StathamQuotes/main.py`

 * *Files identical despite different names*

