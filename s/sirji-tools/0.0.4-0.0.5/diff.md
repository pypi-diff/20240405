# Comparing `tmp/sirji-tools-0.0.4.tar.gz` & `tmp/sirji-tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-tools-0.0.4.tar", last modified: Thu Apr  4 13:10:02 2024, max compression
+gzip compressed data, was "sirji-tools-0.0.5.tar", last modified: Fri Apr  5 08:25:22 2024, max compression
```

## Comparing `sirji-tools-0.0.4.tar` & `sirji-tools-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.016637 sirji-tools-0.0.4/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1614 2024-04-04 13:10:02.015834 sirji-tools-0.0.4/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1222 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 13:10:02.016820 sirji-tools-0.0.4/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.000570 sirji-tools-0.0.4/sirji_tools/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.004395 sirji-tools-0.0.4/sirji_tools/config/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/config/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/config/config_loader.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.008957 sirji-tools-0.0.4/sirji_tools/crawler/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/github_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/web_page_handler.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.010009 sirji-tools-0.0.4/sirji_tools/logger/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/logger/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3587 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/logger/logger.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.011130 sirji-tools-0.0.4/sirji_tools/search/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/search/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/search/search.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.014963 sirji-tools-0.0.4/sirji_tools.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1614 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.014003 sirji-tools-0.0.4/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/tests/test_crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/tests/test_logger.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/tests/test_pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/tests/test_search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.562761 sirji-tools-0.0.5/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1614 2024-04-05 08:25:22.561864 sirji-tools-0.0.5/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1222 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 08:25:22.562899 sirji-tools-0.0.5/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.541966 sirji-tools-0.0.5/sirji_tools/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.544637 sirji-tools-0.0.5/sirji_tools/config/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/config/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/config/config_loader.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.551241 sirji-tools-0.0.5/sirji_tools/crawler/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/github_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/crawler/web_page_handler.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.553288 sirji-tools-0.0.5/sirji_tools/logger/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/logger/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3847 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/logger/logger.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.555324 sirji-tools-0.0.5/sirji_tools/search/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/search/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/sirji_tools/search/search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.559943 sirji-tools-0.0.5/sirji_tools.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1614 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-05 08:25:22.000000 sirji-tools-0.0.5/sirji_tools.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:25:22.558820 sirji-tools-0.0.5/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/tests/test_crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/tests/test_logger.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/tests/test_pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-05 08:25:05.000000 sirji-tools-0.0.5/tests/test_search.py
```

### Comparing `sirji-tools-0.0.4/LICENSE` & `sirji-tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/PKG-INFO` & `sirji-tools-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sirji-tools-0.0.4/README.md` & `sirji-tools-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/setup.py` & `sirji-tools-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-tools',
-    version='0.0.4',
+    version='0.0.5',
     author='Sirji',
     description='Crawler and search tools used by Sirji.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-tools-0.0.4/sirji_tools/crawler/base.py` & `sirji-tools-0.0.5/sirji_tools/crawler/base.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/sirji_tools/crawler/crawler.py` & `sirji-tools-0.0.5/sirji_tools/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/sirji_tools/crawler/factory.py` & `sirji-tools-0.0.5/sirji_tools/crawler/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/sirji_tools/crawler/github_handler.py` & `sirji-tools-0.0.5/sirji_tools/crawler/github_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/sirji_tools/crawler/pdf_handler.py` & `sirji-tools-0.0.5/sirji_tools/crawler/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/sirji_tools/crawler/web_page_handler.py` & `sirji-tools-0.0.5/sirji_tools/crawler/web_page_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/sirji_tools/logger/logger.py` & `sirji-tools-0.0.5/sirji_tools/logger/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,29 @@
 # Singleton class to create loggers
 class LoggerSingleton:
 
     def __init__(self, file_name, log_level):
         self.logger = self._setup_logger(file_name, log_level)
     
     def _log_folder(self):
-        return os.path.join(self._get_workspace_folder(), '.sirji', "logs")
+        return os.path.join(self._get_workspace_folder(), '.sirji', self._get_run_id_folder(), "logs")
     
     def _get_workspace_folder(self):
         workspace = os.environ.get("SIRJI_WORKSPACE")
         if workspace is None:
             raise ValueError(
                 "SIRJI_WORKSPACE is not set as an environment variable")
         return workspace
+
+    def _get_run_id_folder(self):
+        run_id = os.environ.get("SIRJI_RUN_ID")
+        if run_id is None:
+            raise ValueError(
+                "SIRJI_RUN_ID is not set as an environment variable")
+        return run_id 
     
     def _log_file_path(self, file_name):
         return os.path.join(self._log_folder(), file_name)
         
     def _setup_logger(self, file_name, log_level):
         # Create a folder named "logs" if it doesn't exist
         if not os.path.exists(self._log_folder()):
```

### Comparing `sirji-tools-0.0.4/sirji_tools/search/search.py` & `sirji-tools-0.0.5/sirji_tools/search/search.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/sirji_tools.egg-info/PKG-INFO` & `sirji-tools-0.0.5/sirji_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sirji-tools-0.0.4/sirji_tools.egg-info/SOURCES.txt` & `sirji-tools-0.0.5/sirji_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/tests/test_crawler.py` & `sirji-tools-0.0.5/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/tests/test_logger.py` & `sirji-tools-0.0.5/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/tests/test_pdf_handler.py` & `sirji-tools-0.0.5/tests/test_pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.4/tests/test_search.py` & `sirji-tools-0.0.5/tests/test_search.py`

 * *Files identical despite different names*

