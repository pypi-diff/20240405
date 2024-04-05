# Comparing `tmp/hexfrost_toolbox-0.1.1.tar.gz` & `tmp/hexfrost_toolbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexfrost_toolbox-0.1.1.tar", max compression
+gzip compressed data, was "hexfrost_toolbox-0.1.2.tar", max compression
```

## Comparing `hexfrost_toolbox-0.1.1.tar` & `hexfrost_toolbox-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2024-03-13 22:55:09.761005 hexfrost_toolbox-0.1.1/LICENSE
--rw-r--r--   0        0        0      118 2024-03-13 22:55:09.761005 hexfrost_toolbox-0.1.1/README.md
--rw-r--r--   0        0        0      453 2024-03-13 22:55:09.761005 hexfrost_toolbox-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       25 2024-03-13 22:55:09.761005 hexfrost_toolbox-0.1.1/toolbox/__init__.py
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 hexfrost_toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-05 12:46:09.356061 hexfrost_toolbox-0.1.2/LICENSE
+-rw-r--r--   0        0        0      118 2024-04-05 12:46:09.356061 hexfrost_toolbox-0.1.2/README.md
+-rw-r--r--   0        0        0      453 2024-04-05 12:46:09.356061 hexfrost_toolbox-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       25 2024-04-05 12:46:09.356061 hexfrost_toolbox-0.1.2/toolbox/__init__.py
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 hexfrost_toolbox-0.1.2/PKG-INFO
```

### Comparing `hexfrost_toolbox-0.1.1/LICENSE` & `hexfrost_toolbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hexfrost_toolbox-0.1.1/PKG-INFO` & `hexfrost_toolbox-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexfrost-toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: Open source library with useful tools for fast development apps on FastAPI, Aiogram and SQLAlchemy
 Author: Kaziamov
 Author-email: kaziamov@outlook.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

