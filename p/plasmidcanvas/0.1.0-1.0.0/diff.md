# Comparing `tmp/plasmidcanvas-0.1.0.tar.gz` & `tmp/plasmidcanvas-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plasmidcanvas-0.1.0.tar", max compression
+gzip compressed data, was "plasmidcanvas-1.0.0.tar", max compression
```

## Comparing `plasmidcanvas-0.1.0.tar` & `plasmidcanvas-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1091 2024-01-22 09:28:27.604486 plasmidcanvas-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-01 19:28:32.485933 plasmidcanvas-0.1.0/plasmidcanvas/__init__.py
--rw-r--r--   0        0        0     6694 2024-04-02 21:18:53.789931 plasmidcanvas-0.1.0/plasmidcanvas/curvedtext.py
--rw-r--r--   0        0        0    21806 2024-04-03 19:40:18.414282 plasmidcanvas-0.1.0/plasmidcanvas/feature.py
--rw-r--r--   0        0        0    13480 2024-04-03 19:15:52.602941 plasmidcanvas-0.1.0/plasmidcanvas/plasmid.py
--rw-r--r--   0        0        0    25280 2024-04-01 19:28:32.493935 plasmidcanvas-0.1.0/plasmidcanvas/sequence.gb
--rw-r--r--   0        0        0      870 2024-04-02 19:33:11.184805 plasmidcanvas-0.1.0/plasmidcanvas/utils.py
--rw-r--r--   0        0        0     1045 2024-04-03 20:00:07.714672 plasmidcanvas-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      147 2024-04-03 19:47:48.717070 plasmidcanvas-0.1.0/README.md
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 plasmidcanvas-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-01-22 09:28:27.604486 plasmidcanvas-1.0.0/LICENSE
+-rw-r--r--   0        0        0      637 2024-04-04 23:44:50.497744 plasmidcanvas-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1354 2024-04-04 17:37:01.461143 plasmidcanvas-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 22:03:37.968186 plasmidcanvas-1.0.0/src/plasmidcanvas/__init__.py
+-rw-r--r--   0        0        0     6694 2024-04-03 22:03:37.969187 plasmidcanvas-1.0.0/src/plasmidcanvas/_curvedtext.py
+-rw-r--r--   0        0        0      870 2024-04-03 22:03:37.973189 plasmidcanvas-1.0.0/src/plasmidcanvas/_utils.py
+-rw-r--r--   0        0        0    35684 2024-04-04 01:34:50.815052 plasmidcanvas-1.0.0/src/plasmidcanvas/feature.py
+-rw-r--r--   0        0        0    26804 2024-04-04 23:26:50.181033 plasmidcanvas-1.0.0/src/plasmidcanvas/plasmid.py
+-rw-r--r--   0        0        0    25280 2024-04-03 22:03:37.972192 plasmidcanvas-1.0.0/src/plasmidcanvas/sequence.gb
+-rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 plasmidcanvas-1.0.0/PKG-INFO
```

### Comparing `plasmidcanvas-0.1.0/LICENSE` & `plasmidcanvas-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plasmidcanvas-0.1.0/plasmidcanvas/curvedtext.py` & `plasmidcanvas-1.0.0/src/plasmidcanvas/_curvedtext.py`

 * *Files identical despite different names*

### Comparing `plasmidcanvas-0.1.0/plasmidcanvas/sequence.gb` & `plasmidcanvas-1.0.0/src/plasmidcanvas/sequence.gb`

 * *Files identical despite different names*

### Comparing `plasmidcanvas-0.1.0/plasmidcanvas/utils.py` & `plasmidcanvas-1.0.0/src/plasmidcanvas/_utils.py`

 * *Files identical despite different names*

