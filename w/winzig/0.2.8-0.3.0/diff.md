# Comparing `tmp/winzig-0.2.8.tar.gz` & `tmp/winzig-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winzig-0.2.8.tar", max compression
+gzip compressed data, was "winzig-0.3.0.tar", max compression
```

## Comparing `winzig-0.2.8.tar` & `winzig-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1051 2024-03-13 16:34:56.468996 winzig-0.2.8/LICENSE
--rw-r--r--   0        0        0     6858 2024-03-24 15:09:36.698910 winzig-0.2.8/README.md
--rw-r--r--   0        0        0      870 2024-03-25 07:45:22.291470 winzig-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-10 23:01:38.883435 winzig-0.2.8/winzig/__init__.py
--rw-r--r--   0        0        0      124 2024-03-23 19:58:14.447350 winzig-0.2.8/winzig/commands/__init__.py
--rw-r--r--   0        0        0     1940 2024-03-25 07:17:53.912980 winzig-0.2.8/winzig/commands/crawl.py
--rw-r--r--   0        0        0     1469 2024-03-23 20:28:31.508519 winzig-0.2.8/winzig/commands/search.py
--rw-r--r--   0        0        0      457 2024-03-23 20:23:25.839389 winzig-0.2.8/winzig/commands/tui.py
--rw-r--r--   0        0        0      585 2024-03-19 16:19:26.741566 winzig-0.2.8/winzig/config.py
--rw-r--r--   0        0        0       54 2024-03-22 17:22:38.871866 winzig-0.2.8/winzig/console.py
--rw-r--r--   0        0        0     6857 2024-03-25 07:15:48.525956 winzig-0.2.8/winzig/crawler.py
--rw-r--r--   0        0        0      487 2024-03-19 16:19:26.741566 winzig-0.2.8/winzig/database.py
--rw-r--r--   0        0        0      508 2024-03-23 20:41:27.782850 winzig-0.2.8/winzig/main.py
--rw-r--r--   0        0        0     1532 2024-03-25 07:26:59.406254 winzig-0.2.8/winzig/models.py
--rw-r--r--   0        0        0     2629 2024-03-23 11:43:24.146280 winzig-0.2.8/winzig/search_engine.py
--rw-r--r--   0        0        0     1454 2024-03-22 18:37:02.319908 winzig-0.2.8/winzig/tf_idf.py
--rw-r--r--   0        0        0     2627 2024-03-24 14:41:48.574090 winzig-0.2.8/winzig/tui.py
--rw-r--r--   0        0        0      137 2024-03-23 10:58:50.710710 winzig-0.2.8/winzig/tui.tcss
--rw-r--r--   0        0        0      835 2024-03-23 11:33:21.553129 winzig-0.2.8/winzig/utils.py
--rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 winzig-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1051 2024-03-27 08:29:21.678862 winzig-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8192 2024-04-01 13:27:37.086231 winzig-0.3.0/README.md
+-rw-r--r--   0        0        0      928 2024-04-02 14:13:29.152612 winzig-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-27 08:29:21.682862 winzig-0.3.0/winzig/__init__.py
+-rw-r--r--   0        0        0      166 2024-03-28 15:09:01.786335 winzig-0.3.0/winzig/commands/__init__.py
+-rw-r--r--   0        0        0     3035 2024-03-29 16:07:42.786750 winzig-0.3.0/winzig/commands/crawl.py
+-rw-r--r--   0        0        0     2683 2024-03-29 16:16:32.663562 winzig-0.3.0/winzig/commands/export.py
+-rw-r--r--   0        0        0     1847 2024-04-01 13:06:50.414359 winzig-0.3.0/winzig/commands/search.py
+-rw-r--r--   0        0        0      457 2024-03-27 08:29:21.682862 winzig-0.3.0/winzig/commands/tui.py
+-rw-r--r--   0        0        0      585 2024-03-27 08:29:21.682862 winzig-0.3.0/winzig/config.py
+-rw-r--r--   0        0        0       54 2024-03-27 08:29:21.682862 winzig-0.3.0/winzig/console.py
+-rw-r--r--   0        0        0     7303 2024-04-01 07:19:41.817831 winzig-0.3.0/winzig/crawler.py
+-rw-r--r--   0        0        0      487 2024-03-27 08:29:21.682862 winzig-0.3.0/winzig/database.py
+-rw-r--r--   0        0        0      540 2024-03-29 15:04:17.649649 winzig-0.3.0/winzig/main.py
+-rw-r--r--   0        0        0     3888 2024-03-29 16:14:49.968180 winzig-0.3.0/winzig/management.py
+-rw-r--r--   0        0        0     1701 2024-03-29 15:49:17.725400 winzig-0.3.0/winzig/models.py
+-rw-r--r--   0        0        0     2958 2024-04-01 13:15:31.529004 winzig-0.3.0/winzig/search_engine.py
+-rw-r--r--   0        0        0     1454 2024-03-27 08:29:21.686862 winzig-0.3.0/winzig/tf_idf.py
+-rw-r--r--   0        0        0     4165 2024-04-05 13:48:39.009995 winzig-0.3.0/winzig/tui.py
+-rw-r--r--   0        0        0      266 2024-04-05 13:49:03.789810 winzig-0.3.0/winzig/tui.tcss
+-rw-r--r--   0        0        0      805 2024-03-29 14:51:47.362164 winzig-0.3.0/winzig/utils.py
+-rw-r--r--   0        0        0     9178 1970-01-01 00:00:00.000000 winzig-0.3.0/PKG-INFO
```

### Comparing `winzig-0.2.8/LICENSE` & `winzig-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `winzig-0.2.8/README.md` & `winzig-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -108,51 +108,81 @@
 ```
 
 #### Feeds
 
 The `feeds` subcommand allows you to fetch and extract content from the posts of the specified feeds provided. The feeds are stored in the database so there is no need to provide a file every time.
 
 ```bash
-winzig crawl feeds --file="feeds"
+winzig crawl feeds --file feeds.txt
 ```
 
 ```bash
 winzig crawl feeds
 ```
 
