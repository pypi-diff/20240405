# Comparing `tmp/devine-3.3.0.tar.gz` & `tmp/devine-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devine-3.3.0.tar", max compression
+gzip compressed data, was "devine-3.3.1.tar", max compression
```

## Comparing `devine-3.3.0.tar` & `devine-3.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    54122 2024-04-02 21:00:25.663346 devine-3.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    35822 2024-04-02 21:00:25.663346 devine-3.3.0/LICENSE
--rw-r--r--   0        0        0    19888 2024-04-02 21:00:25.663346 devine-3.3.0/README.md
--rw-r--r--   0        0        0       80 2024-04-02 21:00:25.663346 devine-3.3.0/devine/__main__.py
--rw-r--r--   0        0        0        0 2024-04-02 21:00:25.663346 devine-3.3.0/devine/commands/__init__.py
--rw-r--r--   0        0        0     3254 2024-04-02 21:00:25.663346 devine-3.3.0/devine/commands/cfg.py
--rw-r--r--   0        0        0    45664 2024-04-02 21:00:25.663346 devine-3.3.0/devine/commands/dl.py
--rw-r--r--   0        0        0     2247 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/env.py
--rw-r--r--   0        0        0     7986 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/kv.py
--rw-r--r--   0        0        0     6574 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/search.py
--rw-r--r--   0        0        0     1743 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/serve.py
--rw-r--r--   0        0        0     9243 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/util.py
--rw-r--r--   0        0        0     9920 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/wvd.py
--rw-r--r--   0        0        0       22 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/__init__.py
--rw-r--r--   0        0        0     2857 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/__main__.py
--rw-r--r--   0        0        0     6195 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/cacher.py
--rw-r--r--   0        0        0     1215 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/commands.py
--rw-r--r--   0        0        0     4481 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/config.py
--rw-r--r--   0        0        0    15343 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/console.py
--rw-r--r--   0        0        0     1065 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/constants.py
--rw-r--r--   0        0        0     3380 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/credential.py
--rw-r--r--   0        0        0      159 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/downloaders/__init__.py
--rw-r--r--   0        0        0    13339 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/downloaders/aria2c.py
--rw-r--r--   0        0        0    11697 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/downloaders/curl_impersonate.py
--rw-r--r--   0        0        0    11931 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/downloaders/requests.py
--rw-r--r--   0        0        0      199 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/drm/__init__.py
--rw-r--r--   0        0        0     4020 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/drm/clearkey.py
--rw-r--r--   0        0        0    11898 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/drm/widevine.py
--rw-r--r--   0        0        0     2753 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/events.py
--rw-r--r--   0        0        0       71 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/manifests/__init__.py
--rw-r--r--   0        0        0    31228 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/manifests/dash.py
--rw-r--r--   0        0        0    28214 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/manifests/hls.py
--rw-r--r--   0        0        0      117 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/__init__.py
--rw-r--r--   0        0        0     1958 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/basic.py
--rw-r--r--   0        0        0     2290 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/hola.py
--rw-r--r--   0        0        0     5565 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/nordvpn.py
--rw-r--r--   0        0        0     1048 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/proxy.py
--rw-r--r--   0        0        0     1714 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/search_result.py
--rw-r--r--   0        0        0    12729 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/service.py
--rw-r--r--   0        0        0     3001 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/services.py
--rw-r--r--   0        0        0      298 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/__init__.py
--rw-r--r--   0        0        0     8002 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/episode.py
--rw-r--r--   0        0        0     5538 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/movie.py
--rw-r--r--   0        0        0     4689 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/song.py
--rw-r--r--   0        0        0     2595 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/title.py
--rw-r--r--   0        0        0      277 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/tracks/__init__.py
--rw-r--r--   0        0        0     2132 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/tracks/attachment.py
--rw-r--r--   0        0        0     5001 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/tracks/audio.py
--rw-r--r--   0        0        0     2961 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/chapter.py
--rw-r--r--   0        0        0     5352 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/chapters.py
--rw-r--r--   0        0        0    23318 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/subtitle.py
--rw-r--r--   0        0        0    21426 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/track.py
--rw-r--r--   0        0        0    17269 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/tracks.py
--rw-r--r--   0        0        0    13118 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/video.py
--rw-r--r--   0        0        0    10741 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utilities.py
--rw-r--r--   0        0        0        0 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/__init__.py
--rw-r--r--   0        0        0     6227 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/click_types.py
--rw-r--r--   0        0        0     1532 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/collections.py
--rw-r--r--   0        0        0     3699 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/sslciphers.py
--rw-r--r--   0        0        0      845 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/subprocess.py
--rw-r--r--   0        0        0      791 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/xml.py
--rw-r--r--   0        0        0     1711 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/vault.py
--rw-r--r--   0        0        0     2518 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/vaults.py
--rw-r--r--   0        0        0     6414 2024-04-02 21:00:25.671346 devine-3.3.0/devine/vaults/API.py
--rw-r--r--   0        0        0     8485 2024-04-02 21:00:25.671346 devine-3.3.0/devine/vaults/MySQL.py
--rw-r--r--   0        0        0     6076 2024-04-02 21:00:25.671346 devine-3.3.0/devine/vaults/SQLite.py
--rw-r--r--   0        0        0        0 2024-04-02 21:00:25.671346 devine-3.3.0/devine/vaults/__init__.py
--rw-r--r--   0        0        0     2650 2024-04-02 21:00:25.671346 devine-3.3.0/pyproject.toml
--rw-r--r--   0        0        0    22374 1970-01-01 00:00:00.000000 devine-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0    54605 2024-04-05 11:32:20.168872 devine-3.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35822 2024-04-05 11:32:20.168872 devine-3.3.1/LICENSE
+-rw-r--r--   0        0        0    20080 2024-04-05 11:32:20.168872 devine-3.3.1/README.md
+-rw-r--r--   0        0        0       80 2024-04-05 11:32:20.168872 devine-3.3.1/devine/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/__init__.py
+-rw-r--r--   0        0        0     3254 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/cfg.py
+-rw-r--r--   0        0        0    45886 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/dl.py
+-rw-r--r--   0        0        0     2247 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/env.py
+-rw-r--r--   0        0        0     7986 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/kv.py
+-rw-r--r--   0        0        0     6574 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/search.py
+-rw-r--r--   0        0        0     1743 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/serve.py
+-rw-r--r--   0        0        0     9243 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/util.py
+-rw-r--r--   0        0        0     9920 2024-04-05 11:32:20.172872 devine-3.3.1/devine/commands/wvd.py
+-rw-r--r--   0        0        0       22 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/__init__.py
+-rw-r--r--   0        0        0     2857 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/__main__.py
+-rw-r--r--   0        0        0     6195 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/cacher.py
+-rw-r--r--   0        0        0     1215 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/commands.py
+-rw-r--r--   0        0        0     4481 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/config.py
+-rw-r--r--   0        0        0    15343 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/console.py
+-rw-r--r--   0        0        0     1065 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/constants.py
+-rw-r--r--   0        0        0     3380 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/credential.py
+-rw-r--r--   0        0        0      159 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/downloaders/__init__.py
+-rw-r--r--   0        0        0    13339 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/downloaders/aria2c.py
+-rw-r--r--   0        0        0    11697 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/downloaders/curl_impersonate.py
+-rw-r--r--   0        0        0    11930 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/downloaders/requests.py
+-rw-r--r--   0        0        0      199 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/drm/__init__.py
+-rw-r--r--   0        0        0     4020 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/drm/clearkey.py
+-rw-r--r--   0        0        0    11898 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/drm/widevine.py
+-rw-r--r--   0        0        0     2818 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/events.py
+-rw-r--r--   0        0        0       71 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/manifests/__init__.py
+-rw-r--r--   0        0        0    31280 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/manifests/dash.py
+-rw-r--r--   0        0        0    28266 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/manifests/hls.py
+-rw-r--r--   0        0        0      117 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/__init__.py
+-rw-r--r--   0        0        0     1958 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/basic.py
+-rw-r--r--   0        0        0     2290 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/hola.py
+-rw-r--r--   0        0        0     5565 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/nordvpn.py
+-rw-r--r--   0        0        0     1048 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/proxy.py
+-rw-r--r--   0        0        0     1714 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/search_result.py
+-rw-r--r--   0        0        0    12729 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/service.py
+-rw-r--r--   0        0        0     3001 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/services.py
+-rw-r--r--   0        0        0      298 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/__init__.py
+-rw-r--r--   0        0        0     8002 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/episode.py
+-rw-r--r--   0        0        0     5538 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/movie.py
+-rw-r--r--   0        0        0     4689 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/song.py
+-rw-r--r--   0        0        0     2595 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/title.py
+-rw-r--r--   0        0        0      277 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/__init__.py
+-rw-r--r--   0        0        0     2132 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/attachment.py
+-rw-r--r--   0        0        0     5001 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/audio.py
+-rw-r--r--   0        0        0     2976 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/chapter.py
+-rw-r--r--   0        0        0     5352 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/chapters.py
+-rw-r--r--   0        0        0    23374 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/subtitle.py
+-rw-r--r--   0        0        0    21612 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/tracks/track.py
+-rw-r--r--   0        0        0    17269 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/tracks/tracks.py
+-rw-r--r--   0        0        0    13118 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/tracks/video.py
+-rw-r--r--   0        0        0    10741 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utilities.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/__init__.py
+-rw-r--r--   0        0        0     6227 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/click_types.py
+-rw-r--r--   0        0        0     1532 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/collections.py
+-rw-r--r--   0        0        0     3699 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/sslciphers.py
+-rw-r--r--   0        0        0      845 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/subprocess.py
+-rw-r--r--   0        0        0      791 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/xml.py
+-rw-r--r--   0        0        0     1711 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/vault.py
+-rw-r--r--   0        0        0     2518 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/vaults.py
+-rw-r--r--   0        0        0     6414 2024-04-05 11:32:20.176872 devine-3.3.1/devine/vaults/API.py
+-rw-r--r--   0        0        0     8485 2024-04-05 11:32:20.176872 devine-3.3.1/devine/vaults/MySQL.py
+-rw-r--r--   0        0        0     6076 2024-04-05 11:32:20.176872 devine-3.3.1/devine/vaults/SQLite.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:32:20.176872 devine-3.3.1/devine/vaults/__init__.py
+-rw-r--r--   0        0        0     2650 2024-04-05 11:32:20.176872 devine-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0    22566 1970-01-01 00:00:00.000000 devine-3.3.1/PKG-INFO
```

### Comparing `devine-3.3.0/CHANGELOG.md` & `devine-3.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,34 @@
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Versions [3.0.0] and older use a format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 but versions thereafter use a custom changelog format using [git-cliff](https://git-cliff.org).
 
+## [3.3.1] - 2024-04-05
+
+### Features
+
+- *dl*: Add *new* --workers to set download threads/workers
+
+### Bug Fixes
+
+- *Chapter*: Cast values to int prior to formatting
+- *requests*: Fix multithreaded downloads
+- *Events*: Dereference subscription store from ephemeral store
+
+### Changes
+
+- *dl*: Change --workers to --downloads
+
+### New Contributors
+
+- [knowhere01](https://github.com/knowhere01)
+
 ## [3.3.0] - 2024-04-02
 
 ### Features
 
 - Add support for MKV Attachments via Attachment class
 - *dl*: Automatically attach fonts used within SSAv4 subs
 - *dl*: Try find SSAv4 fonts in System OS fonts folder
@@ -744,14 +764,15 @@
 - Fixed crash when adding a Cookie using `auth add` to a Service that has no directory yet.
 - Fixed crash when adding a Credential using `auth add` when it's the first ever credential, or first for the Service.
 
 ## [1.0.0] - 2023-02-06
 
 Initial public release under the name Devine.
 
+[3.3.1]: https://github.com/devine-dl/devine/releases/tag/v3.3.1
 [3.3.0]: https://github.com/devine-dl/devine/releases/tag/v3.3.0
 [3.2.0]: https://github.com/devine-dl/devine/releases/tag/v3.2.0
 [3.1.0]: https://github.com/devine-dl/devine/releases/tag/v3.1.0
 [3.0.0]: https://github.com/devine-dl/devine/releases/tag/v3.0.0
 [2.2.0]: https://github.com/devine-dl/devine/releases/tag/v2.2.0
 [2.1.0]: https://github.com/devine-dl/devine/releases/tag/v2.1.0
 [2.0.1]: https://github.com/devine-dl/devine/releases/tag/v2.0.1
```

### Comparing `devine-3.3.0/LICENSE` & `devine-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/README.md` & `devine-3.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -337,14 +337,15 @@
 <a href="https://github.com/shirt-dev"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/2660574?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="shirt-dev"/></a>
 <a href="https://github.com/nyuszika7h"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/482367?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="nyuszika7h"/></a>
 <a href="https://github.com/bccornfo"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/98013276?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="bccornfo"/></a>
 <a href="https://github.com/Arias800"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/24809312?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Arias800"/></a>
 <a href="https://github.com/varyg1001"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/88599103?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="varyg1001"/></a>
 <a href="https://github.com/Hollander-1908"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/93162595?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Hollander-1908"/></a>
 <a href="https://github.com/Shivelight"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/20620780?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Shivelight"/></a>
+<a href="https://github.com/knowhere01"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/113712042?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="knowhere01"/></a>
 
 ## Licensing
 
 This software is licensed under the terms of [GNU General Public License, Version 3.0](LICENSE).  
 You can find a copy of the license in the LICENSE file in the root folder.
 
 * * *
```

### Comparing `devine-3.3.0/devine/commands/cfg.py` & `devine-3.3.1/devine/commands/cfg.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/commands/dl.py` & `devine-3.3.1/devine/commands/dl.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,18 @@
                   help="Only use CDM, or only use Key Vaults for retrieval of Decryption Keys.")
     @click.option("--no-proxy", is_flag=True, default=False,
                   help="Force disable all proxy use.")
     @click.option("--no-folder", is_flag=True, default=False,
                   help="Disable folder creation for TV Shows.")
     @click.option("--no-source", is_flag=True, default=False,
                   help="Disable the source tag from the output file name and path.")
-    @click.option("--workers", type=int, default=1,
-                  help="Max concurrent workers to use throughout the code, particularly downloads.")
+    @click.option("--workers", type=int, default=None,
+                  help="Max workers/threads to download with per-track. Default depends on the downloader.")
+    @click.option("--downloads", type=int, default=1,
+                  help="Amount of tracks to download concurrently.")
     @click.pass_context
     def cli(ctx: click.Context, **kwargs: Any) -> dl:
         return dl(ctx, **kwargs)
 
     DRM_TABLE_LOCK = Lock()
 
     def __init__(
@@ -271,15 +273,16 @@
         list_titles: bool,
         skip_dl: bool,
         export: Optional[Path],
         cdm_only: Optional[bool],
         no_proxy: bool,
         no_folder: bool,
         no_source: bool,
-        workers: int,
+        workers: Optional[int],
+        downloads: int,
         *_: Any,
         **__: Any
     ) -> None:
         start_time = time.time()
 
         if cdm_only is None:
             vaults_only = None
@@ -498,15 +501,15 @@
                     Padding(
                         download_table,
                         (1, 5)
                     ),
                     console=console,
                     refresh_per_second=5
                 ):
