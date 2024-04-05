# Comparing `tmp/trmnl-colors-4.0.8.tar.gz` & `tmp/trmnl-colors-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trmnl-colors-4.0.8.tar", last modified: Thu Apr  4 10:10:02 2024, max compression
+gzip compressed data, was "trmnl-colors-4.0.9.tar", last modified: Fri Apr  5 08:36:16 2024, max compression
```

## Comparing `trmnl-colors-4.0.8.tar` & `trmnl-colors-4.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:10:02.940660 trmnl-colors-4.0.8/
--rw-rw-rw-   0        0        0     1090 2024-04-04 08:54:00.000000 trmnl-colors-4.0.8/LICENSE
--rw-rw-rw-   0        0        0     2533 2024-04-04 10:10:02.938660 trmnl-colors-4.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2188 2024-04-04 09:51:36.000000 trmnl-colors-4.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 10:10:02.940660 trmnl-colors-4.0.8/setup.cfg
--rw-rw-rw-   0        0        0      556 2024-04-04 09:35:59.000000 trmnl-colors-4.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:10:02.930660 trmnl-colors-4.0.8/trmnl_colors/
--rw-rw-rw-   0        0        0     1742 2024-04-04 09:06:14.000000 trmnl-colors-4.0.8/trmnl_colors/__init__.py
--rw-rw-rw-   0        0        0     2538 2024-04-04 09:35:43.000000 trmnl-colors-4.0.8/trmnl_colors/constants.py
--rw-rw-rw-   0        0        0     5210 2024-04-04 09:36:55.000000 trmnl-colors-4.0.8/trmnl_colors/functions.py
--rw-rw-rw-   0        0        0       47 2024-04-04 09:21:08.000000 trmnl-colors-4.0.8/trmnl_colors/test.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:10:02.937660 trmnl-colors-4.0.8/trmnl_colors.egg-info/
--rw-rw-rw-   0        0        0     2533 2024-04-04 10:10:02.000000 trmnl-colors-4.0.8/trmnl_colors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-04 10:10:02.000000 trmnl-colors-4.0.8/trmnl_colors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:10:02.000000 trmnl-colors-4.0.8/trmnl_colors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 10:10:02.000000 trmnl-colors-4.0.8/trmnl_colors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 08:36:16.753104 trmnl-colors-4.0.9/
+-rw-rw-rw-   0        0        0     1090 2024-04-04 08:54:00.000000 trmnl-colors-4.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2531 2024-04-05 08:36:16.752108 trmnl-colors-4.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2186 2024-04-04 10:30:18.000000 trmnl-colors-4.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 08:36:16.753104 trmnl-colors-4.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-04-05 08:35:49.000000 trmnl-colors-4.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 08:36:16.749118 trmnl-colors-4.0.9/trmnl_colors/
+-rw-rw-rw-   0        0        0     1742 2024-04-04 09:06:14.000000 trmnl-colors-4.0.9/trmnl_colors/__init__.py
+-rw-rw-rw-   0        0        0     2538 2024-04-04 09:35:43.000000 trmnl-colors-4.0.9/trmnl_colors/constants.py
+-rw-rw-rw-   0        0        0     5210 2024-04-04 09:36:55.000000 trmnl-colors-4.0.9/trmnl_colors/functions.py
+-rw-rw-rw-   0        0        0       47 2024-04-04 09:21:08.000000 trmnl-colors-4.0.9/trmnl_colors/test.py
+drwxrwxrwx   0        0        0        0 2024-04-05 08:36:16.751111 trmnl-colors-4.0.9/trmnl_colors.egg-info/
+-rw-rw-rw-   0        0        0     2531 2024-04-05 08:36:16.000000 trmnl-colors-4.0.9/trmnl_colors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-05 08:36:16.000000 trmnl-colors-4.0.9/trmnl_colors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 08:36:16.000000 trmnl-colors-4.0.9/trmnl_colors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 08:36:16.000000 trmnl-colors-4.0.9/trmnl_colors.egg-info/top_level.txt
```

### Comparing `trmnl-colors-4.0.8/LICENSE` & `trmnl-colors-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trmnl-colors-4.0.8/PKG-INFO` & `trmnl-colors-4.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trmnl-colors
-Version: 4.0.8
+Version: 4.0.9
 Summary: Colors, text formats, decorations and much more for TERMINAL
 Home-page: https://github.com/Idrisvohra9/colors
 Author: Idris-Vohra
 Author-email: idrishaider987@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -63,8 +63,8 @@
 ## Terminal Application Screenshots with trmnl_colors:
 ### Create Terminal programs such as the below examples. Only your imagination and python skills are a limit!
 
 ![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20171908.png?raw=true)
 ![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20172610.png?raw=true)
 > Explore & stay Creative
 
->## by: [Idris Vohra]("https://github.com/Idrisvohra9")
+>## by: [Idris Vohra](https://github.com/Idrisvohra9)
```

### Comparing `trmnl-colors-4.0.8/README.md` & `trmnl-colors-4.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 ## Terminal Application Screenshots with trmnl_colors:
 ### Create Terminal programs such as the below examples. Only your imagination and python skills are a limit!
 
 ![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20171908.png?raw=true)
 ![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20172610.png?raw=true)
 > Explore & stay Creative
 
->## by: [Idris Vohra]("https://github.com/Idrisvohra9")
+>## by: [Idris Vohra](https://github.com/Idrisvohra9)
```

### Comparing `trmnl-colors-4.0.8/setup.py` & `trmnl-colors-4.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
-
+# TODO: Increment the version number and release it.
 setuptools.setup(
     name="trmnl-colors",
-    version="4.0.8",
+    version="4.0.9",
     author="Idris-Vohra",
     author_email="idrishaider987@gmail.com",
     packages=["trmnl_colors"],
     description="Colors, text formats, decorations and much more for TERMINAL",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/Idrisvohra9/colors",
```

### Comparing `trmnl-colors-4.0.8/trmnl_colors/__init__.py` & `trmnl-colors-4.0.9/trmnl_colors/__init__.py`

 * *Files identical despite different names*

### Comparing `trmnl-colors-4.0.8/trmnl_colors/constants.py` & `trmnl-colors-4.0.9/trmnl_colors/constants.py`

 * *Files identical despite different names*

### Comparing `trmnl-colors-4.0.8/trmnl_colors/functions.py` & `trmnl-colors-4.0.9/trmnl_colors/functions.py`

 * *Files identical despite different names*

### Comparing `trmnl-colors-4.0.8/trmnl_colors.egg-info/PKG-INFO` & `trmnl-colors-4.0.9/trmnl_colors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trmnl-colors
-Version: 4.0.8
+Version: 4.0.9
 Summary: Colors, text formats, decorations and much more for TERMINAL
 Home-page: https://github.com/Idrisvohra9/colors
 Author: Idris-Vohra
 Author-email: idrishaider987@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -63,8 +63,8 @@
 ## Terminal Application Screenshots with trmnl_colors:
 ### Create Terminal programs such as the below examples. Only your imagination and python skills are a limit!
 
 ![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20171908.png?raw=true)
 ![Screenshots](https://github.com/Idrisvohra9/trmnl-colors/blob/main/static/Screenshot%202023-08-24%20172610.png?raw=true)
 > Explore & stay Creative
 
->## by: [Idris Vohra]("https://github.com/Idrisvohra9")
+>## by: [Idris Vohra](https://github.com/Idrisvohra9)
```