+You can also provide feed URLs directly as arguments. This feeds, if valid, will also be saved to the database.  
+
+```bash
+winzig crawl feeds https://chriscoyier.net/feed/
+```
+
 #### Posts
 
 By using the `posts` subcommand, you can extract content directly from the posts listed in the provided file.  
 
 ```bash
 winzig crawl posts --file="posts"
 ```
 
+Or, if you prefer it, you can pass the URLs as arguments:  
+
+```bash
+winzig crawl posts https://textual.textualize.io/blog/2024/02/11/file-magic-with-the-python-standard-library/
+```
+
 ### Searching
 
 The following command starts a search for content matching the provided query and after a few seconds will return a list of relevant links.  
 
 ```bash
 winzig search --query="async databases with sqlalchemy"
 ```
 
 By default the number of results is `5` but you can change this by using the `-n` flag.  
 
 ```bash
 winzig search --query="async databases with sqlalchemy" -n 10
 ```
 
+You can add filters to your search results by using the `--filter` flag. Currently, the only filter supported is `domain`, which allows you to specify one or more domains to filter the search results.
+
+```bash
+winzig search --query "read large files" --filter domain='motherduck, textualize'
+```
+
 ### TUI
 
 If you prefer you can use the TUI to interact with the search engine. The TUI is its early stage but it offers basic functionality and faster search experiences compared to the `search` command since the content is indexed once and not each time you want to search something.  
 
 ```bash
 winzig tui
 ```
 
+### Export
+
+You can export your feeds and your posts to plain text or CSV format using the `export` command and the `feeds` and `posts` subcommands.  
+
+```bash
+winzig export feeds --format csv --output feeds.csv
+```
+
+```bash
+winzig export posts
+```
+
 ## More feeds, please
 
 If you're looking to expand your feed collection significantly, you can get a curated list of feeds from the [blogs.hn](https://github.com/surprisetalk/blogs.hn) repository with just a couple of commands.  
 
 1. Download the JSON file containing the relevant information from the `blogs.hn` repository.
 
 ```bash
@@ -163,24 +193,32 @@
 
 ```bash
 jq -r '.[] | select(.feed != null) | .feed' hn.json >> urls
 ```
 
 > Incorporating feeds from the resultant file will significantly increase the number of requests made. Based on my experience, fetching posts from each feed, extracting content, and performing other operations may take approximately 20 to 30 minutes, depending on your Internet connection speed. The search speed will still be pretty fast.
 
+## About the ranking function
+
+Like the `microsearch` project, the ranking function used in winzig is the [Okapi BM25](https://en.wikipedia.org/wiki/Okapi_BM25). However, I am planning to add support for other variants of BM25, such as BM25+.
+
+### BM11 and BM15 variants
+
+If you're using the CLI for search, you have the flexibility to adjust the `k1` and `b` parameters. By manipulating the later to `0` or `1`, you can transform the BM25 ranking function into BM15 and BM11 variants, respectively:  
+
+```bash
+winzig search --query="build search engine" --b 0 # BM15
+winzig search --query="build search engine" --b 1 # BM11
+```
+
 ## Roadmap
 
-- [x] Add a TUI using [`textual`](https://textual.textualize.io/).  
-- [x] Build inverted index after crawling.  
-- [x] Make the CLI nicer.  
-- [x] Improve logging.
-- [x] Improve error handling.
-- [x] Add support for crawling individual posts.
 - [ ] Improve TUI.
 - [ ] Add tests.  
+- [ ] Add multiple ranking functions.
 - [ ] Add support for documents like markdown or plain text files.  
 - [ ] Add support for PDFs and other formats.  
 - [ ] Add commands to manage the SQLite database.  
 - [ ] Add support for advanced queries.  
 
 ## Contributing
```