-                    with ThreadPoolExecutor(workers) as pool:
+                    with ThreadPoolExecutor(downloads) as pool:
                         for download in futures.as_completed((
                             pool.submit(
                                 track.download,
                                 session=service.session,
                                 prepare_drm=partial(
                                     partial(
                                         self.prepare_drm,
@@ -524,29 +527,30 @@
                                         title=title,
                                         track=track
                                     ),
                                     cdm_only=cdm_only,
                                     vaults_only=vaults_only,
                                     export=export
                                 ),
+                                max_workers=workers,
                                 progress=tracks_progress_callables[i]
                             )
                             for i, track in enumerate(title.tracks)
                         )):
                             download.result()
             except KeyboardInterrupt:
                 console.print(Padding(
                     ":x: Download Cancelled...",
                     (0, 5, 1, 5)
                 ))
                 return
             except Exception as e:  # noqa
                 error_messages = [
                     ":x: Download Failed...",
-                    "   One of the download workers had an error!",
+                    "   One of the track downloads had an error!",
                     "   See the error trace above for more information."
                 ]
                 if isinstance(e, subprocess.CalledProcessError):
                     # ignore process exceptions as proper error logs are already shown
                     error_messages.append(f"   Process exit code: {e.returncode}")
                 else:
                     console.print_exception()
