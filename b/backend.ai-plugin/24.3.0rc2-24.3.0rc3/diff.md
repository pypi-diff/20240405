# Comparing `tmp/backend.ai-plugin-24.3.0rc2.tar.gz` & `tmp/backend.ai-plugin-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-plugin-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:11 2024, max compression
+gzip compressed data, was "backend.ai-plugin-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:37 2024, max compression
```

## Comparing `backend.ai-plugin-24.3.0rc2.tar` & `backend.ai-plugin-24.3.0rc3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.239447 backend.ai-plugin-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:10.000000 backend.ai-plugin-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-31 14:09:11.239447 backend.ai-plugin-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.235447 backend.ai-plugin-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.239447 backend.ai-plugin-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.239447 backend.ai-plugin-24.3.0rc2/ai/backend/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:10.000000 backend.ai-plugin-24.3.0rc2/ai/backend/plugin/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 14:09:10.000000 backend.ai-plugin-24.3.0rc2/ai/backend/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-03-31 14:09:10.000000 backend.ai-plugin-24.3.0rc2/ai/backend/plugin/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:10.000000 backend.ai-plugin-24.3.0rc2/ai/backend/plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.239447 backend.ai-plugin-24.3.0rc2/backend.ai_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-31 14:09:11.000000 backend.ai-plugin-24.3.0rc2/backend.ai_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-31 14:09:11.000000 backend.ai-plugin-24.3.0rc2/backend.ai_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-plugin-24.3.0rc2/backend.ai_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-plugin-24.3.0rc2/backend.ai_plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-plugin-24.3.0rc2/backend.ai_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:11.000000 backend.ai-plugin-24.3.0rc2/backend.ai_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:10.000000 backend.ai-plugin-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:11.239447 backend.ai-plugin-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-31 14:09:10.000000 backend.ai-plugin-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.118040 backend.ai-plugin-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:36.000000 backend.ai-plugin-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 02:25:37.118040 backend.ai-plugin-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.114040 backend.ai-plugin-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.114040 backend.ai-plugin-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.118040 backend.ai-plugin-24.3.0rc3/ai/backend/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:36.000000 backend.ai-plugin-24.3.0rc3/ai/backend/plugin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:36.000000 backend.ai-plugin-24.3.0rc3/ai/backend/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-05 02:25:36.000000 backend.ai-plugin-24.3.0rc3/ai/backend/plugin/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:36.000000 backend.ai-plugin-24.3.0rc3/ai/backend/plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.118040 backend.ai-plugin-24.3.0rc3/backend.ai_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 02:25:37.000000 backend.ai-plugin-24.3.0rc3/backend.ai_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 02:25:37.000000 backend.ai-plugin-24.3.0rc3/backend.ai_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-plugin-24.3.0rc3/backend.ai_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-plugin-24.3.0rc3/backend.ai_plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-plugin-24.3.0rc3/backend.ai_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:37.000000 backend.ai-plugin-24.3.0rc3/backend.ai_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:36.000000 backend.ai-plugin-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:37.118040 backend.ai-plugin-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-05 02:25:36.000000 backend.ai-plugin-24.3.0rc3/setup.py
```

### Comparing `backend.ai-plugin-24.3.0rc2/PKG-INFO` & `backend.ai-plugin-24.3.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,17 +12,17 @@
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
 
 Backend.AI Plugin Subsystem
 ===========================
 
 Package Structure
 -----------------
```

### Comparing `backend.ai-plugin-24.3.0rc2/ai/backend/plugin/entrypoint.py` & `backend.ai-plugin-24.3.0rc3/ai/backend/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-24.3.0rc2/backend.ai_plugin.egg-info/PKG-INFO` & `backend.ai-plugin-24.3.0rc3/backend.ai_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,17 +12,17 @@
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
 
 Backend.AI Plugin Subsystem
 ===========================
 
 Package Structure
 -----------------
```

### Comparing `backend.ai-plugin-24.3.0rc2/backend_shim.py` & `backend.ai-plugin-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-24.3.0rc2/setup.py` & `backend.ai-plugin-24.3.0rc3/setup.py`

 * *Files 2% similar despite different names*

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
     'description': 'Backend.AI Plugin Subsystem',
     'install_requires': (
     ),
     'license': 'MIT',
     'long_description': """Backend.AI Plugin Subsystem
@@ -44,13 +44,13 @@
     'packages': (
         'ai.backend.plugin',
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

