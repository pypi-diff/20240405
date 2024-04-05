# Comparing `tmp/kv-fs-0.1.0.tar.gz` & `tmp/kv-fs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv-fs-0.1.0.tar", last modified: Thu Apr  4 15:30:25 2024, max compression
+gzip compressed data, was "kv-fs-0.1.1.tar", last modified: Thu Apr  4 15:31:42 2024, max compression
```

## Comparing `kv-fs-0.1.0.tar` & `kv-fs-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:30:25.169926 kv-fs-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      279 2024-04-04 15:30:25.169926 kv-fs-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-03 05:12:32.000000 kv-fs-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      508 2024-04-03 05:14:19.000000 kv-fs-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 15:30:25.169926 kv-fs-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:30:25.169926 kv-fs-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:30:25.169926 kv-fs-0.1.0/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:30:25.169926 kv-fs-0.1.0/src/kv/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-03 06:44:38.000000 kv-fs-0.1.0/src/kv/fs/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:30:25.169926 kv-fs-0.1.0/src/kv/fs/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-03 07:40:08.000000 kv-fs-0.1.0/src/kv/fs/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2589 2024-04-04 07:14:35.000000 kv-fs-0.1.0/src/kv/fs/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:30:25.169926 kv-fs-0.1.0/src/kv/fs/api/json/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-03 07:40:26.000000 kv-fs-0.1.0/src/kv/fs/api/json/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-03 07:40:29.000000 kv-fs-0.1.0/src/kv/fs/api/json/json.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:30:25.169926 kv-fs-0.1.0/src/kv/fs/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-04 06:44:40.000000 kv-fs-0.1.0/src/kv/fs/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1891 2024-04-04 07:14:33.000000 kv-fs-0.1.0/src/kv/fs/ops/ops.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:30:25.169926 kv-fs-0.1.0/src/kv_fs.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      279 2024-04-04 15:30:25.000000 kv-fs-0.1.0/src/kv_fs.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      362 2024-04-04 15:30:25.000000 kv-fs-0.1.0/src/kv_fs.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 15:30:25.000000 kv-fs-0.1.0/src/kv_fs.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-04 15:30:25.000000 kv-fs-0.1.0/src/kv_fs.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-04 15:30:25.000000 kv-fs-0.1.0/src/kv_fs.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:31:42.933899 kv-fs-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      333 2024-04-04 15:31:42.933899 kv-fs-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-03 05:12:32.000000 kv-fs-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-04-04 15:31:39.000000 kv-fs-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 15:31:42.933899 kv-fs-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:31:42.933899 kv-fs-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:31:42.933899 kv-fs-0.1.1/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:31:42.933899 kv-fs-0.1.1/src/kv/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-03 06:44:38.000000 kv-fs-0.1.1/src/kv/fs/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:31:42.933899 kv-fs-0.1.1/src/kv/fs/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-03 07:40:08.000000 kv-fs-0.1.1/src/kv/fs/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2589 2024-04-04 07:14:35.000000 kv-fs-0.1.1/src/kv/fs/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:31:42.933899 kv-fs-0.1.1/src/kv/fs/api/json/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-03 07:40:26.000000 kv-fs-0.1.1/src/kv/fs/api/json/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-03 07:40:29.000000 kv-fs-0.1.1/src/kv/fs/api/json/json.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:31:42.933899 kv-fs-0.1.1/src/kv/fs/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-04 06:44:40.000000 kv-fs-0.1.1/src/kv/fs/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1891 2024-04-04 07:14:33.000000 kv-fs-0.1.1/src/kv/fs/ops/ops.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:31:42.933899 kv-fs-0.1.1/src/kv_fs.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      333 2024-04-04 15:31:42.000000 kv-fs-0.1.1/src/kv_fs.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      362 2024-04-04 15:31:42.000000 kv-fs-0.1.1/src/kv_fs.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 15:31:42.000000 kv-fs-0.1.1/src/kv_fs.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-04 15:31:42.000000 kv-fs-0.1.1/src/kv_fs.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-04 15:31:42.000000 kv-fs-0.1.1/src/kv_fs.egg-info/top_level.txt
```

### Comparing `kv-fs-0.1.0/src/kv/fs/api/api.py` & `kv-fs-0.1.1/src/kv/fs/api/api.py`

 * *Files identical despite different names*

### Comparing `kv-fs-0.1.0/src/kv/fs/ops/ops.py` & `kv-fs-0.1.1/src/kv/fs/ops/ops.py`

 * *Files identical despite different names*

