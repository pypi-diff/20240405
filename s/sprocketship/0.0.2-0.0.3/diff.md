# Comparing `tmp/sprocketship-0.0.2.tar.gz` & `tmp/sprocketship-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.0.2.tar", last modified: Fri Apr  5 15:33:29 2024, max compression
+gzip compressed data, was "sprocketship-0.0.3.tar", last modified: Fri Apr  5 16:04:22 2024, max compression
```

## Comparing `sprocketship-0.0.2.tar` & `sprocketship-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:29.385696 sprocketship-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 15:33:24.000000 sprocketship-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8626 2024-04-05 15:33:29.385696 sprocketship-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-05 15:33:24.000000 sprocketship-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 15:33:24.000000 sprocketship-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:33:29.385696 sprocketship-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:29.385696 sprocketship-0.0.2/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-05 15:33:24.000000 sprocketship-0.0.2/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:29.385696 sprocketship-0.0.2/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8626 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 15:33:29.000000 sprocketship-0.0.2/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:04:22.122514 sprocketship-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 16:04:17.000000 sprocketship-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-05 16:04:22.118514 sprocketship-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-05 16:04:17.000000 sprocketship-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 16:04:17.000000 sprocketship-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:04:22.122514 sprocketship-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:04:22.118514 sprocketship-0.0.3/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-05 16:04:17.000000 sprocketship-0.0.3/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:04:22.118514 sprocketship-0.0.3/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.0.2/LICENSE` & `sprocketship-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.2/pyproject.toml` & `sprocketship-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
     "click",
     "snowflake",
```

### Comparing `sprocketship-0.0.2/sprocketship/cli.py` & `sprocketship-0.0.3/sprocketship/cli.py`

 * *Files identical despite different names*

