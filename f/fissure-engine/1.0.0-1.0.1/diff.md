# Comparing `tmp/fissure_engine-1.0.0.tar.gz` & `tmp/fissure-engine-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fissure_engine-1.0.0.tar", last modified: Fri Apr  5 16:18:15 2024, max compression
+gzip compressed data, was "fissure-engine-1.0.1.tar", last modified: Fri Apr  5 16:33:36 2024, max compression
```

## Comparing `fissure_engine-1.0.0.tar` & `fissure-engine-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 16:18:15.793820 fissure_engine-1.0.0/
--rw-rw-rw-   0        0        0      387 2024-04-05 16:18:15.792820 fissure_engine-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 16:18:15.791812 fissure_engine-1.0.0/fissure_engine.egg-info/
--rw-rw-rw-   0        0        0      387 2024-04-05 16:18:15.000000 fissure_engine-1.0.0/fissure_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2024-04-05 16:18:15.000000 fissure_engine-1.0.0/fissure_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 16:18:15.000000 fissure_engine-1.0.0/fissure_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 16:18:15.000000 fissure_engine-1.0.0/fissure_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 16:18:15.793820 fissure_engine-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      706 2024-04-05 16:16:31.000000 fissure_engine-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:33:36.251317 fissure-engine-1.0.1/
+-rw-rw-rw-   0        0        0      485 2024-04-05 16:33:36.250322 fissure-engine-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 16:33:36.243318 fissure-engine-1.0.1/fissure_engine/
+-rw-rw-rw-   0        0        0        0 2024-04-05 16:22:54.000000 fissure-engine-1.0.1/fissure_engine/__init__.py
+-rw-rw-rw-   0        0        0    75962 2024-03-27 20:54:24.000000 fissure-engine-1.0.1/fissure_engine/common.py
+-rw-rw-rw-   0        0        0    17668 2024-04-05 16:29:31.000000 fissure-engine-1.0.1/fissure_engine/fissure_engine.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:33:36.249312 fissure-engine-1.0.1/fissure_engine.egg-info/
+-rw-rw-rw-   0        0        0      485 2024-04-05 16:33:36.000000 fissure-engine-1.0.1/fissure_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-05 16:33:36.000000 fissure-engine-1.0.1/fissure_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:33:36.000000 fissure-engine-1.0.1/fissure_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-05 16:33:36.000000 fissure-engine-1.0.1/fissure_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-05 16:33:36.000000 fissure-engine-1.0.1/fissure_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 16:33:36.251317 fissure-engine-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      749 2024-04-05 16:33:17.000000 fissure-engine-1.0.1/setup.py
```

