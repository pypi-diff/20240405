# Comparing `tmp/supercut-0.3.0.tar.gz` & `tmp/supercut-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supercut-0.3.0.tar", max compression
+gzip compressed data, was "supercut-0.4.0.tar", max compression
```

## Comparing `supercut-0.3.0.tar` & `supercut-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1068 2024-04-04 09:14:15.049523 supercut-0.3.0/LICENSE
--rw-r--r--   0        0        0     5222 2024-04-04 09:14:15.049523 supercut-0.3.0/README.md
--rw-r--r--   0        0        0     1241 2024-04-04 09:14:15.049523 supercut-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/__init__.py
--rw-r--r--   0        0        0    10503 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/ffmpeg.py
--rw-r--r--   0        0        0     1442 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/subtitles.py
--rw-r--r--   0        0        0    15398 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/supercut.py
--rw-r--r--   0        0        0     2447 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/vlc.py
--rw-r--r--   0        0        0     5880 1970-01-01 00:00:00.000000 supercut-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-05 12:20:48.253283 supercut-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5222 2024-04-05 12:20:48.253283 supercut-0.4.0/README.md
+-rw-r--r--   0        0        0     1241 2024-04-05 12:20:48.257283 supercut-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 12:20:48.257283 supercut-0.4.0/src/supercut/__init__.py
+-rw-r--r--   0        0        0    10503 2024-04-05 12:20:48.257283 supercut-0.4.0/src/supercut/ffmpeg.py
+-rw-r--r--   0        0        0     4506 2024-04-05 12:20:48.257283 supercut-0.4.0/src/supercut/mlt.py
+-rw-r--r--   0        0        0     1442 2024-04-05 12:20:48.257283 supercut-0.4.0/src/supercut/subtitles.py
+-rw-r--r--   0        0        0    16919 2024-04-05 12:20:48.257283 supercut-0.4.0/src/supercut/supercut.py
+-rw-r--r--   0        0        0     2447 2024-04-05 12:20:48.257283 supercut-0.4.0/src/supercut/vlc.py
+-rw-r--r--   0        0        0     5880 1970-01-01 00:00:00.000000 supercut-0.4.0/PKG-INFO
```

### Comparing `supercut-0.3.0/LICENSE` & `supercut-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `supercut-0.3.0/README.md` & `supercut-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `supercut-0.3.0/pyproject.toml` & `supercut-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supercut"
-version = "0.3.0"
+version = "0.4.0"
 description = "Subtitle-based automatic supercut creation"
 authors = ["Tamir Bahar"]
 license = "MIT"
 readme = "README.md"
 
 
 [build-system]
```

### Comparing `supercut-0.3.0/src/supercut/ffmpeg.py` & `supercut-0.4.0/src/supercut/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `supercut-0.3.0/src/supercut/subtitles.py` & `supercut-0.4.0/src/supercut/subtitles.py`

 * *Files identical despite different names*

### Comparing `supercut-0.3.0/src/supercut/supercut.py` & `supercut-0.4.0/src/supercut/supercut.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import more_itertools
 import pysubs2  # type: ignore[import-untyped]
 import rich.console
 import rich.progress
 import rich.table
 import typer
 
-from supercut import ffmpeg, vlc
+from supercut import ffmpeg, mlt, vlc
 from supercut.subtitles import get_external_subs
 
 app = typer.Typer(
     help="Subtitle-based automatic supercut generator",
     pretty_exceptions_show_locals=False,
 )
 edit_app = typer.Typer(
@@ -205,14 +205,56 @@
                     end=event.end,
                 )
                 video_parts.append(part)
 
         ffmpeg.supercut_free(video_parts, output=output)
 
 
+@app.command()
+def export_mlt(
+    videos: typing.Annotated[
+        list[Path], typer.Argument(help="The videos to supercut, in order.")
+    ],
+    query: typing.Annotated[str, typer.Option(help="String to search in subtitles")],
+    output: typing.Annotated[Path, typer.Option(help="Ouptut file")],
+    language: typing.Annotated[
+        str, typer.Option(help="Subtitle language to use")
+    ] = "eng",
+    name: typing.Annotated[
+        Optional[str], typer.Option(help="Name of the speaker.")
+    ] = None,
+    cache_dir: typing.Annotated[
+        Optional[Path],
+        typer.Option(help="Cache directory location. Speeds up repeated runs."),
+    ] = None,
+    external_subs: typing.Annotated[
+        bool, typer.Option(help="Search for external subs.")
+    ] = False,
+):
+    """
+    Generate a ShotCut .mlt project of the supercut.
+    """
+    videos = sorted(videos)
+    with Core.from_dir(cache_dir, external_subs=external_subs) as core:
+        video_parts = []
+        all_subs = get_all_subs(videos, core, language)
+        for video, subs in zip(videos, all_subs):
+            events = query_events(subs, query, name=name)
+            for event in events:
+                part = ffmpeg.VideoPart(
+                    video=video,
+                    subs=trim_subs(subs, event.start, event.end).to_string("ass"),
+                    start=event.start,
+                    end=event.end,
+                )
+                video_parts.append(part)
+
+    output.write_text(mlt.write_mlt(video_parts))
+
+
 @app.command(name="list")
 def list_subs(
     videos: typing.Annotated[
         list[Path], typer.Argument(help="The videos to supercut, in order.")
     ],
     query: typing.Annotated[str, typer.Option(help="String to search in subtitles")],
     language: typing.Annotated[
```

### Comparing `supercut-0.3.0/src/supercut/vlc.py` & `supercut-0.4.0/src/supercut/vlc.py`

 * *Files identical despite different names*

### Comparing `supercut-0.3.0/PKG-INFO` & `supercut-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supercut
-Version: 0.3.0
+Version: 0.4.0
 Summary: Subtitle-based automatic supercut creation
 License: MIT
 Author: Tamir Bahar
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