### Comparing `winzig-0.2.8/winzig/commands/crawl.py` & `winzig-0.3.0/winzig/commands/crawl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,115 @@
 import asyncio
-from pathlib import Path
 import click
 from sqlalchemy.ext.asyncio import AsyncSession
 from winzig.crawler import crawl_from_feeds, crawl_links
 from winzig.tf_idf import recalculate_tf_idf
+from winzig.management import get_feeds_from_csv, get_posts_from_csv, remove_empty_feeds
 
 
 @click.group(
     invoke_without_command=True,
     help="Crawl and extract content from feeds and posts. If no subcommand is provided, it automatically crawls previously saved feeds by default.",
 )
 @click.pass_context
 def crawl(ctx):
     if ctx.invoked_subcommand is None:
-        asyncio.run(_crawl_feeds(ctx.obj["engine"], None, None))
+        asyncio.run(_crawl_feeds(ctx.obj["engine"], [], None, False, True))
 
 
 @click.command(
     name="feeds",
     help="Crawl and extract content from the posts of the specified feeds.",
 )
 @click.option(
     "-f",
     "--file",
-    type=Path,
+    type=click.File(),
     default=None,
     help="Path to the file containing feed sources. If empty, previous feeds added to the database will be used.",
 )
 @click.option(
     "-m",
     "--max",
     type=int,
     default=None,
     help="Maximum number of posts to crawl from each feed.",
 )
+@click.option(
+    "-p",
+    "--prune",
+    type=bool,
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Remove feeds without any posts associated from the database after crawling.",
+)
+@click.option(
+    "--fetch/--no-fetch",
+    type=bool,
+    is_flag=True,
+    show_default=True,
+    default=True,
+    help="Toggle to enable or disable fetching content.",
+)
+@click.argument("urls", nargs=-1)
 @click.pass_context
-def crawl_feeds(ctx, file: Path, max: int):
-    asyncio.run(_crawl_feeds(ctx.obj["engine"], file, max))
+def crawl_feeds(ctx, file, urls, max, prune, fetch):
+    feed_urls = []
+
+    if file:
+        if file.name.endswith(".csv"):
+            feed_urls = get_feeds_from_csv(file)
+        else:
+            feed_urls = file.read().splitlines()
+
+    if urls:
+        feed_urls.extend(urls)
 
+    asyncio.run(_crawl_feeds(ctx.obj["engine"], feed_urls, max, prune, fetch))
 
-async def _crawl_feeds(engine, file: Path | None, max: int | None):
+
+async def _crawl_feeds(engine, urls: list, max: int | None, prune: bool, fetch: bool):
     async with AsyncSession(engine) as session:
-        await crawl_from_feeds(
-            session,
-            file,
-            max,
-        )
-        await recalculate_tf_idf(session)
+        if fetch:
+            await crawl_from_feeds(session, urls, max)
+            await recalculate_tf_idf(session)
+
+        if prune:
+            await remove_empty_feeds(session)
 
 
 @click.command(
     name="posts",
     help="Crawl and extract content from the posts specified in a file.",
 )
 @click.option(
     "-f",
     "--file",
-    type=Path,
+    type=click.File(),
     help="Path to the file containing the links to crawl.",
 )
+@click.argument("urls", nargs=-1)
 @click.pass_context
-def crawl_posts(ctx, file: Path):
-    asyncio.run(_crawl_posts(ctx.obj["engine"], file))
+def crawl_posts(ctx, file, urls):
+    post_urls = []
+
+    if file:
+        if file.name.endswith(".csv"):
+            post_urls = get_posts_from_csv(file)
+        else:
+            post_urls = file.read().splitlines()
+
+    if urls:
+        post_urls.extend(urls)
+
+    asyncio.run(_crawl_posts(ctx.obj["engine"], post_urls))
 
 
-async def _crawl_posts(engine, file: Path):
+async def _crawl_posts(engine, urls: list):
     async with AsyncSession(engine) as session:
-        await crawl_links(session, file)
+        await crawl_links(session, urls)
         await recalculate_tf_idf(session)
 
 
 crawl.add_command(crawl_posts)
 crawl.add_command(crawl_feeds)
```

### Comparing `winzig-0.2.8/winzig/commands/search.py` & `winzig-0.3.0/winzig/commands/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from typing import Tuple
 import click
 from sqlalchemy.ext.asyncio import AsyncSession
 from winzig.search_engine import SearchEngine
 from winzig.utils import get_top_urls
 from winzig.console import console
 
 
@@ -23,32 +24,51 @@
     type=float,
     default=1.5,
     help="Term saturation factor. Higher values prioritize the frequency of query terms in a document.",
     show_default=True,
 )
 @click.option(
     "--b",
-    type=float,
+    type=click.FloatRange(0.0, 1.0),
     default=0.75,
     help="Length normalization factor. on the relevance score. Lower values favor shorter documents.",
     show_default=True,
 )
 @click.option(
     "-n",
     type=int,
     default=5,
     help="Maximum number of search results to display.",
     show_default=True,
 )
+@click.option(
+    "--filter",
+    "-f",
+    type=str,
+    multiple=True,
+    help="Filter search results by 'key=value' pairs.",
+)
 @click.pass_context
-def search(ctx, query: str, k1: float, b: float, n: int):
-    asyncio.run(_search(ctx.obj["engine"], query, k1, b, n))
+def search(ctx, query: str, k1: float, b: float, n: int, filter: Tuple[str]):
+    filters = {}
+    for f in filter:
+        key, value = f.split("=")
+        filters[key] = value
+
+    asyncio.run(_search(ctx.obj["engine"], query, k1, b, n, filters))
 
 
-async def _search(engine, query: str, k1: float, b: float, n: int):
+async def _search(
+    engine,
+    query: str,
+    k1: float,
+    b: float,
+    n: int,
+    filters: dict[str, str],
+):
     async with AsyncSession(engine) as session:
-        search_engine = SearchEngine(session, k1=k1, b=b)
+        search_engine = SearchEngine(session, filters=filters, k1=k1, b=b)
         search_results = await search_engine.search(query)
         search_results = get_top_urls(search_results, n)
 
         for result in search_results:
             console.print(f"- [green]{result}[/green]")
```

### Comparing `winzig-0.2.8/winzig/config.py` & `winzig-0.3.0/winzig/config.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.8/winzig/crawler.py` & `winzig-0.3.0/winzig/crawler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 from collections import Counter
-from pathlib import Path
-from itertools import batched
-import httpx
+import aiohttp
 import feedparser
+import tldextract
 from sqlalchemy import select
 from sqlalchemy.ext.asyncio import AsyncSession
 from selectolax.parser import HTMLParser
 from winzig.models import Feed, Occurrence, Post
 from winzig.utils import normalize_text
 from winzig.console import console
 
@@ -15,108 +14,107 @@
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:123.0) Gecko/20100101 Firefox/123.0",
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8",
     "Accept-Encoding": "gzip, deflate",
     "Accept-Language": "en-GB,en;q=0.6",
 }
 
 
-async def fetch_content(client: httpx.AsyncClient, url: str) -> bytes | None:
+async def fetch_content(client: aiohttp.ClientSession, url: str) -> str | None:
     try:
-        async with client.stream("GET", url) as response:
-            if response.status_code >= 400:
+        async with client.get(url) as resp:
+            if resp.status >= 400:
                 console.log(
-                    f"[red bold]Error[/red bold]: Bad status from '{url}': {response.status_code}"
+                    f"[red bold]ERROR[/red bold]: Bad status from '{url}': {resp.status}"
                 )
                 return None
 
-            return await response.aread()
-    except httpx.HTTPError:
-        console.log(f"[red bold]Error[/red bold]: Got HTTP error from '{url}'")
-        return None
-    except ValueError as e:
-        console.log(f"[red bold]Error[/red bold]: Failed to fetch '{url}': {e}")
+            return await resp.text()
+    except aiohttp.ClientError as e:
+        console.log(f"[red bold]ERROR[/red bold]: Failed to fetch '{url}': {e}")
         return None
 
 
