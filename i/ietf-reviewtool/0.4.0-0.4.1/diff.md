# Comparing `tmp/ietf_reviewtool-0.4.0.tar.gz` & `tmp/ietf_reviewtool-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ietf_reviewtool-0.4.0.tar", max compression
+gzip compressed data, was "ietf_reviewtool-0.4.1.tar", max compression
```

## Comparing `ietf_reviewtool-0.4.0.tar` & `ietf_reviewtool-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    18092 2024-04-04 14:25:57.261864 ietf_reviewtool-0.4.0/LICENSE
--rw-r--r--   0        0        0     6700 2024-04-04 14:25:57.261864 ietf_reviewtool-0.4.0/README.md
--rw-r--r--   0        0        0      285 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/__init__.py
--rw-r--r--   0        0        0      146 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/__main__.py
--rw-r--r--   0        0        0     1183 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/agenda.py
--rw-r--r--   0        0        0    14293 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/boilerplate.py
--rw-r--r--   0        0        0     5478 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/doc.py
--rw-r--r--   0        0        0     4313 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/grammar.py
--rwxr-xr-x   0        0        0    30210 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/ietf_reviewtool.py
--rw-r--r--   0        0        0     2527 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/inclusive.py
--rw-r--r--   0        0        0     4829 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/metadata.py
--rw-r--r--   0        0        0    10968 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/references.py
--rw-r--r--   0        0        0    10872 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/review.py
--rw-r--r--   0        0        0        0 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/__init__.py
--rw-r--r--   0        0        0     2970 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/docposition.py
--rw-r--r--   0        0        0    11251 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/fetch.py
--rw-r--r--   0        0        0     2936 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/format.py
--rw-r--r--   0        0        0    11478 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/text.py
--rw-r--r--   0        0        0     2319 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/ietf_reviewtool/util/utils.py
--rw-r--r--   0        0        0     1400 2024-04-04 14:25:57.265864 ietf_reviewtool-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7794 1970-01-01 00:00:00.000000 ietf_reviewtool-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5287 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/README.md
+-rw-r--r--   0        0        0      285 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/__main__.py
+-rw-r--r--   0        0        0     1183 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/agenda.py
+-rw-r--r--   0        0        0    14293 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/boilerplate.py
+-rw-r--r--   0        0        0     5478 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/doc.py
+-rw-r--r--   0        0        0     4313 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/grammar.py
+-rwxr-xr-x   0        0        0    30210 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/ietf_reviewtool.py
+-rw-r--r--   0        0        0     2527 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/inclusive.py
+-rw-r--r--   0        0        0     4829 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/metadata.py
+-rw-r--r--   0        0        0    10968 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/references.py
+-rw-r--r--   0        0        0    10872 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/review.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/util/__init__.py
+-rw-r--r--   0        0        0     2970 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/util/docposition.py
+-rw-r--r--   0        0        0    11251 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/util/fetch.py
+-rw-r--r--   0        0        0     2936 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/util/format.py
+-rw-r--r--   0        0        0    11478 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/util/text.py
+-rw-r--r--   0        0        0     2319 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/ietf_reviewtool/util/utils.py
+-rw-r--r--   0        0        0     1400 2024-04-05 05:10:07.980124 ietf_reviewtool-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 ietf_reviewtool-0.4.1/PKG-INFO
```

### Comparing `ietf_reviewtool-0.4.0/LICENSE` & `ietf_reviewtool-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/README.md` & `ietf_reviewtool-0.4.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: ietf-reviewtool
+Version: 0.4.1
+Summary: Review tool for IETF documents
+Home-page: https://github.com/larseggert/ietf-reviewtool
+License: GPL-2.0-only
+Author: Lars Eggert
+Author-email: lars@eggert.org
+Requires-Python: >=3.11,<4
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyYAML (>=5.4.1)
+Requires-Dist: appdirs (>=1.4.4)
+Requires-Dist: charset-normalizer (>=2.0.6)
+Requires-Dist: click (>=7.1.2)
+Requires-Dist: json-five (>=0.8.0)
+Requires-Dist: language-tool-python (>=2.5.3)
+Requires-Dist: num2words (>=0.5.10)
+Requires-Dist: requests (>=2.28.2)
+Requires-Dist: requests-cache (>=1.0.0)
+Requires-Dist: setuptools (>=69.0.2,<70.0.0)
+Requires-Dist: urlextract (>=1.5.0)
+Requires-Dist: urllib3 (>=1.26.15)
+Project-URL: Repository, https://github.com/larseggert/ietf-reviewtool
+Description-Content-Type: text/markdown
+
 # ietf-reviewtool
 
 This is a simple Python 3 tool to download and review IETF documents, such as
 Internet-Drafts or RFCs, and comes packaged as a single `ietf-reviewtool`
 script.
 
 ## About