```

### Comparing `devine-3.3.0/devine/commands/env.py` & `devine-3.3.1/devine/commands/env.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/commands/kv.py` & `devine-3.3.1/devine/commands/kv.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/commands/search.py` & `devine-3.3.1/devine/commands/search.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/commands/serve.py` & `devine-3.3.1/devine/commands/serve.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/commands/util.py` & `devine-3.3.1/devine/commands/util.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/commands/wvd.py` & `devine-3.3.1/devine/commands/wvd.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/__main__.py` & `devine-3.3.1/devine/core/__main__.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/cacher.py` & `devine-3.3.1/devine/core/cacher.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/commands.py` & `devine-3.3.1/devine/core/commands.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/config.py` & `devine-3.3.1/devine/core/config.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/console.py` & `devine-3.3.1/devine/core/console.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/constants.py` & `devine-3.3.1/devine/core/constants.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/credential.py` & `devine-3.3.1/devine/core/credential.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/downloaders/aria2c.py` & `devine-3.3.1/devine/core/downloaders/aria2c.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/downloaders/curl_impersonate.py` & `devine-3.3.1/devine/core/downloaders/curl_impersonate.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/downloaders/requests.py` & `devine-3.3.1/devine/core/downloaders/requests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import os
 import time
-from concurrent import futures
+from concurrent.futures import as_completed
 from concurrent.futures.thread import ThreadPoolExecutor
 from http.cookiejar import CookieJar
 from pathlib import Path
 from typing import Any, Generator, MutableMapping, Optional, Union
 
 from requests import Session
 from requests.adapters import HTTPAdapter