-def clean_content(html: bytes) -> str:
+def clean_content(html: str) -> str:
     tree = HTMLParser(html)
     for tag in tree.css(
         "script, style, link, noscript, object, img, embed, iframe, svg, canvas, form, audio, video"
     ):
         tag.decompose()
     text = "".join(node.text(deep=True) for node in tree.css("main"))
     lines = (line.strip() for line in text.splitlines())
     chunks = (phrase.strip() for line in lines for phrase in line.split(" "))
     cleaned_text = " ".join(chunk for chunk in chunks if chunk)
 
     return cleaned_text
 
 
-def is_feed(url: str) -> bool:
-    try:
-        feed = feedparser.parse(url)
-        return True if feed.version else False
-    except Exception as e:
-        console.log(f"[red bold]Error[/red bold]: Parsing feed '{url}': {e}")
-        return False
-
-
 async def get_posts_from_feed(
-    session: AsyncSession, feed_id: int, url: str, max: int | None
+    session: AsyncSession,
+    client: aiohttp.ClientSession,
+    feed: Feed,
+    max: int | None,
 ) -> list[str]:
     try:
-        feed = feedparser.parse(url)
-        statement = select(Post).where(Post.feed_id == feed_id)
+        resp_text = await fetch_content(client, feed.url)
+        if not resp_text:
+            console.log(
+                f"[bold red]ERROR[/bold red]: Failed to get posts from '{feed.url}'"
+            )
+            return []
+
+        d = feedparser.parse(resp_text)
+        statement = select(Post).where(Post.feed_id == feed.id)
         results = await session.execute(statement)
         results = results.scalars()
         posts_db_urls = {post.url for post in results}
 
         if max:
             return [
                 entry.link
-                for entry in feed.entries[:max]
+                for entry in d.entries[:max]
                 if entry.link not in posts_db_urls
             ]
         else:
             return [
-                entry.link for entry in feed.entries if entry.link not in posts_db_urls
+                entry.link for entry in d.entries if entry.link not in posts_db_urls
             ]
     except Exception as e:
-        console.log(f"[red bold]Error[/red bold]: Parsing feed '{url}': {e}")
+        console.log(f"[red bold]ERROR[/red bold]: Parsing feed '{feed.url}': {e}")
         return []
 
 
 async def process_post(
     session: AsyncSession,
-    client: httpx.AsyncClient,
+    client: aiohttp.ClientSession,
     feed: Feed | None,
     url: str,
 ) -> None:
     try:
-        response_text = await fetch_content(client, url)
-        if not response_text:
+        resp_text = await fetch_content(client, url)
+        if not resp_text:
             return None
     except Exception as e:
         console.log(
-            f"[red bold]Error[/red bold]: Failed to extract content from '{url}': {e}"
+            f"[red bold]ERROR[/red bold]: Failed to extract content from '{url}': {e}"
         )
         return None
 
     try:
-        cleaned_content = clean_content(response_text)
+        cleaned_content = clean_content(resp_text)
         if not cleaned_content:
             return
     except Exception as e:
         console.log(
-            f"[red bold]Error[/red bold]: Failed to clean content from '{url}': {e}"
+            f"[red bold]ERROR[/red bold]: Failed to clean content from '{url}': {e}"
         )
         return None
 
     post = Post(
         url=url,
+        domain=tldextract.extract(url).domain,
         content=cleaned_content,
         feed=feed,
         length=len(cleaned_content),
     )
     session.add(post)
 
     words = Counter(normalize_text(post.content).split(" "))
@@ -124,80 +122,112 @@
         Occurrence(word=word, count=count, post=post)
         for word, count in words.items()
         if len(word) > 2
     ]
     session.add_all(occurrences)
 
 
-async def add_feeds_from_file(session: AsyncSession, file: Path):
-    if not file.exists():
-        console.log(f"[bold red]ERROR[/bold red]: File '{file}' doesn't exist")
-        return
+async def save_feed(
+    session: AsyncSession, client: aiohttp.ClientSession, url: str
+) -> None:
+    resp_text = await fetch_content(client, url)
+    if not resp_text:
+        console.log(
+            f"[bold red]ERROR[/bold red]: URL '{url}' doesn't seem to be a valid RSS feed"
+        )
+        return None
+
+    d = feedparser.parse(resp_text)
+    feed_title = d.feed.get("title", None)
+    feed_description = d.feed.get("description", None)
+
+    session.add(
+        Feed(
+            url=url,
+            title=feed_title,
+            description=feed_description,
+        )
+    )
+    console.log(f"[bold green]SUCCESS[/bold green]: New feed '{url}' added")
+
 
