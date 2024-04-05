# Comparing `tmp/backend.ai-cli-24.3.0rc2.tar.gz` & `tmp/backend.ai-cli-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-cli-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:12 2024, max compression
+gzip compressed data, was "backend.ai-cli-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:37 2024, max compression
```

## Comparing `backend.ai-cli-24.3.0rc2.tar` & `backend.ai-cli-24.3.0rc3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.359462 backend.ai-cli-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-31 14:09:12.359462 backend.ai-cli-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.355462 backend.ai-cli-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.355462 backend.ai-cli-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.359462 backend.ai-cli-24.3.0rc2/ai/backend/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/ai/backend/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.359462 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-31 14:09:12.000000 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-31 14:09:12.000000 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:12.000000 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-31 14:09:12.000000 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:12.000000 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:12.000000 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-31 14:09:12.000000 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:12.000000 backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:12.359462 backend.ai-cli-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-31 14:09:11.000000 backend.ai-cli-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.862047 backend.ai-cli-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-05 02:25:37.862047 backend.ai-cli-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.858047 backend.ai-cli-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.858047 backend.ai-cli-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.862047 backend.ai-cli-24.3.0rc3/ai/backend/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/ai/backend/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.862047 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:37.862047 backend.ai-cli-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-05 02:25:37.000000 backend.ai-cli-24.3.0rc3/setup.py
```

### Comparing `backend.ai-cli-24.3.0rc2/PKG-INFO` & `backend.ai-cli-24.3.0rc3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-cli
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Command Line Interface Helper
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,22 @@
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
+Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: click~=8.1.7
+Requires-Dist: trafaret~=2.1
 
 # backend.ai-cli
 
 Unified command-line interface for Backend.AI
 
 
 ## How to adopt in CLI-enabled Backend.AI packages
```

### Comparing `backend.ai-cli-24.3.0rc2/ai/backend/cli/extensions.py` & `backend.ai-cli-24.3.0rc3/ai/backend/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-24.3.0rc2/ai/backend/cli/interaction.py` & `backend.ai-cli-24.3.0rc3/ai/backend/cli/interaction.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-24.3.0rc2/ai/backend/cli/loader.py` & `backend.ai-cli-24.3.0rc3/ai/backend/cli/loader.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-24.3.0rc2/ai/backend/cli/main.py` & `backend.ai-cli-24.3.0rc3/ai/backend/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-24.3.0rc2/ai/backend/cli/params.py` & `backend.ai-cli-24.3.0rc3/ai/backend/cli/params.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-24.3.0rc2/ai/backend/cli/types.py` & `backend.ai-cli-24.3.0rc3/ai/backend/cli/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/PKG-INFO` & `backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-cli
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Command Line Interface Helper
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,22 @@
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
+Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: click~=8.1.7
+Requires-Dist: trafaret~=2.1
 
 # backend.ai-cli
 
 Unified command-line interface for Backend.AI
 
 
 ## How to adopt in CLI-enabled Backend.AI packages
```

### Comparing `backend.ai-cli-24.3.0rc2/backend.ai_cli.egg-info/SOURCES.txt` & `backend.ai-cli-24.3.0rc3/backend.ai_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-24.3.0rc2/backend_shim.py` & `backend.ai-cli-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-24.3.0rc2/setup.py` & `backend.ai-cli-24.3.0rc3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,26 @@
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
     'description': 'Backend.AI Command Line Interface Helper',
     'entry_points': {
         'console_scripts': [
             'backend.ai = ai.backend.cli.__main__:main',
         ],
     },
     'install_requires': (
         'attrs>=20.3',
-        """backend.ai-plugin==24.03.0rc2
+        """backend.ai-plugin==24.03.0rc3
 """,
         'click~=8.1.7',
         'trafaret~=2.1',
     ),
     'license': 'MIT',
     'long_description': """# backend.ai-cli
 
@@ -70,13 +70,13 @@
     'packages': (
         'ai.backend.cli',
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

