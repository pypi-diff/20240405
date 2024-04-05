# Comparing `tmp/pants-backend-mdbook-0.3.0.tar.gz` & `tmp/pants_backend_mdbook-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants-backend-mdbook-0.3.0.tar", last modified: Tue Nov 21 17:15:26 2023, max compression
+gzip compressed data, was "pants_backend_mdbook-0.4.0.tar", last modified: Fri Apr  5 14:47:07 2024, max compression
```

## Comparing `pants-backend-mdbook-0.3.0.tar` & `pants_backend_mdbook-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/LICENSE-MIT.txt
--rw-r--r--   0        0        0      726 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/README.md
--rw-r--r--   0        0        0        9 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/__init__.py
--rw-r--r--   0        0        0       99 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/goals/__init__.py
--rw-r--r--   0        0        0     1022 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/goals/package.py
--rw-r--r--   0        0        0      255 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/register.py
--rw-r--r--   0        0        0     1440 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/subsystem.py
--rw-r--r--   0        0        0      727 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/targets.py
--rw-r--r--   0        0        0      153 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/util_rules/__init__.py
--rw-r--r--   0        0        0     1398 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/util_rules/build.py
--rw-r--r--   0        0        0     2088 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pants_backend_mdbook/util_rules/prepare.py
--rw-r--r--   0        0        0     1098 2023-11-21 17:15:26.254964 pants-backend-mdbook-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1412 1970-01-01 00:00:00.000000 pants-backend-mdbook-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/LICENSE-MIT.txt
+-rw-r--r--   0        0        0      726 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/README.md
+-rw-r--r--   0        0        0        9 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/goals/__init__.py
+-rw-r--r--   0        0        0     1022 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/goals/package.py
+-rw-r--r--   0        0        0      255 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/register.py
+-rw-r--r--   0        0        0     1440 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/subsystem.py
+-rw-r--r--   0        0        0      727 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/targets.py
+-rw-r--r--   0        0        0      153 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/build.py
+-rw-r--r--   0        0        0     2379 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/prepare.py
+-rw-r--r--   0        0        0     1093 2024-04-05 14:47:07.983885 pants_backend_mdbook-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 pants_backend_mdbook-0.4.0/PKG-INFO
```

### Comparing `pants-backend-mdbook-0.3.0/LICENSE-MIT.txt` & `pants_backend_mdbook-0.4.0/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `pants-backend-mdbook-0.3.0/README.md` & `pants_backend_mdbook-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pants-backend-mdbook-0.3.0/pants_backend_mdbook/goals/package.py` & `pants_backend_mdbook-0.4.0/pants_backend_mdbook/goals/package.py`

 * *Files identical despite different names*

### Comparing `pants-backend-mdbook-0.3.0/pants_backend_mdbook/subsystem.py` & `pants_backend_mdbook-0.4.0/pants_backend_mdbook/subsystem.py`

 * *Files identical despite different names*

### Comparing `pants-backend-mdbook-0.3.0/pants_backend_mdbook/targets.py` & `pants_backend_mdbook-0.4.0/pants_backend_mdbook/targets.py`

 * *Files identical despite different names*

### Comparing `pants-backend-mdbook-0.3.0/pants_backend_mdbook/util_rules/build.py` & `pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/build.py`

 * *Files identical despite different names*

### Comparing `pants-backend-mdbook-0.3.0/pyproject.toml` & `pants_backend_mdbook-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pants_backend_mdbook"
 description = "A  MdBook documentation builder plugin for the Pants buildsystem."
-version = "0.3.0"
+version = "0.4.0"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = []
 readme = "README.md"
 keywords = [
     "pantsbuild",
@@ -42,10 +42,10 @@
 include_trailing_comma = true
 
 [tool.black]
 line-length = 100
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend>2.0",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

