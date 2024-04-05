# Comparing `tmp/haskellian-0.2.2.tar.gz` & `tmp/haskellian-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-0.2.2.tar", last modified: Thu Apr  4 09:00:04 2024, max compression
+gzip compressed data, was "haskellian-0.2.3.tar", last modified: Fri Apr  5 18:01:18 2024, max compression
```

## Comparing `haskellian-0.2.2.tar` & `haskellian-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.599822 haskellian-0.2.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-04 09:00:04.599822 haskellian-0.2.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-04-02 04:47:51.000000 haskellian-0.2.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-04 08:58:13.000000 haskellian-0.2.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 09:00:04.599822 haskellian-0.2.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.589822 haskellian-0.2.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.589822 haskellian-0.2.2/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.589822 haskellian-0.2.2/src/haskellian/core/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-04-02 05:09:49.000000 haskellian-0.2.2/src/haskellian/core/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1111 2024-04-04 08:59:29.000000 haskellian-0.2.2/src/haskellian/core/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      412 2024-04-02 05:09:41.000000 haskellian-0.2.2/src/haskellian/core/lazy.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.589822 haskellian-0.2.2/src/haskellian.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-04 09:00:04.000000 haskellian-0.2.2/src/haskellian.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      265 2024-04-04 09:00:04.000000 haskellian-0.2.2/src/haskellian.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 09:00:04.000000 haskellian-0.2.2/src/haskellian.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-04 09:00:04.000000 haskellian-0.2.2/src/haskellian.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 18:01:18.137810 haskellian-0.2.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-05 18:01:18.137810 haskellian-0.2.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-04-02 04:47:51.000000 haskellian-0.2.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-05 18:01:15.000000 haskellian-0.2.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-05 18:01:18.137810 haskellian-0.2.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 18:01:18.127810 haskellian-0.2.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 18:01:18.137810 haskellian-0.2.3/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 18:01:18.137810 haskellian-0.2.3/src/haskellian/core/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-04-02 05:09:49.000000 haskellian-0.2.3/src/haskellian/core/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1111 2024-04-04 08:59:29.000000 haskellian-0.2.3/src/haskellian/core/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      412 2024-04-02 05:09:41.000000 haskellian-0.2.3/src/haskellian/core/lazy.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 18:01:18.137810 haskellian-0.2.3/src/haskellian.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-05 18:01:18.000000 haskellian-0.2.3/src/haskellian.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      265 2024-04-05 18:01:18.000000 haskellian-0.2.3/src/haskellian.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-05 18:01:18.000000 haskellian-0.2.3/src/haskellian.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-05 18:01:18.000000 haskellian-0.2.3/src/haskellian.egg-info/top_level.txt
```

### Comparing `haskellian-0.2.2/src/haskellian/core/funcs.py` & `haskellian-0.2.3/src/haskellian/core/funcs.py`

 * *Files identical despite different names*