-    with open(file, "r") as f:
-        for line in f:
-            url = line.strip()
+async def add_new_feeds(
+    session: AsyncSession,
+    client: aiohttp.ClientSession,
+    urls: list[str],
+) -> None:
+    with console.status("Processing feeds...", spinner="earth"):
+        tasks = []
+        for url in urls:
+            url = url.strip()
             feed = await session.execute(select(Feed).where(Feed.url == url))
             feed = feed.scalar()
-            if not feed:
-                if not is_feed(url):
-                    console.log(
-                        f"[bold red]ERROR[/bold red]: URL '{url}' doesn't seem to be a valid RSS feed."
-                    )
-                    continue
+            if feed:
+                continue
 
-                new_feed = Feed(url=url)
-                session.add(new_feed)
-                console.log(f"[bold green]SUCCESS[/bold green]: Feed '{url}' added")
+            tasks.append(save_feed(session, client, url))
 
-        await session.commit()
+        if not tasks:
+            console.log("[yellow bold]WARNING[/yellow bold]: No new feeds found")
+        else:
+            console.log(
+                f"[green bold]SUCCESS[/green bold]: Found {len(tasks)} new feeds"
+            )
+
+        await asyncio.gather(*tasks)
 
+    await session.commit()
+    console.log("[green bold]SUCCESS[/green bold]: Feeds processed")
 
-async def crawl_links(session: AsyncSession, file: Path, batch_size: int = 20):
-    if not file.exists():
-        console.log(f"[bold red]ERROR[/bold red]: File '{file}' doesn't exist")
+
+async def crawl_links(session: AsyncSession, urls: list[str]):
+    if len(urls) == 0:
+        console.log("[red bold]ERROR[/red bold]: No URLs received")
         return
 
-    urls = []
-    with open(file, "r") as f:
-        for line in f:
-            url = line.strip()
-            post = await session.execute(select(Post).where(Post.url == url))
-            post = post.scalar()
-            if not post:
-                urls.append(url)
+    post_urls = []
+    for url in urls:
+        url = url.strip()
+        post = await session.execute(select(Post).where(Post.url == url))
+        post = post.scalar()
+        if not post:
+            post_urls.append(url)
 
-    async with httpx.AsyncClient(headers=headers, follow_redirects=True) as client:
+    async with aiohttp.ClientSession(headers=headers) as client:
         with console.status("Fetching posts...", spinner="earth") as status:
-            for batch in batched(urls, batch_size):
-                tasks = [process_post(session, client, None, url) for url in batch]
+            tasks = [process_post(session, client, None, url) for url in post_urls]
 
-                status.update("Fetching posts...")
-                await asyncio.gather(*tasks)
-                await session.commit()
+            status.update("Fetching posts...")
+            await asyncio.gather(*tasks)
 
+        await session.commit()
         console.log("[green bold]SUCCESS[/green bold]: Posts fetched")
 
 
 async def crawl_from_feeds(
-    session: AsyncSession, file: Path | None = None, max: int | None = None
+    session: AsyncSession,
+    urls: list[str],
+    max: int | None = None,
 ):
-    if file is not None:
-        await add_feeds_from_file(session, file)
-
-    feeds = await session.execute(select(Feed))
-    feeds = feeds.scalars().all()
-    if not feeds:
-        console.log("[red]Error[/red]: No feeds found!")
-        return
+    async with aiohttp.ClientSession(headers=headers) as client:
+        if len(urls) > 0:
+            await add_new_feeds(session, client, urls)
+
+        feeds = await session.execute(select(Feed))
+        feeds = feeds.scalars().all()
+        if not feeds:
+            console.log("[red]ERROR[/red]: No feeds found!")
+            return
 
-    async with httpx.AsyncClient(headers=headers, follow_redirects=True) as client:
         with console.status("Fetching posts...", spinner="earth") as status:
             for idx, feed in enumerate(feeds):
-                posts = await get_posts_from_feed(session, feed.id, feed.url, max)
+                posts = await get_posts_from_feed(session, client, feed, max)
+                if not posts:
+                    continue
+
                 tasks = [process_post(session, client, feed, post) for post in posts]
 
                 status.update(
                     f"[bold][{idx + 1}/{len(feeds)}][/bold] Fetching posts from '{feed.url}'"
                 )
                 await asyncio.gather(*tasks)
```

### Comparing `winzig-0.2.8/winzig/models.py` & `winzig-0.3.0/winzig/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,26 @@
     pass
 
 
 class Feed(Base):
     __tablename__ = "feeds"
 
     id: Mapped[int] = mapped_column(primary_key=True)
