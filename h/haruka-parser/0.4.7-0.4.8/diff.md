# Comparing `tmp/haruka_parser-0.4.7.tar.gz` & `tmp/haruka_parser-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka_parser-0.4.7.tar", last modified: Wed Apr  3 21:47:12 2024, max compression
+gzip compressed data, was "haruka_parser-0.4.8.tar", last modified: Fri Apr  5 04:58:24 2024, max compression
```

## Comparing `haruka_parser-0.4.7.tar` & `haruka_parser-0.4.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.564712 haruka_parser-0.4.7/haruka_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.564712 haruka_parser-0.4.7/haruka_parser/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/dictionary/banned_selectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/dictionary/boilerplate_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/dictionary/latex_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/latex_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/line_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/meta_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/haruka_parser/mmltex/
--rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/cmarkup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/entities.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/glayout.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/scripts.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/tables.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/tokens.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/readablity_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/time_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/tree_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    27212 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/tree_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/haruka_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:58:24.888939 haruka_parser-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-05 04:58:24.888939 haruka_parser-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:58:24.884939 haruka_parser-0.4.8/haruka_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:58:24.884939 haruka_parser-0.4.8/haruka_parser/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/dictionary/banned_selectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/dictionary/boilerplate_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/dictionary/latex_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/latex_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/line_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/meta_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:58:24.888939 haruka_parser-0.4.8/haruka_parser/mmltex/
+-rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/mmltex/cmarkup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/mmltex/entities.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/mmltex/glayout.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/mmltex/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/mmltex/scripts.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/mmltex/tables.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/mmltex/tokens.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/readablity_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/time_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/tree_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27212 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/tree_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/haruka_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:58:24.888939 haruka_parser-0.4.8/haruka_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-05 04:58:24.000000 haruka_parser-0.4.8/haruka_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-05 04:58:24.000000 haruka_parser-0.4.8/haruka_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:58:24.000000 haruka_parser-0.4.8/haruka_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 04:58:24.000000 haruka_parser-0.4.8/haruka_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 04:58:24.000000 haruka_parser-0.4.8/haruka_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:58:24.888939 haruka_parser-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 04:58:17.000000 haruka_parser-0.4.8/setup.py
```

### Comparing `haruka_parser-0.4.7/PKG-INFO` & `haruka_parser-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.7
+Version: 0.4.8
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.7 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.8 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.7/README.md` & `haruka_parser-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/dictionary/banned_selectors.txt` & `haruka_parser-0.4.8/haruka_parser/dictionary/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/dictionary/boilerplate_words.txt` & `haruka_parser-0.4.8/haruka_parser/dictionary/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/dictionary/latex_words.txt` & `haruka_parser-0.4.8/haruka_parser/dictionary/latex_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/extract.py` & `haruka_parser-0.4.8/haruka_parser/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,15 +393,16 @@
             info["found_latex_text"] = True
         math_config = get_math_config(tree.document.html)
         if math_config is not None:
             info["found_latex_script"] = True
         extract_math(tree, replacement_manager, info)
     if config["extract_image_and_link"]:
         extract_image_and_link(tree, info)
-    extract_tree(tree, replacement_manager, config, info)
+    try: extract_tree(tree, replacement_manager, config, info)
+    except: pass
 
     lxml_tree = get_lxml_tree(str(tree))
     if lxml_tree is not None:
         # info["title"] = info["title"] or restore_replacements(
         #     get_title(lxml_tree), replacement_manager, config
         # )
         parser_config = ParserConfig(
```

### Comparing `haruka_parser-0.4.7/haruka_parser/latex_processing.py` & `haruka_parser-0.4.8/haruka_parser/latex_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/line_processing.py` & `haruka_parser-0.4.8/haruka_parser/line_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/meta_processing.py` & `haruka_parser-0.4.8/haruka_parser/meta_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/mmltex/cmarkup.xsl` & `haruka_parser-0.4.8/haruka_parser/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/mmltex/entities.xsl` & `haruka_parser-0.4.8/haruka_parser/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/mmltex/glayout.xsl` & `haruka_parser-0.4.8/haruka_parser/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/mmltex/mmltex.xsl` & `haruka_parser-0.4.8/haruka_parser/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/mmltex/scripts.xsl` & `haruka_parser-0.4.8/haruka_parser/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/mmltex/tables.xsl` & `haruka_parser-0.4.8/haruka_parser/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/mmltex/tokens.xsl` & `haruka_parser-0.4.8/haruka_parser/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/readablity_lxml.py` & `haruka_parser-0.4.8/haruka_parser/readablity_lxml.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/time_formatter.py` & `haruka_parser-0.4.8/haruka_parser/time_formatter.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/tree_cleaning.py` & `haruka_parser-0.4.8/haruka_parser/tree_cleaning.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/tree_processing.py` & `haruka_parser-0.4.8/haruka_parser/tree_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser/utils.py` & `haruka_parser-0.4.8/haruka_parser/utils.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/haruka_parser.egg-info/PKG-INFO` & `haruka_parser-0.4.8/haruka_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.7
+Version: 0.4.8
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.7 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.8 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.7/haruka_parser.egg-info/SOURCES.txt` & `haruka_parser-0.4.8/haruka_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.7/setup.py` & `haruka_parser-0.4.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # 0.1 version from OpenWebMath: https://github.com/keirp/OpenWebMath
 # OpenWebMath is made available under an ODC-By 1.0 license; users should also abide by the CommonCrawl ToU: https://commoncrawl.org/terms-of-use/. We do not alter the license of any of the underlying data.
 setup(
     name="haruka_parser",
-    version="0.4.7",
+    version="0.4.8",
     description="A simple HTML Parser",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="papersnake",
     author_email="prnake@gmail.com",
     url="https://github.com/prnake/haruka-parser",
     packages=["haruka_parser"],
```