@@ -15,19 +15,22 @@
 from devine.core.utilities import get_extension
 
 MAX_ATTEMPTS = 5
 RETRY_WAIT = 2
 CHUNK_SIZE = 1024
 PROGRESS_WINDOW = 5
 
+DOWNLOAD_SIZES = []
+LAST_SPEED_REFRESH = time.time()
 
 def download(
     url: str,
     save_path: Path,
     session: Optional[Session] = None,
+    segmented: bool = False,
     **kwargs: Any
 ) -> Generator[dict[str, Any], None, None]:
     """
     Download a file using Python Requests.
     https://requests.readthedocs.io
 
     Yields the following download status updates while chunks are downloading:
@@ -44,18 +47,21 @@
     Parameters:
         url: Web URL of a file to download.
         save_path: The path to save the file to. If the save path's directory does not
             exist then it will be made automatically.
         session: The Requests Session to make HTTP requests with. Useful to set Header,
             Cookie, and Proxy data. Connections are saved and re-used with the session
             so long as the server keeps the connection alive.
+        segmented: If downloads are segments or parts of one bigger file.
         kwargs: Any extra keyword arguments to pass to the session.get() call. Use this
             for one-time request changes like a header, cookie, or proxy. For example,
             to request Byte-ranges use e.g., `headers={"Range": "bytes=0-128"}`.
     """
+    global LAST_SPEED_REFRESH
+
     session = session or Session()
 
     save_dir = save_path.parent
     control_file = save_path.with_name(f"{save_path.name}.!dev")
 
     save_dir.mkdir(parents=True, exist_ok=True)
 
@@ -65,63 +71,76 @@
         control_file.unlink()
     elif save_path.exists():
         # if it exists, and no control file, then it should be safe
         yield dict(
             file_downloaded=save_path,
             written=save_path.stat().st_size
         )
+        # TODO: This should return, potential recovery bug
 
     # TODO: Design a control file format so we know how much of the file is missing
     control_file.write_bytes(b"")
 
     attempts = 1
     try:
         while True:
             written = 0
+
+            # these are for single-url speed calcs only
             download_sizes = []
             last_speed_refresh = time.time()
 
             try:
                 stream = session.get(url, stream=True, **kwargs)
                 stream.raise_for_status()
 
