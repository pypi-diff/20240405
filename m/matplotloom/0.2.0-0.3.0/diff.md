# Comparing `tmp/matplotloom-0.2.0.tar.gz` & `tmp/matplotloom-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotloom-0.2.0.tar", max compression
+gzip compressed data, was "matplotloom-0.3.0.tar", max compression
```

## Comparing `matplotloom-0.2.0.tar` & `matplotloom-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-04-03 12:22:57.741227 matplotloom-0.2.0/LICENSE
--rw-r--r--   0        0        0       46 2024-04-03 12:22:57.741227 matplotloom-0.2.0/README.md
--rw-r--r--   0        0        0       23 2024-04-03 21:15:12.710441 matplotloom-0.2.0/matplotloom/__init__.py
--rw-r--r--   0        0        0     3356 2024-04-05 04:59:22.434786 matplotloom-0.2.0/matplotloom/loom.py
--rw-r--r--   0        0        0      416 2024-04-05 05:58:21.534921 matplotloom-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 matplotloom-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-05 12:53:08.255332 matplotloom-0.3.0/LICENSE
+-rw-r--r--   0        0        0       66 2024-04-05 12:53:08.255332 matplotloom-0.3.0/README.md
+-rw-r--r--   0        0        0       23 2024-04-05 12:53:08.255332 matplotloom-0.3.0/matplotloom/__init__.py
+-rw-r--r--   0        0        0     3393 2024-04-05 12:53:08.255332 matplotloom-0.3.0/matplotloom/loom.py
+-rw-r--r--   0        0        0      439 2024-04-05 12:53:08.255332 matplotloom-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 matplotloom-0.3.0/PKG-INFO
```

### Comparing `matplotloom-0.2.0/LICENSE` & `matplotloom-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotloom-0.2.0/matplotloom/loom.py` & `matplotloom-0.3.0/matplotloom/loom.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import subprocess
+from typing import Union
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import matplotlib.pyplot as plt
 import matplotlib.animation as anim
 
 from IPython.display import Video, Image
 
 class Loom:
     def __init__(
         self,
-        output_filepath: str | Path,
-        frames_directory: str | Path = Path(TemporaryDirectory().name),
+        output_filepath: Union[Path, str],
+        frames_directory: Union[Path, str] = Path(TemporaryDirectory().name),
         fps: int = 30,
         keep_frames: bool = False,
         overwrite: bool = False,
         verbose: bool = False,
         savefig_kwargs: dict = {}
     ) -> None:
         self.output_filepath = Path(output_filepath)
```

### Comparing `matplotloom-0.2.0/PKG-INFO` & `matplotloom-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: matplotloom
-Version: 0.2.0
-Summary: Easy matplotlib animations!
+Version: 0.3.0
+Summary: Weave your frames into easy matplotlib animations.
 License: MIT
 Author: ali-ramadhan
 Author-email: ali.hh.ramadhan@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,9 +14,10 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ipython (>=8.0.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # matplotloom
-Easy animations with matplotlib
+
+Weave your frames into easy matplotlib animations.
```

