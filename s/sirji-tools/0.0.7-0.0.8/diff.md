# Comparing `tmp/sirji-tools-0.0.7.tar.gz` & `tmp/sirji-tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-tools-0.0.7.tar", last modified: Fri Apr  5 15:46:19 2024, max compression
+gzip compressed data, was "sirji-tools-0.0.8.tar", last modified: Fri Apr  5 16:01:58 2024, max compression
```

## Comparing `sirji-tools-0.0.7.tar` & `sirji-tools-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.714948 sirji-tools-0.0.7/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3963 2024-04-05 15:46:19.714430 sirji-tools-0.0.7/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3571 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 15:46:19.715105 sirji-tools-0.0.7/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.703808 sirji-tools-0.0.7/sirji_tools/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.709362 sirji-tools-0.0.7/sirji_tools/crawler/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/github_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/crawler/web_page_handler.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.710415 sirji-tools-0.0.7/sirji_tools/logger/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/logger/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/logger/logger.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.711377 sirji-tools-0.0.7/sirji_tools/search/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/search/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1776 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/sirji_tools/search/search.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.713802 sirji-tools-0.0.7/sirji_tools.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3963 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      681 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 15:46:19.000000 sirji-tools-0.0.7/sirji_tools.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 15:46:19.713203 sirji-tools-0.0.7/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/tests/test_crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/tests/test_logger.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/tests/test_pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2022 2024-04-05 15:46:15.000000 sirji-tools-0.0.7/tests/test_search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.933234 sirji-tools-0.0.8/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3979 2024-04-05 16:01:58.932506 sirji-tools-0.0.8/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3587 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 16:01:58.933497 sirji-tools-0.0.8/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.918079 sirji-tools-0.0.8/sirji_tools/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.926242 sirji-tools-0.0.8/sirji_tools/crawler/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/github_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/crawler/web_page_handler.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.927555 sirji-tools-0.0.8/sirji_tools/logger/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/logger/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/logger/logger.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.928724 sirji-tools-0.0.8/sirji_tools/search/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/search/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1776 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/sirji_tools/search/search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.931676 sirji-tools-0.0.8/sirji_tools.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3979 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      681 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 16:01:58.000000 sirji-tools-0.0.8/sirji_tools.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:01:58.931014 sirji-tools-0.0.8/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/tests/test_crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/tests/test_logger.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/tests/test_pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2022 2024-04-05 16:01:54.000000 sirji-tools-0.0.8/tests/test_search.py
```

### Comparing `sirji-tools-0.0.7/LICENSE` & `sirji-tools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/PKG-INFO` & `sirji-tools-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,15 +57,15 @@
 source venv/bin/activate
 ```
 
 ### Install Package
 
 Install the package from PyPi:
 
-```
+```zsh
 pip install sirji-tools
 ```
 
 ## Usage
 
 ### Environment Variables
 
@@ -120,17 +120,17 @@
 
 ```zsh
 pip install -e .
 ```
 
 ## Running Tests and Coverage Analysis
 
-Tests can be run, and coverage can be analyzed in a few simple steps:
+Follow the above mentioned steps for "contributors", before running the test cases.
 
-```bash
+```zsh
 # Install testing dependencies
 pip install pytest coverage
 
 # Execute tests
 pytest
 
 # Measure coverage, excluding test files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.7 Summary: Crawler and
+Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.8 Summary: Crawler and
 search tools used by Sirji. Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji License: MIT Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests==2.31.0 Requires-
 Dist: pypdf2==3.0.1 Requires-Dist: markdownify==0.11.6 Requires-Dist:
 playwright==1.42.0
                                  _[_S_i_r_j_i_ _L_o_g_o_]
             SSiirrjjii iiss aann OOppeenn SSoouurrccee AAII SSooffttwwaarree DDeevveellooppmmeenntt AAggeenntt..
@@ -12,15 +12,15 @@
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
 project-specific packages without conflicting with system-wide installations.
 ```zsh python3 -m venv venv source venv/bin/activate ``` ### Install Package