-                try:
-                    content_length = int(stream.headers.get("Content-Length", "0"))
-                except ValueError:
-                    content_length = 0
-
-                if content_length > 0:
-                    yield dict(total=math.ceil(content_length / CHUNK_SIZE))
-                else:
-                    # we have no data to calculate total chunks
-                    yield dict(total=None)  # indeterminate mode
+                if not segmented:
+                    try:
+                        content_length = int(stream.headers.get("Content-Length", "0"))
+                    except ValueError:
+                        content_length = 0
+
+                    if content_length > 0:
+                        yield dict(total=math.ceil(content_length / CHUNK_SIZE))
+                    else:
+                        # we have no data to calculate total chunks
+                        yield dict(total=None)  # indeterminate mode
 
                 with open(save_path, "wb") as f:
                     for chunk in stream.iter_content(chunk_size=CHUNK_SIZE):
                         download_size = len(chunk)
                         f.write(chunk)
                         written += download_size
 
-                        yield dict(advance=1)
-
-                        now = time.time()
-                        time_since = now - last_speed_refresh
-
-                        download_sizes.append(download_size)
-                        if time_since > PROGRESS_WINDOW or download_size < CHUNK_SIZE:
-                            data_size = sum(download_sizes)
-                            download_speed = math.ceil(data_size / (time_since or 1))
-                            yield dict(downloaded=f"{filesize.decimal(download_speed)}/s")
-                            last_speed_refresh = now
-                            download_sizes.clear()
-
-                yield dict(
-                    file_downloaded=save_path,
-                    written=written
-                )
+                        if not segmented:
+                            yield dict(advance=1)
+                            now = time.time()
+                            time_since = now - last_speed_refresh
+                            download_sizes.append(download_size)
+                            if time_since > PROGRESS_WINDOW or download_size < CHUNK_SIZE:
+                                data_size = sum(download_sizes)
+                                download_speed = math.ceil(data_size / (time_since or 1))
+                                yield dict(downloaded=f"{filesize.decimal(download_speed)}/s")
+                                last_speed_refresh = now
+                                download_sizes.clear()
+
+                yield dict(file_downloaded=save_path, written=written)
+
+                if segmented:
+                    yield dict(advance=1)
+                    now = time.time()
+                    time_since = now - LAST_SPEED_REFRESH
+                    if written:  # no size == skipped dl
+                        DOWNLOAD_SIZES.append(written)
+                    if DOWNLOAD_SIZES and time_since > PROGRESS_WINDOW:
+                        data_size = sum(DOWNLOAD_SIZES)
+                        download_speed = math.ceil(data_size / (time_since or 1))
+                        yield dict(downloaded=f"{filesize.decimal(download_speed)}/s")
+                        LAST_SPEED_REFRESH = now
+                        DOWNLOAD_SIZES.clear()
                 break
             except Exception as e:
                 save_path.unlink(missing_ok=True)
                 if DOWNLOAD_CANCELLED.is_set() or attempts == MAX_ATTEMPTS:
                     raise e
                 time.sleep(RETRY_WAIT)
                 attempts += 1
@@ -233,63 +252,41 @@
     if cookies:
         session.cookies.update(cookies)
     if proxy:
         session.proxies.update({"all": proxy})
 
     yield dict(total=len(urls))
 
-    download_sizes = []
-    last_speed_refresh = time.time()
-
-    with ThreadPoolExecutor(max_workers=max_workers) as pool:
-        for i, future in enumerate(futures.as_completed((
-            pool.submit(
-                download,
-                session=session,
-                **url
-            )
-            for url in urls
-        ))):
-            file_path, download_size = None, None
-            try:
-                for status_update in future.result():
-                    if status_update.get("file_downloaded") and status_update.get("written"):
-                        file_path = status_update["file_downloaded"]
-                        download_size = status_update["written"]
-                    elif len(urls) == 1:
-                        # these are per-chunk updates, only useful if it's one big file
-                        yield status_update
-            except KeyboardInterrupt:
-                DOWNLOAD_CANCELLED.set()  # skip pending track downloads
-                yield dict(downloaded="[yellow]CANCELLING")
-                pool.shutdown(wait=True, cancel_futures=True)
-                yield dict(downloaded="[yellow]CANCELLED")
-                # tell dl that it was cancelled
-                # the pool is already shut down, so exiting loop is fine
-                raise
-            except Exception:
-                DOWNLOAD_CANCELLED.set()  # skip pending track downloads
-                yield dict(downloaded="[red]FAILING")
-                pool.shutdown(wait=True, cancel_futures=True)
-                yield dict(downloaded="[red]FAILED")
-                # tell dl that it failed
-                # the pool is already shut down, so exiting loop is fine
-                raise
-            else:
-                yield dict(file_downloaded=file_path, written=download_size)
-                yield dict(advance=1)
-
-                now = time.time()
-                time_since = now - last_speed_refresh
-
-                if download_size:  # no size == skipped dl
-                    download_sizes.append(download_size)
-
-                if download_sizes and (time_since > PROGRESS_WINDOW or i == len(urls)):
-                    data_size = sum(download_sizes)
-                    download_speed = math.ceil(data_size / (time_since or 1))
-                    yield dict(downloaded=f"{filesize.decimal(download_speed)}/s")
-                    last_speed_refresh = now
-                    download_sizes.clear()
+    try:
+        with ThreadPoolExecutor(max_workers=max_workers) as pool:
+            for future in as_completed(
+                pool.submit(
+                    download,
+                    session=session,
+                    segmented=True,
+                    **url
+                )
+                for url in urls
+            ):
+                try:
+                    yield from future.result()
+                except KeyboardInterrupt:
+                    DOWNLOAD_CANCELLED.set()  # skip pending track downloads
+                    yield dict(downloaded="[yellow]CANCELLING")
+                    pool.shutdown(wait=True, cancel_futures=True)
+                    yield dict(downloaded="[yellow]CANCELLED")
+                    # tell dl that it was cancelled
+                    # the pool is already shut down, so exiting loop is fine
+                    raise
+                except Exception:
+                    DOWNLOAD_CANCELLED.set()  # skip pending track downloads
+                    yield dict(downloaded="[red]FAILING")
+                    pool.shutdown(wait=True, cancel_futures=True)
+                    yield dict(downloaded="[red]FAILED")
+                    # tell dl that it failed
+                    # the pool is already shut down, so exiting loop is fine
+                    raise
+    finally:
+        DOWNLOAD_SIZES.clear()
 
 
 __all__ = ("requests",)
