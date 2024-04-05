# Comparing `tmp/backend.ai-test-24.3.0rc3.tar.gz` & `tmp/backend.ai-test-24.3.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-test-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:36 2024, max compression
+gzip compressed data, was "backend.ai-test-24.3.0rc4.tar", last modified: Fri Apr  5 03:40:04 2024, max compression
```

## Comparing `backend.ai-test-24.3.0rc3.tar` & `backend.ai-test-24.3.0rc4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.694037 backend.ai-test-24.3.0rc3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.694037 backend.ai-test-24.3.0rc3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.694037 backend.ai-test-24.3.0rc3/ai/backend/test/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/ai/backend/test/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.173375 backend.ai-test-24.3.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-05 03:40:04.173375 backend.ai-test-24.3.0rc4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.169375 backend.ai-test-24.3.0rc4/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.169375 backend.ai-test-24.3.0rc4/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.169375 backend.ai-test-24.3.0rc4/ai/backend/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/ai/backend/test/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/ai/backend/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.173375 backend.ai-test-24.3.0rc4/ai/backend/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/ai/backend/test/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/ai/backend/test/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/ai/backend/test/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/ai/backend/test/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/ai/backend/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:04.173375 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-05 03:40:04.000000 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:40:04.173375 backend.ai-test-24.3.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-05 03:40:03.000000 backend.ai-test-24.3.0rc4/setup.py
```

### Comparing `backend.ai-test-24.3.0rc3/PKG-INFO` & `backend.ai-test-24.3.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 24.3.0rc3
+Version: 24.3.0rc4
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-test-24.3.0rc3/ai/backend/test/cli/__main__.py` & `backend.ai-test-24.3.0rc4/ai/backend/test/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-24.3.0rc3/ai/backend/test/cli/utils.py` & `backend.ai-test-24.3.0rc4/ai/backend/test/cli/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/PKG-INFO` & `backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 24.3.0rc3
+Version: 24.3.0rc4
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/SOURCES.txt` & `backend.ai-test-24.3.0rc4/backend.ai_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-test-24.3.0rc3/backend_shim.py` & `backend.ai-test-24.3.0rc4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-24.3.0rc3/setup.py` & `backend.ai-test-24.3.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,11 +65,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc3
+    'version': """24.03.0rc4
 """,
     'zip_safe': False,
 })
```