+    title: Mapped[str] = mapped_column(nullable=True)
+    description: Mapped[str] = mapped_column(nullable=True)
     url: Mapped[str] = mapped_column(index=True)
 
     posts: Mapped[List["Post"]] = relationship(back_populates="feed")
 
 
 class Post(Base):
     __tablename__ = "posts"
 
     id: Mapped[int] = mapped_column(primary_key=True)
+    domain: Mapped[str] = mapped_column(nullable=True)
     url: Mapped[str] = mapped_column(index=True)
     content: Mapped[str]
     length: Mapped[int] = mapped_column(default=0)
 
     feed_id: Mapped[int] = mapped_column(ForeignKey("feeds.id"), nullable=True)
     feed: Mapped[Feed] = relationship(back_populates="posts")
```

### Comparing `winzig-0.2.8/winzig/search_engine.py` & `winzig-0.3.0/winzig/search_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from sqlalchemy import func, select
+from sqlalchemy import func, or_, select
 from sqlalchemy.ext.asyncio import AsyncSession
 from winzig.models import Post, Occurrence, Keyword
 from winzig.utils import update_url_scores, normalize_text
 from winzig.console import console
 
 
 class SearchEngine:
     def __init__(
         self,
         session: AsyncSession,
+        filters: dict[str, str] = {},
         k1: float = 1.5,
         b: float = 0.75,
     ) -> None:
+        self.session = session
+        self.filters = filters
         self.k1 = k1
         self.b = b
-        self.session = session
+
         self._avdl = None
 
     async def avdl(self) -> float | None:
         if self._avdl is not None:
             return self._avdl
 
         statement = select(func.count()).select_from(Post)
@@ -47,17 +50,21 @@
         if not keyword:
             return 0.0
 
         return keyword.score
 
     async def bm25(self, kw: str) -> dict[str, float]:
         avdl = await self.avdl()
