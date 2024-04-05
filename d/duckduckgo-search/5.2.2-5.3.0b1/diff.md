# Comparing `tmp/duckduckgo_search-5.2.2.tar.gz` & `tmp/duckduckgo_search-5.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-5.2.2.tar", last modified: Sat Mar 30 22:38:16 2024, max compression
+gzip compressed data, was "duckduckgo_search-5.3.0b1.tar", last modified: Wed Apr  3 23:37:51 2024, max compression
```

## Comparing `duckduckgo_search-5.2.2.tar` & `duckduckgo_search-5.3.0b1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:38:16.223034 duckduckgo_search-5.2.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    20706 2024-03-30 22:38:16.223034 duckduckgo_search-5.2.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    19284 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:38:16.219034 duckduckgo_search-5.2.2/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      539 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    40392 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:38:16.223034 duckduckgo_search-5.2.2/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20706 2024-03-30 22:38:16.000000 duckduckgo_search-5.2.2/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-30 22:38:16.000000 duckduckgo_search-5.2.2/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 22:38:16.000000 duckduckgo_search-5.2.2/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-30 22:38:16.000000 duckduckgo_search-5.2.2/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-30 22:38:16.000000 duckduckgo_search-5.2.2/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-30 22:38:16.000000 duckduckgo_search-5.2.2/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 22:38:16.223034 duckduckgo_search-5.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:38:16.223034 duckduckgo_search-5.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-30 22:38:06.000000 duckduckgo_search-5.2.2/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40880 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-5.2.2/LICENSE.md` & `duckduckgo_search-5.3.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.2.2/duckduckgo_search/__init__.py` & `duckduckgo_search-5.3.0b1/duckduckgo_search/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """Duckduckgo_search.
 
 Search for words, documents, images, videos, news, maps and text translation
 using the DuckDuckGo.com search engine.
 """
 
+import asyncio
 import logging
+import sys
 
-# ruff: noqa: F401
 from .duckduckgo_search import DDGS
 from .duckduckgo_search_async import AsyncDDGS
 from .version import __version__
 
 __all__ = ["DDGS", "AsyncDDGS", "__version__", "cli"]
 
+# bypass curl_cffi warning on windows: https://github.com/yifeikong/curl_cffi/blob/418e452c99dee5da176f0b0a768337cd5509c4c5/curl_cffi/aio.py#L14
+if sys.platform == "win32":
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+
+
 # A do-nothing logging handler
 # https://docs.python.org/3.3/howto/logging.html#configuring-logging-for-a-library
 logging.getLogger("duckduckgo_search").addHandler(logging.NullHandler())
```

### Comparing `duckduckgo_search-5.2.2/duckduckgo_search/cli.py` & `duckduckgo_search-5.3.0b1/duckduckgo_search/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from urllib.parse import unquote
 
 import click
-from curl_cffi import requests
+import httpx
 
 from .duckduckgo_search import DDGS
-from .utils import json_dumps
+from .utils import _get_ssl_context, json_dumps
 from .version import __version__
 
 logger = logging.getLogger(__name__)
 
 COLORS = {
     0: "black",
     1: "red",
@@ -77,27 +77,26 @@
         .replace(" ", "")
     )
     return keywords
 
 
 def _download_file(url, dir_path, filename, proxy):
     try:
-        resp = requests.get(url, proxies=proxy, impersonate="chrome", timeout=10)
+        resp = httpx.get(url, proxy=proxy, timeout=10, follow_redirects=True, verify=_get_ssl_context())
         resp.raise_for_status()
         with open(os.path.join(dir_path, filename[:200]), "wb") as file:
             file.write(resp.content)
     except Exception as ex:
-        logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
+        logger.info(f"download_file url={url} {type(ex).__name__} {ex}")
 
 
 def _download_results(keywords, results, images=False, proxy=None, threads=None):
     path_type = "images" if images else "text"
     path = f"{path_type}_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     os.makedirs(path, exist_ok=True)
