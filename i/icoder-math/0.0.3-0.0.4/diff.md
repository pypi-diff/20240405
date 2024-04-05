# Comparing `tmp/icoder_math-0.0.3.tar.gz` & `tmp/icoder_math-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icoder_math-0.0.3.tar", last modified: Tue Apr  2 19:44:59 2024, max compression
+gzip compressed data, was "icoder_math-0.0.4.tar", last modified: Fri Apr  5 09:30:05 2024, max compression
```

## Comparing `icoder_math-0.0.3.tar` & `icoder_math-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 19:44:59.857834 icoder_math-0.0.3/
--rw-rw-rw-   0        0        0      279 2024-04-02 19:44:59.852838 icoder_math-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      683 2024-04-02 17:58:23.000000 icoder_math-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 19:44:59.720838 icoder_math-0.0.3/icoder_math/
--rw-rw-rw-   0        0        0       56 2024-04-02 19:44:00.000000 icoder_math-0.0.3/icoder_math/__init__.py
--rw-rw-rw-   0        0        0      517 2024-04-02 16:29:12.000000 icoder_math-0.0.3/icoder_math/calculate.py
-drwxrwxrwx   0        0        0        0 2024-04-02 19:44:59.849838 icoder_math-0.0.3/icoder_math.egg-info/
--rw-rw-rw-   0        0        0      279 2024-04-02 19:44:58.000000 icoder_math-0.0.3/icoder_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-02 19:44:58.000000 icoder_math-0.0.3/icoder_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 19:44:58.000000 icoder_math-0.0.3/icoder_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 19:44:58.000000 icoder_math-0.0.3/icoder_math.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 19:44:59.858835 icoder_math-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      407 2024-04-02 19:44:10.000000 icoder_math-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:30:05.204496 icoder_math-0.0.4/
+-rw-rw-rw-   0        0        0      279 2024-04-05 09:30:05.201492 icoder_math-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2024-04-02 17:58:23.000000 icoder_math-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 09:30:05.126530 icoder_math-0.0.4/icoder_math/
+-rw-rw-rw-   0        0        0       51 2024-04-05 09:24:23.000000 icoder_math-0.0.4/icoder_math/__init__.py
+-rw-rw-rw-   0        0        0      485 2024-04-03 06:28:42.000000 icoder_math-0.0.4/icoder_math/calculate.py
+-rw-rw-rw-   0        0        0     3677 2024-04-05 09:23:44.000000 icoder_math-0.0.4/icoder_math/frequency.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:30:05.198491 icoder_math-0.0.4/icoder_math.egg-info/
+-rw-rw-rw-   0        0        0      279 2024-04-05 09:30:03.000000 icoder_math-0.0.4/icoder_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-04-05 09:30:03.000000 icoder_math-0.0.4/icoder_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 09:30:03.000000 icoder_math-0.0.4/icoder_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-05 09:30:03.000000 icoder_math-0.0.4/icoder_math.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 09:30:05.204496 icoder_math-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      407 2024-04-03 06:27:42.000000 icoder_math-0.0.4/setup.py
```

### Comparing `icoder_math-0.0.3/README.md` & `icoder_math-0.0.4/README.md`

 * *Files identical despite different names*

