# Comparing `tmp/windowsregistry-0.1.0.tar.gz` & `tmp/windowsregistry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windowsregistry-0.1.0.tar", max compression
+gzip compressed data, was "windowsregistry-0.1.1.tar", max compression
```

## Comparing `windowsregistry-0.1.0.tar` & `windowsregistry-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      447 2024-04-04 11:39:58.991658 windowsregistry-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-20 15:48:08.622855 windowsregistry-0.1.0/README.md
--rw-r--r--   0        0        0      448 2024-04-03 12:47:24.791368 windowsregistry-0.1.0/windowsregistry/__init__.py
--rw-r--r--   0        0        0     4284 2024-04-03 15:01:34.954247 windowsregistry-0.1.0/windowsregistry/_backend.py
--rw-r--r--   0        0        0     1510 2024-04-03 15:02:11.711534 windowsregistry-0.1.0/windowsregistry/_lowlevel.py
--rw-r--r--   0        0        0     5146 2024-04-03 12:43:00.032892 windowsregistry-0.1.0/windowsregistry/core.py
--rw-r--r--   0        0        0       50 2024-01-20 16:09:24.321620 windowsregistry-0.1.0/windowsregistry/errors.py
--rw-r--r--   0        0        0      522 2024-04-02 10:07:41.474792 windowsregistry-0.1.0/windowsregistry/models/__init__.py
--rw-r--r--   0        0        0      434 2024-04-02 10:07:41.476324 windowsregistry-0.1.0/windowsregistry/models/data.py
--rw-r--r--   0        0        0     2777 2024-04-01 13:51:14.444092 windowsregistry-0.1.0/windowsregistry/models/enums.py
--rw-r--r--   0        0        0     2300 2024-04-03 12:33:54.931151 windowsregistry-0.1.0/windowsregistry/regpath.py
--rw-r--r--   0        0        0      377 2024-04-02 15:35:52.786369 windowsregistry-0.1.0/windowsregistry/utils.py
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 windowsregistry-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1120 2024-04-05 12:39:11.058256 windowsregistry-0.1.1/LICENSE
+-rw-r--r--   0        0        0      464 2024-04-05 12:39:11.059283 windowsregistry-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-20 15:48:08.622855 windowsregistry-0.1.1/README.md
+-rw-r--r--   0        0        0      476 2024-04-05 12:39:11.060258 windowsregistry-0.1.1/windowsregistry/__init__.py
+-rw-r--r--   0        0        0     4284 2024-04-03 15:01:34.954247 windowsregistry-0.1.1/windowsregistry/_backend.py
+-rw-r--r--   0        0        0     1510 2024-04-03 15:02:11.711534 windowsregistry-0.1.1/windowsregistry/_lowlevel.py
+-rw-r--r--   0        0        0     5146 2024-04-04 15:00:34.353575 windowsregistry-0.1.1/windowsregistry/core.py
+-rw-r--r--   0        0        0       50 2024-01-20 16:09:24.321620 windowsregistry-0.1.1/windowsregistry/errors.py
+-rw-r--r--   0        0        0      522 2024-04-02 10:07:41.474792 windowsregistry-0.1.1/windowsregistry/models/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-02 10:07:41.476324 windowsregistry-0.1.1/windowsregistry/models/data.py
+-rw-r--r--   0        0        0     2777 2024-04-01 13:51:14.444092 windowsregistry-0.1.1/windowsregistry/models/enums.py
+-rw-r--r--   0        0        0     2300 2024-04-03 12:33:54.931151 windowsregistry-0.1.1/windowsregistry/regpath.py
+-rw-r--r--   0        0        0      377 2024-04-02 15:35:52.786369 windowsregistry-0.1.1/windowsregistry/utils.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 windowsregistry-0.1.1/PKG-INFO
```

### Comparing `windowsregistry-0.1.0/windowsregistry/_backend.py` & `windowsregistry-0.1.1/windowsregistry/_backend.py`

 * *Files identical despite different names*

### Comparing `windowsregistry-0.1.0/windowsregistry/_lowlevel.py` & `windowsregistry-0.1.1/windowsregistry/_lowlevel.py`

 * *Files identical despite different names*

### Comparing `windowsregistry-0.1.0/windowsregistry/core.py` & `windowsregistry-0.1.1/windowsregistry/core.py`

 * *Files identical despite different names*

### Comparing `windowsregistry-0.1.0/windowsregistry/models/__init__.py` & `windowsregistry-0.1.1/windowsregistry/models/__init__.py`

 * *Files identical despite different names*

### Comparing `windowsregistry-0.1.0/windowsregistry/models/enums.py` & `windowsregistry-0.1.1/windowsregistry/models/enums.py`

 * *Files identical despite different names*

### Comparing `windowsregistry-0.1.0/windowsregistry/regpath.py` & `windowsregistry-0.1.1/windowsregistry/regpath.py`

 * *Files identical despite different names*