-    proxy = {"http": proxy, "https": proxy}
 
     threads = 10 if threads is None else threads
     with ThreadPoolExecutor(max_workers=threads) as executor:
         futures = []
         for i, res in enumerate(results, start=1):
             url = res["image"] if images else res["href"]
             filename = unquote(url.split("/")[-1].split("?")[0])
@@ -140,15 +139,15 @@
 @click.option("-o", "--output", default="print", help="csv, json (save the results to a csv or json file)")
 @click.option("-d", "--download", is_flag=True, default=False, help="download results to 'keywords' folder")
 @click.option("-b", "--backend", default="api", type=click.Choice(["api", "html", "lite"]), help="which backend to use")
 @click.option("-th", "--threads", default=10, help="download threads, default=10")
 @click.option("-p", "--proxy", default=None, help="the proxy to send requests, example: socks5://localhost:9150")
 def text(keywords, region, safesearch, timelimit, backend, output, download, threads, max_results, proxy):
     """CLI function to perform a text search using DuckDuckGo API."""
-    data = DDGS(proxies=proxy).text(
+    data = DDGS(proxy=proxy).text(
         keywords=keywords,
         region=region,
         safesearch=safesearch,
         timelimit=timelimit,
         backend=backend,
         max_results=max_results,
     )
@@ -166,15 +165,15 @@
 
 @cli.command()
 @click.option("-k", "--keywords", required=True, help="answers search, keywords for query")
 @click.option("-o", "--output", default="print", help="csv, json (save the results to a csv or json file)")
 @click.option("-p", "--proxy", default=None, help="the proxy to send requests, example: socks5://localhost:9150")
 def answers(keywords, output, proxy):
     """CLI function to perform a answers search using DuckDuckGo API."""
-    data = DDGS(proxies=proxy).answers(keywords=keywords)
+    data = DDGS(proxy=proxy).answers(keywords=keywords)
     filename = f"answers_{_sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
         _print_data(data)
     elif output == "csv":
         _save_csv(f"{filename}.csv", data)
     elif output == "json":
         _save_json(f"{filename}.json", data)
@@ -237,15 +236,15 @@
     download,
     threads,
     max_results,
     output,
     proxy,
 ):
     """CLI function to perform a images search using DuckDuckGo API."""
