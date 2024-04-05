# Comparing `tmp/apptrackr-0.1.0.tar.gz` & `tmp/apptrackr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.0.tar", max compression
+gzip compressed data, was "apptrackr-0.1.1.tar", max compression
```

## Comparing `apptrackr-0.1.0.tar` & `apptrackr-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.0/README.md
--rw-r--r--   0        0        0     4772 2024-04-05 08:52:36.304435 apptrackr-0.1.0/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.0/apptrackr/model/__init__.py
--rw-r--r--   0        0        0      598 2024-04-04 18:12:10.777458 apptrackr-0.1.0/apptrackr/model/model.py
--rw-r--r--   0        0        0      412 2024-04-05 09:00:05.927908 apptrackr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.1/README.md
+-rw-r--r--   0        0        0     4772 2024-04-05 11:41:48.188446 apptrackr-0.1.1/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.1/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0      598 2024-04-04 18:12:10.777458 apptrackr-0.1.1/apptrackr/model/model.py
+-rw-r--r--   0        0        0      414 2024-04-05 11:46:28.424294 apptrackr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 apptrackr-0.1.1/PKG-INFO
```

### Comparing `apptrackr-0.1.0/apptrackr/main.py` & `apptrackr-0.1.1/apptrackr/main.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.1.0/apptrackr/model/model.py` & `apptrackr-0.1.1/apptrackr/model/model.py`

 * *Files identical despite different names*

