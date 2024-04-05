# Comparing `tmp/sirji-tools-0.0.6.tar.gz` & `tmp/sirji-tools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-tools-0.0.6.tar", last modified: Fri Apr  5 15:25:01 2024, max compression
+gzip compressed data, was "sirji-tools-0.0.7.tar", last modified: Fri Apr  5 15:46:19 2024, max compression
```

## Comparing `sirji-tools-0.0.6.tar` & `sirji-tools-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.625248 sirji-tools-0.0.6/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3964 2024-04-05 15:25:01.624216 sirji-tools-0.0.6/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3572 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 15:25:01.625406 sirji-tools-0.0.6/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.612950 sirji-tools-0.0.6/sirji_tools/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.617357 sirji-tools-0.0.6/sirji_tools/crawler/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/github_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/crawler/web_page_handler.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.618102 sirji-tools-0.0.6/sirji_tools/logger/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/logger/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/logger/logger.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.618848 sirji-tools-0.0.6/sirji_tools/search/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/search/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1776 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/sirji_tools/search/search.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.622547 sirji-tools-0.0.6/sirji_tools.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3964 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      681 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 15:25:01.000000 sirji-tools-0.0.6/sirji_tools.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:25:01.621243 sirji-tools-0.0.6/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/tests/test_crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/tests/test_logger.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/tests/test_pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2022 2024-04-05 15:24:57.000000 sirji-tools-0.0.6/tests/test_search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.714948 sirji-tools-0.0.7/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3963 2024-04-05 15:46:19.714430 sirji-tools-0.0.7/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3571 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 15:46:19.715105 sirji-tools-0.0.7/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.703808 sirji-tools-0.0.7/sirji_tools/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.709362 sirji-tools-0.0.7/sirji_tools/crawler/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/github_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/web_page_handler.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.710415 sirji-tools-0.0.7/sirji_tools/logger/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/logger/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/logger/logger.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.711377 sirji-tools-0.0.7/sirji_tools/search/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/search/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1776 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/search/search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.713802 sirji-tools-0.0.7/sirji_tools.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3963 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      681 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.713203 sirji-tools-0.0.7/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/tests/test_crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/tests/test_logger.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/tests/test_pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2022 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/tests/test_search.py
```

### Comparing `sirji-tools-0.0.6/LICENSE` & `sirji-tools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/PKG-INFO` & `sirji-tools-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,15 +18,15 @@
 </p>
 
 <p align="center">
   <em>Sirji is an Open Source AI Software Development Agent.</em>
 </p>
 
 <p align="center">
-  Built with :heart: by <a href="https://truesparrow.com/" target="_blank">True Sparrow</a>
+  Built with ❤️ by <a href="https://truesparrow.com/" target="_blank">True Sparrow</a>
 </p>
 
 <p align="center">
   <img alt="GitHub License" src="https://img.shields.io/github/license/sirji-ai/sirji">
   <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/m/sirji-ai/sirji">
   <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues/sirji-ai/sirji">
   <img alt="PyPI sirji-tools" src="https://img.shields.io/pypi/v/sirji-tools.svg">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.6 Summary: Crawler and
+Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.7 Summary: Crawler and
 search tools used by Sirji. Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji License: MIT Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests==2.31.0 Requires-
 Dist: pypdf2==3.0.1 Requires-Dist: markdownify==0.11.6 Requires-Dist:
 playwright==1.42.0
                                  _[_S_i_r_j_i_ _L_o_g_o_]
             SSiirrjjii iiss aann OOppeenn SSoouurrccee AAII SSooffttwwaarree DDeevveellooppmmeenntt AAggeenntt..
-                      Built with :heart: by _T_r_u_e_ _S_p_a_r_r_o_w
+                       Built with â¤ï¸ by _T_r_u_e_ _S_p_a_r_r_o_w
  [GitHub License][GitHub commit activity][GitHub Issues or Pull Requests][PyPI
                                  sirji-tools]
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
```

### Comparing `sirji-tools-0.0.6/README.md` & `sirji-tools-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 <p align="center">
   <em>Sirji is an Open Source AI Software Development Agent.</em>
 </p>
 
 <p align="center">
