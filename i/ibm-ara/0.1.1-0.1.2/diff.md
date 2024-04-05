# Comparing `tmp/ibm_ara-0.1.1.tar.gz` & `tmp/ibm_ara-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm_ara-0.1.1.tar", max compression
+gzip compressed data, was "ibm_ara-0.1.2.tar", max compression
```

## Comparing `ibm_ara-0.1.1.tar` & `ibm_ara-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       45 2024-04-05 07:28:39.636381 ibm_ara-0.1.1/ibm_ara/__init__.py
--rw-r--r--   0        0        0     1773 2024-03-18 08:06:12.723518 ibm_ara-0.1.1/ibm_ara/myfunctions.py
--rw-r--r--   0        0        0      389 2024-04-05 07:35:32.631304 ibm_ara-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 12:14:08.327202 ibm_ara-0.1.1/README.md
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 ibm_ara-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-05 07:55:34.974895 ibm_ara-0.1.2/ibm_ara/__init__.py
+-rw-r--r--   0        0        0     1773 2024-03-18 08:06:12.723518 ibm_ara-0.1.2/ibm_ara/myfunctions/myfunctions.py
+-rw-r--r--   0        0        0      389 2024-04-05 07:58:45.091302 ibm_ara-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 12:14:08.327202 ibm_ara-0.1.2/README.md
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 ibm_ara-0.1.2/PKG-INFO
```

### Comparing `ibm_ara-0.1.1/ibm_ara/myfunctions.py` & `ibm_ara-0.1.2/ibm_ara/myfunctions/myfunctions.py`

 * *Files identical despite different names*

