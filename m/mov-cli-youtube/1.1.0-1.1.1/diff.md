# Comparing `tmp/mov-cli-youtube-1.1.0.tar.gz` & `tmp/mov-cli-youtube-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-youtube-1.1.0.tar", last modified: Thu Mar 21 15:30:09 2024, max compression
+gzip compressed data, was "mov-cli-youtube-1.1.1.tar", last modified: Fri Apr  5 12:09:32 2024, max compression
```

## Comparing `mov-cli-youtube-1.1.0.tar` & `mov-cli-youtube-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-21 15:30:09.761804 mov-cli-youtube-1.1.0/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov-cli-youtube-1.1.0/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2956 2024-03-21 15:30:09.761804 mov-cli-youtube-1.1.0/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov-cli-youtube-1.1.0/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-21 15:30:09.761804 mov-cli-youtube-1.1.0/mov_cli_youtube/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      289 2024-03-21 15:22:05.000000 mov-cli-youtube-1.1.0/mov_cli_youtube/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2315 2024-03-21 15:22:05.000000 mov-cli-youtube-1.1.0/mov_cli_youtube/youtube.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-21 15:30:09.761804 mov-cli-youtube-1.1.0/mov_cli_youtube.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2956 2024-03-21 15:30:09.000000 mov-cli-youtube-1.1.0/mov_cli_youtube.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      281 2024-03-21 15:30:09.000000 mov-cli-youtube-1.1.0/mov_cli_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-03-21 15:30:09.000000 mov-cli-youtube-1.1.0/mov_cli_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       80 2024-03-21 15:30:09.000000 mov-cli-youtube-1.1.0/mov_cli_youtube.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-03-21 15:30:09.000000 mov-cli-youtube-1.1.0/mov_cli_youtube.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1271 2024-03-03 19:56:21.000000 mov-cli-youtube-1.1.0/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-03-21 15:30:09.761804 mov-cli-youtube-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 12:09:32.352796 mov-cli-youtube-1.1.1/
+-rw-rw-rw-   0        0        0     1085 2024-04-05 12:02:31.000000 mov-cli-youtube-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3041 2024-04-05 12:09:32.350795 mov-cli-youtube-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2024-04-05 12:02:31.000000 mov-cli-youtube-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 12:09:32.326789 mov-cli-youtube-1.1.1/mov_cli_youtube/
+-rw-rw-rw-   0        0        0      304 2024-04-05 12:08:32.000000 mov-cli-youtube-1.1.1/mov_cli_youtube/__init__.py
+-rw-rw-rw-   0        0        0     2670 2024-04-05 12:06:10.000000 mov-cli-youtube-1.1.1/mov_cli_youtube/youtube.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:09:32.348793 mov-cli-youtube-1.1.1/mov_cli_youtube.egg-info/
+-rw-rw-rw-   0        0        0     3041 2024-04-05 12:09:32.000000 mov-cli-youtube-1.1.1/mov_cli_youtube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-04-05 12:09:32.000000 mov-cli-youtube-1.1.1/mov_cli_youtube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 12:09:32.000000 mov-cli-youtube-1.1.1/mov_cli_youtube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-05 12:09:32.000000 mov-cli-youtube-1.1.1/mov_cli_youtube.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-05 12:09:32.000000 mov-cli-youtube-1.1.1/mov_cli_youtube.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1320 2024-04-05 12:02:31.000000 mov-cli-youtube-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 12:09:32.352796 mov-cli-youtube-1.1.1/setup.cfg
```

### Comparing `mov-cli-youtube-1.1.0/PKG-INFO` & `mov-cli-youtube-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-Metadata-Version: 2.1
-Name: mov-cli-youtube
-Version: 1.1.0
-Summary: A mov-cli v4 plugin for watching youtube.
-Author-email: Goldy <goldy@devgoldy.xyz>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-youtube
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-youtube/issues
-Keywords: amazing mov-cli plugin
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: pytube
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-<div align="center">
-
-  # mov-cli-youtube
-  <sub>A mov-cli v4 plugin for watching youtube.</sub>
-
-  <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
-
-</div>
-
-> [!NOTE]
-> Currently work in progress, expect slow speeds.
-
-## Installation 🛠️
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-youtube
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-youtube = "mov-cli-youtube"
-```
-
-## Usage 🖱️
-```sh
-mov-cli -s youtube nyan cat
-```
-
-### Audio Only 🔉
-```sh
-mov-cli -s youtube nyan cat -- --audio
-```
+Metadata-Version: 2.1
+Name: mov-cli-youtube
+Version: 1.1.1
+Summary: A mov-cli v4 plugin for watching youtube.
+Author-email: Goldy <goldy@devgoldy.xyz>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/mov-cli/mov-cli-youtube
+Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-youtube/issues
+Keywords: amazing mov-cli plugin
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: pytube
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+
+<div align="center">
+
+  # mov-cli-youtube
+  <sub>A mov-cli v4 plugin for watching youtube.</sub>
+
+  <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
+
+</div>
+
+> [!NOTE]
+> Currently work in progress, expect slow speeds.
+
+## Installation 🛠️
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-youtube
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+youtube = "mov-cli-youtube"
+```
+
+## Usage 🖱️
+```sh
+mov-cli -s youtube nyan cat
+```
+
+### Audio Only 🔉
+```sh
+mov-cli -s youtube nyan cat -- --audio
+```
```

### Comparing `mov-cli-youtube-1.1.0/README.md` & `mov-cli-youtube-1.1.1/README.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-<div align="center">
-
-  # mov-cli-youtube
-  <sub>A mov-cli v4 plugin for watching youtube.</sub>
-
-  <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
-
-</div>
-
-> [!NOTE]
-> Currently work in progress, expect slow speeds.
-
-## Installation 🛠️
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-youtube
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-youtube = "mov-cli-youtube"
-```
-
-## Usage 🖱️
-```sh
-mov-cli -s youtube nyan cat
-```
-
-### Audio Only 🔉
-```sh
-mov-cli -s youtube nyan cat -- --audio
-```
+<div align="center">
+
+  # mov-cli-youtube
+  <sub>A mov-cli v4 plugin for watching youtube.</sub>
+
+  <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
+
+</div>
+
+> [!NOTE]
+> Currently work in progress, expect slow speeds.
+
+## Installation 🛠️
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-youtube
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+youtube = "mov-cli-youtube"
+```
+
+## Usage 🖱️
+```sh
+mov-cli -s youtube nyan cat
+```
+
+### Audio Only 🔉
+```sh
+mov-cli -s youtube nyan cat -- --audio
+```
```

### Comparing `mov-cli-youtube-1.1.0/mov_cli_youtube/youtube.py` & `mov-cli-youtube-1.1.1/mov_cli_youtube/youtube.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,77 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import List, Optional, Dict, Generator, Any
-
-    from mov_cli import Config
-    from mov_cli.http_client import HTTPClient
-
-import os
-import sys
-from pytube import YouTube, Search
-
-from mov_cli import utils
-from mov_cli.scraper import Scraper
-from mov_cli import Series, Movie, Metadata, MetadataType
-
-__all__ = ("YouTubeScraper",)
-
-class YouTubeScraper(Scraper):
-    def __init__(self, config: Config, http_client: HTTPClient) -> None:
-        super().__init__(config, http_client)
-
-    def search(self, query: str, limit: int = None) -> Generator[Metadata, Any, None]:
-        search_query = Search(query)
-        search_results: List[YouTube] = search_query.results
-
-        max_videos = 20 if limit is None else limit
-
-        # suppress pytube's stupid errors from getting to the console and ruining fzf output.
-        sys.stderr = open(os.devnull, "w")
-
-        for index, video in enumerate(search_results):
-            if (index + 1) == len(search_results) and not (index + 1) >= max_videos:
-                search_query.get_next_results()
-
-            yield Metadata(
-                id = video.watch_url, 
-                title = f"{video.title} ~ {video.author}", 
-                type = MetadataType.MOVIE, 
-                year = str(video.publish_date.year)
-            )
-
-        # restore the console.
-        sys.stderr = sys.__stderr__
-
-    def scrape(self, metadata: Metadata, episode: Optional[utils.EpisodeSelector] = None, **kwargs: Dict[str, bool]) -> Series | Movie:
-        audio_only: bool = kwargs.get("audio", False)
-
-        if episode is None:
-            episode = utils.EpisodeSelector()
-
-        watch_url = metadata.id
-        video = YouTube(watch_url)
-
-        if audio_only:
-            url = video.streams.get_audio_only().url
-        else:
-            url = video.streams.get_highest_resolution().url
-
-        return Movie(
-            url = url, 
-            title = metadata.title, 
-            referrer = "", 
-            year = metadata.year, 
-            subtitles = None
-        )
-
-    def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[None, int]:
-        # Returning None as search does not return any metadata of type series.
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import List, Optional, Dict, Generator, Any
+
+    from mov_cli import Config
+    from mov_cli.http_client import HTTPClient
+
+import os
+import sys
+from pytube import YouTube, Search
+
+from mov_cli import utils
+from mov_cli.scraper import Scraper
+from mov_cli import Series, Movie, Metadata, MetadataType
+
+__all__ = ("YouTubeScraper",)
+
+class YouTubeScraper(Scraper):
+    def __init__(self, config: Config, http_client: HTTPClient) -> None:
+        super().__init__(config, http_client)
+
+    def search(self, query: str, limit: int = None) -> Generator[Metadata, Any, None]:
+        search_query = Search(query)
+        search_results: List[YouTube] = search_query.results
+
+        max_videos = 20 if limit is None else limit
+
+        # suppress pytube's stupid errors from getting to the console and ruining fzf output.
+        sys.stderr = open(os.devnull, "w")
+
+        for index, video in enumerate(search_results):
+            if (index + 1) == len(search_results) and not (index + 1) >= max_videos:
+                search_query.get_next_results()
+
+            yield Metadata(
+                id = video.watch_url, 
+                title = f"{video.title} ~ {video.author}", 
+                type = MetadataType.MOVIE, 
+                year = str(video.publish_date.year)
+            )
+
+        # restore the console.
+        sys.stderr = sys.__stderr__
+
+    def scrape(self, metadata: Metadata, episode: Optional[utils.EpisodeSelector] = None, **kwargs: Dict[str, bool]) -> Series | Movie:
+        audio_only: bool = kwargs.get("audio", False)
+
+        if episode is None:
+            episode = utils.EpisodeSelector()
+
+        watch_url = metadata.id
+        video = YouTube(watch_url)
+
+        if audio_only:
+            url = video.streams.get_audio_only().url
+        else:
+            if self.config.resolution is not None:
+                url = video.streams.get_by_resolution(f"{self.config.resolution}p").url
+                
+                if url is None:
+                    url = video.streams.get_highest_resolution().url
+            else:
+                url = video.streams.get_highest_resolution().url
+
+        return Movie(
+            url = url, 
+            title = metadata.title, 
+            referrer = "", 
+            year = metadata.year, 
+            subtitles = None
+        )
+
+    def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[None, int]:
+        # Returning None as search does not return any metadata of type series.
         return {None: 1}