-    data = DDGS(proxies=proxy).images(
+    data = DDGS(proxy=proxy).images(
         keywords=keywords,
         region=region,
         safesearch=safesearch,
         timelimit=timelimit,
         size=size,
         color=color,
         type_image=type_image,
@@ -274,15 +273,15 @@
 @click.option("-d", "--duration", default=None, type=click.Choice(["short", "medium", "long"]))
 @click.option("-lic", "--license_videos", default=None, type=click.Choice(["creativeCommon", "youtube"]))
 @click.option("-m", "--max_results", default=50, help="maximum number of results, default=50")
 @click.option("-o", "--output", default="print", help="csv, json (save the results to a csv or json file)")
 @click.option("-p", "--proxy", default=None, help="the proxy to send requests, example: socks5://localhost:9150")
 def videos(keywords, region, safesearch, timelimit, resolution, duration, license_videos, max_results, output, proxy):
     """CLI function to perform a videos search using DuckDuckGo API."""
-    data = DDGS(proxies=proxy).videos(
+    data = DDGS(proxy=proxy).videos(
         keywords=keywords,
         region=region,
         safesearch=safesearch,
         timelimit=timelimit,
         resolution=resolution,
         duration=duration,
         license_videos=license_videos,
@@ -303,15 +302,15 @@
 @click.option("-s", "--safesearch", default="moderate", type=click.Choice(["on", "moderate", "off"]))
 @click.option("-t", "--timelimit", default=None, type=click.Choice(["d", "w", "m", "y"]), help="day, week, month, year")
 @click.option("-m", "--max_results", default=25, help="maximum number of results, default=25")
 @click.option("-o", "--output", default="print", help="csv, json (save the results to a csv or json file)")
 @click.option("-p", "--proxy", default=None, help="the proxy to send requests, example: socks5://localhost:9150")
 def news(keywords, region, safesearch, timelimit, max_results, output, proxy):
     """CLI function to perform a news search using DuckDuckGo API."""
-    data = DDGS(proxies=proxy).news(
+    data = DDGS(proxy=proxy).news(
         keywords=keywords, region=region, safesearch=safesearch, timelimit=timelimit, max_results=max_results
     )
     filename = f"news_{_sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
         _print_data(data)
     elif output == "csv":
         _save_csv(f"{filename}.csv", data)
@@ -347,15 +346,15 @@
     longitude,
     radius,
     max_results,
     output,
     proxy,
 ):
     """CLI function to perform a maps search using DuckDuckGo API."""
-    data = DDGS(proxies=proxy).maps(
+    data = DDGS(proxy=proxy).maps(
         keywords=keywords,
         place=place,
         street=street,
         city=city,
         county=county,
         state=state,
         country=country,
@@ -378,15 +377,15 @@
 @click.option("-k", "--keywords", required=True, help="text for translation")
 @click.option("-f", "--from_", help="What language to translate from (defaults automatically)")
 @click.option("-t", "--to", default="en", help="de, ru, fr, etc. What language to translate, defaults='en'")
 @click.option("-o", "--output", default="print", help="csv, json (save the results to a csv or json file)")
 @click.option("-p", "--proxy", default=None, help="the proxy to send requests, example: socks5://localhost:9150")
 def translate(keywords, from_, to, output, proxy):
     """CLI function to perform translate using DuckDuckGo API."""
-    data = DDGS(proxies=proxy).translate(keywords=keywords, from_=from_, to=to)
+    data = DDGS(proxy=proxy).translate(keywords=keywords, from_=from_, to=to)
     filename = f"translate_{_sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
         _print_data(data)
     elif output == "csv":
         _save_csv(f"{filename}.csv", data)
     elif output == "json":
         _save_json(f"{filename}.json", data)
@@ -395,15 +394,15 @@
 @cli.command()
 @click.option("-k", "--keywords", required=True, help="keywords for query")
 @click.option("-r", "--region", default="wt-wt", help="wt-wt, us-en, ru-ru, etc. -region https://duckduckgo.com/params")
 @click.option("-o", "--output", default="print", help="csv, json (save the results to a csv or json file)")
 @click.option("-p", "--proxy", default=None, help="the proxy to send requests, example: socks5://localhost:9150")
 def suggestions(keywords, region, output, proxy):
     """CLI function to perform a suggestions search using DuckDuckGo API."""
-    data = DDGS(proxies=proxy).suggestions(keywords=keywords, region=region)
+    data = DDGS(proxy=proxy).suggestions(keywords=keywords, region=region)
     filename = f"suggestions_{_sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print":
         _print_data(data)
     elif output == "csv":
         _save_csv(f"{filename}.csv", data)
     elif output == "json":
         _save_json(f"{filename}.json", data)
```

### Comparing `duckduckgo_search-5.2.2/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-5.3.0b1/duckduckgo_search/duckduckgo_search.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,42 +5,51 @@
 from typing import Any, Awaitable, Dict, Optional, Type, Union
 
 from .duckduckgo_search_async import AsyncDDGS
 
 
 class DDGS(AsyncDDGS):
     _loop: asyncio.AbstractEventLoop = asyncio.new_event_loop()
-    Thread(target=_loop.run_forever, daemon=True).start()  # Start the event loop run in a separate thread.
+    Thread(target=_loop.run_forever, daemon=True).start()  # Start the event loop in a separate thread.
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
-        proxies: Union[Dict[str, str], str, None] = None,
+        proxy: Optional[str] = None,
+        proxies: Union[Dict[str, str], str, None] = None,  # deprecated
         timeout: Optional[int] = 10,
     ) -> None:
-        super().__init__(headers=headers, proxies=proxies, timeout=timeout)
+        """Initialize the DDGS object.
+
+        Args:
+            headers (dict, optional): Dictionary of headers for the HTTP client. Defaults to None.
+            proxy (str, optional): proxy for the HTTP client, supports http/https/socks5 protocols.
+                example: "http://user:pass@example.com:3128". Defaults to None.
+            timeout (int, optional): Timeout value for the HTTP client. Defaults to 10.
+        """
+        super().__init__(headers=headers, proxy=proxy, proxies=proxies, timeout=timeout)
 
     def __enter__(self) -> "DDGS":
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         self._close_session()
 
     def __del__(self) -> None:
-        if self._asession._closed is False:
+        if self._asession.is_closed is False:
             self._close_session()
 
     def _close_session(self) -> None:
         """Close the curl-cffi async session."""
-        self._run_async_in_thread(self._asession.close())
+        self._run_async_in_thread(self._asession.aclose())
 
     def _run_async_in_thread(self, coro: Awaitable[Any]) -> Any:
         """Runs an async coroutine in a separate thread."""
         future: Future[Any] = asyncio.run_coroutine_threadsafe(coro, self._loop)
         result = future.result()
         return result
```

### Comparing `duckduckgo_search-5.2.2/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-5.3.0b1/duckduckgo_search/duckduckgo_search_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import asyncio
 import logging
 import warnings
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import suppress
 from datetime import datetime, timezone
 from decimal import Decimal
-from functools import partial
+from functools import cached_property, partial
 from itertools import cycle, islice
 from types import TracebackType
-from typing import Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
-from curl_cffi import requests
+import httpx
 
 try:
+    from lxml.html import Element, document_fromstring
     from lxml.html import HTMLParser as LHTMLParser
-    from lxml.html import document_fromstring
 
     LXML_AVAILABLE = True
 except ImportError:
     LXML_AVAILABLE = False
 
 from .exceptions import DuckDuckGoSearchException, RatelimitException, TimeoutException
 from .utils import (
     _calculate_distance,
     _extract_vqd,
+    _get_headers,
+    _get_ssl_context,
     _normalize,
     _normalize_url,
     _text_extract_json,
     json_loads,
 )
 
 logger = logging.getLogger("duckduckgo_search.AsyncDDGS")
@@ -37,86 +39,97 @@
     """DuckDuckgo_search async class to get search results from duckduckgo.com."""
 
     _executor: Optional[ThreadPoolExecutor] = None
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
-        proxies: Union[Dict[str, str], str, None] = None,
+        proxy: Optional[str] = None,
+        proxies: Union[Dict[str, str], str, None] = None,  # deprecated
         timeout: Optional[int] = 10,
     ) -> None:
         """Initialize the AsyncDDGS object.
 
         Args:
             headers (dict, optional): Dictionary of headers for the HTTP client. Defaults to None.
-            proxies (Union[dict, str], optional): Proxies for the HTTP client (can be dict or str). Defaults to None.
+            proxy (str, optional): proxy for the HTTP client, supports http/https/socks5 protocols.
+                example: "http://user:pass@example.com:3128". Defaults to None.
             timeout (int, optional): Timeout value for the HTTP client. Defaults to 10.
         """
-        self.proxies = {"all": proxies} if isinstance(proxies, str) else proxies
-        self._asession = requests.AsyncSession(
-            headers=headers,
-            proxies=self.proxies,
+        self.proxy: Optional[str] = proxy
+        assert self.proxy is None or isinstance(self.proxy, str), "proxy must be a str"
+        if not proxy and proxies:
+            warnings.warn("'proxies' is deprecated, use 'proxy' instead.", stacklevel=1)
+            self.proxy = proxies.get("http") or proxies.get("https") if isinstance(proxies, dict) else proxies
+        self._asession = httpx.AsyncClient(
+            headers=_get_headers() if headers is None else headers,
+            proxy=self.proxy,
             timeout=timeout,
-            impersonate="chrome",
-            allow_redirects=False,
+            follow_redirects=False,
+            http2=True,
+            verify=_get_ssl_context(),
         )
         self._asession.headers["Referer"] = "https://duckduckgo.com/"
-        self._parser: Optional[LHTMLParser] = None
         self._exception_event = asyncio.Event()
 
     async def __aenter__(self) -> "AsyncDDGS":
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[BaseException] = None,
+        exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        await self._asession.close()
+        await self._asession.aclose()
 
     def __del__(self) -> None:
-        if self._asession._closed is False:
+        if self._asession.is_closed is False:
             with suppress(RuntimeError):
-                asyncio.create_task(self._asession.close())
+                asyncio.create_task(self._asession.aclose())
 
-    def _get_parser(self) -> "LHTMLParser":
+    @cached_property
+    def parser(self) -> "LHTMLParser":
         """Get HTML parser."""
-        if self._parser is None:
-            self._parser = LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
-        return self._parser
+        return LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
 
-    def _get_executor(self, max_workers: int = 1) -> ThreadPoolExecutor:
+    @classmethod
+    def _get_executor(cls, max_workers: int = 1) -> ThreadPoolExecutor:
         """Get ThreadPoolExecutor. Default max_workers=1, because >=2 leads to a big overhead"""
-        if AsyncDDGS._executor is None:
-            AsyncDDGS._executor = ThreadPoolExecutor(max_workers=max_workers)
-        return AsyncDDGS._executor
+        if cls._executor is None:
+            cls._executor = ThreadPoolExecutor(max_workers=max_workers)
+        return cls._executor
+
+    @property
+    def executor(cls) -> ThreadPoolExecutor:
+        return cls._get_executor()
 
     async def _aget_url(
         self,
         method: str,
         url: str,
-        data: Optional[Union[Dict[str, str], bytes]] = None,
+        content: Optional[Union[str, bytes]] = None,
+        data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, str]] = None,
     ) -> bytes:
         if self._exception_event.is_set():
             raise DuckDuckGoSearchException("Exception occurred in previous call.")
         try:
-            resp = await self._asession.request(method, url, data=data, params=params)
+            resp = await self._asession.request(method, url, content=content, data=data, params=params)
+        except httpx.TimeoutException as ex:
+            self._exception_event.set()
+            raise TimeoutException(f"{url} {type(ex).__name__}: {ex}") from ex
         except Exception as ex:
             self._exception_event.set()
-            if "time" in str(ex).lower():
-                raise TimeoutException(f"{url} {type(ex).__name__}: {ex}") from ex
             raise DuckDuckGoSearchException(f"{url} {type(ex).__name__}: {ex}") from ex
-        logger.debug(f"_aget_url() {resp.url} {resp.status_code} {resp.elapsed:.2f} {len(resp.content)}")
         if resp.status_code == 200:
-            return cast(bytes, resp.content)
+            return resp.content
         self._exception_event.set()
         if resp.status_code in (202, 301, 403):
-            raise RatelimitException(f"{resp.url} {resp.status_code}")
+            raise RatelimitException(f"{resp.url} {resp.status_code} Ratelimit")
         raise DuckDuckGoSearchException(f"{resp.url} return None. {params=} {data=}")
 
     async def _aget_vqd(self, keywords: str) -> str:
         """Get vqd value for a search query."""
         resp_content = await self._aget_url("POST", "https://duckduckgo.com", data={"q": keywords})
         return _extract_vqd(resp_content, keywords)
 
@@ -290,16 +303,16 @@
         async def _text_html_page(s: int, page: int) -> None:
             priority = page * 100
             payload["s"] = f"{s}"
             resp_content = await self._aget_url("POST", "https://html.duckduckgo.com/html", data=payload)
             if b"No  results." in resp_content:
                 return
 
-            tree = await self._asession.loop.run_in_executor(
-                self._get_executor(), partial(document_fromstring, resp_content, self._get_parser())
+            tree: Element = await asyncio.get_running_loop().run_in_executor(
+                self.executor, partial(document_fromstring, resp_content, self.parser)
             )
 
             for e in tree.xpath("//div[h2]"):
                 href = e.xpath("./a/@href")
                 href = href[0] if href else None
                 if (
                     href
@@ -369,16 +382,16 @@
         async def _text_lite_page(s: int, page: int) -> None:
             priority = page * 100
             payload["s"] = f"{s}"
             resp_content = await self._aget_url("POST", "https://lite.duckduckgo.com/lite/", data=payload)
             if b"No more results." in resp_content:
                 return
 
-            tree = await self._asession.loop.run_in_executor(
-                self._get_executor(), partial(document_fromstring, resp_content, self._get_parser())
+            tree: Element = await asyncio.get_running_loop().run_in_executor(
+                self.executor, partial(document_fromstring, resp_content, self.parser)
             )
 
             data = zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr"))
             for i, e in data:
                 if i == 1:
                     href = e.xpath(".//a//@href")
                     href = href[0] if href else None
@@ -841,15 +854,15 @@
             lat_b, lon_r = Decimal(coordinates[0]), Decimal(coordinates[3])
 
         # if a radius is specified, expand the search square
         lat_t += Decimal(radius) * Decimal(0.008983)
         lat_b -= Decimal(radius) * Decimal(0.008983)
         lon_l -= Decimal(radius) * Decimal(0.008983)
         lon_r += Decimal(radius) * Decimal(0.008983)
-        logger.debug(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
+        logger.info(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
 
         cache = set()
         results: List[Dict[str, str]] = []
 
         async def _maps_page(
             bbox: Tuple[Decimal, Decimal, Decimal, Decimal],
         ) -> Optional[List[Dict[str, str]]]:
@@ -968,15 +981,15 @@
         results = []
 
         async def _translate_keyword(keyword: str) -> None:
             resp_content = await self._aget_url(
                 "POST",
                 "https://duckduckgo.com/translation.js",
                 params=payload,
-                data=keyword.encode(),
+                content=keyword,
             )
             page_data = json_loads(resp_content)
             page_data["original"] = keyword
             results.append(page_data)
 
         if isinstance(keywords, str):
             keywords = [keywords]
```

### Comparing `duckduckgo_search-5.2.2/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.2.2/pyproject.toml` & `duckduckgo_search-5.3.0b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "click>=8.1.7",    
-    "curl_cffi>=0.6.2",
+    "click>=8.1.7",  
+    "httpx[brotli, http2, socks]>=0.27.0",
     "orjson>=3.10.0",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
@@ -46,31 +46,33 @@
 [project.optional-dependencies]
 lxml = [
     "lxml>=5.1.1",
 ]
 dev = [
     "mypy>=1.9.0",
     "pytest>=8.1.1",
-    "ruff>=0.3.4",
+    "ruff>=0.3.5",
 ]
 
 [tool.ruff]
 line-length = 120
-target-version = "py38"
 exclude = ["tests"]
 
 [tool.ruff.lint]
 select = [
     "E",  # pycodestyle
     "F",  # Pyflakes
     "UP",  # pyupgrade
     "B",  # flake8-bugbear
     "SIM",  # flake8-simplify
     "I",  # isort
 ]
 ignore = ["D100"]
 
+[tool.ruff.per-file-ignores]
+"utils.py" = ["E501"]
+
 [tool.mypy]
 python_version = "3.8"
-ignore_missing_imports = true
 strict = true
 exclude = ['cli\.py$', '__main__\.py$', "tests/", "build/"]
+
```

### Comparing `duckduckgo_search-5.2.2/tests/test_cli.py` & `duckduckgo_search-5.3.0b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.2.2/tests/test_duckduckgo_search.py` & `duckduckgo_search-5.3.0b1/tests/test_duckduckgo_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 def test_text_lite():
     results = DDGS().text("dog", backend="lite", max_results=30)
     assert 27 <= len(results) <= 30
 
 
 def test_images():
-    results = DDGS().images("airplane", max_results=140)
-    assert 135 <= len(results) <= 140
+    results = DDGS().images("flower", max_results=200)
+    assert 100 <= len(results) <= 200
 
 
 def test_videos():
     results = DDGS().videos("sea", max_results=40)
     assert 37 <= len(results) <= 40
```

