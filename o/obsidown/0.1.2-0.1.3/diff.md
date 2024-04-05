# Comparing `tmp/obsidown-0.1.2.tar.gz` & `tmp/obsidown-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsidown-0.1.2.tar", max compression
+gzip compressed data, was "obsidown-0.1.3.tar", max compression
```

## Comparing `obsidown-0.1.2.tar` & `obsidown-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2024-03-10 14:25:15.990154 obsidown-0.1.2/LICENSE
--rw-r--r--   0        0        0     1543 2024-04-05 13:43:10.893560 obsidown-0.1.2/README.md
--rw-r--r--   0        0        0      128 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/__init__.py
--rw-r--r--   0        0        0      338 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/__main__.py
--rw-r--r--   0        0        0      605 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/config.py
--rw-r--r--   0        0        0     4929 2024-04-05 13:14:40.336833 obsidown-0.1.2/obsidown/main.py
--rw-r--r--   0        0        0     1202 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/operations/base.py
--rw-r--r--   0        0        0     1092 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/operations/dispatch.py
--rw-r--r--   0        0        0     1043 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/operations/link_convert.py
--rw-r--r--   0        0        0      560 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/operations/math_convert.py
--rw-r--r--   0        0        0      601 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/operations/remove_after_string.py
--rw-r--r--   0        0        0     1197 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/operations/update_frontmatter.py
--rw-r--r--   0        0        0      692 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/operations/write_file.py
--rw-r--r--   0        0        0     4244 2024-04-05 13:13:48.556831 obsidown-0.1.2/obsidown/utils.py
--rw-r--r--   0        0        0     1805 2024-04-05 14:16:36.553630 obsidown-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2117 1970-01-01 00:00:00.000000 obsidown-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 14:49:49.143949 obsidown-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1608 2024-04-05 14:49:49.143949 obsidown-0.1.3/README.md
+-rw-r--r--   0        0        0      128 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/__init__.py
+-rw-r--r--   0        0        0      338 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/__main__.py
+-rw-r--r--   0        0        0      605 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/config.py
+-rw-r--r--   0        0        0     4929 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/main.py
+-rw-r--r--   0        0        0     1202 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/operations/base.py
+-rw-r--r--   0        0        0     1092 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/operations/dispatch.py
+-rw-r--r--   0        0        0     1043 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/operations/link_convert.py
+-rw-r--r--   0        0        0      560 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/operations/math_convert.py
+-rw-r--r--   0        0        0      601 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/operations/remove_after_string.py
+-rw-r--r--   0        0        0     1197 2024-04-05 14:49:49.143949 obsidown-0.1.3/obsidown/operations/update_frontmatter.py
+-rw-r--r--   0        0        0      692 2024-04-05 14:49:49.147949 obsidown-0.1.3/obsidown/operations/write_file.py
+-rw-r--r--   0        0        0     4244 2024-04-05 14:49:49.147949 obsidown-0.1.3/obsidown/utils.py
+-rw-r--r--   0        0        0     1812 2024-04-05 14:49:49.147949 obsidown-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 obsidown-0.1.3/PKG-INFO
```

### Comparing `obsidown-0.1.2/LICENSE` & `obsidown-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/README.md` & `obsidown-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 - Use obsidian to write for Jekyll web pages. 
 
 ## How to use
 
 Define a configuration file `config.yaml`. In the repo it is provided one as example.
 Install the `poetry` dependencies and then you just need to run `poetry run python -m obsidown --config path/to/config.yaml`
 
-Installation as a python package is still on todo!
+It's possible to install from `pypi` index by `pip install obsidown`.
+Then you can run it with `python -m obsidown`
 
 ## Feedback
 
 This project is a hobby project used to automate some things I use myself. Currently it is a early early project!
 If you need additional features or report some issues or need help, feel free to open a new issue.
 
 ## Documentation
```

### Comparing `obsidown-0.1.2/obsidown/config.py` & `obsidown-0.1.3/obsidown/config.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/main.py` & `obsidown-0.1.3/obsidown/main.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/operations/base.py` & `obsidown-0.1.3/obsidown/operations/base.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/operations/dispatch.py` & `obsidown-0.1.3/obsidown/operations/dispatch.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/operations/link_convert.py` & `obsidown-0.1.3/obsidown/operations/link_convert.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/operations/math_convert.py` & `obsidown-0.1.3/obsidown/operations/math_convert.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/operations/remove_after_string.py` & `obsidown-0.1.3/obsidown/operations/remove_after_string.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/operations/update_frontmatter.py` & `obsidown-0.1.3/obsidown/operations/update_frontmatter.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/operations/write_file.py` & `obsidown-0.1.3/obsidown/operations/write_file.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/obsidown/utils.py` & `obsidown-0.1.3/obsidown/utils.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.2/pyproject.toml` & `obsidown-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "obsidown"
-version = "0.1.2"
+version = "0.1.3"
 description = "A quick way to convert obsidian markdown docs to markdown static pages"
 authors = ["Angelo 'Flecart' Huang <xuanqiang.huang@studio.unibo.it>"]
-license = "GPLv3"
+license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pyyaml = "^6.0.1"
 python-frontmatter = "^1.1.0"
 pydantic = "^2.6.3"
```

### Comparing `obsidown-0.1.2/PKG-INFO` & `obsidown-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: obsidown
-Version: 0.1.2
+Version: 0.1.3
 Summary: A quick way to convert obsidian markdown docs to markdown static pages
-License: GPLv3
+License: GPL-3.0-only
 Author: Angelo 'Flecart' Huang
 Author-email: xuanqiang.huang@studio.unibo.it
 Requires-Python: >=3.11,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: python-frontmatter (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # ObsiDown
 
@@ -24,15 +25,16 @@
 - Use obsidian to write for Jekyll web pages. 
 
 ## How to use
 
 Define a configuration file `config.yaml`. In the repo it is provided one as example.
 Install the `poetry` dependencies and then you just need to run `poetry run python -m obsidown --config path/to/config.yaml`
 
-Installation as a python package is still on todo!
+It's possible to install from `pypi` index by `pip install obsidown`.
+Then you can run it with `python -m obsidown`
 
 ## Feedback
 
 This project is a hobby project used to automate some things I use myself. Currently it is a early early project!
 If you need additional features or report some issues or need help, feel free to open a new issue.
 
 ## Documentation
```

