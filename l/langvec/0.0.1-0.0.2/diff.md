# Comparing `tmp/langvec-0.0.1.tar.gz` & `tmp/langvec-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langvec-0.0.1.tar", last modified: Sat Dec 23 06:50:49 2023, max compression
+gzip compressed data, was "langvec-0.0.2.tar", last modified: Fri Apr  5 10:11:28 2024, max compression
```

## Comparing `langvec-0.0.1.tar` & `langvec-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sim        (501) staff       (20)        0 2023-12-23 06:50:49.070854 langvec-0.0.1/
--rw-r--r--   0 sim        (501) staff       (20)     1073 2023-12-16 16:01:19.000000 langvec-0.0.1/LICENSE
--rw-r--r--   0 sim        (501) staff       (20)     2770 2023-12-23 06:50:49.070665 langvec-0.0.1/PKG-INFO
--rw-r--r--   0 sim        (501) staff       (20)     1659 2023-12-23 06:41:49.000000 langvec-0.0.1/README.md
-drwxr-xr-x   0 sim        (501) staff       (20)        0 2023-12-23 06:50:49.069742 langvec-0.0.1/langvec/
--rw-r--r--   0 sim        (501) staff       (20)      124 2023-12-23 06:41:49.000000 langvec-0.0.1/langvec/__init__.py
--rw-r--r--   0 sim        (501) staff       (20)      206 2023-12-20 04:16:21.000000 langvec-0.0.1/langvec/constants.py
--rw-r--r--   0 sim        (501) staff       (20)     1713 2023-12-23 06:48:20.000000 langvec-0.0.1/langvec/langvec.py
--rw-r--r--   0 sim        (501) staff       (20)      896 2023-12-23 06:41:49.000000 langvec-0.0.1/langvec/test.py
-drwxr-xr-x   0 sim        (501) staff       (20)        0 2023-12-23 06:50:49.070470 langvec-0.0.1/langvec.egg-info/
--rw-r--r--   0 sim        (501) staff       (20)     2770 2023-12-23 06:50:49.000000 langvec-0.0.1/langvec.egg-info/PKG-INFO
--rw-r--r--   0 sim        (501) staff       (20)      256 2023-12-23 06:50:49.000000 langvec-0.0.1/langvec.egg-info/SOURCES.txt
--rw-r--r--   0 sim        (501) staff       (20)        1 2023-12-23 06:50:49.000000 langvec-0.0.1/langvec.egg-info/dependency_links.txt
--rw-r--r--   0 sim        (501) staff       (20)        6 2023-12-23 06:50:49.000000 langvec-0.0.1/langvec.egg-info/requires.txt
--rw-r--r--   0 sim        (501) staff       (20)        8 2023-12-23 06:50:49.000000 langvec-0.0.1/langvec.egg-info/top_level.txt
--rw-r--r--   0 sim        (501) staff       (20)       38 2023-12-23 06:50:49.070898 langvec-0.0.1/setup.cfg
--rw-r--r--   0 sim        (501) staff       (20)     1398 2023-12-23 06:43:13.000000 langvec-0.0.1/setup.py
+drwxr-xr-x   0 sim        (501) staff       (20)        0 2024-04-05 10:11:28.273096 langvec-0.0.2/
+-rw-r--r--   0 sim        (501) staff       (20)     1073 2023-12-16 16:01:19.000000 langvec-0.0.2/LICENSE
+-rw-r--r--   0 sim        (501) staff       (20)     4384 2024-04-05 10:11:28.272907 langvec-0.0.2/PKG-INFO
+-rw-r--r--   0 sim        (501) staff       (20)     3273 2024-04-05 10:01:42.000000 langvec-0.0.2/README.md
+drwxr-xr-x   0 sim        (501) staff       (20)        0 2024-04-05 10:11:28.271850 langvec-0.0.2/langvec/
+-rw-r--r--   0 sim        (501) staff       (20)      125 2023-12-27 07:05:09.000000 langvec-0.0.2/langvec/__init__.py
+-rw-r--r--   0 sim        (501) staff       (20)      345 2024-04-05 09:59:54.000000 langvec-0.0.2/langvec/constants.py
+-rw-r--r--   0 sim        (501) staff       (20)    10081 2024-04-05 10:09:44.000000 langvec-0.0.2/langvec/langvec.py
+-rw-r--r--   0 sim        (501) staff       (20)     3805 2024-04-05 09:59:54.000000 langvec-0.0.2/langvec/test_langvec.py
+drwxr-xr-x   0 sim        (501) staff       (20)        0 2024-04-05 10:11:28.272685 langvec-0.0.2/langvec.egg-info/
+-rw-r--r--   0 sim        (501) staff       (20)     4384 2024-04-05 10:11:28.000000 langvec-0.0.2/langvec.egg-info/PKG-INFO
+-rw-r--r--   0 sim        (501) staff       (20)      264 2024-04-05 10:11:28.000000 langvec-0.0.2/langvec.egg-info/SOURCES.txt
+-rw-r--r--   0 sim        (501) staff       (20)        1 2024-04-05 10:11:28.000000 langvec-0.0.2/langvec.egg-info/dependency_links.txt
+-rw-r--r--   0 sim        (501) staff       (20)        6 2024-04-05 10:11:28.000000 langvec-0.0.2/langvec.egg-info/requires.txt
+-rw-r--r--   0 sim        (501) staff       (20)        8 2024-04-05 10:11:28.000000 langvec-0.0.2/langvec.egg-info/top_level.txt
+-rw-r--r--   0 sim        (501) staff       (20)       38 2024-04-05 10:11:28.273147 langvec-0.0.2/setup.cfg
+-rw-r--r--   0 sim        (501) staff       (20)     1398 2024-04-05 09:56:57.000000 langvec-0.0.2/setup.py
```

### Comparing `langvec-0.0.1/LICENSE` & `langvec-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langvec-0.0.1/setup.py` & `langvec-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="langvec",
-    version="0.0.1",
+    version="0.0.2",
     author="Simeon Emanuilov",
     author_email="simeon.emanuilov@gmail.com",
     description="Language of Vectors (LangVec) is a simple Python library designed for transforming numerical vector data into a language-like structure using a predefined set of words (lexicon).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=["langvec"],
```