```

### Comparing `mov-cli-youtube-1.1.0/mov_cli_youtube.egg-info/PKG-INFO` & `mov-cli-youtube-1.1.1/mov_cli_youtube.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-Metadata-Version: 2.1
-Name: mov-cli-youtube
-Version: 1.1.0
-Summary: A mov-cli v4 plugin for watching youtube.
-Author-email: Goldy <goldy@devgoldy.xyz>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-youtube
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-youtube/issues
-Keywords: amazing mov-cli plugin
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: pytube
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-<div align="center">
-
-  # mov-cli-youtube
-  <sub>A mov-cli v4 plugin for watching youtube.</sub>
-
-  <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
-
-</div>
-
-> [!NOTE]
-> Currently work in progress, expect slow speeds.
-
-## Installation 🛠️
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-youtube
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-youtube = "mov-cli-youtube"
-```
-
-## Usage 🖱️
-```sh
-mov-cli -s youtube nyan cat
-```
-
-### Audio Only 🔉
-```sh
-mov-cli -s youtube nyan cat -- --audio
-```
+Metadata-Version: 2.1
+Name: mov-cli-youtube
+Version: 1.1.1
+Summary: A mov-cli v4 plugin for watching youtube.
+Author-email: Goldy <goldy@devgoldy.xyz>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/mov-cli/mov-cli-youtube
+Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-youtube/issues
+Keywords: amazing mov-cli plugin
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: pytube
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+
+<div align="center">
+
+  # mov-cli-youtube
+  <sub>A mov-cli v4 plugin for watching youtube.</sub>
+
+  <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
+
+</div>
+
+> [!NOTE]
+> Currently work in progress, expect slow speeds.
+
+## Installation 🛠️
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-youtube
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+youtube = "mov-cli-youtube"
+```
+
+## Usage 🖱️
+```sh
+mov-cli -s youtube nyan cat
+```
+
+### Audio Only 🔉
+```sh
+mov-cli -s youtube nyan cat -- --audio
+```
```

### Comparing `mov-cli-youtube-1.1.0/pyproject.toml` & `mov-cli-youtube-1.1.1/pyproject.toml`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-[project]
-name = "mov-cli-youtube"
-description = "A mov-cli v4 plugin for watching youtube."
-authors = [
-    {name = "Goldy", email = "goldy@devgoldy.xyz"}
-]
-readme = {file = "README.md", content-type = "text/markdown"}
-requires-python = ">=3.8"
-license = { file = "LICENSE" }
-keywords = [
-    "amazing mov-cli plugin"
-]
-classifiers = [
-	'Operating System :: Microsoft :: Windows :: Windows 11',
-    'Operating System :: Microsoft :: Windows :: Windows 10',
-    'Operating System :: POSIX :: Linux',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-	'Programming Language :: Python :: 3.11'
-]
-dependencies = [
-    "requests",
-    "importlib-metadata; python_version<'3.8'",
-
-    "pytube"
-]
-
-dynamic = ["version"]
-
-[project.optional-dependencies]
-dev = [
-    "ruff",
-    "build"
-]
-
-[project.urls]
-GitHub = "https://github.com/mov-cli/mov-cli-youtube"
-BugTracker = "https://github.com/mov-cli/mov-cli-youtube/issues"
-
-[tool.setuptools.dynamic]
-version = { attr = "mov_cli_youtube.__version__" }
-
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages.find]
+[project]
+name = "mov-cli-youtube"
+description = "A mov-cli v4 plugin for watching youtube."
+authors = [
+    {name = "Goldy", email = "goldy@devgoldy.xyz"}
+]
+readme = {file = "README.md", content-type = "text/markdown"}
+requires-python = ">=3.8"
+license = { file = "LICENSE" }
+keywords = [
+    "amazing mov-cli plugin"
+]
+classifiers = [
+	'Operating System :: Microsoft :: Windows :: Windows 11',
+    'Operating System :: Microsoft :: Windows :: Windows 10',
+    'Operating System :: POSIX :: Linux',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+	'Programming Language :: Python :: 3.11'
+]
+dependencies = [
+    "requests",
+    "importlib-metadata; python_version<'3.8'",
+
+    "pytube"
+]
+
+dynamic = ["version"]
+
+[project.optional-dependencies]
+dev = [
+    "ruff",
+    "build"
+]
+
+[project.urls]
+GitHub = "https://github.com/mov-cli/mov-cli-youtube"
+BugTracker = "https://github.com/mov-cli/mov-cli-youtube/issues"
+
+[tool.setuptools.dynamic]
+version = { attr = "mov_cli_youtube.__version__" }
+
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
 include = ["mov_cli_youtube*"]
```

