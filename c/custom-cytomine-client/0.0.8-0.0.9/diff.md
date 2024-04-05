# Comparing `tmp/custom_cytomine_client-0.0.8.tar.gz` & `tmp/custom_cytomine_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_cytomine_client-0.0.8.tar", max compression
+gzip compressed data, was "custom_cytomine_client-0.0.9.tar", max compression
```

## Comparing `custom_cytomine_client-0.0.8.tar` & `custom_cytomine_client-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.8/README.md
--rw-r--r--   0        0        0       82 2024-04-04 08:22:45.857833 custom_cytomine_client-0.0.8/custom_cytomine_client/__init__.py
--rw-r--r--   0        0        0     7084 2024-04-04 08:21:59.692699 custom_cytomine_client-0.0.8/custom_cytomine_client/converter.py
--rw-r--r--   0        0        0        0 2024-04-04 08:21:59.692773 custom_cytomine_client-0.0.8/custom_cytomine_client/interface/__init__.py
--rw-r--r--   0        0        0      667 2024-04-04 08:21:59.692900 custom_cytomine_client-0.0.8/custom_cytomine_client/interface/converter.py
--rw-r--r--   0        0        0        0 2024-04-04 08:21:59.693022 custom_cytomine_client-0.0.8/custom_cytomine_client/object/__init__.py
--rw-r--r--   0        0        0      594 2024-04-04 08:21:59.693147 custom_cytomine_client-0.0.8/custom_cytomine_client/object/converter.py
--rw-r--r--   0        0        0        0 2024-04-04 08:21:59.693627 custom_cytomine_client-0.0.8/custom_cytomine_client/util/__init__.py
--rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.8/custom_cytomine_client/util/custom_exception.py
--rw-r--r--   0        0        0     2220 2024-04-04 08:21:59.693785 custom_cytomine_client-0.0.8/custom_cytomine_client/util/fit_util.py
--rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.8/custom_cytomine_client/util/normal_util.py
--rw-r--r--   0        0        0      726 2024-04-04 08:22:45.854078 custom_cytomine_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.9/README.md
+-rw-r--r--   0        0        0      124 2024-04-04 08:28:30.381656 custom_cytomine_client-0.0.9/custom_cytomine_client/__init__.py
+-rw-r--r--   0        0        0     7084 2024-04-04 08:21:59.692699 custom_cytomine_client-0.0.9/custom_cytomine_client/converter.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:21:59.692773 custom_cytomine_client-0.0.9/custom_cytomine_client/interface/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-04 08:21:59.692900 custom_cytomine_client-0.0.9/custom_cytomine_client/interface/converter.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:21:59.693022 custom_cytomine_client-0.0.9/custom_cytomine_client/object/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-04 08:21:59.693147 custom_cytomine_client-0.0.9/custom_cytomine_client/object/converter.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:21:59.693627 custom_cytomine_client-0.0.9/custom_cytomine_client/util/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.9/custom_cytomine_client/util/custom_exception.py
+-rw-r--r--   0        0        0     2220 2024-04-04 08:21:59.693785 custom_cytomine_client-0.0.9/custom_cytomine_client/util/fit_util.py
+-rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.9/custom_cytomine_client/util/normal_util.py
+-rw-r--r--   0        0        0      726 2024-04-04 08:28:34.704166 custom_cytomine_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.9/PKG-INFO
```

### Comparing `custom_cytomine_client-0.0.8/custom_cytomine_client/converter.py` & `custom_cytomine_client-0.0.9/custom_cytomine_client/converter.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.0.8/custom_cytomine_client/interface/converter.py` & `custom_cytomine_client-0.0.9/custom_cytomine_client/interface/converter.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.0.8/custom_cytomine_client/object/converter.py` & `custom_cytomine_client-0.0.9/custom_cytomine_client/object/converter.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.0.8/custom_cytomine_client/util/fit_util.py` & `custom_cytomine_client-0.0.9/custom_cytomine_client/util/fit_util.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.0.8/pyproject.toml` & `custom_cytomine_client-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "custom-cytomine-client"
-version = "0.0.8"
+version = "0.0.9"
 description = "Custom Cytomine client for Python"
 authors = ["punrabbit <tjdmsch2201@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 annotated-types = "0.6.0"
```

### Comparing `custom_cytomine_client-0.0.8/PKG-INFO` & `custom_cytomine_client-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-cytomine-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Custom Cytomine client for Python
 Author: punrabbit
 Author-email: tjdmsch2201@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

