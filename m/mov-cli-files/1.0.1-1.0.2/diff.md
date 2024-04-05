# Comparing `tmp/mov-cli-files-1.0.1.tar.gz` & `tmp/mov-cli-files-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-files-1.0.1.tar", last modified: Fri Apr  5 05:59:33 2024, max compression
+gzip compressed data, was "mov-cli-files-1.0.2.tar", last modified: Fri Apr  5 06:01:58 2024, max compression
```

## Comparing `mov-cli-files-1.0.1.tar` & `mov-cli-files-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 05:59:33.371242 mov-cli-files-1.0.1/
--rw-rw-rw-   0        0        0     1085 2024-04-05 05:34:53.000000 mov-cli-files-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2970 2024-04-05 05:59:33.369243 mov-cli-files-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      574 2024-04-05 05:55:40.000000 mov-cli-files-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 05:59:33.354238 mov-cli-files-1.0.1/mov_cli_files/
--rw-rw-rw-   0        0        0      351 2024-04-05 05:54:56.000000 mov-cli-files-1.0.1/mov_cli_files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 05:59:33.366241 mov-cli-files-1.0.1/mov_cli_files/files/
--rw-rw-rw-   0        0        0       22 2024-03-21 12:20:57.000000 mov-cli-files-1.0.1/mov_cli_files/files/__init__.py
--rw-rw-rw-   0        0        0     2688 2024-04-05 05:58:46.000000 mov-cli-files-1.0.1/mov_cli_files/files/scraper.py
-drwxrwxrwx   0        0        0        0 2024-04-05 05:59:33.368241 mov-cli-files-1.0.1/mov_cli_files.egg-info/
--rw-rw-rw-   0        0        0     2970 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1377 2024-04-05 05:41:14.000000 mov-cli-files-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 05:59:33.371242 mov-cli-files-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 06:01:58.817435 mov-cli-files-1.0.2/
+-rw-rw-rw-   0        0        0     1085 2024-04-05 05:34:53.000000 mov-cli-files-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2970 2024-04-05 06:01:58.816435 mov-cli-files-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-04-05 05:55:40.000000 mov-cli-files-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 06:01:58.794429 mov-cli-files-1.0.2/mov_cli_files/
+-rw-rw-rw-   0        0        0      351 2024-04-05 06:01:35.000000 mov-cli-files-1.0.2/mov_cli_files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:01:58.812434 mov-cli-files-1.0.2/mov_cli_files/files/
+-rw-rw-rw-   0        0        0       22 2024-03-21 12:20:57.000000 mov-cli-files-1.0.2/mov_cli_files/files/__init__.py
+-rw-rw-rw-   0        0        0     2675 2024-04-05 06:00:40.000000 mov-cli-files-1.0.2/mov_cli_files/files/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:01:58.814436 mov-cli-files-1.0.2/mov_cli_files.egg-info/
+-rw-rw-rw-   0        0        0     2970 2024-04-05 06:01:58.000000 mov-cli-files-1.0.2/mov_cli_files.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-05 06:01:58.000000 mov-cli-files-1.0.2/mov_cli_files.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 06:01:58.000000 mov-cli-files-1.0.2/mov_cli_files.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-04-05 06:01:58.000000 mov-cli-files-1.0.2/mov_cli_files.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 06:01:58.000000 mov-cli-files-1.0.2/mov_cli_files.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1377 2024-04-05 05:41:14.000000 mov-cli-files-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 06:01:58.818436 mov-cli-files-1.0.2/setup.cfg
```

### Comparing `mov-cli-files-1.0.1/LICENSE` & `mov-cli-files-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-files-1.0.1/PKG-INFO` & `mov-cli-files-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-files
-Version: 1.0.1
+Version: 1.0.2
 Summary:  A mov-cli v4 plugin for watching files on your device.
 Author-email: Ananas <ananas@r3tr0ananas.lol>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-files-1.0.1/README.md` & `mov-cli-files-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mov-cli-files-1.0.1/mov_cli_files/files/scraper.py` & `mov-cli-files-1.0.2/mov_cli_files/files/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from mov_cli.scraper import Scraper
 from mov_cli import Single, Metadata, MetadataType
 import os
 from datetime import datetime
 
 __all__ = ("FilesScraper", )
 
-media_formats_playable_by_mpv = ["3g2", "3ga", "3gp", "3gpp", "aac", "ac3", "adt", "adts", "aif", "aifc", "aiff", "amr", "asf", "asx", "av", "avi", "bmp", "cue", "dat", "divx", "dv", "dvr-ms", "eac3", "evo", "f4v", "flac", "flc", "fli", "flv", "gif", "gsm", "ifo", "ismv", "ivf", "m1v", "m2p", "m2t", "m2ts", "m2v", "m3u", "m4a", "m4b", "m4p", "m4v", "mk3d", "mkv", "mod", "mov", "mp2", "mp2v", "mp3", "mp4", "mp4v", "mpe", "mpeg", "mpeg1", "mpeg2", "mpeg4", "mpg", "mpg2", "mpv", "mts", "mxf", "nsv", "nuv", "oga", "ogg", "ogm", "ogv", "ogx", "oma", "opus", "pva", "qt", "ra", "ram", "rm", "rmvb", "s3m", "sdp", "spx", "thd", "tivo", "tod", "tp", "ts", "tta", "vob", "voc", "vqf", "w64", "wav", "webm", "wma", "wmv", "wv", "xesc", "xspf"]
+video_extensions = ["3g2", "3ga", "3gp", "3gpp", "aac", "ac3", "adt", "adts", "aif", "aifc", "aiff", "amr", "asf", "asx", "av", "avi", "bmp", "cue", "dat", "divx", "dv", "dvr-ms", "eac3", "evo", "f4v", "flac", "flc", "fli", "flv", "gif", "gsm", "ifo", "ismv", "ivf", "m1v", "m2p", "m2t", "m2ts", "m2v", "m3u", "m4a", "m4b", "m4p", "m4v", "mk3d", "mkv", "mod", "mov", "mp2", "mp2v", "mp3", "mp4", "mp4v", "mpe", "mpeg", "mpeg1", "mpeg2", "mpeg4", "mpg", "mpg2", "mpv", "mts", "mxf", "nsv", "nuv", "oga", "ogg", "ogm", "ogv", "ogx", "oma", "opus", "pva", "qt", "ra", "ram", "rm", "rmvb", "s3m", "sdp", "spx", "thd", "tivo", "tod", "tp", "ts", "tta", "vob", "voc", "vqf", "w64", "wav", "webm", "wma", "wmv", "wv", "xesc", "xspf"]
 
 class FilesScraper(Scraper):
     def __init__(self, config: Config, http_client: HTTPClient) -> None:
         self.base_url = None
         super().__init__(config, http_client)
 
     def search(self, query: str, limit: int = 10) -> Generator[Metadata, Any, None]:
```

### Comparing `mov-cli-files-1.0.1/mov_cli_files.egg-info/PKG-INFO` & `mov-cli-files-1.0.2/mov_cli_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-files
-Version: 1.0.1
+Version: 1.0.2
 Summary:  A mov-cli v4 plugin for watching files on your device.
 Author-email: Ananas <ananas@r3tr0ananas.lol>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-files-1.0.1/pyproject.toml` & `mov-cli-files-1.0.2/pyproject.toml`

 * *Files identical despite different names*

