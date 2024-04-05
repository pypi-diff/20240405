# Comparing `tmp/rocat-0.1.13.tar.gz` & `tmp/rocat-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocat-0.1.13.tar", last modified: Tue Apr  2 07:05:15 2024, max compression
+gzip compressed data, was "rocat-0.1.14.tar", last modified: Fri Apr  5 05:06:35 2024, max compression
```

## Comparing `rocat-0.1.13.tar` & `rocat-0.1.14.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:05:15.365456 rocat-0.1.13/
--rw-rw-rw-   0        0        0     1081 2024-04-02 05:31:45.000000 rocat-0.1.13/LICENSE
--rw-rw-rw-   0        0        0       28 2024-04-02 05:31:45.000000 rocat-0.1.13/MANIFEST.in
--rw-rw-rw-   0        0        0     2117 2024-04-02 07:05:15.364457 rocat-0.1.13/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2024-04-02 07:04:17.000000 rocat-0.1.13/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 07:05:15.352458 rocat-0.1.13/rocat/
--rw-rw-rw-   0        0        0      146 2024-04-02 06:47:50.000000 rocat-0.1.13/rocat/__init__.py
--rw-rw-rw-   0        0        0     2479 2024-04-02 07:04:18.000000 rocat-0.1.13/rocat/chatbot_modules.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:05:15.363458 rocat-0.1.13/rocat.egg-info/
--rw-rw-rw-   0        0        0     2117 2024-04-02 07:05:15.000000 rocat-0.1.13/rocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-04-02 07:05:15.000000 rocat-0.1.13/rocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:05:15.000000 rocat-0.1.13/rocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-02 07:05:15.000000 rocat-0.1.13/rocat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 07:05:15.000000 rocat-0.1.13/rocat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 07:05:15.365456 rocat-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0      678 2024-04-02 07:04:15.000000 rocat-0.1.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:05:15.363458 rocat-0.1.13/tests/
--rw-rw-rw-   0        0        0      458 2024-04-02 07:04:15.000000 rocat-0.1.13/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-05 05:06:35.809868 rocat-0.1.14/
+-rw-rw-rw-   0        0        0     1081 2024-04-05 05:02:16.000000 rocat-0.1.14/LICENSE
+-rw-rw-rw-   0        0        0       28 2024-04-05 05:02:16.000000 rocat-0.1.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     2170 2024-04-05 05:06:35.808866 rocat-0.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2024-04-05 05:02:16.000000 rocat-0.1.14/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 05:06:35.789867 rocat-0.1.14/rocat/
+-rw-rw-rw-   0        0        0      146 2024-04-05 05:02:16.000000 rocat-0.1.14/rocat/__init__.py
+-rw-rw-rw-   0        0        0     2479 2024-04-05 05:02:16.000000 rocat-0.1.14/rocat/chatbot_modules.py
+drwxrwxrwx   0        0        0        0 2024-04-05 05:06:35.807867 rocat-0.1.14/rocat.egg-info/
+-rw-rw-rw-   0        0        0     2170 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 05:06:35.809868 rocat-0.1.14/setup.cfg
+-rw-rw-rw-   0        0        0      722 2024-04-05 05:04:36.000000 rocat-0.1.14/setup.py
```

### Comparing `rocat-0.1.13/LICENSE` & `rocat-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `rocat-0.1.13/PKG-INFO` & `rocat-0.1.14/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.1.13
+Version: 0.1.14
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/Yumeta-Lab/rocat
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
+Requires-Dist: anthropic
 Requires-Dist: streamlit
+Requires-Dist: matplotlib
 
 # 😺🚀RoCat
 
 RoCat is a Python library that provides a simple and user-friendly interface for integrating AI services into your projects.
 
 ## Installation
```

### Comparing `rocat-0.1.13/README.md` & `rocat-0.1.14/README.md`

 * *Files identical despite different names*

### Comparing `rocat-0.1.13/rocat/chatbot_modules.py` & `rocat-0.1.14/rocat/chatbot_modules.py`

 * *Files identical despite different names*

### Comparing `rocat-0.1.13/rocat.egg-info/PKG-INFO` & `rocat-0.1.14/rocat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.1.13
+Version: 0.1.14
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/Yumeta-Lab/rocat
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
+Requires-Dist: anthropic
 Requires-Dist: streamlit
+Requires-Dist: matplotlib
 
 # 😺🚀RoCat
 
 RoCat is a Python library that provides a simple and user-friendly interface for integrating AI services into your projects.
 
 ## Installation
```

### Comparing `rocat-0.1.13/setup.py` & `rocat-0.1.14/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="rocat",
-    version="0.1.13",
+    version="0.1.14",
     description="A simple and user-friendly library for AI services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="YumetaLab",
     author_email="root@yumeta.kr",
     url="https://github.com/Yumeta-Lab/rocat",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "openai",
+        "anthropic",
         "streamlit",
+        "matplotlib"
     ],
     package_data={
         "": ["*.py"],
     },
     include_package_data=True,
 )
```

