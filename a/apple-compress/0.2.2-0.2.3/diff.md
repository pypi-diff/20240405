# Comparing `tmp/apple_compress-0.2.2.tar.gz` & `tmp/apple_compress-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple_compress-0.2.2.tar", max compression
+gzip compressed data, was "apple_compress-0.2.3.tar", max compression
```

## Comparing `apple_compress-0.2.2.tar` & `apple_compress-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2024-01-16 15:48:13.491257 apple_compress-0.2.2/LICENSE
--rw-r--r--   0        0        0     1351 2024-01-16 15:48:13.491257 apple_compress-0.2.2/README.md
--rw-r--r--   0        0        0      243 2024-01-16 15:48:13.491257 apple_compress-0.2.2/apple_compress/__init__.py
--rw-r--r--   0        0        0     2661 2024-01-16 15:48:13.491257 apple_compress-0.2.2/apple_compress/__main__.py
--rw-r--r--   0        0        0      273 2024-01-16 15:48:13.491257 apple_compress-0.2.2/apple_compress/_lib.py
--rw-r--r--   0        0        0     2932 2024-01-16 15:48:13.491257 apple_compress-0.2.2/apple_compress/compress.py
--rw-r--r--   0        0        0      144 2024-01-16 15:48:13.491257 apple_compress-0.2.2/apple_compress/errors.py
--rw-r--r--   0        0        0      712 2024-01-16 15:48:13.491257 apple_compress-0.2.2/apple_compress/types.py
--rw-r--r--   0        0        0      681 2024-01-16 15:48:13.491257 apple_compress-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 apple_compress-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-05 00:06:16.258982 apple_compress-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1351 2024-04-05 00:06:16.258982 apple_compress-0.2.3/README.md
+-rw-r--r--   0        0        0      243 2024-04-05 00:06:16.258982 apple_compress-0.2.3/apple_compress/__init__.py
+-rw-r--r--   0        0        0     2674 2024-04-05 00:06:16.258982 apple_compress-0.2.3/apple_compress/__main__.py
+-rw-r--r--   0        0        0      273 2024-04-05 00:06:16.258982 apple_compress-0.2.3/apple_compress/_lib.py
+-rw-r--r--   0        0        0     2951 2024-04-05 00:06:16.258982 apple_compress-0.2.3/apple_compress/compress.py
+-rw-r--r--   0        0        0      144 2024-04-05 00:06:16.258982 apple_compress-0.2.3/apple_compress/errors.py
+-rw-r--r--   0        0        0      712 2024-04-05 00:06:16.258982 apple_compress-0.2.3/apple_compress/types.py
+-rw-r--r--   0        0        0      718 2024-04-05 00:06:16.258982 apple_compress-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 apple_compress-0.2.3/PKG-INFO
```

### Comparing `apple_compress-0.2.2/LICENSE` & `apple_compress-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apple_compress-0.2.2/README.md` & `apple_compress-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `apple_compress-0.2.2/apple_compress/__main__.py` & `apple_compress-0.2.3/apple_compress/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     """A Python CLI tool for compression using Apple's libcompression."""
 
     if verbose:
         logger.remove()
         logger.add(
             sys.stderr,
             level='DEBUG',
-            format='[{time:MMM D YYYY - hh:mm:ss A zz}] {level} {module}:{line} {message}',
+            format='[{time:MMM D YYYY - hh:mm:ss A zz}] {level} | {module}:{function}:{line} {message}',
         )
         logger.enable(__package__)
     else:
         sys.tracebacklimit = 0
 
     if sys.platform != 'darwin':
         click.echo('[ERROR] Only Darwin systems are supported. Exiting.')
```

### Comparing `apple_compress-0.2.2/apple_compress/compress.py` & `apple_compress-0.2.3/apple_compress/compress.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     Raises:
         CompressionError: If the decompression fails.
     """
     logger.info(
         f'Decompressing data ({len(data)} bytes) with algorithm: {algorithm.name}'
     )
 
-    if decmp_size is None:
+    if decmp_size is None or decmp_size == 0:
         logger.debug(
             f'No decompressed size provided, assuming data length * 2 ({len(data) * 2})'
         )
         decmp_size = len(data) * 2
 
     while True:
         logger.debug(f'Creating buffer of size: {decmp_size}')
```

### Comparing `apple_compress-0.2.2/apple_compress/types.py` & `apple_compress-0.2.3/apple_compress/types.py`

 * *Files identical despite different names*

### Comparing `apple_compress-0.2.2/pyproject.toml` & `apple_compress-0.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "apple-compress"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python bindings for Apple's libcompression."
 authors = ["m1stadev <adamhamdi31@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 acompress = "apple_compress.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.7"
 loguru = "^0.7.2"
 
+[tool.ruff]
+target-version = "py38"
+
 [tool.ruff.lint]
 extend-select = ["I"]
 ignore = ["E722"]
 
 [tool.ruff.format]
 quote-style = "single"
```

### Comparing `apple_compress-0.2.2/PKG-INFO` & `apple_compress-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apple-compress
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python bindings for Apple's libcompression.
 Author: m1stadev
 Author-email: adamhamdi31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