-        results = await self.session.execute(
-            select(Occurrence, Post).join(Post).where(Occurrence.word == kw)
-        )
+        statement = select(Occurrence, Post).join(Post).where(Occurrence.word == kw)
+        if "domain" in self.filters:
+            domain_filters = self.filters["domain"].split(",")
+            conditions = [Post.domain == domain.strip() for domain in domain_filters]
+            statement = statement.filter(or_(*conditions))
+
+        results = await self.session.execute(statement)
         occurrences = results.fetchall()
 
         search_results = {}
         for occurrence, post in occurrences:
             kw_score = await self.get_kw_score(kw)
             numerator = occurrence.count * (self.k1 + 1)
             denominator = occurrence.count + self.k1 * (
```

### Comparing `winzig-0.2.8/winzig/tf_idf.py` & `winzig-0.3.0/winzig/tf_idf.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.8/winzig/utils.py` & `winzig-0.3.0/winzig/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 import string
 import emoji
 
 emojis = set(emoji.EMOJI_DATA.keys())
+punctuation_and_emojis = set(string.punctuation + "“”’‘¶■▌▲▼└│─√©" + "".join(emojis))
 
-translation_table = str.maketrans(
-    {char: " " for char in string.punctuation + "“”’‘¶■▌▲▼└│─√©" + "".join(emojis)}
-)
+translation_table = str.maketrans(({char: " " for char in punctuation_and_emojis}))
 
 
 def update_url_scores(old: dict[str, float], new: dict[str, float]) -> dict[str, float]:
     for url, score in new.items():
-        if url in old:
-            old[url] += score
-        else:
-            old[url] = score
+        old[url] = old.get(url, 0.0) + score
 
     return old
 
 
 def normalize_text(text: str) -> str:
     normalized = text.translate(translation_table).lower()
     normalized = " ".join(normalized.split())
     return normalized
 
 
 def get_top_urls(scores_dict: dict, n: int):
     sorted_urls = sorted(scores_dict.items(), key=lambda x: x[1], reverse=True)
-    top_n_urls = sorted_urls[:n]
-    top_n_dict = dict(top_n_urls)
+    top_n_dict = dict(sorted_urls[:n])
     return top_n_dict
```

### Comparing `winzig-0.2.8/PKG-INFO` & `winzig-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: winzig
-Version: 0.2.8
+Version: 0.3.0
 Summary: A tiny search engine for personal use.
 Home-page: https://github.com/dnlzrgz/winzig
 License: MIT
 Keywords: search,crawl,sqlite,async,feeds
 Author: dnlzrgz
 Author-email: 24715931+dnlzrgz@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp[speedups] (>=3.9.3,<4.0.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: emoji (>=2.10.1,<3.0.0)
 Requires-Dist: feedparser (>=6.0.11,<7.0.0)
-Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: selectolax (>=0.3.20,<0.4.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.28,<3.0.0)
 Requires-Dist: textual (>=0.52.1,<0.53.0)
+Requires-Dist: tldextract (>=5.1.2,<6.0.0)
 Project-URL: Repository, https://github.com/dnlzrgz/winzig
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # [winzig](https://pypi.org/project/winzig/)
 
@@ -133,51 +134,81 @@
 ```
 
 #### Feeds
 
 The `feeds` subcommand allows you to fetch and extract content from the posts of the specified feeds provided. The feeds are stored in the database so there is no need to provide a file every time.
 
 ```bash
-winzig crawl feeds --file="feeds"
+winzig crawl feeds --file feeds.txt
 ```
 
 ```bash
 winzig crawl feeds
 ```
 
+You can also provide feed URLs directly as arguments. This feeds, if valid, will also be saved to the database.  
+
+```bash
+winzig crawl feeds https://chriscoyier.net/feed/
+```
+
 #### Posts
 
 By using the `posts` subcommand, you can extract content directly from the posts listed in the provided file.  
 
 ```bash
 winzig crawl posts --file="posts"
 ```
 
+Or, if you prefer it, you can pass the URLs as arguments:  
+
+```bash
+winzig crawl posts https://textual.textualize.io/blog/2024/02/11/file-magic-with-the-python-standard-library/
+```
+
 ### Searching
 
 The following command starts a search for content matching the provided query and after a few seconds will return a list of relevant links.  
 
 ```bash
 winzig search --query="async databases with sqlalchemy"
 ```
 
 By default the number of results is `5` but you can change this by using the `-n` flag.  
 
 ```bash
 winzig search --query="async databases with sqlalchemy" -n 10
 ```
 
+You can add filters to your search results by using the `--filter` flag. Currently, the only filter supported is `domain`, which allows you to specify one or more domains to filter the search results.
+
+```bash
+winzig search --query "read large files" --filter domain='motherduck, textualize'
+```
+
 ### TUI
 
 If you prefer you can use the TUI to interact with the search engine. The TUI is its early stage but it offers basic functionality and faster search experiences compared to the `search` command since the content is indexed once and not each time you want to search something.  
 
 ```bash
 winzig tui
 ```
 
+### Export
+
+You can export your feeds and your posts to plain text or CSV format using the `export` command and the `feeds` and `posts` subcommands.  
+
+```bash
+winzig export feeds --format csv --output feeds.csv
+```
+
+```bash
+winzig export posts
+```
+
 ## More feeds, please
 
 If you're looking to expand your feed collection significantly, you can get a curated list of feeds from the [blogs.hn](https://github.com/surprisetalk/blogs.hn) repository with just a couple of commands.  
 
 1. Download the JSON file containing the relevant information from the `blogs.hn` repository.
 
 ```bash
@@ -188,24 +219,32 @@
 
 ```bash
 jq -r '.[] | select(.feed != null) | .feed' hn.json >> urls
 ```
 
 > Incorporating feeds from the resultant file will significantly increase the number of requests made. Based on my experience, fetching posts from each feed, extracting content, and performing other operations may take approximately 20 to 30 minutes, depending on your Internet connection speed. The search speed will still be pretty fast.
 
+## About the ranking function
+
+Like the `microsearch` project, the ranking function used in winzig is the [Okapi BM25](https://en.wikipedia.org/wiki/Okapi_BM25). However, I am planning to add support for other variants of BM25, such as BM25+.
+
+### BM11 and BM15 variants
+
+If you're using the CLI for search, you have the flexibility to adjust the `k1` and `b` parameters. By manipulating the later to `0` or `1`, you can transform the BM25 ranking function into BM15 and BM11 variants, respectively:  
+
+```bash
+winzig search --query="build search engine" --b 0 # BM15
+winzig search --query="build search engine" --b 1 # BM11
+```
+
 ## Roadmap
 
-- [x] Add a TUI using [`textual`](https://textual.textualize.io/).  
-- [x] Build inverted index after crawling.  
-- [x] Make the CLI nicer.  
-- [x] Improve logging.
-- [x] Improve error handling.
-- [x] Add support for crawling individual posts.
 - [ ] Improve TUI.
 - [ ] Add tests.  
+- [ ] Add multiple ranking functions.
 - [ ] Add support for documents like markdown or plain text files.  
 - [ ] Add support for PDFs and other formats.  
 - [ ] Add commands to manage the SQLite database.  
 - [ ] Add support for advanced queries.  
 
 ## Contributing
```

