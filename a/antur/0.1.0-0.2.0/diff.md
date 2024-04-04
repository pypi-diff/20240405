# Comparing `tmp/antur-0.1.0.tar.gz` & `tmp/antur-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antur-0.1.0.tar", max compression
+gzip compressed data, was "antur-0.2.0.tar", max compression
```

## Comparing `antur-0.1.0.tar` & `antur-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2024-04-04 21:46:42.745346 antur-0.1.0/LICENSE
--rw-r--r--   0        0        0      401 2024-04-04 22:04:53.222524 antur-0.1.0/README.md
--rw-r--r--   0        0        0      120 2024-04-04 22:53:45.511941 antur-0.1.0/antur/__init__.py
--rw-r--r--   0        0        0      206 2024-04-04 22:57:17.466205 antur-0.1.0/antur/__main__.py
--rw-r--r--   0        0        0      324 2024-04-04 22:09:16.513629 antur-0.1.0/antur/antur.tcss
--rw-r--r--   0        0        0     1608 2024-04-04 22:56:23.812636 antur-0.1.0/antur/app.py
--rw-r--r--   0        0        0     3575 2024-04-04 22:50:25.514397 antur-0.1.0/antur/utils/sitemap_parser.py
--rw-r--r--   0        0        0     1732 2024-04-04 22:08:36.106791 antur-0.1.0/antur/widgets/node_info.py
--rw-r--r--   0        0        0     2491 2024-04-04 22:09:20.130311 antur-0.1.0/antur/widgets/search_bar.py
--rw-r--r--   0        0        0     4288 2024-04-04 22:08:47.853508 antur-0.1.0/antur/widgets/sitemap_tree.py
--rw-r--r--   0        0        0     1454 2024-04-04 23:05:09.254944 antur-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 antur-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-04 21:46:42.745346 antur-0.2.0/LICENSE
+-rw-r--r--   0        0        0      580 2024-04-04 23:24:44.615411 antur-0.2.0/README.md
+-rw-r--r--   0        0        0      107 2024-04-04 23:42:06.212306 antur-0.2.0/antur/__init__.py
+-rw-r--r--   0        0        0      206 2024-04-04 22:57:17.466205 antur-0.2.0/antur/__main__.py
+-rw-r--r--   0        0        0      324 2024-04-04 22:09:16.513629 antur-0.2.0/antur/antur.tcss
+-rw-r--r--   0        0        0     1608 2024-04-04 22:56:23.812636 antur-0.2.0/antur/app.py
+-rw-r--r--   0        0        0     3575 2024-04-04 22:50:25.514397 antur-0.2.0/antur/utils/sitemap_parser.py
+-rw-r--r--   0        0        0     1732 2024-04-04 22:08:36.106791 antur-0.2.0/antur/widgets/node_info.py
+-rw-r--r--   0        0        0     2491 2024-04-04 22:09:20.130311 antur-0.2.0/antur/widgets/search_bar.py
+-rw-r--r--   0        0        0     4288 2024-04-04 22:08:47.853508 antur-0.2.0/antur/widgets/sitemap_tree.py
+-rw-r--r--   0        0        0     1454 2024-04-04 23:42:27.479233 antur-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1651 1970-01-01 00:00:00.000000 antur-0.2.0/PKG-INFO
```

### Comparing `antur-0.1.0/LICENSE` & `antur-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antur-0.1.0/antur/app.py` & `antur-0.2.0/antur/app.py`

 * *Files identical despite different names*

### Comparing `antur-0.1.0/antur/utils/sitemap_parser.py` & `antur-0.2.0/antur/utils/sitemap_parser.py`

 * *Files identical despite different names*

### Comparing `antur-0.1.0/antur/widgets/node_info.py` & `antur-0.2.0/antur/widgets/node_info.py`

 * *Files identical despite different names*

### Comparing `antur-0.1.0/antur/widgets/search_bar.py` & `antur-0.2.0/antur/widgets/search_bar.py`

 * *Files identical despite different names*

### Comparing `antur-0.1.0/antur/widgets/sitemap_tree.py` & `antur-0.2.0/antur/widgets/sitemap_tree.py`

 * *Files identical despite different names*

### Comparing `antur-0.1.0/pyproject.toml` & `antur-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antur"
-version = "0.1.0"
+version = "0.2.0"
 description = "Antur is a Python TUI tool for browsing and debugging sitemap data."
 license = "MIT"
 authors = ["Joe Banks <joe@jb3.dev>"]
 readme = "README.md"
 homepage = "https://github.com/jb3/antur"
 repository = "https://github.com/jb3/antur"
 keywords = ["sitemap", "xml", "tui", "cli", "debugging", "browser"]
@@ -16,15 +16,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Internet :: WWW/HTTP :: Site Management",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.12"
 textual = "^0.55.1"
 aiohttp = "^3.9.3"
 humanize = "^4.9.0"
 lxml = "^5.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `antur-0.1.0/PKG-INFO` & `antur-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: antur
-Version: 0.1.0
+Version: 0.2.0
 Summary: Antur is a Python TUI tool for browsing and debugging sitemap data.
 Home-page: https://github.com/jb3/antur
 License: MIT
 Keywords: sitemap,xml,tui,cli,debugging,browser
 Author: Joe Banks
 Author-email: joe@jb3.dev
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Utilities
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: humanize (>=4.9.0,<5.0.0)
 Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: textual (>=0.55.1,<0.56.0)
 Project-URL: Repository, https://github.com/jb3/antur
 Description-Content-Type: text/markdown
 
 # Antur
 
+![PyPI - Version](https://img.shields.io/pypi/v/antur?style=for-the-badge)
+![PyPI - License](https://img.shields.io/pypi/l/antur?style=for-the-badge)
+![GitHub Repo stars](https://img.shields.io/github/stars/jb3/antur?style=for-the-badge)
+
 Antur is a Python TUI tool for browsing and debugging sitemap data.
 
 > [!NOTE]
 > This project is under development and may error/have bugs.
 
 ## Demo
 
 ![Demo](./resources/demo.gif)
 
 ## Installation
 
 ```bash
-$ git clone git@github.com:jb3/antur.git
-$ cd antur
-$ poetry install
+$ pip install antur
 ```
 
 ## Usage
 
 ```bash
-$ poetry run antur
+$ antur
 ```
 
 ## License
 
 MIT License. See [LICENSE](LICENSE) for more information.
```