```

### Comparing `devine-3.3.0/devine/core/drm/clearkey.py` & `devine-3.3.1/devine/core/drm/clearkey.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/drm/widevine.py` & `devine-3.3.1/devine/core/drm/widevine.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/events.py` & `devine-3.3.1/devine/core/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from copy import deepcopy
 from enum import Enum
 from typing import Any, Callable
 
 
 class Events:
     class Types(Enum):
         _reserved = 0
@@ -21,18 +22,19 @@
     def __init__(self):
         self.__subscriptions: dict[Events.Types, list[Callable]] = {}
         self.__ephemeral: dict[Events.Types, list[Callable]] = {}
         self.reset()
 
     def reset(self):
         """Reset Event Observer clearing all Subscriptions."""
-        self.__subscriptions = self.__ephemeral = {
+        self.__subscriptions = {
             k: []
             for k in Events.Types.__members__.values()
         }
+        self.__ephemeral = deepcopy(self.__subscriptions)
 
     def subscribe(self, event_type: Events.Types, callback: Callable, ephemeral: bool = False) -> None:
         """
         Subscribe to an Event with a Callback.
 
         Parameters:
             event_type: The Events.Type to subscribe to.
```

### Comparing `devine-3.3.0/devine/core/manifests/dash.py` & `devine-3.3.1/devine/core/manifests/dash.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,15 @@
     def download_track(
         track: AnyTrack,
         save_path: Path,
         save_dir: Path,
         progress: partial,
         session: Optional[Session] = None,
         proxy: Optional[str] = None,
+        max_workers: Optional[int] = None,
         license_widevine: Optional[Callable] = None
     ):
         if not session:
             session = Session()
         elif not isinstance(session, Session):
             raise TypeError(f"Expected session to be a {Session}, not {session!r}")
 
@@ -468,15 +469,15 @@
                 for url, bytes_range in segments
             ],
             output_dir=save_dir,
             filename="{i:0%d}.mp4" % (len(str(len(segments)))),
             headers=session.headers,
             cookies=session.cookies,
             proxy=proxy,
-            max_workers=16
+            max_workers=max_workers
         ):
             file_downloaded = status_update.get("file_downloaded")
             if file_downloaded:
                 events.emit(events.Types.SEGMENT_DOWNLOADED, track=track, segment=file_downloaded)
             else:
                 downloaded = status_update.get("downloaded")
                 if downloaded and downloaded.endswith("/s"):
```

### Comparing `devine-3.3.0/devine/core/manifests/hls.py` & `devine-3.3.1/devine/core/manifests/hls.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,15 @@
     def download_track(
         track: AnyTrack,
         save_path: Path,
         save_dir: Path,
         progress: partial,
         session: Optional[Session] = None,
         proxy: Optional[str] = None,
+        max_workers: Optional[int] = None,
         license_widevine: Optional[Callable] = None
     ) -> None:
         if not session:
             session = Session()
         elif not isinstance(session, Session):
             raise TypeError(f"Expected session to be a {Session}, not {session!r}")
 
@@ -276,15 +277,15 @@
         for status_update in downloader(
             urls=urls,
             output_dir=segment_save_dir,
             filename="{i:0%d}{ext}" % len(str(len(urls))),
             headers=session.headers,
             cookies=session.cookies,
             proxy=proxy,
-            max_workers=16
+            max_workers=max_workers
         ):
             file_downloaded = status_update.get("file_downloaded")
             if file_downloaded:
                 events.emit(events.Types.SEGMENT_DOWNLOADED, track=track, segment=file_downloaded)
             else:
                 downloaded = status_update.get("downloaded")
                 if downloaded and downloaded.endswith("/s"):
```

### Comparing `devine-3.3.0/devine/core/proxies/basic.py` & `devine-3.3.1/devine/core/proxies/basic.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/proxies/hola.py` & `devine-3.3.1/devine/core/proxies/hola.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/proxies/nordvpn.py` & `devine-3.3.1/devine/core/proxies/nordvpn.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/proxies/proxy.py` & `devine-3.3.1/devine/core/proxies/proxy.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/search_result.py` & `devine-3.3.1/devine/core/search_result.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/service.py` & `devine-3.3.1/devine/core/service.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/services.py` & `devine-3.3.1/devine/core/services.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/titles/episode.py` & `devine-3.3.1/devine/core/titles/episode.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/titles/movie.py` & `devine-3.3.1/devine/core/titles/movie.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/titles/song.py` & `devine-3.3.1/devine/core/titles/song.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/titles/title.py` & `devine-3.3.1/devine/core/titles/title.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/tracks/attachment.py` & `devine-3.3.1/devine/core/tracks/attachment.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/tracks/audio.py` & `devine-3.3.1/devine/core/tracks/audio.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/tracks/chapter.py` & `devine-3.3.1/devine/core/tracks/chapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 seconds, ms = divmod(remainder, 1000)
             elif isinstance(timestamp, float):  # seconds.ms
                 hours, remainder = divmod(timestamp, 60 * 60)
                 minutes, remainder = divmod(remainder, 60)
                 seconds, ms = divmod(int(remainder * 1000), 1000)
             else:
                 raise TypeError
-            timestamp = f"{hours:02}:{minutes:02}:{seconds:02}.{str(ms).zfill(3)[:3]}"
+            timestamp = f"{int(hours):02}:{int(minutes):02}:{int(seconds):02}.{str(ms).zfill(3)[:3]}"
 
         timestamp_m = TIMESTAMP_FORMAT.match(timestamp)
         if not timestamp_m:
             raise ValueError(f"The timestamp format is invalid: {timestamp}")
 
         hour, minute, second, ms = timestamp_m.groups()
         if not ms:
```

### Comparing `devine-3.3.0/devine/core/tracks/chapters.py` & `devine-3.3.1/devine/core/tracks/chapters.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/tracks/subtitle.py` & `devine-3.3.1/devine/core/tracks/subtitle.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,17 +149,18 @@
             track_name += flag
         return track_name or None
 
     def download(
         self,
         session: requests.Session,
         prepare_drm: partial,
+        max_workers: Optional[int] = None,
         progress: Optional[partial] = None
     ):
-        super().download(session, prepare_drm, progress)
+        super().download(session, prepare_drm, max_workers, progress)
         if not self.path:
             return
 
         if self.codec == Subtitle.Codec.fTTML:
             self.convert(Subtitle.Codec.TimedTextMarkupLang)
         elif self.codec == Subtitle.Codec.fVTT:
             self.convert(Subtitle.Codec.WebVTT)
```

### Comparing `devine-3.3.0/devine/core/tracks/track.py` & `devine-3.3.1/devine/core/tracks/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, Track) and self.id == other.id
 
     def download(
         self,
         session: Session,
         prepare_drm: partial,
+        max_workers: Optional[int] = None,
         progress: Optional[partial] = None
     ):
         """Download and optionally Decrypt this Track."""
         from devine.core.manifests import DASH, HLS
 
         if DOWNLOAD_LICENCE_ONLY.is_set():
             progress(downloaded="[yellow]SKIPPING")
@@ -187,24 +188,26 @@
                 HLS.download_track(
                     track=self,
                     save_path=save_path,
                     save_dir=save_dir,
                     progress=progress,
                     session=session,
                     proxy=proxy,
+                    max_workers=max_workers,
                     license_widevine=prepare_drm
                 )
             elif self.descriptor == self.Descriptor.DASH:
                 DASH.download_track(
                     track=self,
                     save_path=save_path,
                     save_dir=save_dir,
                     progress=progress,
                     session=session,
                     proxy=proxy,
+                    max_workers=max_workers,
                     license_widevine=prepare_drm
                 )
             elif self.descriptor == self.Descriptor.URL:
                 try:
                     if not self.drm and track_type in ("Video", "Audio"):
                         # the service might not have explicitly defined the `drm` property
                         # try find widevine DRM information from the init data of URL
@@ -232,15 +235,16 @@
                     else:
                         for status_update in self.downloader(
                             urls=self.url,
                             output_dir=save_path.parent,
                             filename=save_path.name,
                             headers=session.headers,
                             cookies=session.cookies,
-                            proxy=proxy
+                            proxy=proxy,
+                            max_workers=max_workers
                         ):
                             file_downloaded = status_update.get("file_downloaded")
                             if not file_downloaded:
                                 progress(**status_update)
 
                         # see https://github.com/devine-dl/devine/issues/71
                         save_path.with_suffix(f"{save_path.suffix}.aria2__temp").unlink(missing_ok=True)
```

### Comparing `devine-3.3.0/devine/core/tracks/tracks.py` & `devine-3.3.1/devine/core/tracks/tracks.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/tracks/video.py` & `devine-3.3.1/devine/core/tracks/video.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/utilities.py` & `devine-3.3.1/devine/core/utilities.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/utils/click_types.py` & `devine-3.3.1/devine/core/utils/click_types.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/utils/collections.py` & `devine-3.3.1/devine/core/utils/collections.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/utils/sslciphers.py` & `devine-3.3.1/devine/core/utils/sslciphers.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/utils/subprocess.py` & `devine-3.3.1/devine/core/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/utils/xml.py` & `devine-3.3.1/devine/core/utils/xml.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/vault.py` & `devine-3.3.1/devine/core/vault.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/core/vaults.py` & `devine-3.3.1/devine/core/vaults.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/vaults/API.py` & `devine-3.3.1/devine/vaults/API.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/vaults/MySQL.py` & `devine-3.3.1/devine/vaults/MySQL.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/devine/vaults/SQLite.py` & `devine-3.3.1/devine/vaults/SQLite.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.0/pyproject.toml` & `devine-3.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "devine"
-version = "3.3.0"
+version = "3.3.1"
 description = "Modular Movie, TV, and Music Archival Software."
 license = "GPL-3.0-only"
 authors = ["rlaphoenix <rlaphoenix@pm.me>"]
 readme = "README.md"
 homepage = "https://github.com/devine-dl/devine"
 repository = "https://github.com/devine-dl/devine"
 keywords = ["python", "downloader", "drm", "widevine"]
@@ -69,15 +69,15 @@
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.7.0"
 mypy = "^1.9.0"
 mypy-protobuf = "^3.6.0"
 types-protobuf = "^4.24.0.20240311"
 types-PyMySQL = "^1.1.0.1"
-types-requests = "^2.31.0.20240402"
+types-requests = "^2.31.0.20240403"
 isort = "^5.13.2"
 ruff = "~0.3.5"
 
 [tool.poetry.scripts]
 devine = "devine.core.__main__:main"
 
 [tool.ruff]
```

### Comparing `devine-3.3.0/PKG-INFO` & `devine-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devine
-Version: 3.3.0
+Version: 3.3.1
 Summary: Modular Movie, TV, and Music Archival Software.
 Home-page: https://github.com/devine-dl/devine
 License: GPL-3.0-only
 Keywords: python,downloader,drm,widevine
 Author: rlaphoenix
 Author-email: rlaphoenix@pm.me
 Requires-Python: >=3.9,<4.0
@@ -395,14 +395,15 @@
 <a href="https://github.com/shirt-dev"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/2660574?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="shirt-dev"/></a>
 <a href="https://github.com/nyuszika7h"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/482367?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="nyuszika7h"/></a>
 <a href="https://github.com/bccornfo"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/98013276?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="bccornfo"/></a>
 <a href="https://github.com/Arias800"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/24809312?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Arias800"/></a>
 <a href="https://github.com/varyg1001"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/88599103?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="varyg1001"/></a>
 <a href="https://github.com/Hollander-1908"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/93162595?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Hollander-1908"/></a>
 <a href="https://github.com/Shivelight"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/20620780?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Shivelight"/></a>
+<a href="https://github.com/knowhere01"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/113712042?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="knowhere01"/></a>
 
 ## Licensing
 
 This software is licensed under the terms of [GNU General Public License, Version 3.0](LICENSE).  
 You can find a copy of the license in the LICENSE file in the root folder.
 
 * * *
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: devine Version: 3.3.0 Summary: Modular Movie, TV,
+Metadata-Version: 2.1 Name: devine Version: 3.3.1 Summary: Modular Movie, TV,
 and Music Archival Software. Home-page: https://github.com/devine-dl/devine
 License: GPL-3.0-only Keywords: python,downloader,drm,widevine Author:
 rlaphoenix Author-email: rlaphoenix@pm.me Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
@@ -253,11 +253,11 @@
 this includes Widevine Provision Keys, Content Encryption Keys, or Service API
 Calls or Code. 3. The Core codebase is meant to stay Free and Open-Source while
 the Service code should be kept private. 4. Do not sell any part of this
 project, neither alone nor as part of a bundle. If you paid for this software
 or received it as part of a bundle following payment, you should demand your
 money back immediately. 5. Be kind to one another and do not single anyone out.
 ## Contributors _[_r_l_a_p_h_o_e_n_i_x_]_[_m_n_m_l_l_]_[_s_h_i_r_t_-_d_e_v_]_[_n_y_u_s_z_i_k_a_7_h_]_[_b_c_c_o_r_n_f_o_]_[_A_r_i_a_s_8_0_0_]
-_[_v_a_r_y_g_1_0_0_1_]_[_H_o_l_l_a_n_d_e_r_-_1_9_0_8_]_[_S_h_i_v_e_l_i_g_h_t_]## Licensing This software is licensed
-under the terms of [GNU General Public License, Version 3.0](LICENSE). You can
-find a copy of the license in the LICENSE file in the root folder. * * * Â©
-rlaphoenix 2019-2024
+_[_v_a_r_y_g_1_0_0_1_]_[_H_o_l_l_a_n_d_e_r_-_1_9_0_8_]_[_S_h_i_v_e_l_i_g_h_t_]_[_k_n_o_w_h_e_r_e_0_1_]## Licensing This software
+is licensed under the terms of [GNU General Public License, Version 3.0]
+(LICENSE). You can find a copy of the license in the LICENSE file in the root
+folder. * * * Â© rlaphoenix 2019-2024
```

