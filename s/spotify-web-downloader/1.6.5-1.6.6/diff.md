# Comparing `tmp/spotify_web_downloader-1.6.5.tar.gz` & `tmp/spotify_web_downloader-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_web_downloader-1.6.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spotify_web_downloader-1.6.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spotify_web_downloader-1.6.5.tar` & `spotify_web_downloader-1.6.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1137 2024-04-03 17:51:40.113597 spotify_web_downloader-1.6.5/.github/workflows/main.yml
--rw-r--r--   0        0        0       96 2024-04-03 17:51:40.113597 spotify_web_downloader-1.6.5/.gitignore
--rw-r--r--   0        0        0     8433 2024-04-03 17:51:40.113597 spotify_web_downloader-1.6.5/README.md
--rw-r--r--   0        0        0      533 2024-04-03 17:51:40.113597 spotify_web_downloader-1.6.5/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-03 17:51:40.113597 spotify_web_downloader-1.6.5/requirements.txt
--rw-r--r--   0        0        0       22 2024-04-03 17:51:40.113597 spotify_web_downloader-1.6.5/spotify_web_downloader/__init__.py
--rw-r--r--   0        0        0       30 2024-04-03 17:51:40.113597 spotify_web_downloader-1.6.5/spotify_web_downloader/__main__.py
--rw-r--r--   0        0        0    21483 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/cli.py
--rw-r--r--   0        0        0      507 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/constants.py
--rw-r--r--   0        0        0     8546 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/downloader.py
--rw-r--r--   0        0        0    11677 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/downloader_music_video.py
--rw-r--r--   0        0        0     9274 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/downloader_song.py
--rw-r--r--   0        0        0      177 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/enums.py
--rw-r--r--   0        0        0     4015 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/hardcoded_wvd.py
--rw-r--r--   0        0        0      707 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/models.py
--rw-r--r--   0        0        0     7738 2024-04-03 17:51:40.117597 spotify_web_downloader-1.6.5/spotify_web_downloader/spotify_api.py
--rw-r--r--   0        0        0     8844 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-05 14:54:24.724287 spotify_web_downloader-1.6.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2024-04-05 14:54:24.724287 spotify_web_downloader-1.6.6/.gitignore
+-rw-r--r--   0        0        0     8433 2024-04-05 14:54:24.724287 spotify_web_downloader-1.6.6/README.md
+-rw-r--r--   0        0        0      533 2024-04-05 14:54:24.724287 spotify_web_downloader-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/requirements.txt
+-rw-r--r--   0        0        0       22 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/__main__.py
+-rw-r--r--   0        0        0    21484 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/cli.py
+-rw-r--r--   0        0        0      507 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/constants.py
+-rw-r--r--   0        0        0     8546 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/downloader.py
+-rw-r--r--   0        0        0    11677 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/downloader_music_video.py
+-rw-r--r--   0        0        0     9274 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/downloader_song.py
+-rw-r--r--   0        0        0      177 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/hardcoded_wvd.py
+-rw-r--r--   0        0        0      707 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/models.py
+-rw-r--r--   0        0        0     7738 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/spotify_api.py
+-rw-r--r--   0        0        0     8844 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.6/PKG-INFO
```

### Comparing `spotify_web_downloader-1.6.5/.github/workflows/main.yml` & `spotify_web_downloader-1.6.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/README.md` & `spotify_web_downloader-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/pyproject.toml` & `spotify_web_downloader-1.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/spotify_web_downloader/cli.py` & `spotify_web_downloader-1.6.6/spotify_web_downloader/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
             and not downloader.nm3u8dlre_path_full
         ):
             logger.critical(X_NOT_FOUND_STRING.format("nm3u8dlre", nm3u8dlre_path))
             return
         if not spotify_api.is_premium and premium_quality:
             logger.critical("Cannot download in premium quality with a free account")
             return
-        if download_mode_video and not spotify_api.is_premium:
+        if not spotify_api.is_premium and download_music_video:
             logger.critical("Cannot download music videos with a free account")
             return
     error_count = 0
     if read_urls_as_txt:
         urls = [url.strip() for url in Path(urls[0]).read_text().splitlines()]
     for url_index, url in enumerate(urls, start=1):
         url_progress = f"URL {url_index}/{len(urls)}"
```

### Comparing `spotify_web_downloader-1.6.5/spotify_web_downloader/downloader.py` & `spotify_web_downloader-1.6.6/spotify_web_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/spotify_web_downloader/downloader_music_video.py` & `spotify_web_downloader-1.6.6/spotify_web_downloader/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/spotify_web_downloader/downloader_song.py` & `spotify_web_downloader-1.6.6/spotify_web_downloader/downloader_song.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/spotify_web_downloader/hardcoded_wvd.py` & `spotify_web_downloader-1.6.6/spotify_web_downloader/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/spotify_web_downloader/models.py` & `spotify_web_downloader-1.6.6/spotify_web_downloader/models.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/spotify_web_downloader/spotify_api.py` & `spotify_web_downloader-1.6.6/spotify_web_downloader/spotify_api.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.5/PKG-INFO` & `spotify_web_downloader-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-web-downloader
-Version: 1.6.5
+Version: 1.6.6
 Summary: Download songs/albums/playlists directly from Spotify in AAC
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: pybase62
 Requires-Dist: pywidevine
```

