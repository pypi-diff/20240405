# Comparing `tmp/enum_with_dict-0.7.1.tar.gz` & `tmp/enum_with_dict-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.7.1.tar", last modified: Thu Apr  4 11:07:21 2024, max compression
+gzip compressed data, was "enum_with_dict-0.7.2.tar", last modified: Fri Apr  5 17:15:47 2024, max compression
```

## Comparing `enum_with_dict-0.7.1.tar` & `enum_with_dict-0.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 11:07:21.927370 enum_with_dict-0.7.1/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.7.1/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     5589 2024-04-04 11:07:21.927124 enum_with_dict-0.7.1/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     4675 2024-04-04 10:45:17.000000 enum_with_dict-0.7.1/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 11:07:21.926004 enum_with_dict-0.7.1/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.7.1/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     6533 2024-04-04 11:07:13.000000 enum_with_dict-0.7.1/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 11:07:21.926570 enum_with_dict-0.7.1/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     5589 2024-04-04 11:07:21.000000 enum_with_dict-0.7.1/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 11:07:21.000000 enum_with_dict-0.7.1/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 11:07:21.000000 enum_with_dict-0.7.1/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 11:07:21.000000 enum_with_dict-0.7.1/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 11:07:21.927416 enum_with_dict-0.7.1/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 11:07:13.000000 enum_with_dict-0.7.1/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 11:07:21.926794 enum_with_dict-0.7.1/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.7.1/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     8057 2024-04-04 11:07:13.000000 enum_with_dict-0.7.1/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-05 17:15:47.034503 enum_with_dict-0.7.2/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.7.2/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     5640 2024-04-05 17:15:47.034295 enum_with_dict-0.7.2/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     4675 2024-04-04 10:45:17.000000 enum_with_dict-0.7.2/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-05 17:15:47.033251 enum_with_dict-0.7.2/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.7.2/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     6533 2024-04-04 11:07:13.000000 enum_with_dict-0.7.2/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-05 17:15:47.033742 enum_with_dict-0.7.2/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     5640 2024-04-05 17:15:47.000000 enum_with_dict-0.7.2/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-05 17:15:47.000000 enum_with_dict-0.7.2/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-05 17:15:47.000000 enum_with_dict-0.7.2/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-05 17:15:47.000000 enum_with_dict-0.7.2/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-05 17:15:47.034540 enum_with_dict-0.7.2/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1127 2024-04-05 17:14:51.000000 enum_with_dict-0.7.2/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-05 17:15:47.033966 enum_with_dict-0.7.2/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.7.2/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     8057 2024-04-04 11:07:13.000000 enum_with_dict-0.7.2/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.7.1/LICENSE` & `enum_with_dict-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.7.1/PKG-INFO` & `enum_with_dict-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.7.1
+Version: 0.7.2
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py-enum-with-dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EnumWithDict
```

### Comparing `enum_with_dict-0.7.1/README.md` & `enum_with_dict-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.7.1/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.7.2/enum_with_dict/enum_with_dict.py`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.7.1/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.7.2/enum_with_dict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.7.1
+Version: 0.7.2
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py-enum-with-dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EnumWithDict
```

### Comparing `enum_with_dict-0.7.1/setup.py` & `enum_with_dict-0.7.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.7.1',
+    version='0.7.2',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/py-enum-with-dict',
@@ -18,12 +18,13 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7',
     keywords='enum python utilities enum-to-dict enum-with-dict',
 )
```

### Comparing `enum_with_dict-0.7.1/test/test_enum_with_dict.py` & `enum_with_dict-0.7.2/test/test_enum_with_dict.py`

 * *Files identical despite different names*

