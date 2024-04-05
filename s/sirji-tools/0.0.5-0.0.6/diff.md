# Comparing `tmp/sirji-tools-0.0.5.tar.gz` & `tmp/sirji-tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-tools-0.0.5.tar", last modified: Fri Apr  5 08:25:22 2024, max compression
+gzip compressed data, was "sirji-tools-0.0.6.tar", last modified: Fri Apr  5 15:25:01 2024, max compression
```

## Comparing `sirji-tools-0.0.5.tar` & `sirji-tools-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,34 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.562761 sirji-tools-0.0.5/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1614 2024-04-05 08:25:22.561864 sirji-tools-0.0.5/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1222 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 08:25:22.562899 sirji-tools-0.0.5/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.541966 sirji-tools-0.0.5/sirji_tools/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.544637 sirji-tools-0.0.5/sirji_tools/config/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/config/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/config/config_loader.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.551241 sirji-tools-0.0.5/sirji_tools/crawler/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/github_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/web_page_handler.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.553288 sirji-tools-0.0.5/sirji_tools/logger/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/logger/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/logger/logger.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.555324 sirji-tools-0.0.5/sirji_tools/search/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/search/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/search/search.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.559943 sirji-tools-0.0.5/sirji_tools.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1614 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.558820 sirji-tools-0.0.5/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/tests/test_crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/tests/test_logger.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/tests/test_pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/tests/test_search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.625248 sirji-tools-0.0.6/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3964 2024-04-05 15:25:01.624216 sirji-tools-0.0.6/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3572 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 15:25:01.625406 sirji-tools-0.0.6/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.612950 sirji-tools-0.0.6/sirji_tools/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.617357 sirji-tools-0.0.6/sirji_tools/crawler/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/github_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/web_page_handler.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.618102 sirji-tools-0.0.6/sirji_tools/logger/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/logger/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/logger/logger.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.618848 sirji-tools-0.0.6/sirji_tools/search/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/search/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1776 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/search/search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.622547 sirji-tools-0.0.6/sirji_tools.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3964 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      681 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.621243 sirji-tools-0.0.6/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/tests/test_crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/tests/test_logger.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/tests/test_pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2022 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/tests/test_search.py
```

### Comparing `sirji-tools-0.0.5/LICENSE` & `sirji-tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/setup.py` & `sirji-tools-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-tools',
-    version='0.0.5',
+    version='0.0.6',
     author='Sirji',
     description='Crawler and search tools used by Sirji.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-tools-0.0.5/sirji_tools/crawler/base.py` & `sirji-tools-0.0.6/sirji_tools/crawler/base.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/sirji_tools/crawler/crawler.py` & `sirji-tools-0.0.6/sirji_tools/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/sirji_tools/crawler/factory.py` & `sirji-tools-0.0.6/sirji_tools/crawler/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/sirji_tools/crawler/github_handler.py` & `sirji-tools-0.0.6/sirji_tools/crawler/github_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/sirji_tools/crawler/pdf_handler.py` & `sirji-tools-0.0.6/sirji_tools/crawler/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/sirji_tools/crawler/web_page_handler.py` & `sirji-tools-0.0.6/sirji_tools/crawler/web_page_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/sirji_tools/logger/logger.py` & `sirji-tools-0.0.6/sirji_tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/sirji_tools.egg-info/SOURCES.txt` & `sirji-tools-0.0.6/sirji_tools.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 setup.py
 sirji_tools/__init__.py
 sirji_tools.egg-info/PKG-INFO
 sirji_tools.egg-info/SOURCES.txt
 sirji_tools.egg-info/dependency_links.txt
 sirji_tools.egg-info/requires.txt
 sirji_tools.egg-info/top_level.txt
-sirji_tools/config/__init__.py
-sirji_tools/config/config_loader.py
 sirji_tools/crawler/__init__.py
 sirji_tools/crawler/base.py
 sirji_tools/crawler/crawler.py
 sirji_tools/crawler/factory.py
 sirji_tools/crawler/github_handler.py
 sirji_tools/crawler/pdf_handler.py
 sirji_tools/crawler/web_page_handler.py
```

### Comparing `sirji-tools-0.0.5/tests/test_crawler.py` & `sirji-tools-0.0.6/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/tests/test_logger.py` & `sirji-tools-0.0.6/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.5/tests/test_pdf_handler.py` & `sirji-tools-0.0.6/tests/test_pdf_handler.py`

 * *Files identical despite different names*