@@ -154,51 +182,14 @@
 Section 2, paragraph 7, nit:
 -    (5)  It is always possible to aglutenate multiple separate problems
 -                                       ^
 +    (5)  It is always possible to agglutinate multiple separate problems
 +                                    +   ^
 ```
 
-### Using caches
-
-In order to speed up the process, and to operate while being offline, you can
-set various environment variables to point the tool at directories in which you
-[cache various IETF document via
-`rsync`](https://www.ietf.org/standards/ids/internet-draft-mirror-sites/).
-
-These environment variables are named:
-
-* `IETF_CHARTERS`
-* `IETF_CONFLICT_REVIEWS`
-* `IETF_IDS`
-* `IETF_RFCS`
-* `IETF_STATUS_CHANGES`
-
-When the tool finds a given item to review in the cache, it will refrain from
-downloading it from the web.
-
-Note that the tool will **not** place items into the cache directories when they are not present; you **will** need to update the cache via `rsync`.
-
 ## Acknowledgments
 
 The ideas for some of these tools came from some of Henrik Levkowetz's earlier
 `bash` scripts. In the case of the `strip` tool, most of the original regular
 expressions were taken from his
 [`rfcstrip`](https://tools.ietf.org/tools/rfcstrip/about) `awk` script.
 
-
-## License
-
-Copyright (C) 2021-2022  Lars Eggert
-
-This program is free software; you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation; either version 2 of the License, or (at your option) any later
-version.
-
-This program is distributed in the hope that it will be useful, but WITHOUT ANY
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with
-this program; if not, write to the Free Software Foundation, Inc., 51 Franklin
-Street, Fifth Floor, Boston, MA  02110-1301, USA.
```

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/agenda.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/agenda.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/boilerplate.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/boilerplate.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/doc.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/doc.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/grammar.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/grammar.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/ietf_reviewtool.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/ietf_reviewtool.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/inclusive.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/inclusive.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/metadata.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/metadata.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/references.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/references.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/review.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/review.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/util/docposition.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/util/docposition.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/util/fetch.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/util/fetch.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/util/format.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/util/format.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/util/text.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/util/text.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/ietf_reviewtool/util/utils.py` & `ietf_reviewtool-0.4.1/ietf_reviewtool/util/utils.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.4.0/pyproject.toml` & `ietf_reviewtool-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "ietf-reviewtool"
-version = "0.4.0"
+version = "0.4.1"
 description = "Review tool for IETF documents"
 authors = ["Lars Eggert <lars@eggert.org>"]
 readme = "README.md"
 homepage = "https://github.com/larseggert/ietf-reviewtool"
 repository = "https://github.com/larseggert/ietf-reviewtool"
 license = "GPL-2.0-only"
 
 [tool.poetry.dependencies]
-python = ">=3.10, <4"
+python = ">=3.11, <4"
 requests-cache = ">=1.0.0"
 appdirs = ">=1.4.4"
 click = ">=7.1.2"
 language-tool-python = ">=2.5.3"
 PyYAML = ">=5.4.1"
 charset-normalizer = ">=2.0.6"
 urlextract = ">=1.5.0"
```

