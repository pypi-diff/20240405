# Comparing `tmp/seguid-0.0.5.tar.gz` & `tmp/seguid-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seguid-0.0.5.tar", max compression
+gzip compressed data, was "seguid-0.0.6.tar", max compression
```

## Comparing `seguid-0.0.5.tar` & `seguid-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1092 2024-02-24 08:04:03.542547 seguid-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     1585 2024-03-02 07:57:23.509033 seguid-0.0.5/README.md
--rw-r--r--   0        0        0      683 2024-03-02 08:51:57.786028 seguid-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      649 2024-03-02 08:43:38.317663 seguid-0.0.5/src/seguid/__init__.py
--rw-r--r--   0        0        0     2203 2024-03-02 07:57:27.053032 seguid-0.0.5/src/seguid/__main__.py
--rw-r--r--   0        0        0     3373 2024-03-02 07:57:27.053032 seguid-0.0.5/src/seguid/_asserts.py
--rw-r--r--   0        0        0     3503 2024-03-02 07:57:27.053032 seguid-0.0.5/src/seguid/_manip.py
--rw-r--r--   0        0        0     1398 2024-03-02 07:57:27.053032 seguid-0.0.5/src/seguid/_tables.py
--rw-r--r--   0        0        0     8455 2024-03-02 07:57:27.053032 seguid-0.0.5/src/seguid/chksum.py
--rw-r--r--   0        0        0      765 2024-03-02 07:57:27.053032 seguid-0.0.5/src/seguid/config.py
--rw-r--r--   0        0        0     3001 2024-03-02 07:57:27.053032 seguid-0.0.5/src/seguid/reprutils.py
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 seguid-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-05 16:04:17.488066 seguid-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1585 2024-04-05 16:04:17.492066 seguid-0.0.6/README.md
+-rw-r--r--   0        0        0      683 2024-04-05 16:04:17.492066 seguid-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      649 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/__init__.py
+-rw-r--r--   0        0        0     2203 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/__main__.py
+-rw-r--r--   0        0        0     3373 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/_asserts.py
+-rw-r--r--   0        0        0     3503 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/_manip.py
+-rw-r--r--   0        0        0     1398 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/_tables.py
+-rw-r--r--   0        0        0     8455 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/chksum.py
+-rw-r--r--   0        0        0      765 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/config.py
+-rw-r--r--   0        0        0     3001 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/reprutils.py
+-rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 seguid-0.0.6/PKG-INFO
```

### Comparing `seguid-0.0.5/LICENSE.txt` & `seguid-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/README.md` & `seguid-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/pyproject.toml` & `seguid-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seguid"
-version = "0.0.5"
+version = "0.0.6"
 description = "Sequence Globally Unique Identifier (SEGUID) Checksums for Linear, Circular, Single-Stranded and Double-Stranded Biological Sequences"
 authors = [
   "Bjorn Johansson <bjornjobb@gmail.com>",
   "Henrik Bengtsson",
   "Louis Abraham"
 ]
 license = "MIT"
```

### Comparing `seguid-0.0.5/src/seguid/__init__.py` & `seguid-0.0.6/src/seguid/__init__.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/src/seguid/__main__.py` & `seguid-0.0.6/src/seguid/__main__.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/src/seguid/_asserts.py` & `seguid-0.0.6/src/seguid/_asserts.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/src/seguid/_manip.py` & `seguid-0.0.6/src/seguid/_manip.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/src/seguid/_tables.py` & `seguid-0.0.6/src/seguid/_tables.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/src/seguid/chksum.py` & `seguid-0.0.6/src/seguid/chksum.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/src/seguid/config.py` & `seguid-0.0.6/src/seguid/config.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/src/seguid/reprutils.py` & `seguid-0.0.6/src/seguid/reprutils.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.5/PKG-INFO` & `seguid-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seguid
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sequence Globally Unique Identifier (SEGUID) Checksums for Linear, Circular, Single-Stranded and Double-Stranded Biological Sequences
 License: MIT
 Author: Bjorn Johansson
 Author-email: bjornjobb@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

