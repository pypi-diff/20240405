# Comparing `tmp/py404-0.1.2.tar.gz` & `tmp/py404-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py404-0.1.2.tar", max compression
+gzip compressed data, was "py404-0.1.3.tar", max compression
```

## Comparing `py404-0.1.2.tar` & `py404-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      639 2024-02-16 10:54:59.007002 py404-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-02-16 10:55:25.576919 py404-0.1.2/py404/__init__.py
--rw-r--r--   0        0        0     5433 2024-03-07 00:31:44.846725 py404-0.1.2/py404/main.py
--rw-r--r--   0        0        0      559 2024-03-07 00:31:58.737683 py404-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 py404-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      639 2024-02-16 10:54:59.007002 py404-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-02-16 10:55:25.576919 py404-0.1.3/py404/__init__.py
+-rw-r--r--   0        0        0     5416 2024-04-04 20:08:23.154986 py404-0.1.3/py404/main.py
+-rw-r--r--   0        0        0      538 2024-04-04 20:08:06.218967 py404-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1490 1970-01-01 00:00:00.000000 py404-0.1.3/PKG-INFO
```

### Comparing `py404-0.1.2/README.md` & `py404-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py404-0.1.2/py404/main.py` & `py404-0.1.3/py404/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pythonads
 import typer
 from typing_extensions import Annotated
 import requests
 from bs4 import BeautifulSoup
 from urllib.parse import urljoin, urlparse
 from urllib3.exceptions import InsecureRequestWarning
 import asyncio
```

### Comparing `py404-0.1.2/pyproject.toml` & `py404-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "py404"
-version = "0.1.2"
+version = "0.1.3"
 description = "py404 is a CLI tool for finding deadlinks on a website."
 license = "MIT"
 authors = ["WillDenby <119456795+WillDenby@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/WillDenby/py404"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = "^0.9.0"
 beautifulsoup4 = "^4.12.3"
 requests = "^2.31.0"
 aiohttp = "^3.9.3"
-pythonads = "^0.1.0"
 
 [tool.poetry.scripts]
 py404 = "py404.main:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py404-0.1.2/PKG-INFO` & `py404-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: py404
-Version: 0.1.2
+Version: 0.1.3
 Summary: py404 is a CLI tool for finding deadlinks on a website.
 Home-page: https://github.com/WillDenby/py404
 License: MIT
 Author: WillDenby
 Author-email: 119456795+WillDenby@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
-Requires-Dist: pythonads (>=0.1.0,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/WillDenby/py404
 Description-Content-Type: text/markdown
 
 # py404
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: py404 Version: 0.1.2 Summary: py404 is a CLI tool
+Metadata-Version: 2.1 Name: py404 Version: 0.1.3 Summary: py404 is a CLI tool
 for finding deadlinks on a website. Home-page: https://github.com/WillDenby/
 py404 License: MIT Author: WillDenby Author-email:
 119456795+WillDenby@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: beautifulsoup4
-(>=4.12.3,<5.0.0) Requires-Dist: pythonads (>=0.1.0,<0.2.0) Requires-Dist:
-requests (>=2.31.0,<3.0.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Project-URL:
-Repository, https://github.com/WillDenby/py404 Description-Content-Type: text/
-markdown # py404 py404 is a CLI tool for finding deadlinks on a website. It
-checks for 404s on all kinds of links: hrefs, imgs, scripts in
+(>=4.12.3,<5.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
+typer (>=0.9.0,<0.10.0) Project-URL: Repository, https://github.com/WillDenby/
+py404 Description-Content-Type: text/markdown # py404 py404 is a CLI tool for
+finding deadlinks on a website. It checks for 404s on all kinds of links:
+hrefs, imgs, scripts in
 , etc. It was a fun way to learn some asyncio. ## Installation Use the package
 manager [pip](https://pip.pypa.io/en/stable/) to install py404. It requires
 Python >=3.9. ```shell $ pip install py404 ``` ## Usage Type `py404` followed
 by the URL you want to check. Deadlinks and their location are saved to a CSV
 file. ```shell $ py404 https://example.com ``` ## License Made by [Will](https:
 //github.com/WillDenby) and released under the [MIT](https://
 choosealicense.com/licenses/mit/) License
```

