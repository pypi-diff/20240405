# Comparing `tmp/nbresult-0.0.9.tar.gz` & `tmp/nbresult-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbresult-0.0.9.tar", last modified: Mon Nov 21 16:41:37 2022, max compression
+gzip compressed data, was "nbresult-0.1.0.tar", last modified: Thu Apr  4 07:59:30 2024, max compression
```

## Comparing `nbresult-0.0.9.tar` & `nbresult-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,14 @@
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.128810 nbresult-0.0.9/
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.120303 nbresult-0.0.9/.github/
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.122060 nbresult-0.0.9/.github/workflows/
--rw-r--r--   0 gmanchon   (501) staff       (20)      547 2022-11-17 14:40:46.000000 nbresult-0.0.9/.github/workflows/test.yml
--rw-r--r--   0 gmanchon   (501) staff       (20)       54 2022-11-17 14:40:46.000000 nbresult-0.0.9/.gitignore
--rw-r--r--   0 gmanchon   (501) staff       (20)      565 2022-11-21 16:19:47.000000 nbresult-0.0.9/CHANGELOG.md
--rw-r--r--   0 gmanchon   (501) staff       (20)     1065 2021-09-06 12:08:58.000000 nbresult-0.0.9/LICENSE
--rw-r--r--   0 gmanchon   (501) staff       (20)        1 2022-11-17 14:40:46.000000 nbresult-0.0.9/MANIFEST.in
--rw-r--r--   0 gmanchon   (501) staff       (20)      493 2022-11-17 14:40:46.000000 nbresult-0.0.9/Makefile
--rw-r--r--   0 gmanchon   (501) staff       (20)     2631 2022-11-21 16:41:37.128699 nbresult-0.0.9/PKG-INFO
--rw-r--r--   0 gmanchon   (501) staff       (20)     2355 2022-11-17 14:40:46.000000 nbresult-0.0.9/README.md
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.126361 nbresult-0.0.9/img/
--rw-r--r--   0 gmanchon   (501) staff       (20)   297702 2021-09-06 12:08:58.000000 nbresult-0.0.9/img/make_check.png
--rw-r--r--   0 gmanchon   (501) staff       (20)   225387 2021-09-06 12:08:58.000000 nbresult-0.0.9/img/notebook_check.png
--rw-r--r--   0 gmanchon   (501) staff       (20)   195595 2021-09-06 12:08:58.000000 nbresult-0.0.9/img/pytest_check.png
--rw-r--r--   0 gmanchon   (501) staff       (20)   381897 2022-05-17 13:35:52.000000 nbresult-0.0.9/img/subdir_demo.png
--rw-r--r--   0 gmanchon   (501) staff       (20)    50804 2021-09-06 12:08:58.000000 nbresult-0.0.9/img/variable.png
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.126839 nbresult-0.0.9/nbresult/
--rw-r--r--   0 gmanchon   (501) staff       (20)     3546 2022-11-21 16:19:47.000000 nbresult-0.0.9/nbresult/__init__.py
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.127335 nbresult-0.0.9/nbresult.egg-info/
--rw-r--r--   0 gmanchon   (501) staff       (20)     2631 2022-11-21 16:41:37.000000 nbresult-0.0.9/nbresult.egg-info/PKG-INFO
--rw-r--r--   0 gmanchon   (501) staff       (20)      837 2022-11-21 16:41:37.000000 nbresult-0.0.9/nbresult.egg-info/SOURCES.txt
--rw-r--r--   0 gmanchon   (501) staff       (20)        1 2022-11-21 16:41:37.000000 nbresult-0.0.9/nbresult.egg-info/dependency_links.txt
--rw-r--r--   0 gmanchon   (501) staff       (20)        9 2022-11-21 16:41:37.000000 nbresult-0.0.9/nbresult.egg-info/top_level.txt
--rw-r--r--   0 gmanchon   (501) staff       (20)        1 2022-11-17 14:40:46.000000 nbresult-0.0.9/requirements.txt
--rw-r--r--   0 gmanchon   (501) staff       (20)       38 2022-11-21 16:41:37.128843 nbresult-0.0.9/setup.cfg
--rw-r--r--   0 gmanchon   (501) staff       (20)      579 2022-11-21 16:19:47.000000 nbresult-0.0.9/setup.py
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.127505 nbresult-0.0.9/tests/
--rw-r--r--   0 gmanchon   (501) staff       (20)        0 2022-11-17 14:40:46.000000 nbresult-0.0.9/tests/__init__.py
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.120842 nbresult-0.0.9/tests/fixtures/
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.120677 nbresult-0.0.9/tests/fixtures/package_challenge/
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.127733 nbresult-0.0.9/tests/fixtures/package_challenge/toto/
--rw-r--r--   0 gmanchon   (501) staff       (20)      121 2022-11-17 14:40:46.000000 nbresult-0.0.9/tests/fixtures/package_challenge/toto/handler.py
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.127946 nbresult-0.0.9/tests/fixtures/package_challenge/toto/tests/
--rw-r--r--   0 gmanchon   (501) staff       (20)        0 2022-11-17 14:40:46.000000 nbresult-0.0.9/tests/fixtures/package_challenge/toto/tests/__init__.py
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.128108 nbresult-0.0.9/tests/fixtures/package_challenge/toto/tests/first_tests/
--rw-r--r--   0 gmanchon   (501) staff       (20)        0 2022-11-17 14:40:46.000000 nbresult-0.0.9/tests/fixtures/package_challenge/toto/tests/first_tests/__init__.py
--rw-r--r--   0 gmanchon   (501) staff       (20)      164 2022-11-17 14:40:46.000000 nbresult-0.0.9/tests/fixtures/package_challenge/toto/tests/first_tests/test_unicity.py
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.128318 nbresult-0.0.9/tests/fixtures/simple_challenge_directory/
--rw-r--r--   0 gmanchon   (501) staff       (20)        1 2022-11-17 14:40:46.000000 nbresult-0.0.9/tests/fixtures/simple_challenge_directory/challenge.py
-drwxr-xr-x   0 gmanchon   (501) staff       (20)        0 2022-11-21 16:41:37.128540 nbresult-0.0.9/tests/fixtures/simple_challenge_directory/tests/
--rw-r--r--   0 gmanchon   (501) staff       (20)        0 2022-11-17 14:40:46.000000 nbresult-0.0.9/tests/fixtures/simple_challenge_directory/tests/__init__.py
--rw-r--r--   0 gmanchon   (501) staff       (20)      166 2022-11-17 14:40:46.000000 nbresult-0.0.9/tests/fixtures/simple_challenge_directory/tests/test_unicity.py
--rw-r--r--   0 gmanchon   (501) staff       (20)     4399 2022-11-21 16:19:47.000000 nbresult-0.0.9/tests/test_challenge_result.py
+drwxr-xr-x   0 seb        (501) staff       (20)        0 2024-04-04 07:59:30.037471 nbresult-0.1.0/
+-rw-r--r--   0 seb        (501) staff       (20)     1065 2020-12-18 09:40:42.000000 nbresult-0.1.0/LICENSE
+-rw-r--r--   0 seb        (501) staff       (20)        1 2024-04-04 07:31:21.000000 nbresult-0.1.0/MANIFEST.in
+-rw-r--r--   0 seb        (501) staff       (20)     3704 2024-04-04 07:59:30.037068 nbresult-0.1.0/PKG-INFO
+-rw-r--r--   0 seb        (501) staff       (20)     2355 2024-04-04 07:31:21.000000 nbresult-0.1.0/README.md
+drwxr-xr-x   0 seb        (501) staff       (20)        0 2024-04-04 07:59:30.035316 nbresult-0.1.0/nbresult/
+-rw-r--r--   0 seb        (501) staff       (20)     3551 2024-04-04 07:56:15.000000 nbresult-0.1.0/nbresult/__init__.py
+drwxr-xr-x   0 seb        (501) staff       (20)        0 2024-04-04 07:59:30.036560 nbresult-0.1.0/nbresult.egg-info/
+-rw-r--r--   0 seb        (501) staff       (20)     3704 2024-04-04 07:59:29.000000 nbresult-0.1.0/nbresult.egg-info/PKG-INFO
+-rw-r--r--   0 seb        (501) staff       (20)      187 2024-04-04 07:59:30.000000 nbresult-0.1.0/nbresult.egg-info/SOURCES.txt
+-rw-r--r--   0 seb        (501) staff       (20)        1 2024-04-04 07:59:29.000000 nbresult-0.1.0/nbresult.egg-info/dependency_links.txt
+-rw-r--r--   0 seb        (501) staff       (20)        9 2024-04-04 07:59:29.000000 nbresult-0.1.0/nbresult.egg-info/top_level.txt
+-rw-r--r--   0 seb        (501) staff       (20)       38 2024-04-04 07:59:30.037571 nbresult-0.1.0/setup.cfg
+-rw-r--r--   0 seb        (501) staff       (20)      579 2024-04-04 07:59:05.000000 nbresult-0.1.0/setup.py
```

### Comparing `nbresult-0.0.9/LICENSE` & `nbresult-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbresult-0.0.9/PKG-INFO` & `nbresult-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: nbresult
-Version: 0.0.9
-Summary: Extract results from Jupyter notebooks
-Home-page: https://github.com/lewagon/nbresult
-Author: Kevin Robert
-Author-email: kevin@lewagon.org
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nbresult
 
 A simple package to test Jupyter notebook result for the Le Wagon's Data Science Bootcamp.
 
 ## 1. Installation
 
 Installation with `pip` from [Pypi](https://pypi.org/):
```

### Comparing `nbresult-0.0.9/nbresult/__init__.py` & `nbresult-0.1.0/nbresult/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         with open(result_file, 'wb') as file:
             pickle.dump(self, file)
 
     def check(self):
         """returns test output on the ChallengeResult"""
         tests_path = self._locate_tests()
         file_path = f"test_{self.name}.py"
-        command = ["python3", "-m", "pytest", "-v", "--color=yes", file_path]
+        command = [sys.executable, "-m", "pytest", "-v", "--color=yes", file_path]
         sub_process = subprocess.Popen(command,
                              cwd=tests_path, # set current working directory
                              stdin=subprocess.PIPE,
                              stdout=subprocess.PIPE,
                              stderr=subprocess.PIPE)
         output, error = sub_process.communicate(b"")  # binary input passed as parameter
         result = output.decode("utf-8")
```

### Comparing `nbresult-0.0.9/setup.py` & `nbresult-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='nbresult',
-      version='0.0.9',
+      version='0.1.0',
       description='Extract results from Jupyter notebooks',
       license="MIT",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/lewagon/nbresult",
       author='Kevin Robert',
       author_email='kevin@lewagon.org',
```

