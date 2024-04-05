# Comparing `tmp/media-archon-0.1.3.tar.gz` & `tmp/media-archon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media-archon-0.1.3.tar", last modified: Mon Oct  2 02:45:21 2023, max compression
+gzip compressed data, was "media-archon-0.1.4.tar", last modified: Fri Apr  5 20:49:56 2024, max compression
```

## Comparing `media-archon-0.1.3.tar` & `media-archon-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34523 2022-07-24 22:09:44.179046 media-archon-0.1.3/LICENSE
--rw-r--r--   0        0        0     3284 2023-10-02 02:30:09.228328 media-archon-0.1.3/README.md
--rw-r--r--   0        0        0      144 2023-10-02 02:43:11.860467 media-archon-0.1.3/media_archon/__about__.py
--rw-r--r--   0        0        0      122 2022-07-25 00:49:58.551757 media-archon-0.1.3/media_archon/__init__.py
--rw-r--r--   0        0        0      153 2022-07-28 01:50:56.484002 media-archon-0.1.3/media_archon/__main__.py
--rw-r--r--   0        0        0     1217 2022-08-07 15:45:29.917344 media-archon-0.1.3/media_archon/cli.py
--rw-r--r--   0        0        0    17785 2022-08-07 19:56:06.553894 media-archon-0.1.3/media_archon/walker.py
--rw-r--r--   0        0        0     1655 2023-10-02 02:29:14.318010 media-archon-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      122 2022-07-25 00:50:06.707501 media-archon-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 media-archon-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-07-24 22:09:44.179046 media-archon-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3284 2023-10-02 02:30:09.228328 media-archon-0.1.4/README.md
+-rw-r--r--   0        0        0      144 2024-04-05 19:25:15.992239 media-archon-0.1.4/media_archon/__about__.py
+-rw-r--r--   0        0        0      122 2022-07-25 00:49:58.551757 media-archon-0.1.4/media_archon/__init__.py
+-rw-r--r--   0        0        0      153 2022-07-28 01:50:56.484002 media-archon-0.1.4/media_archon/__main__.py
+-rw-r--r--   0        0        0     1324 2024-04-05 19:24:23.841807 media-archon-0.1.4/media_archon/cli.py
+-rw-r--r--   0        0        0    17785 2022-08-07 19:56:06.553894 media-archon-0.1.4/media_archon/walker.py
+-rw-r--r--   0        0        0     1655 2023-10-02 02:29:14.318010 media-archon-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      122 2022-07-25 00:50:06.707501 media-archon-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 media-archon-0.1.4/PKG-INFO
```

### Comparing `media-archon-0.1.3/LICENSE` & `media-archon-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `media-archon-0.1.3/README.md` & `media-archon-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `media-archon-0.1.3/media_archon/cli.py` & `media-archon-0.1.4/media_archon/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,19 +22,29 @@
     exit(-1)
 
 
 @click.command()
 @click.option(
     "-c",
     "--config",
-    type=click.Path(exists=False),
+    type=click.Path(
+        exists=False,
+        path_type=Path,
+    ),
     help="Specify a config file.",
 )
 @click.argument(
-    "src", type=click.Path(exists=True, file_okay=False, dir_okay=True, readable=True)
+    "src",
+    type=click.Path(
+        exists=True,
+        file_okay=False,
+        dir_okay=True,
+        readable=True,
+        path_type=Path,
+    ),
 )
 @click.version_option()
 def main(config: Optional[Path], src: Path) -> None:
     try:
         ranger = Walker.from_toml(src_dir=src, config_path=config)
     except FileNotFoundError:
         click.echo(f"Could not find configuration file {CONFIG_FILE_NAME}.\n")
```

### Comparing `media-archon-0.1.3/media_archon/walker.py` & `media-archon-0.1.4/media_archon/walker.py`

 * *Files identical despite different names*

### Comparing `media-archon-0.1.3/pyproject.toml` & `media-archon-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.10",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Operating System :: POSIX :: BSD",
     "Operating System :: Unix",
     "Intended Audience :: End Users/Desktop",
 ]
-version = "0.1.3"
+version = "0.1.4"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.scripts]
 media-archon = "media_archon.cli:main"
```

### Comparing `media-archon-0.1.3/PKG-INFO` & `media-archon-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-archon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Mirror a directory tree of media files, converting the files to a new format if newer or missing
 License: AGPL-3.0-or-later
 Author-email: Matthew Swabey <matthew@swabey.org>
 Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

