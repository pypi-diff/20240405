# Comparing `tmp/matplotloom-0.1.0.tar.gz` & `tmp/matplotloom-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotloom-0.1.0.tar", max compression
+gzip compressed data, was "matplotloom-0.2.0.tar", max compression
```

## Comparing `matplotloom-0.1.0.tar` & `matplotloom-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-04-03 12:22:57.741227 matplotloom-0.1.0/LICENSE
--rw-r--r--   0        0        0       46 2024-04-03 12:22:57.741227 matplotloom-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:59:24.094405 matplotloom-0.1.0/matplotloom/__init__.py
--rw-r--r--   0        0        0     3367 2024-04-03 21:03:32.286415 matplotloom-0.1.0/matplotloom/loom.py
--rw-r--r--   0        0        0      341 2024-04-03 21:00:30.342408 matplotloom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 matplotloom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-03 12:22:57.741227 matplotloom-0.2.0/LICENSE
+-rw-r--r--   0        0        0       46 2024-04-03 12:22:57.741227 matplotloom-0.2.0/README.md
+-rw-r--r--   0        0        0       23 2024-04-03 21:15:12.710441 matplotloom-0.2.0/matplotloom/__init__.py
+-rw-r--r--   0        0        0     3356 2024-04-05 04:59:22.434786 matplotloom-0.2.0/matplotloom/loom.py
+-rw-r--r--   0        0        0      416 2024-04-05 05:58:21.534921 matplotloom-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 matplotloom-0.2.0/PKG-INFO
```

### Comparing `matplotloom-0.1.0/LICENSE` & `matplotloom-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotloom-0.1.0/matplotloom/loom.py` & `matplotloom-0.2.0/matplotloom/loom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import subprocess
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import matplotlib.pyplot as plt
 import matplotlib.animation as anim
 
-# from IPython.display import Video, Image
+from IPython.display import Video, Image
 
 class Loom:
     def __init__(
         self,
         output_filepath: str | Path,
         frames_directory: str | Path = Path(TemporaryDirectory().name),
         fps: int = 30,
@@ -90,12 +90,12 @@
             print(stderr.decode())
 
         if not self.keep_frames:
             for frame_filename in self.frame_filepaths:
                 if frame_filename.exists():
                     frame_filename.unlink()
 
-    # def show(self):
-    #     if self.file_format in {"mp4", "mkv"}:
-    #         return Video(str(self.output_filepath))
-    #     elif self.file_format in {"gif", "apng"}:
-    #         return Image(str(self.output_filepath))
+    def show(self):
+        if self.file_format in {"mp4", "mkv"}:
+            return Video(str(self.output_filepath))
+        elif self.file_format in {"gif", "apng"}:
+            return Image(str(self.output_filepath))
```

