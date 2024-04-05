# Comparing `tmp/backend.ai-test-24.3.0rc2.tar.gz` & `tmp/backend.ai-test-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-test-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:10 2024, max compression
+gzip compressed data, was "backend.ai-test-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:36 2024, max compression
```

## Comparing `backend.ai-test-24.3.0rc2.tar` & `backend.ai-test-24.3.0rc3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.847441 backend.ai-test-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-31 14:09:10.847441 backend.ai-test-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.847441 backend.ai-test-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.847441 backend.ai-test-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.847441 backend.ai-test-24.3.0rc2/ai/backend/test/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/ai/backend/test/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/ai/backend/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.847441 backend.ai-test-24.3.0rc2/ai/backend/test/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/ai/backend/test/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/ai/backend/test/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/ai/backend/test/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/ai/backend/test/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/ai/backend/test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.847441 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:10.847441 backend.ai-test-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-31 14:09:10.000000 backend.ai-test-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.694037 backend.ai-test-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.694037 backend.ai-test-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.694037 backend.ai-test-24.3.0rc3/ai/backend/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/ai/backend/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/ai/backend/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:36.698037 backend.ai-test-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-05 02:25:36.000000 backend.ai-test-24.3.0rc3/setup.py
```

### Comparing `backend.ai-test-24.3.0rc2/PKG-INFO` & `backend.ai-test-24.3.0rc3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,23 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
+Requires-Dist: attrs>=20.3
+Requires-Dist: click~=8.1.7
+Requires-Dist: pytest-dependency>=0.5.1
+Requires-Dist: pytest>=7.3.1
+Requires-Dist: types-setuptools
 
 # Backend.AI Testing Toolkit
 
 Automated test suites to validate an installation and integration of clients and servers
 
 
 ## How to run CLI-based integration test
```

### Comparing `backend.ai-test-24.3.0rc2/ai/backend/test/cli/__main__.py` & `backend.ai-test-24.3.0rc3/ai/backend/test/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-24.3.0rc2/ai/backend/test/cli/utils.py` & `backend.ai-test-24.3.0rc3/ai/backend/test/cli/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/PKG-INFO` & `backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,23 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
+Requires-Dist: attrs>=20.3
+Requires-Dist: click~=8.1.7
+Requires-Dist: pytest-dependency>=0.5.1
+Requires-Dist: pytest>=7.3.1
+Requires-Dist: types-setuptools
 
 # Backend.AI Testing Toolkit
 
 Automated test suites to validate an installation and integration of clients and servers
 
 
 ## How to run CLI-based integration test
```

### Comparing `backend.ai-test-24.3.0rc2/backend.ai_test.egg-info/SOURCES.txt` & `backend.ai-test-24.3.0rc3/backend.ai_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-test-24.3.0rc2/backend_shim.py` & `backend.ai-test-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-24.3.0rc2/setup.py` & `backend.ai-test-24.3.0rc3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: MIT License',
     ],
     'description': 'Backend.AI Integration Test Suite',
     'entry_points': {
         'backendai_cli_v10': [
             'test = ai.backend.test.cli.__main__:main',
         ],
@@ -63,13 +63,13 @@
         'ai.backend.test',
         'ai.backend.test.cli',
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
-    'python_requires': '>=3.11,<3.12',
+    'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc2
+    'version': """24.03.0rc3
 """,
     'zip_safe': False,
 })
```

