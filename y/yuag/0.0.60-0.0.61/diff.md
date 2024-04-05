# Comparing `tmp/yuag-0.0.60.tar.gz` & `tmp/yuag-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.60.tar", last modified: Thu Apr  4 15:32:56 2024, max compression
+gzip compressed data, was "yuag-0.0.61.tar", last modified: Thu Apr  4 21:30:12 2024, max compression
```

## Comparing `yuag-0.0.60.tar` & `yuag-0.0.61.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:32:56.071735 yuag-0.0.60/
--rw-rw-rw-   0        0        0       52 2024-04-04 15:32:56.068737 yuag-0.0.60/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-04 15:32:56.071735 yuag-0.0.60/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-04-04 15:32:48.000000 yuag-0.0.60/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:32:56.037712 yuag-0.0.60/yuag/
--rw-rw-rw-   0        0        0     2619 2024-04-01 20:27:54.000000 yuag-0.0.60/yuag/__init__.py
--rw-rw-rw-   0        0        0    31119 2024-04-04 15:32:31.000000 yuag-0.0.60/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:32:56.067736 yuag-0.0.60/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-04-04 15:32:55.000000 yuag-0.0.60/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-04 15:32:55.000000 yuag-0.0.60/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:32:55.000000 yuag-0.0.60/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-04 15:32:55.000000 yuag-0.0.60/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 21:30:12.167625 yuag-0.0.61/
+-rw-rw-rw-   0        0        0       52 2024-04-04 21:30:12.166625 yuag-0.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-04 21:30:12.168624 yuag-0.0.61/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-04-04 21:29:49.000000 yuag-0.0.61/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:30:12.139424 yuag-0.0.61/yuag/
+-rw-rw-rw-   0        0        0     2621 2024-04-04 21:30:03.000000 yuag-0.0.61/yuag/__init__.py
+-rw-rw-rw-   0        0        0    31119 2024-04-04 15:32:31.000000 yuag-0.0.61/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:30:12.164630 yuag-0.0.61/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-04-04 21:30:11.000000 yuag-0.0.61/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-04 21:30:11.000000 yuag-0.0.61/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 21:30:11.000000 yuag-0.0.61/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-04 21:30:11.000000 yuag-0.0.61/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.60/yuag/__init__.py` & `yuag-0.0.61/yuag/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 -----------------
 ```
 combine_json_files()
 uncombine_json_file()
 ```
 \n\n
 
-دوال لملفات القراء:
+دوال لملفات القراءة:
 -----------------
 ```
 combine_pdf_files()
 ```
 \n\n
 
 دوال النصوص:
```

### Comparing `yuag-0.0.60/yuag/yuag.py` & `yuag-0.0.61/yuag/yuag.py`

 * *Files identical despite different names*

