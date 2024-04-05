# Comparing `tmp/deezer_oauth_cli-1.2.4.tar.gz` & `tmp/deezer_oauth_cli-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_oauth_cli-1.2.4.tar", max compression
+gzip compressed data, was "deezer_oauth_cli-1.2.5.tar", max compression
```

## Comparing `deezer_oauth_cli-1.2.4.tar` & `deezer_oauth_cli-1.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2024-03-29 03:12:57.922160 deezer_oauth_cli-1.2.4/LICENSE
--rw-r--r--   0        0        0     5506 2024-03-29 03:12:57.922160 deezer_oauth_cli-1.2.4/README.md
--rw-r--r--   0        0        0     3412 2024-03-29 03:13:00.450164 deezer_oauth_cli-1.2.4/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-29 03:13:00.450164 deezer_oauth_cli-1.2.4/src/deezer_oauth/__init__.py
--rw-r--r--   0        0        0       53 2024-03-29 03:12:57.926160 deezer_oauth_cli-1.2.4/src/deezer_oauth/__main__.py
--rw-r--r--   0        0        0     1833 2024-03-29 03:12:57.926160 deezer_oauth_cli-1.2.4/src/deezer_oauth/client.py
--rw-r--r--   0        0        0      115 2024-03-29 03:12:57.926160 deezer_oauth_cli-1.2.4/src/deezer_oauth/constants.py
--rw-r--r--   0        0        0     1003 2024-03-29 03:12:57.926160 deezer_oauth_cli-1.2.4/src/deezer_oauth/files.py
--rw-r--r--   0        0        0     1044 2024-03-29 03:12:57.926160 deezer_oauth_cli-1.2.4/src/deezer_oauth/main.py
--rw-r--r--   0        0        0        0 2024-03-29 03:12:57.926160 deezer_oauth_cli-1.2.4/src/deezer_oauth/py.typed
--rw-r--r--   0        0        0     3238 2024-03-29 03:12:57.926160 deezer_oauth_cli-1.2.4/src/deezer_oauth/server.py
--rw-r--r--   0        0        0     6989 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/LICENSE
+-rw-r--r--   0        0        0     5506 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/README.md
+-rw-r--r--   0        0        0     3412 2024-04-05 08:06:38.946786 deezer_oauth_cli-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-05 08:06:38.946786 deezer_oauth_cli-1.2.5/src/deezer_oauth/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/src/deezer_oauth/__main__.py
+-rw-r--r--   0        0        0     1833 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/src/deezer_oauth/client.py
+-rw-r--r--   0        0        0      115 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/src/deezer_oauth/constants.py
+-rw-r--r--   0        0        0     1003 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/src/deezer_oauth/files.py
+-rw-r--r--   0        0        0     1044 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/src/deezer_oauth/main.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/src/deezer_oauth/py.typed
+-rw-r--r--   0        0        0     3238 2024-04-05 08:06:36.270773 deezer_oauth_cli-1.2.5/src/deezer_oauth/server.py
+-rw-r--r--   0        0        0     6989 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.2.5/PKG-INFO
```

### Comparing `deezer_oauth_cli-1.2.4/LICENSE` & `deezer_oauth_cli-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.4/README.md` & `deezer_oauth_cli-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.4/pyproject.toml` & `deezer_oauth_cli-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-oauth-cli"
-version = "1.2.4"
+version = "1.2.5"
 description = "A small CLI to quickly obtain an API token for Deezer API."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/deezer-oauth-cli"
 documentation = "https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md"
 classifiers = [
@@ -28,15 +28,15 @@
 [tool.poetry.scripts]
 deezer-oauth = "deezer_oauth.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.27"
 rich = ">=10"
-typer = {extras = ["all"], version = "^0.11.0"}
+typer = {extras = ["all"], version = "^0.12.0"}
 
 [tool.poetry.group.dev.dependencies]
 pyfakefs = "^5.0"
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.6"
 responses = "^0.25.0"
```

### Comparing `deezer_oauth_cli-1.2.4/src/deezer_oauth/client.py` & `deezer_oauth_cli-1.2.5/src/deezer_oauth/client.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.4/src/deezer_oauth/files.py` & `deezer_oauth_cli-1.2.5/src/deezer_oauth/files.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.4/src/deezer_oauth/main.py` & `deezer_oauth_cli-1.2.5/src/deezer_oauth/main.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.4/src/deezer_oauth/server.py` & `deezer_oauth_cli-1.2.5/src/deezer_oauth/server.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.4/PKG-INFO` & `deezer_oauth_cli-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-oauth-cli
-Version: 1.2.4
+Version: 1.2.5
 Summary: A small CLI to quickly obtain an API token for Deezer API.
 Home-page: https://github.com/browniebroke/deezer-oauth-cli
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: requests (>=2.27,<3.0)
 Requires-Dist: rich (>=10)
-Requires-Dist: typer[all] (>=0.11.0,<0.12.0)
+Requires-Dist: typer[all] (>=0.12.0,<0.13.0)
 Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-oauth-cli/issues
 Project-URL: Changelog, https://github.com/browniebroke/deezer-oauth-cli/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md
 Project-URL: Mastodon, https://fosstodon.org/@browniebroke
 Project-URL: Repository, https://github.com/browniebroke/deezer-oauth-cli
 Project-URL: Twitter, https://twitter.com/_BrunoAlla
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.2.4 Summary: A small
+Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.2.5 Summary: A small
 CLI to quickly obtain an API token for Deezer API. Home-page: https://
 github.com/browniebroke/deezer-oauth-cli License: MIT Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Requires-Dist: requests
 (>=2.27,<3.0) Requires-Dist: rich (>=10) Requires-Dist: typer[all]
-(>=0.11.0,<0.12.0) Project-URL: Bug Tracker, https://github.com/browniebroke/
+(>=0.12.0,<0.13.0) Project-URL: Bug Tracker, https://github.com/browniebroke/
 deezer-oauth-cli/issues Project-URL: Changelog, https://github.com/
 browniebroke/deezer-oauth-cli/blob/main/CHANGELOG.md Project-URL:
 Documentation, https://github.com/browniebroke/deezer-oauth-cli/blob/main/
 README.md Project-URL: Mastodon, https://fosstodon.org/@browniebroke Project-
 URL: Repository, https://github.com/browniebroke/deezer-oauth-cli Project-URL:
 Twitter, https://twitter.com/_BrunoAlla Description-Content-Type: text/markdown
 # Deezer OAuth CLI
```