-  Built with :heart: by <a href="https://truesparrow.com/" target="_blank">True Sparrow</a>
+  Built with ❤️ by <a href="https://truesparrow.com/" target="_blank">True Sparrow</a>
 </p>
 
 <p align="center">
   <img alt="GitHub License" src="https://img.shields.io/github/license/sirji-ai/sirji">
   <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/m/sirji-ai/sirji">
   <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues/sirji-ai/sirji">
   <img alt="PyPI sirji-tools" src="https://img.shields.io/pypi/v/sirji-tools.svg">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                                  _[_S_i_r_j_i_ _L_o_g_o_]
             SSiirrjjii iiss aann OOppeenn SSoouurrccee AAII SSooffttwwaarree DDeevveellooppmmeenntt AAggeenntt..
-                      Built with :heart: by _T_r_u_e_ _S_p_a_r_r_o_w
+                       Built with â¤ï¸ by _T_r_u_e_ _S_p_a_r_r_o_w
  [GitHub License][GitHub commit activity][GitHub Issues or Pull Requests][PyPI
                                  sirji-tools]
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
```

### Comparing `sirji-tools-0.0.6/setup.py` & `sirji-tools-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-tools',
-    version='0.0.6',
+    version='0.0.7',
     author='Sirji',
     description='Crawler and search tools used by Sirji.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-tools-0.0.6/sirji_tools/crawler/base.py` & `sirji-tools-0.0.7/sirji_tools/crawler/base.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/sirji_tools/crawler/crawler.py` & `sirji-tools-0.0.7/sirji_tools/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/sirji_tools/crawler/factory.py` & `sirji-tools-0.0.7/sirji_tools/crawler/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/sirji_tools/crawler/github_handler.py` & `sirji-tools-0.0.7/sirji_tools/crawler/github_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/sirji_tools/crawler/pdf_handler.py` & `sirji-tools-0.0.7/sirji_tools/crawler/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/sirji_tools/crawler/web_page_handler.py` & `sirji-tools-0.0.7/sirji_tools/crawler/web_page_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/sirji_tools/logger/logger.py` & `sirji-tools-0.0.7/sirji_tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/sirji_tools/search/search.py` & `sirji-tools-0.0.7/sirji_tools/search/search.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/sirji_tools.egg-info/PKG-INFO` & `sirji-tools-0.0.7/sirji_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,15 +18,15 @@
 </p>
 
 <p align="center">
   <em>Sirji is an Open Source AI Software Development Agent.</em>
 </p>
 
 <p align="center">
-  Built with :heart: by <a href="https://truesparrow.com/" target="_blank">True Sparrow</a>
+  Built with ❤️ by <a href="https://truesparrow.com/" target="_blank">True Sparrow</a>
 </p>
 
 <p align="center">
   <img alt="GitHub License" src="https://img.shields.io/github/license/sirji-ai/sirji">
   <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/m/sirji-ai/sirji">
   <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues/sirji-ai/sirji">
   <img alt="PyPI sirji-tools" src="https://img.shields.io/pypi/v/sirji-tools.svg">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.6 Summary: Crawler and
+Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.7 Summary: Crawler and
 search tools used by Sirji. Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji License: MIT Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests==2.31.0 Requires-
 Dist: pypdf2==3.0.1 Requires-Dist: markdownify==0.11.6 Requires-Dist:
 playwright==1.42.0
                                  _[_S_i_r_j_i_ _L_o_g_o_]
             SSiirrjjii iiss aann OOppeenn SSoouurrccee AAII SSooffttwwaarree DDeevveellooppmmeenntt AAggeenntt..
-                      Built with :heart: by _T_r_u_e_ _S_p_a_r_r_o_w
+                       Built with â¤ï¸ by _T_r_u_e_ _S_p_a_r_r_o_w
  [GitHub License][GitHub commit activity][GitHub Issues or Pull Requests][PyPI
                                  sirji-tools]
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
```

### Comparing `sirji-tools-0.0.6/sirji_tools.egg-info/SOURCES.txt` & `sirji-tools-0.0.7/sirji_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/tests/test_crawler.py` & `sirji-tools-0.0.7/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/tests/test_logger.py` & `sirji-tools-0.0.7/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/tests/test_pdf_handler.py` & `sirji-tools-0.0.7/tests/test_pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.6/tests/test_search.py` & `sirji-tools-0.0.7/tests/test_search.py`

 * *Files identical despite different names*

