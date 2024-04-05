# Comparing `tmp/lxt-0.1.tar.gz` & `tmp/lxt-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxt-0.1.tar", last modified: Tue Apr  2 16:56:33 2024, max compression
+gzip compressed data, was "lxt-0.5.tar", last modified: Fri Apr  5 15:43:28 2024, max compression
```

## Comparing `lxt-0.1.tar` & `lxt-0.5.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-02 16:56:33.848002 lxt-0.1/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     2156 2024-04-02 16:36:14.000000 lxt-0.1/LICENSE
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      281 2024-04-02 16:56:33.848002 lxt-0.1/PKG-INFO
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       30 2024-04-02 16:38:49.000000 lxt-0.1/README.md
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-02 16:56:33.848002 lxt-0.1/lxt/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       22 2024-04-02 16:40:25.000000 lxt-0.1/lxt/__init__.py
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-02 16:56:33.848002 lxt-0.1/lxt.egg-info/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      281 2024-04-02 16:56:33.000000 lxt-0.1/lxt.egg-info/PKG-INFO
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      176 2024-04-02 16:56:33.000000 lxt-0.1/lxt.egg-info/SOURCES.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        1 2024-04-02 16:56:33.000000 lxt-0.1/lxt.egg-info/dependency_links.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        6 2024-04-02 16:56:33.000000 lxt-0.1/lxt.egg-info/requires.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        4 2024-04-02 16:56:33.000000 lxt-0.1/lxt.egg-info/top_level.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       38 2024-04-02 16:56:33.848002 lxt-0.1/setup.cfg
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      486 2024-04-02 16:45:06.000000 lxt-0.1/setup.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 15:43:28.900796 lxt-0.5/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     2156 2024-04-05 14:07:44.000000 lxt-0.5/LICENSE
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5948 2024-04-05 15:43:28.900796 lxt-0.5/PKG-INFO
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5545 2024-04-05 15:40:42.000000 lxt-0.5/README.md
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 15:43:28.900796 lxt-0.5/lxt/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 14:07:44.000000 lxt-0.5/lxt/__init__.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      785 2024-04-05 14:18:02.000000 lxt-0.5/lxt/check.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    15189 2024-04-05 14:07:45.000000 lxt-0.5/lxt/core.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    14635 2024-04-05 14:16:05.000000 lxt-0.5/lxt/functional.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     2678 2024-04-05 14:07:45.000000 lxt-0.5/lxt/modules.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    13091 2024-04-05 14:28:12.000000 lxt-0.5/lxt/rules.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3435 2024-04-05 14:44:58.000000 lxt-0.5/lxt/utils.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 15:43:28.900796 lxt-0.5/lxt.egg-info/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5948 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/PKG-INFO
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      305 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/SOURCES.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        1 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/dependency_links.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       63 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/requires.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        4 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/top_level.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       38 2024-04-05 15:43:28.900796 lxt-0.5/setup.cfg
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      598 2024-04-05 15:20:00.000000 lxt-0.5/setup.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 15:43:28.900796 lxt-0.5/tests/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3799 2024-04-05 14:13:59.000000 lxt-0.5/tests/test_functional.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      717 2024-04-05 14:12:50.000000 lxt-0.5/tests/test_rules.py
```

### Comparing `lxt-0.1/LICENSE` & `lxt-0.5/LICENSE`

 * *Files identical despite different names*