-Install the package from PyPi: ``` pip install sirji-tools ``` ## Usage ###
+Install the package from PyPi: ```zsh pip install sirji-tools ``` ## Usage ###
 Environment Variables Ensure that following environment variables are set:
 ```zsh export SIRJI_WORKSPACE="Absolute folder path for Sirji to use as it's
 workspace. Note that a .sirji folder will be created inside it." export
 SIRJI_RUN_ID='Unique alphanumeric ID for each run. Note that a sub folder named
 by this ID will be created inside of .sirji folder to store logs, etc.' ``` ###
 Crawl URLs Crawl URLs tool will be used to crawl the web pages and extract the
 information from the web pages. And store the information for the further
@@ -33,12 +33,13 @@
 ``` ### Logger Logger tool will be used to log the information in the log file.
 It will be used to log the information to show the progress of the execution.
 ```python from sirji_tools.logger import p_logger p_logger.info("Log line
 here") ``` ## For Contributors 1. Fork and clone the repository. 2. Create and
 activate the virtual environment as described above. 3. Set the environment
 variables as described above. 4. Install the package in editable mode by
 running the following command from repository root: ```zsh pip install -e . ```
-## Running Tests and Coverage Analysis Tests can be run, and coverage can be
-analyzed in a few simple steps: ```bash # Install testing dependencies pip
-install pytest coverage # Execute tests pytest # Measure coverage, excluding
-test files coverage run --omit="tests/*" -m pytest coverage report ``` ##
-License Distributed under the MIT License. See `LICENSE` for more information.
+## Running Tests and Coverage Analysis Follow the above mentioned steps for
+"contributors", before running the test cases. ```zsh # Install testing
+dependencies pip install pytest coverage # Execute tests pytest # Measure
+coverage, excluding test files coverage run --omit="tests/*" -m pytest coverage
+report ``` ## License Distributed under the MIT License. See `LICENSE` for more
+information.
```

### Comparing `sirji-tools-0.0.7/README.md` & `sirji-tools-0.0.8/sirji_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: sirji-tools
+Version: 0.0.8
+Summary: Crawler and search tools used by Sirji.
+Home-page: https://github.com/sirji-ai/sirji
+Author: Sirji
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests==2.31.0
+Requires-Dist: pypdf2==3.0.1
+Requires-Dist: markdownify==0.11.6
+Requires-Dist: playwright==1.42.0
+
 <p align="center">
   <a href="." target="blank"><img src="https://github.com/sirji-ai/sirji/assets/7627517/363fc6dd-69af-4d84-8b7c-a91ec092058d" width="250" alt="Sirji Logo" /></a>
 </p>
 
 <p align="center">
   <em>Sirji is an Open Source AI Software Development Agent.</em>
 </p>
@@ -42,15 +57,15 @@
 source venv/bin/activate
 ```
 
 ### Install Package
 
 Install the package from PyPi:
 
-```
+```zsh
 pip install sirji-tools
 ```
 
 ## Usage
 
 ### Environment Variables
 
@@ -105,17 +120,17 @@
 
 ```zsh
 pip install -e .
 ```
 
 ## Running Tests and Coverage Analysis
 
-Tests can be run, and coverage can be analyzed in a few simple steps:
+Follow the above mentioned steps for "contributors", before running the test cases.
 
-```bash
+```zsh
 # Install testing dependencies
 pip install pytest coverage
 
 # Execute tests
 pytest
 
 # Measure coverage, excluding test files
```

#### html2text {}

```diff
@@ -1,20 +1,26 @@
+Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.8 Summary: Crawler and
+search tools used by Sirji. Home-page: https://github.com/sirji-ai/sirji
+Author: Sirji License: MIT Requires-Python: >=3.6 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: requests==2.31.0 Requires-
+Dist: pypdf2==3.0.1 Requires-Dist: markdownify==0.11.6 Requires-Dist:
+playwright==1.42.0
                                  _[_S_i_r_j_i_ _L_o_g_o_]
             SSiirrjjii iiss aann OOppeenn SSoouurrccee AAII SSooffttwwaarree DDeevveellooppmmeenntt AAggeenntt..
                        Built with â¤ï¸ by _T_r_u_e_ _S_p_a_r_r_o_w
  [GitHub License][GitHub commit activity][GitHub Issues or Pull Requests][PyPI
                                  sirji-tools]
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
 project-specific packages without conflicting with system-wide installations.
 ```zsh python3 -m venv venv source venv/bin/activate ``` ### Install Package
-Install the package from PyPi: ``` pip install sirji-tools ``` ## Usage ###
+Install the package from PyPi: ```zsh pip install sirji-tools ``` ## Usage ###
 Environment Variables Ensure that following environment variables are set:
 ```zsh export SIRJI_WORKSPACE="Absolute folder path for Sirji to use as it's
 workspace. Note that a .sirji folder will be created inside it." export
 SIRJI_RUN_ID='Unique alphanumeric ID for each run. Note that a sub folder named
 by this ID will be created inside of .sirji folder to store logs, etc.' ``` ###
 Crawl URLs Crawl URLs tool will be used to crawl the web pages and extract the
 information from the web pages. And store the information for the further
@@ -27,12 +33,13 @@
 ``` ### Logger Logger tool will be used to log the information in the log file.
 It will be used to log the information to show the progress of the execution.
 ```python from sirji_tools.logger import p_logger p_logger.info("Log line
 here") ``` ## For Contributors 1. Fork and clone the repository. 2. Create and
 activate the virtual environment as described above. 3. Set the environment
 variables as described above. 4. Install the package in editable mode by
 running the following command from repository root: ```zsh pip install -e . ```
-## Running Tests and Coverage Analysis Tests can be run, and coverage can be
-analyzed in a few simple steps: ```bash # Install testing dependencies pip
-install pytest coverage # Execute tests pytest # Measure coverage, excluding
-test files coverage run --omit="tests/*" -m pytest coverage report ``` ##
-License Distributed under the MIT License. See `LICENSE` for more information.
+## Running Tests and Coverage Analysis Follow the above mentioned steps for
+"contributors", before running the test cases. ```zsh # Install testing
+dependencies pip install pytest coverage # Execute tests pytest # Measure
+coverage, excluding test files coverage run --omit="tests/*" -m pytest coverage
+report ``` ## License Distributed under the MIT License. See `LICENSE` for more
+information.
```

### Comparing `sirji-tools-0.0.7/setup.py` & `sirji-tools-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-tools',
-    version='0.0.7',
+    version='0.0.8',
     author='Sirji',
     description='Crawler and search tools used by Sirji.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-tools-0.0.7/sirji_tools/crawler/base.py` & `sirji-tools-0.0.8/sirji_tools/crawler/base.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/sirji_tools/crawler/crawler.py` & `sirji-tools-0.0.8/sirji_tools/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/sirji_tools/crawler/factory.py` & `sirji-tools-0.0.8/sirji_tools/crawler/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/sirji_tools/crawler/github_handler.py` & `sirji-tools-0.0.8/sirji_tools/crawler/github_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/sirji_tools/crawler/pdf_handler.py` & `sirji-tools-0.0.8/sirji_tools/crawler/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/sirji_tools/crawler/web_page_handler.py` & `sirji-tools-0.0.8/sirji_tools/crawler/web_page_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/sirji_tools/logger/logger.py` & `sirji-tools-0.0.8/sirji_tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/sirji_tools/search/search.py` & `sirji-tools-0.0.8/sirji_tools/search/search.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/sirji_tools.egg-info/PKG-INFO` & `sirji-tools-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sirji-tools
-Version: 0.0.7
-Summary: Crawler and search tools used by Sirji.
-Home-page: https://github.com/sirji-ai/sirji
-Author: Sirji
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests==2.31.0
-Requires-Dist: pypdf2==3.0.1
-Requires-Dist: markdownify==0.11.6
-Requires-Dist: playwright==1.42.0
-
 <p align="center">
   <a href="." target="blank"><img src="https://github.com/sirji-ai/sirji/assets/7627517/363fc6dd-69af-4d84-8b7c-a91ec092058d" width="250" alt="Sirji Logo" /></a>
 </p>
 
 <p align="center">
   <em>Sirji is an Open Source AI Software Development Agent.</em>
 </p>
@@ -57,15 +42,15 @@
 source venv/bin/activate
 ```
 
 ### Install Package
 
 Install the package from PyPi:
 
-```
+```zsh
 pip install sirji-tools
 ```
 
 ## Usage
 
 ### Environment Variables
 
@@ -120,17 +105,17 @@
 
 ```zsh
 pip install -e .
 ```
 
 ## Running Tests and Coverage Analysis
 
-Tests can be run, and coverage can be analyzed in a few simple steps:
+Follow the above mentioned steps for "contributors", before running the test cases.
 
-```bash
+```zsh
 # Install testing dependencies
 pip install pytest coverage
 
 # Execute tests
 pytest
 
 # Measure coverage, excluding test files
```

#### html2text {}

```diff
@@ -1,26 +1,20 @@
-Metadata-Version: 2.1 Name: sirji-tools Version: 0.0.7 Summary: Crawler and
-search tools used by Sirji. Home-page: https://github.com/sirji-ai/sirji
-Author: Sirji License: MIT Requires-Python: >=3.6 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: requests==2.31.0 Requires-
-Dist: pypdf2==3.0.1 Requires-Dist: markdownify==0.11.6 Requires-Dist:
-playwright==1.42.0
                                  _[_S_i_r_j_i_ _L_o_g_o_]
             SSiirrjjii iiss aann OOppeenn SSoouurrccee AAII SSooffttwwaarree DDeevveellooppmmeenntt AAggeenntt..
                        Built with â¤ï¸ by _T_r_u_e_ _S_p_a_r_r_o_w
  [GitHub License][GitHub commit activity][GitHub Issues or Pull Requests][PyPI
                                  sirji-tools]
               [GitHub Repo stars][GitHub forks][GitHub watchers]
 ## Sirji Tools `sirji-tools` is a PyPI package that provides tools for: -
 Crawling (downloading web pages to markdown files) - Searching on Google -
 Custom Logging ## Installation ### Setup Virtual Environment We recommend
 setting up a virtual environment to isolate Python dependencies, ensuring
 project-specific packages without conflicting with system-wide installations.
 ```zsh python3 -m venv venv source venv/bin/activate ``` ### Install Package
-Install the package from PyPi: ``` pip install sirji-tools ``` ## Usage ###
+Install the package from PyPi: ```zsh pip install sirji-tools ``` ## Usage ###
 Environment Variables Ensure that following environment variables are set:
 ```zsh export SIRJI_WORKSPACE="Absolute folder path for Sirji to use as it's
 workspace. Note that a .sirji folder will be created inside it." export
 SIRJI_RUN_ID='Unique alphanumeric ID for each run. Note that a sub folder named
 by this ID will be created inside of .sirji folder to store logs, etc.' ``` ###
 Crawl URLs Crawl URLs tool will be used to crawl the web pages and extract the
 information from the web pages. And store the information for the further
@@ -33,12 +27,13 @@
 ``` ### Logger Logger tool will be used to log the information in the log file.
 It will be used to log the information to show the progress of the execution.
 ```python from sirji_tools.logger import p_logger p_logger.info("Log line
 here") ``` ## For Contributors 1. Fork and clone the repository. 2. Create and
 activate the virtual environment as described above. 3. Set the environment
 variables as described above. 4. Install the package in editable mode by
 running the following command from repository root: ```zsh pip install -e . ```
-## Running Tests and Coverage Analysis Tests can be run, and coverage can be
-analyzed in a few simple steps: ```bash # Install testing dependencies pip
-install pytest coverage # Execute tests pytest # Measure coverage, excluding
-test files coverage run --omit="tests/*" -m pytest coverage report ``` ##
-License Distributed under the MIT License. See `LICENSE` for more information.
+## Running Tests and Coverage Analysis Follow the above mentioned steps for
+"contributors", before running the test cases. ```zsh # Install testing
+dependencies pip install pytest coverage # Execute tests pytest # Measure
+coverage, excluding test files coverage run --omit="tests/*" -m pytest coverage
+report ``` ## License Distributed under the MIT License. See `LICENSE` for more
+information.
```

### Comparing `sirji-tools-0.0.7/sirji_tools.egg-info/SOURCES.txt` & `sirji-tools-0.0.8/sirji_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/tests/test_crawler.py` & `sirji-tools-0.0.8/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/tests/test_logger.py` & `sirji-tools-0.0.8/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/tests/test_pdf_handler.py` & `sirji-tools-0.0.8/tests/test_pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.7/tests/test_search.py` & `sirji-tools-0.0.8/tests/test_search.py`

 * *Files identical despite different names*

