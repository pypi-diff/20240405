# Comparing `tmp/alyx_registrator-0.0.1.tar.gz` & `tmp/alyx_registrator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alyx_registrator-0.0.1.tar", last modified: Thu Mar 14 17:57:33 2024, max compression
+gzip compressed data, was "alyx_registrator-0.0.2.tar", last modified: Fri Apr  5 00:50:05 2024, max compression
```

## Comparing `alyx_registrator-0.0.1.tar` & `alyx_registrator-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6234 2024-03-14 17:57:24.109165 alyx_registrator-0.0.1/one_registrator/README.md
--rw-r--r--   0        0        0       52 2024-03-14 17:57:24.109165 alyx_registrator-0.0.1/one_registrator/__init__.py
--rw-r--r--   0        0        0    28212 2024-03-14 17:57:24.113165 alyx_registrator-0.0.1/one_registrator/registration.py
--rw-r--r--   0        0        0     9845 2024-03-14 17:57:24.113165 alyx_registrator-0.0.1/one_registrator/rules.json
--rw-r--r--   0        0        0     2904 2024-03-14 17:57:24.113165 alyx_registrator-0.0.1/one_registrator/utils.py
--rw-r--r--   0        0        0      660 2024-03-14 17:57:33.461088 alyx_registrator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6234 2024-04-05 00:49:56.033694 alyx_registrator-0.0.2/one_registrator/README.md
+-rw-r--r--   0        0        0       51 2024-04-05 00:49:56.033694 alyx_registrator-0.0.2/one_registrator/__init__.py
+-rw-r--r--   0        0        0    28212 2024-04-05 00:49:56.037694 alyx_registrator-0.0.2/one_registrator/registration.py
+-rw-r--r--   0        0        0     9845 2024-04-05 00:49:56.037694 alyx_registrator-0.0.2/one_registrator/rules.json
+-rw-r--r--   0        0        0     2904 2024-04-05 00:49:56.037694 alyx_registrator-0.0.2/one_registrator/utils.py
+-rw-r--r--   0        0        0      660 2024-04-05 00:50:05.969614 alyx_registrator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.2/PKG-INFO
```

### Comparing `alyx_registrator-0.0.1/one_registrator/README.md` & `alyx_registrator-0.0.2/one_registrator/README.md`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.1/one_registrator/registration.py` & `alyx_registrator-0.0.2/one_registrator/registration.py`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.1/one_registrator/rules.json` & `alyx_registrator-0.0.2/one_registrator/rules.json`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.1/one_registrator/utils.py` & `alyx_registrator-0.0.2/one_registrator/utils.py`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.1/pyproject.toml` & `alyx_registrator-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dependencies = [
     "numpy>=1.23",
     "alyx-connector>=1.16",
     "pandas>=1.4",
 ]
 requires-python = ">=3.11"
 dynamic = []
-version = "0.0.1"
+version = "0.0.2"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

