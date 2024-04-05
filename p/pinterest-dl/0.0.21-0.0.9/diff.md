# Comparing `tmp/pinterest-dl-0.0.21.tar.gz` & `tmp/pinterest-dl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinterest-dl-0.0.21.tar", last modified: Fri Apr  5 10:47:36 2024, max compression
+gzip compressed data, was "pinterest-dl-0.0.9.tar", last modified: Sun Mar 31 15:03:09 2024, max compression
```

## Comparing `pinterest-dl-0.0.21.tar` & `pinterest-dl-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 10:47:36.495099 pinterest-dl-0.0.21/
--rw-rw-rw-   0        0        0    11340 2024-03-30 14:57:38.000000 pinterest-dl-0.0.21/LICENSE
--rw-rw-rw-   0        0        0     5161 2024-04-05 10:47:36.495099 pinterest-dl-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0     4335 2024-04-03 16:56:37.000000 pinterest-dl-0.0.21/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 10:47:36.482508 pinterest-dl-0.0.21/pinterest_dl/
--rw-rw-rw-   0        0        0        0 2024-03-31 15:22:58.000000 pinterest-dl-0.0.21/pinterest_dl/__init__.py
--rw-rw-rw-   0        0        0     5171 2024-04-05 10:45:38.000000 pinterest-dl-0.0.21/pinterest_dl/api.py
--rw-rw-rw-   0        0        0     2096 2024-04-03 16:55:42.000000 pinterest-dl-0.0.21/pinterest_dl/cli_parser.py
--rw-rw-rw-   0        0        0     2582 2024-04-03 18:19:13.000000 pinterest-dl-0.0.21/pinterest_dl/downloader.py
--rw-rw-rw-   0        0        0     1535 2024-03-31 15:22:58.000000 pinterest-dl-0.0.21/pinterest_dl/driver_installer.py
--rw-rw-rw-   0        0        0     2358 2024-03-31 15:22:58.000000 pinterest-dl-0.0.21/pinterest_dl/io.py
--rw-rw-rw-   0        0        0     1550 2024-04-04 15:25:09.000000 pinterest-dl-0.0.21/pinterest_dl/main.py
--rw-rw-rw-   0        0        0      237 2024-04-05 10:47:19.000000 pinterest-dl-0.0.21/pinterest_dl/manifest.json
--rw-rw-rw-   0        0        0     6602 2024-04-03 18:34:03.000000 pinterest-dl-0.0.21/pinterest_dl/scraper.py
--rw-rw-rw-   0        0        0     1611 2024-04-03 18:28:13.000000 pinterest-dl-0.0.21/pinterest_dl/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 10:47:36.494096 pinterest-dl-0.0.21/pinterest_dl.egg-info/
--rw-rw-rw-   0        0        0     5161 2024-04-05 10:47:36.000000 pinterest-dl-0.0.21/pinterest_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2024-04-05 10:47:36.000000 pinterest-dl-0.0.21/pinterest_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 10:47:36.000000 pinterest-dl-0.0.21/pinterest_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-05 10:47:36.000000 pinterest-dl-0.0.21/pinterest_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2024-04-05 10:47:36.000000 pinterest-dl-0.0.21/pinterest_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 10:47:36.000000 pinterest-dl-0.0.21/pinterest_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 10:47:36.495099 pinterest-dl-0.0.21/setup.cfg
--rw-rw-rw-   0        0        0     1395 2024-04-03 11:49:16.000000 pinterest-dl-0.0.21/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-31 15:03:09.870368 pinterest-dl-0.0.9/
+-rw-rw-rw-   0        0        0    11340 2024-03-30 14:57:38.000000 pinterest-dl-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4596 2024-03-31 15:03:09.869861 pinterest-dl-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3879 2024-03-31 15:02:25.000000 pinterest-dl-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-31 15:03:09.854436 pinterest-dl-0.0.9/pinterest_dl/
+-rw-rw-rw-   0        0        0        0 2024-03-29 16:53:40.000000 pinterest-dl-0.0.9/pinterest_dl/__init__.py
+-rw-rw-rw-   0        0        0     2024 2024-03-31 14:55:58.000000 pinterest-dl-0.0.9/pinterest_dl/cli_parser.py
+-rw-rw-rw-   0        0        0     1947 2024-03-31 11:57:09.000000 pinterest-dl-0.0.9/pinterest_dl/downloader.py
+-rw-rw-rw-   0        0        0     1535 2024-03-31 14:55:58.000000 pinterest-dl-0.0.9/pinterest_dl/driver_installer.py
+-rw-rw-rw-   0        0        0     2358 2024-03-30 12:01:50.000000 pinterest-dl-0.0.9/pinterest_dl/io.py
+-rw-rw-rw-   0        0        0     2253 2024-03-31 14:55:58.000000 pinterest-dl-0.0.9/pinterest_dl/main.py
+-rw-rw-rw-   0        0        0      236 2024-03-31 15:01:02.000000 pinterest-dl-0.0.9/pinterest_dl/manifest.json
+-rw-rw-rw-   0        0        0     5528 2024-03-31 14:55:58.000000 pinterest-dl-0.0.9/pinterest_dl/scraper.py
+-rw-rw-rw-   0        0        0      425 2024-03-31 11:18:06.000000 pinterest-dl-0.0.9/pinterest_dl/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-31 15:03:09.869354 pinterest-dl-0.0.9/pinterest_dl.egg-info/
+-rw-rw-rw-   0        0        0     4596 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-03-31 15:03:09.000000 pinterest-dl-0.0.9/pinterest_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-31 15:03:09.870368 pinterest-dl-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1376 2024-03-31 14:56:39.000000 pinterest-dl-0.0.9/setup.py
```

### Comparing `pinterest-dl-0.0.21/LICENSE` & `pinterest-dl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pinterest-dl-0.0.21/PKG-INFO` & `pinterest-dl-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinterest-dl
-Version: 0.0.21
+Version: 0.0.9
 Summary: An unofficial Pinterest image downloader
 Home-page: https://github.com/sean1832/pinterest-dl
 Author: Zeke Zhang
 License: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,42 +12,40 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Console
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: selenium>=4.9.0
-Requires-Dist: pillow>=10.1.0
-Requires-Dist: tqdm
-Requires-Dist: pyexiv2
-
-# Pinterest Image Downloader CLI (pinterest-dl)
-[![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)](https://pypi.org/project/pinterest-dl/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pinterest-dl)](https://pypi.org/project/pinterest-dl/)
-[![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)](https://github.com/sean1832/pinterest-dl/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/badge/pinterest-dl)](https://pepy.tech/project/pinterest-dl)
+
+# Pinterest Image Scraper CLI
+![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)
+![Static Badge](https://img.shields.io/badge/python-3.10%2B-yellow)
+![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)
+
 
 
 This CLI (Command Line Interface) tool facilitates the scraping and downloading of images from [Pinterest](https://pinterest.com). Using [Selenium](https://selenium.dev) for automation, it enables users to extract images from a specified Pinterest URL and save them to a chosen directory.
 
 > **⚠️ Disclaimer:**  
 > This project is independent and not affiliated with Pinterest. It's designed solely for educational purposes. Please be aware that automating the scraping of websites might conflict with their [Terms of Service](https://developers.pinterest.com/terms/). The repository owner disclaims any liability for misuse of this tool. Use it responsibly and at your own legal risk.
 
 > **🗒️ Note:**  
 > This project draws inspiration from [pinterest-image-scraper](https://github.com/xjdeng/pinterest-image-scraper).
 
 ## 🌟 Features
 - ✅ Scrape images directly from a Pinterest URL.
 - ✅ Asynchronously download images from a list of URLs. ([see pull request](https://github.com/sean1832/pinterest-dl/pull/1))
-- ✅ Save scraped URLs to a JSON file for future access.
-- ✅ Incognito mode to keep your scraping discreet.
+- ✅ Configure the output directory to your liking.
+- ✅ Save scraped URLs to a JSON file for easy access.
+- ✅ Utilize incognito mode to keep your scraping discreet.
 - ✅ Access detailed output for effective debugging.
-- ✅ Support for the Firefox browser.
-- ✅ Insert `alt` text for images as metadata `comment` in the downloaded image for searchability.
+- ✅ Perform dry-runs to receive URLs without downloading the images.
+- ✅ Full support for the Firefox browser.
+- ✅ Customize scroll threshold and page persistence for tailored scraping.
 
 ## 🚩 Known Issues
 - 🔲 Experimental Firefox browser support might not perform as expected.
 - 🔲 Limited functionality with Pinterest URLs requiring login.
 - 🔲 Incompatibility with Pinterest URLs that include search queries.
 - 🔲 Currently does not support MacOS and Linux platforms.
 
@@ -72,62 +70,55 @@
 ## 🛠 Usage
 
 ### General Command Structure
 ```bash
 pinterest-dl [command] [options]
 ```
 
----
-### Examples
-
-**Scraping Images:**
-
-Scrape images to the `./images/art` directory from the Pinterest URL `https://www.pinterest.com/pin/1234567` with a limit of `30` images and a minimum resolution of `512x512`. Save scraped URLs to a `JSON` file.
-```bash
-pinterest-dl scrape "https://www.pinterest.com/pin/1234567" "images/art" -l 30 -r 512x512 --json
-```
-
-**Downloading Images:**
-
-Download images from the `art.json` file to the `./downloaded_imgs` directory with a minimum resolution of `1024x1024`.
-```bash
-pinterest-dl download art.json -o downloaded_imgs -r 1024x1024
-```
----
 ### Commands
 
 #### 1. Scrape
 Extract images from a specified Pinterest URL.
 
 **Syntax:**
 ```bash
-pinterest-dl scrape [url] [output_dir] [options]
+pinterest-dl scrape [url] [options]
 ```
 
 **Options:**
-- `-l`, `--limit [number]`: Max number of image to download (default: 100).
+- `-o`, `--output [directory]`: Set the directory to save images (default: `imgs`).
+- `-w`, `--write [file]`: Save scraped URLs to a JSON file.
+- `-t`, `--threshold [number]`: Set the number of page scrolls (default: 20).
+- `-p`, `--persistence [seconds]`: Wait time for page loading (default: 120 seconds).
 - `-r`, `--resolution [width]x[height]`: Minimum image resolution for download (e.g., 512x512).
-- `--timeout [second]`: Timeout in seconds for requests (default: 3).
 - `--incognito`: Activate incognito mode for scraping.
-- `--json`: Save scraped URLs to a JSON file.
 - `--dry-run`: Execute scrape without downloading images.
 - `--firefox`: Opt for Firefox as the scraping browser.
-- `--headful`: Run in headful mode with browser window.
 - `--verbose`: Enable detailed output for debugging.
 
 #### 2. Download
 Download images from a list of URLs provided in a file.
 
 **Syntax:**
 ```bash
 pinterest-dl download [url_list] [options]
 ```
 
 **Options:**
-- `-o`, `--output [directory]`: Output directory (default: ./<json_filename>).
+- `-o`, `--output [directory]`: Specify the output directory for the images (default: `imgs`).
 - `-r`, `--resolution [width]x[height]`: minimum resolution to download (e.g. 512x512).
 - `--verbose`: Enable verbose output.
 
+### Examples
+
+**Scraping Images:**
+```bash
+pinterest-dl scrape "https://www.pinterest.com/exampleBoard" -o myimages -t 30 --verbose
+```
 
+**Downloading Images:**
+```bash
+pinterest-dl download urls.json -o downloaded_imgs --verbose
+```
 
 ## 📜 License
 [Apache License 2.0](LICENSE)
```

### Comparing `pinterest-dl-0.0.21/README.md` & `pinterest-dl-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-# Pinterest Image Downloader CLI (pinterest-dl)
-[![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)](https://pypi.org/project/pinterest-dl/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pinterest-dl)](https://pypi.org/project/pinterest-dl/)
-[![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)](https://github.com/sean1832/pinterest-dl/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/badge/pinterest-dl)](https://pepy.tech/project/pinterest-dl)
+# Pinterest Image Scraper CLI
+![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)
+![Static Badge](https://img.shields.io/badge/python-3.10%2B-yellow)
+![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)
+
 
 
 This CLI (Command Line Interface) tool facilitates the scraping and downloading of images from [Pinterest](https://pinterest.com). Using [Selenium](https://selenium.dev) for automation, it enables users to extract images from a specified Pinterest URL and save them to a chosen directory.
 
 > **⚠️ Disclaimer:**  
 > This project is independent and not affiliated with Pinterest. It's designed solely for educational purposes. Please be aware that automating the scraping of websites might conflict with their [Terms of Service](https://developers.pinterest.com/terms/). The repository owner disclaims any liability for misuse of this tool. Use it responsibly and at your own legal risk.
 
 > **🗒️ Note:**  
 > This project draws inspiration from [pinterest-image-scraper](https://github.com/xjdeng/pinterest-image-scraper).
 
 ## 🌟 Features
 - ✅ Scrape images directly from a Pinterest URL.
 - ✅ Asynchronously download images from a list of URLs. ([see pull request](https://github.com/sean1832/pinterest-dl/pull/1))
-- ✅ Save scraped URLs to a JSON file for future access.
-- ✅ Incognito mode to keep your scraping discreet.
+- ✅ Configure the output directory to your liking.
+- ✅ Save scraped URLs to a JSON file for easy access.
+- ✅ Utilize incognito mode to keep your scraping discreet.
 - ✅ Access detailed output for effective debugging.
-- ✅ Support for the Firefox browser.
-- ✅ Insert `alt` text for images as metadata `comment` in the downloaded image for searchability.
+- ✅ Perform dry-runs to receive URLs without downloading the images.
+- ✅ Full support for the Firefox browser.
+- ✅ Customize scroll threshold and page persistence for tailored scraping.
 
 ## 🚩 Known Issues
 - 🔲 Experimental Firefox browser support might not perform as expected.
 - 🔲 Limited functionality with Pinterest URLs requiring login.
 - 🔲 Incompatibility with Pinterest URLs that include search queries.
 - 🔲 Currently does not support MacOS and Linux platforms.
 
@@ -49,62 +51,55 @@
 ## 🛠 Usage
 
 ### General Command Structure
 ```bash
 pinterest-dl [command] [options]
 ```
 
----
-### Examples
-
-**Scraping Images:**
-
-Scrape images to the `./images/art` directory from the Pinterest URL `https://www.pinterest.com/pin/1234567` with a limit of `30` images and a minimum resolution of `512x512`. Save scraped URLs to a `JSON` file.
-```bash
-pinterest-dl scrape "https://www.pinterest.com/pin/1234567" "images/art" -l 30 -r 512x512 --json
-```
-
-**Downloading Images:**
-
-Download images from the `art.json` file to the `./downloaded_imgs` directory with a minimum resolution of `1024x1024`.
-```bash
-pinterest-dl download art.json -o downloaded_imgs -r 1024x1024
-```
----
 ### Commands
 
 #### 1. Scrape
 Extract images from a specified Pinterest URL.
 
 **Syntax:**
 ```bash
-pinterest-dl scrape [url] [output_dir] [options]
+pinterest-dl scrape [url] [options]
 ```
 
 **Options:**
-- `-l`, `--limit [number]`: Max number of image to download (default: 100).
+- `-o`, `--output [directory]`: Set the directory to save images (default: `imgs`).
+- `-w`, `--write [file]`: Save scraped URLs to a JSON file.
+- `-t`, `--threshold [number]`: Set the number of page scrolls (default: 20).
+- `-p`, `--persistence [seconds]`: Wait time for page loading (default: 120 seconds).
 - `-r`, `--resolution [width]x[height]`: Minimum image resolution for download (e.g., 512x512).
-- `--timeout [second]`: Timeout in seconds for requests (default: 3).
 - `--incognito`: Activate incognito mode for scraping.
-- `--json`: Save scraped URLs to a JSON file.
 - `--dry-run`: Execute scrape without downloading images.
 - `--firefox`: Opt for Firefox as the scraping browser.
-- `--headful`: Run in headful mode with browser window.
 - `--verbose`: Enable detailed output for debugging.
 
 #### 2. Download
 Download images from a list of URLs provided in a file.
 
 **Syntax:**
 ```bash
 pinterest-dl download [url_list] [options]
 ```
 
 **Options:**
-- `-o`, `--output [directory]`: Output directory (default: ./<json_filename>).
+- `-o`, `--output [directory]`: Specify the output directory for the images (default: `imgs`).
 - `-r`, `--resolution [width]x[height]`: minimum resolution to download (e.g. 512x512).
 - `--verbose`: Enable verbose output.
 
+### Examples
+
+**Scraping Images:**
+```bash
+pinterest-dl scrape "https://www.pinterest.com/exampleBoard" -o myimages -t 30 --verbose
+```
 
+**Downloading Images:**
+```bash
+pinterest-dl download urls.json -o downloaded_imgs --verbose
+```
 
 ## 📜 License
 [Apache License 2.0](LICENSE)
```

### Comparing `pinterest-dl-0.0.21/pinterest_dl/cli_parser.py` & `pinterest-dl-0.0.9/pinterest_dl/cli_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,27 +10,26 @@
     parser.add_argument("-v", "--version", action="version", version="v"+meta["version"])
 
     cmd = parser.add_subparsers(dest="cmd", help="Command to run")
 
     # scrape command
     scrape_cmd = cmd.add_parser("scrape", help="Scrape images from Pinterest")
     scrape_cmd.add_argument("url", help="URL to scrape images from")
-    scrape_cmd.add_argument("output", help="Output directory")
-    scrape_cmd.add_argument("-l", "--limit", type=int, default=100, help="Max number of image to scrape (default: 100)")
-    scrape_cmd.add_argument("-r", "--resolution", type=str, help="Minimum resolution to keep (e.g. 512x512).")
-    scrape_cmd.add_argument("--timeout", type=int, default=3, help="Timeout in seconds for requests (default: 3)")
+    scrape_cmd.add_argument("-o", "--output", default="imgs", help="Output directory (default: imgs)")
+    scrape_cmd.add_argument("-w", "--write", help="Write urls to json file")
+    scrape_cmd.add_argument("-t", "--threshold", type=int, default=20, help="Number of scroll to perform (default: 20)")
+    scrape_cmd.add_argument("-p", "--persistence", type=int, default=120, help="Time to wait for page to load (default: 120)")
+    scrape_cmd.add_argument("-r", "--resolution", type=str, help="minimum resolution to keep (e.g. 512x512).")
     scrape_cmd.add_argument("--incognito", action="store_true", help="Incognito mode")
-    scrape_cmd.add_argument("--json", action="store_true", help="Write urls to json file")
     scrape_cmd.add_argument("--dry-run", action="store_true", help="Run without download")
     scrape_cmd.add_argument("--firefox", action="store_true", help="Use Firefox browser")
-    scrape_cmd.add_argument("--headful", action="store_true", help="Run in headful mode with browser window")
     scrape_cmd.add_argument("--verbose", action="store_true", help="Print verbose output")
 
     # download command
     download_cmd = cmd.add_parser("download", help="Download images")
-    download_cmd.add_argument("input", help="Input json file containing image urls")
-    download_cmd.add_argument("-o", "--output", help="Output directory (default: ./<json_filename>)")
+    download_cmd.add_argument("url_list", help="Input file containing image urls")
+    download_cmd.add_argument("-o", "--output", default="imgs", help="Output directory (default: imgs)")
     download_cmd.add_argument("-r", "--resolution", type=str, help="minimum resolution to keep (e.g. 512x512).")
     download_cmd.add_argument("--verbose", action="store_true", help="Print verbose output")
 
     return parser
 # fmt: on
```

### Comparing `pinterest-dl-0.0.21/pinterest_dl/driver_installer.py` & `pinterest-dl-0.0.9/pinterest_dl/driver_installer.py`

 * *Files identical despite different names*

### Comparing `pinterest-dl-0.0.21/pinterest_dl/io.py` & `pinterest-dl-0.0.9/pinterest_dl/io.py`

 * *Files identical despite different names*

### Comparing `pinterest-dl-0.0.21/pinterest_dl/main.py` & `pinterest-dl-0.0.9/pinterest_dl/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,87 @@
-from pathlib import Path
+from pinterest_dl import cli_parser, downloader, io, scraper, utils
 
-from pinterest_dl import api, cli_parser, io, utils
+
+def run_download(img_urls, output, verbose):
+    fallback_urls = [i.replace("/originals/", "/736x/") for i in img_urls]
+    return downloader.download_concurrent_with_fallback(
+        img_urls, output, fallback_urls, verbose=verbose
+    )
+
+
+def run_prune(local_images, min_resolution):
+    if min_resolution:
+        for i in local_images:
+            utils.prune_by_resolution(i, min_resolution)
+
+
+def run_scrape(
+    url,
+    threshold,
+    firefox,
+    output,
+    write,
+    persistence,
+    incognito,
+    dry_run,
+    verbose,
+    min_resolution,
+):
+    browser = scraper.Browser().Chrome(
+        exe_path=utils.get_root().joinpath("bin", "chromedriver.exe"),
+        incognito=incognito,
+    )
+    if firefox:
+        browser = scraper.Browser().Firefox()
+    try:
+        pin_scraper = scraper.Pinterest(browser)
+        img_urls = pin_scraper.scrape(
+            url,
+            threshold=threshold,
+            presistence=persistence,
+            verbose=verbose,
+        )
+    finally:
+        browser.close()
+
+    print(f"Found {len(img_urls)} urls")
+    if write:
+        io.write_json(img_urls, write, indent=4)
+    if not dry_run:
+        downloaded_files = run_download(img_urls, output, verbose)
+
+        # post download
+        run_prune(downloaded_files, min_resolution)
+    else:
+        for i in img_urls:
+            print(i)
 
 
 def main():
     parser = cli_parser.get_parser()
     args = parser.parse_args()
 
     if args.cmd == "scrape":
-        api.run_scrape(
+        run_scrape(
             args.url,
-            args.limit,
+            args.threshold,
+            args.firefox,
             args.output,
-            timeout=args.timeout,
-            json=args.json,
-            firefox=args.firefox,
-            incognito=args.incognito,
-            headful=args.headful,
-            dry_run=args.dry_run,
-            verbose=args.verbose,
-            min_resolution=utils.parse_resolution(args.resolution) if args.resolution else None,
+            args.write,
+            args.persistence,
+            args.incognito,
+            args.dry_run,
+            args.verbose,
+            args.resolution,
         )
         print("\nDone.")
     elif args.cmd == "download":
-        # prepare image url data
-        img_datas = io.read_json(args.input)
-        srcs, alts, fallbacks, origins = [], [], [], []
-        for img_data in img_datas:
-            srcs.append(img_data["src"])
-            alts.append(img_data["alt"])
-            fallbacks.append(img_data["fallback"])
-            origins.append(img_data["origin"])
-
-        output_dir = args.output or str(Path(args.input).stem)
-
-        # download images
-        downloaded_files = api.run_download(srcs, fallbacks, output_dir, args.verbose)
-
-        # post process
-        pruned_idx = api.run_prune(downloaded_files, args.resolution)
-        api.run_caption(downloaded_files, alts, origins, pruned_idx, verbose=args.verbose)
+        img_list = io.read_json(args.url_list)
+        downloaded_files = run_download(img_list, args.output, args.verbose)
+        run_prune(downloaded_files, args.resolution)
         print("\nDone.")
     else:
         parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pinterest-dl-0.0.21/pinterest_dl/scraper.py` & `pinterest-dl-0.0.9/pinterest_dl/scraper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 import copy
 import os
 import random
 import socket
 import time
+from pathlib import Path
 
 from selenium import webdriver
 from selenium.common.exceptions import StaleElementReferenceException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
-from tqdm import tqdm
 
-from pinterest_dl import driver_installer, utils
+from pinterest_dl import downloader, driver_installer, utils
 
 
 def randdelay(a, b):
     time.sleep(random.uniform(a, b))
 
 
 class Browser(object):
     def __init__(self):
         self.browser = None
 
-    def Chrome(
-        self, image_enable=False, incognito=False, exe_path="chromedriver.exe", headful=False
-    ):
+    def Chrome(self, image_enable=False, incognito=False, exe_path="chromedriver.exe"):
         if not os.path.exists(exe_path):
             driver_installer.install_chrome_driver(
-                utils.get_appdata_dir(), version="123.0.6312.86", platform="win64"
+                Path(exe_path).parent, version="123.0.6312.86", platform="win64"
             )
 
         service = webdriver.chrome.service.Service(exe_path)
         chrome_options = webdriver.ChromeOptions()
         # Disable images
         # https://scrapeops.io/selenium-web-scraping-playbook/python-selenium-disable-image-loading/
         chrome_options.add_argument(
             "--blink-settings=imagesEnabled=true"
             if image_enable
             else "--blink-settings=imagesEnabled=false"
         )
-        chrome_options.add_argument("--log-level=3")  # Suppress most logs
         if incognito:
-            print("Running in incognito mode")
             chrome_options.add_argument("--incognito")
-        if not headful:
-            print("Running in headless mode")
-            chrome_options.add_argument("--headless=new")
         browser = webdriver.Chrome(options=chrome_options, service=service)
         return browser
 
-    def Firefox(self, image_enable=False, incognito=False, headful=False):
-        firefox_options = webdriver.FirefoxOptions()
+    def Firefox(self, image_enable=False, incognito=False):
+        firefox_profile = webdriver.FirefoxProfile()
         # Disable images
         if image_enable:
-            firefox_options.set_preference("permissions.default.image", 1)
+            firefox_profile.set_preference("permissions.default.image", 1)
         else:
-            firefox_options.set_preference("permissions.default.image", 2)
+            firefox_profile.set_preference("permissions.default.image", 2)
         if incognito:
-            firefox_options.set_preference("browser.privatebrowsing.autostart", True)
-        if not headful:
-            print("Running in headless mode")
-            firefox_options.add_argument("--headless")
-        browser = webdriver.Firefox(options=firefox_options)
+            firefox_profile.set_preference("browser.privatebrowsing.autostart", True)
+        browser = webdriver.Firefox(firefox_profile=firefox_profile)
         return browser
 
+    def _download_chrome_driver_not_exist(self, exe_path):
+        if not utils.file_exists(exe_path):
+            print("Chrome driver does not exist. Downloading...")
+
+            downloader.download_curl()
+        else:
+            print("Chrome driver exists.")
+
 
 class Pinterest(object):
     def __init__(self, browser=None):
         self.browser: WebDriver = browser
 
     # currently not used
     def login(self, email, password):
@@ -79,81 +77,65 @@
         password_field.send_keys(password)
         randdelay(1, 2)  # delay between 1 and 2 seconds
         password_field.send_keys(Keys.RETURN)
 
     def scrape(
         self,
         url,
-        limit=20,
-        timeout=3,
+        threshold=20,
+        presistence=120,
         verbose=False,
     ):
-        unique_results = set()  # Use a set to store unique results
-        imgs_data = []  # Store image data
+        final_results = []
         previous_divs = []
         tries = 0
-        pbar = tqdm(total=limit, desc="Scraping")
+
         try:
             self.browser.get(url)
-            while len(unique_results) < limit:
+            while threshold > 0:
                 try:
                     divs = self.browser.find_elements(By.CSS_SELECTOR, "div[data-test-id='pin']")
                     if divs == previous_divs:
                         tries += 1
-                        time.sleep(1)  # delay 1 second
                     else:
                         tries = 0
-                    if tries > timeout:
-                        print(f"\nTimeout: no new images in ({timeout}) seconds.")
-                        break
+                    if tries > presistence:
+                        if verbose:
+                            print("Exiting: persistence exceeded")
+                        return final_results
 
                     for div in divs:
-                        if self._is_div_ad(div) or len(unique_results) >= limit:
+                        # if div is an ad, skip
+                        if self._is_div_ad(div):
                             continue
                         images = div.find_elements(By.TAG_NAME, "img")
-                        href = div.find_element(By.TAG_NAME, "a").get_attribute("href")
                         for image in images:
-                            alt = image.get_attribute("alt")
                             src = image.get_attribute("src")
                             if src and "/236x/" in src:
                                 src = src.replace("/236x/", "/originals/")
-                                src_736 = src.replace("/originals/", "/736x/")
-                                if src not in unique_results:
-                                    unique_results.add(src)
-                                    img_data = {
-                                        "src": src,
-                                        "alt": alt,
-                                        "fallback": src_736,
-                                        "origin": href,
-                                    }
-                                    imgs_data.append(img_data)
-                                    pbar.update(1)
-                                    if verbose:
-                                        print(src, alt)
-                                    if len(unique_results) >= limit:
-                                        break
-
+                                final_results.append(src)
+                                if verbose:
+                                    print(src)
                     previous_divs = copy.copy(divs)  # copy to avoid reference
+                    final_results = list(set(final_results))  # remove duplicates
 
                     # Scroll down
                     dummy = self.browser.find_element(By.TAG_NAME, "a")
                     dummy.send_keys(Keys.PAGE_DOWN)
                     randdelay(1, 2)  # delay between 1 and 2 seconds
+                    threshold -= 1
 
                 except StaleElementReferenceException:
-                    if verbose:
-                        print("\nStaleElementReferenceException")
-
+                    print("StaleElementReferenceException")
+                    threshold -= 1
         except (socket.error, socket.timeout):
             print("Socket Error")
-        finally:
-            pbar.close()
-            if verbose:
-                print(f"Scraped {len(imgs_data)} images")
-            return imgs_data
+        except KeyboardInterrupt:
+            return final_results
+        return final_results
 
     def _is_div_ad(self, div: WebElement):
         """Check if div is an ad.
 
         Args:
             div (webElement): div element.
         """
```

### Comparing `pinterest-dl-0.0.21/pinterest_dl.egg-info/PKG-INFO` & `pinterest-dl-0.0.9/pinterest_dl.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinterest-dl
-Version: 0.0.21
+Version: 0.0.9
 Summary: An unofficial Pinterest image downloader
 Home-page: https://github.com/sean1832/pinterest-dl
 Author: Zeke Zhang
 License: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,42 +12,40 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Console
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: selenium>=4.9.0
-Requires-Dist: pillow>=10.1.0
-Requires-Dist: tqdm
-Requires-Dist: pyexiv2
-
-# Pinterest Image Downloader CLI (pinterest-dl)
-[![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)](https://pypi.org/project/pinterest-dl/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pinterest-dl)](https://pypi.org/project/pinterest-dl/)
-[![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)](https://github.com/sean1832/pinterest-dl/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/badge/pinterest-dl)](https://pepy.tech/project/pinterest-dl)
+
+# Pinterest Image Scraper CLI
+![PyPI - Version](https://img.shields.io/pypi/v/pinterest-dl)
+![Static Badge](https://img.shields.io/badge/python-3.10%2B-yellow)
+![PyPI - License](https://img.shields.io/pypi/l/pinterest-dl)
+
 
 
 This CLI (Command Line Interface) tool facilitates the scraping and downloading of images from [Pinterest](https://pinterest.com). Using [Selenium](https://selenium.dev) for automation, it enables users to extract images from a specified Pinterest URL and save them to a chosen directory.
 
 > **⚠️ Disclaimer:**  
 > This project is independent and not affiliated with Pinterest. It's designed solely for educational purposes. Please be aware that automating the scraping of websites might conflict with their [Terms of Service](https://developers.pinterest.com/terms/). The repository owner disclaims any liability for misuse of this tool. Use it responsibly and at your own legal risk.
 
 > **🗒️ Note:**  
 > This project draws inspiration from [pinterest-image-scraper](https://github.com/xjdeng/pinterest-image-scraper).
 
 ## 🌟 Features
 - ✅ Scrape images directly from a Pinterest URL.
 - ✅ Asynchronously download images from a list of URLs. ([see pull request](https://github.com/sean1832/pinterest-dl/pull/1))
-- ✅ Save scraped URLs to a JSON file for future access.
-- ✅ Incognito mode to keep your scraping discreet.
+- ✅ Configure the output directory to your liking.
+- ✅ Save scraped URLs to a JSON file for easy access.
+- ✅ Utilize incognito mode to keep your scraping discreet.
 - ✅ Access detailed output for effective debugging.
-- ✅ Support for the Firefox browser.
-- ✅ Insert `alt` text for images as metadata `comment` in the downloaded image for searchability.
+- ✅ Perform dry-runs to receive URLs without downloading the images.
+- ✅ Full support for the Firefox browser.
+- ✅ Customize scroll threshold and page persistence for tailored scraping.
 
 ## 🚩 Known Issues
 - 🔲 Experimental Firefox browser support might not perform as expected.
 - 🔲 Limited functionality with Pinterest URLs requiring login.
 - 🔲 Incompatibility with Pinterest URLs that include search queries.
 - 🔲 Currently does not support MacOS and Linux platforms.
 
@@ -72,62 +70,55 @@
 ## 🛠 Usage
 
 ### General Command Structure
 ```bash
 pinterest-dl [command] [options]
 ```
 
----
-### Examples
-
-**Scraping Images:**
-
-Scrape images to the `./images/art` directory from the Pinterest URL `https://www.pinterest.com/pin/1234567` with a limit of `30` images and a minimum resolution of `512x512`. Save scraped URLs to a `JSON` file.
-```bash
-pinterest-dl scrape "https://www.pinterest.com/pin/1234567" "images/art" -l 30 -r 512x512 --json
-```
-
-**Downloading Images:**
-
-Download images from the `art.json` file to the `./downloaded_imgs` directory with a minimum resolution of `1024x1024`.
-```bash
-pinterest-dl download art.json -o downloaded_imgs -r 1024x1024
-```
----
 ### Commands
 
 #### 1. Scrape
 Extract images from a specified Pinterest URL.
 
 **Syntax:**
 ```bash
-pinterest-dl scrape [url] [output_dir] [options]
+pinterest-dl scrape [url] [options]
 ```
 
 **Options:**
-- `-l`, `--limit [number]`: Max number of image to download (default: 100).
+- `-o`, `--output [directory]`: Set the directory to save images (default: `imgs`).
+- `-w`, `--write [file]`: Save scraped URLs to a JSON file.
+- `-t`, `--threshold [number]`: Set the number of page scrolls (default: 20).
+- `-p`, `--persistence [seconds]`: Wait time for page loading (default: 120 seconds).
 - `-r`, `--resolution [width]x[height]`: Minimum image resolution for download (e.g., 512x512).
-- `--timeout [second]`: Timeout in seconds for requests (default: 3).
 - `--incognito`: Activate incognito mode for scraping.
-- `--json`: Save scraped URLs to a JSON file.
 - `--dry-run`: Execute scrape without downloading images.
 - `--firefox`: Opt for Firefox as the scraping browser.
-- `--headful`: Run in headful mode with browser window.
 - `--verbose`: Enable detailed output for debugging.
 
 #### 2. Download
 Download images from a list of URLs provided in a file.
 
 **Syntax:**
 ```bash
 pinterest-dl download [url_list] [options]
 ```
 
 **Options:**
-- `-o`, `--output [directory]`: Output directory (default: ./<json_filename>).
+- `-o`, `--output [directory]`: Specify the output directory for the images (default: `imgs`).
 - `-r`, `--resolution [width]x[height]`: minimum resolution to download (e.g. 512x512).
 - `--verbose`: Enable verbose output.
 
+### Examples
+
+**Scraping Images:**
+```bash
+pinterest-dl scrape "https://www.pinterest.com/exampleBoard" -o myimages -t 30 --verbose
+```
 
+**Downloading Images:**
+```bash
+pinterest-dl download urls.json -o downloaded_imgs --verbose
+```
 
 ## 📜 License
 [Apache License 2.0](LICENSE)
```

### Comparing `pinterest-dl-0.0.21/setup.py` & `pinterest-dl-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     packages=find_packages(),
     include_package_data=True,
     package_data={
         "": [
             "manifest.json",
         ]
     },
-    install_requires=["selenium>=4.9.0", "pillow>=10.1.0", "tqdm", "pyexiv2"],
+    install_requires=["selenium>=4.9.0", "pillow>=10.1.0"],
     entry_points={
         "console_scripts": [
             "pinterest-dl = pinterest_dl.main:main",
         ],
     },
     python_rquires=">=3.10",
     # https://pypi.org/classifiers/
```

