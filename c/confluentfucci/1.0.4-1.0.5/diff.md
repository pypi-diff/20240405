# Comparing `tmp/confluentfucci-1.0.4.tar.gz` & `tmp/confluentfucci-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluentfucci-1.0.4.tar", max compression
+gzip compressed data, was "confluentfucci-1.0.5.tar", max compression
```

## Comparing `confluentfucci-1.0.4.tar` & `confluentfucci-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2024-03-01 17:28:22.472316 confluentfucci-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1617 2024-03-01 17:28:22.472316 confluentfucci-1.0.4/README.md
--rw-r--r--   0        0        0      351 2024-03-01 17:28:22.472316 confluentfucci-1.0.4/confluentfucci/__init__.py
--rw-r--r--   0        0        0     4553 2024-03-01 17:28:22.472316 confluentfucci-1.0.4/confluentfucci/data.py
--rw-r--r--   0        0        0    26137 2024-03-01 17:28:22.472316 confluentfucci-1.0.4/confluentfucci/gui.py
--rw-r--r--   0        0        0    28458 2024-03-01 17:28:22.472316 confluentfucci-1.0.4/confluentfucci/math.py
--rw-r--r--   0        0        0     6073 2024-03-01 17:28:22.472316 confluentfucci-1.0.4/confluentfucci/utils.py
--rw-r--r--   0        0        0     2796 2024-03-01 17:30:15.584260 confluentfucci-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 confluentfucci-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-03-01 17:59:42.693348 confluentfucci-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1617 2024-03-01 17:59:42.693348 confluentfucci-1.0.5/README.md
+-rw-r--r--   0        0        0      351 2024-03-01 17:59:42.693348 confluentfucci-1.0.5/confluentfucci/__init__.py
+-rw-r--r--   0        0        0     4553 2024-03-01 17:59:42.693348 confluentfucci-1.0.5/confluentfucci/data.py
+-rw-r--r--   0        0        0    26137 2024-03-01 17:59:42.693348 confluentfucci-1.0.5/confluentfucci/gui.py
+-rw-r--r--   0        0        0    28458 2024-03-01 17:59:42.693348 confluentfucci-1.0.5/confluentfucci/math.py
+-rw-r--r--   0        0        0     6073 2024-03-01 17:59:42.693348 confluentfucci-1.0.5/confluentfucci/utils.py
+-rw-r--r--   0        0        0     2796 2024-03-01 18:01:32.834593 confluentfucci-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 confluentfucci-1.0.5/PKG-INFO
```

### Comparing `confluentfucci-1.0.4/LICENSE.txt` & `confluentfucci-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `confluentfucci-1.0.4/README.md` & `confluentfucci-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `confluentfucci-1.0.4/confluentfucci/data.py` & `confluentfucci-1.0.5/confluentfucci/data.py`

 * *Files identical despite different names*

### Comparing `confluentfucci-1.0.4/confluentfucci/gui.py` & `confluentfucci-1.0.5/confluentfucci/gui.py`

 * *Files identical despite different names*

### Comparing `confluentfucci-1.0.4/confluentfucci/math.py` & `confluentfucci-1.0.5/confluentfucci/math.py`

 * *Files identical despite different names*

### Comparing `confluentfucci-1.0.4/confluentfucci/utils.py` & `confluentfucci-1.0.5/confluentfucci/utils.py`

 * *Files identical despite different names*

### Comparing `confluentfucci-1.0.4/pyproject.toml` & `confluentfucci-1.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ConfluentFUCCI"
-version = "1.0.4"
+version = "1.0.5"
 description = ""
 authors = ["Leo Goldstien <leogoldstien@gmail.com>"]
 readme = "README.md"
 packages = [{include = "confluentfucci"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `confluentfucci-1.0.4/PKG-INFO` & `confluentfucci-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluentfucci
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: Leo Goldstien
 Author-email: leogoldstien@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

