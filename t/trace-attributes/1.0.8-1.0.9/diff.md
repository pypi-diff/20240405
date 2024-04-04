# Comparing `tmp/trace-attributes-1.0.8.tar.gz` & `tmp/trace-attributes-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trace-attributes-1.0.8.tar", last modified: Thu Feb 15 07:32:48 2024, max compression
+gzip compressed data, was "trace-attributes-1.0.9.tar", last modified: Thu Feb 15 18:38:48 2024, max compression
```

## Comparing `trace-attributes-1.0.8.tar` & `trace-attributes-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 07:32:48.380923 trace-attributes-1.0.8/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     1068 2024-02-15 00:23:08.000000 trace-attributes-1.0.8/LICENSE
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      494 2024-02-15 07:32:48.380791 trace-attributes-1.0.8/PKG-INFO
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     6591 2024-02-15 01:50:48.000000 trace-attributes-1.0.8/README.md
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       38 2024-02-15 07:32:48.380972 trace-attributes-1.0.8/setup.cfg
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      960 2024-02-15 07:32:17.000000 trace-attributes-1.0.8/setup.py
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 07:32:48.378571 trace-attributes-1.0.8/src/
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 07:32:48.378807 trace-attributes-1.0.8/src/python/
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 07:32:48.379349 trace-attributes-1.0.8/src/python/langtrace/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       13 2024-02-15 01:53:26.000000 trace-attributes-1.0.8/src/python/langtrace/__init__.py
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 07:32:48.379590 trace-attributes-1.0.8/src/python/langtrace/trace_attributes/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      293 2024-02-15 02:34:55.000000 trace-attributes-1.0.8/src/python/langtrace/trace_attributes/__init__.py
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 07:32:48.380070 trace-attributes-1.0.8/src/python/langtrace/trace_attributes/models/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       13 2024-02-15 01:53:13.000000 trace-attributes-1.0.8/src/python/langtrace/trace_attributes/models/__init__.py
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      305 2024-02-14 23:14:51.000000 trace-attributes-1.0.8/src/python/langtrace/trace_attributes/models/langtrace_span_attributes.py
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     1251 2024-02-15 07:27:58.000000 trace-attributes-1.0.8/src/python/langtrace/trace_attributes/models/openai_span_attributes.py
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      457 2024-02-15 07:27:52.000000 trace-attributes-1.0.8/src/python/langtrace/trace_attributes/models/openai_span_events.py
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      442 2024-02-15 00:23:08.000000 trace-attributes-1.0.8/src/python/langtrace/trace_attributes/module.py
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 07:32:48.380608 trace-attributes-1.0.8/src/python/trace_attributes.egg-info/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      494 2024-02-15 07:32:48.000000 trace-attributes-1.0.8/src/python/trace_attributes.egg-info/PKG-INFO
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      680 2024-02-15 07:32:48.000000 trace-attributes-1.0.8/src/python/trace_attributes.egg-info/SOURCES.txt
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)        1 2024-02-15 07:32:48.000000 trace-attributes-1.0.8/src/python/trace_attributes.egg-info/dependency_links.txt
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       21 2024-02-15 07:32:48.000000 trace-attributes-1.0.8/src/python/trace_attributes.egg-info/requires.txt
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       10 2024-02-15 07:32:48.000000 trace-attributes-1.0.8/src/python/trace_attributes.egg-info/top_level.txt
+drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.225161 trace-attributes-1.0.9/
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     1068 2024-02-15 00:23:08.000000 trace-attributes-1.0.9/LICENSE
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      494 2024-02-15 18:38:48.225045 trace-attributes-1.0.9/PKG-INFO
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     6591 2024-02-15 01:50:48.000000 trace-attributes-1.0.9/README.md
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       38 2024-02-15 18:38:48.225211 trace-attributes-1.0.9/setup.cfg
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      960 2024-02-15 18:38:36.000000 trace-attributes-1.0.9/setup.py
+drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.222703 trace-attributes-1.0.9/src/
+drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.222947 trace-attributes-1.0.9/src/python/
+drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.223592 trace-attributes-1.0.9/src/python/langtrace/
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       13 2024-02-15 01:53:26.000000 trace-attributes-1.0.9/src/python/langtrace/__init__.py
+drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.223921 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      293 2024-02-15 07:33:15.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/__init__.py
+drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.224294 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       13 2024-02-15 01:53:13.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/__init__.py
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      305 2024-02-14 23:14:51.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/langtrace_span_attributes.py
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     1251 2024-02-15 07:27:58.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/openai_span_attributes.py
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      442 2024-02-15 00:23:08.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/module.py
+drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.224881 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      494 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/PKG-INFO
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      613 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)        1 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       21 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/requires.txt
+-rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       10 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/top_level.txt
```

### Comparing `trace-attributes-1.0.8/LICENSE` & `trace-attributes-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trace-attributes-1.0.8/README.md` & `trace-attributes-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `trace-attributes-1.0.8/setup.py` & `trace-attributes-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='trace-attributes',  # Choose a unique name for PyPI
-    version='1.0.8',
+    version='1.0.9',
     author='Karthik Kalyanaraman',
     author_email='karthik@scale3labs.com',
     description='LangTrace - Trace Attributes',
     long_description="LangTrace - Trace Attributes",
     long_description_content_type='text/markdown',
     url='https://github.com/Scale3-Labs/langtrace-trace-attributes',  # Project home page
     package_dir={'': 'src/python'},
```

### Comparing `trace-attributes-1.0.8/src/python/langtrace/trace_attributes/models/openai_span_attributes.py` & `trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/openai_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace-attributes-1.0.8/src/python/trace_attributes.egg-info/SOURCES.txt` & `trace-attributes-1.0.9/src/python/trace_attributes.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,13 +3,12 @@
 setup.py
 src/python/langtrace/__init__.py
 src/python/langtrace/trace_attributes/__init__.py
 src/python/langtrace/trace_attributes/module.py
 src/python/langtrace/trace_attributes/models/__init__.py
 src/python/langtrace/trace_attributes/models/langtrace_span_attributes.py
 src/python/langtrace/trace_attributes/models/openai_span_attributes.py
-src/python/langtrace/trace_attributes/models/openai_span_events.py
 src/python/trace_attributes.egg-info/PKG-INFO
 src/python/trace_attributes.egg-info/SOURCES.txt
 src/python/trace_attributes.egg-info/dependency_links.txt
 src/python/trace_attributes.egg-info/requires.txt
 src/python/trace_attributes.egg-info/top_level.txt
```

