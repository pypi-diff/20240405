# Comparing `tmp/backend.ai-accelerator-cuda-open-24.3.0rc2.tar.gz` & `tmp/backend.ai-accelerator-cuda-open-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-accelerator-cuda-open-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:09 2024, max compression
+gzip compressed data, was "backend.ai-accelerator-cuda-open-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:38 2024, max compression
```

## Comparing `backend.ai-accelerator-cuda-open-24.3.0rc2.tar` & `backend.ai-accelerator-cuda-open-24.3.0rc3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:09.807427 backend.ai-accelerator-cuda-open-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:08.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-31 14:09:09.807427 backend.ai-accelerator-cuda-open-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:09.803427 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:09.803427 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:09.803427 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:09.803427 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/cuda_open/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:08.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/cuda_open/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 14:09:08.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/cuda_open/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-03-31 14:09:08.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/cuda_open/nvidia.py
--rw-r--r--   0 runner    (1001) docker     (127)    14990 2024-03-31 14:09:08.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/cuda_open/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 14:09:08.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/cuda_open/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:09.807427 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-31 14:09:09.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-31 14:09:09.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:09.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-31 14:09:09.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:09.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:09.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-31 14:09:09.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:09.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:08.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:09.807427 backend.ai-accelerator-cuda-open-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-03-31 14:09:08.000000 backend.ai-accelerator-cuda-open-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.322052 backend.ai-accelerator-cuda-open-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:37.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-05 02:25:38.322052 backend.ai-accelerator-cuda-open-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.314051 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.314051 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.314051 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.318052 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/cuda_open/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:37.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/cuda_open/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:37.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/cuda_open/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-04-05 02:25:37.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/cuda_open/nvidia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14990 2024-04-05 02:25:37.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/cuda_open/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 02:25:37.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/cuda_open/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.318052 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-05 02:25:38.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-05 02:25:38.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:38.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 02:25:38.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:38.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:38.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 02:25:38.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:38.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:37.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:38.322052 backend.ai-accelerator-cuda-open-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-05 02:25:37.000000 backend.ai-accelerator-cuda-open-24.3.0rc3/setup.py
```

### Comparing `backend.ai-accelerator-cuda-open-24.3.0rc2/PKG-INFO` & `backend.ai-accelerator-cuda-open-24.3.0rc3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-cuda-open
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Accelerator Plugin for CUDA
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,26 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
+Requires-Dist: aiodocker~=0.21.0
+Requires-Dist: aiotools~=1.7.0
+Requires-Dist: backend.ai-agent==24.03.0rc3
+Requires-Dist: backend.ai-cli==24.03.0rc3
+Requires-Dist: backend.ai-common==24.03.0rc3
+Requires-Dist: backend.ai-kernel-binary==24.03.0rc3
+Requires-Dist: backend.ai-kernel-helper==24.03.0rc3
+Requires-Dist: backend.ai-plugin==24.03.0rc3
 
 Backend.AI Accelerator Plugin for CUDA
 ======================================
 
 Just install this along with Backend.AI agents, using the same virtual environment.
 This will allow the agents to detect CUDA devices on their hosts and make them
 available to Backend.AI kernel sessions.
```

### Comparing `backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/cuda_open/nvidia.py` & `backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/cuda_open/nvidia.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-open-24.3.0rc2/ai/backend/accelerator/cuda_open/plugin.py` & `backend.ai-accelerator-cuda-open-24.3.0rc3/ai/backend/accelerator/cuda_open/plugin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/PKG-INFO` & `backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-cuda-open
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Accelerator Plugin for CUDA
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,26 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
+Requires-Dist: aiodocker~=0.21.0
+Requires-Dist: aiotools~=1.7.0
+Requires-Dist: backend.ai-agent==24.03.0rc3
+Requires-Dist: backend.ai-cli==24.03.0rc3
+Requires-Dist: backend.ai-common==24.03.0rc3
+Requires-Dist: backend.ai-kernel-binary==24.03.0rc3
+Requires-Dist: backend.ai-kernel-helper==24.03.0rc3
+Requires-Dist: backend.ai-plugin==24.03.0rc3
 
 Backend.AI Accelerator Plugin for CUDA
 ======================================
 
 Just install this along with Backend.AI agents, using the same virtual environment.
 This will allow the agents to detect CUDA devices on their hosts and make them
 available to Backend.AI kernel sessions.
```

### Comparing `backend.ai-accelerator-cuda-open-24.3.0rc2/backend.ai_accelerator_cuda_open.egg-info/SOURCES.txt` & `backend.ai-accelerator-cuda-open-24.3.0rc3/backend.ai_accelerator_cuda_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-open-24.3.0rc2/backend_shim.py` & `backend.ai-accelerator-cuda-open-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-open-24.3.0rc2/setup.py` & `backend.ai-accelerator-cuda-open-24.3.0rc3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,37 +12,37 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Accelerator Plugin for CUDA',
     'entry_points': {
         'backendai_accelerator_v21': [
             'cuda = ai.backend.accelerator.cuda_open.plugin:CUDAPlugin',
         ],
     },
     'install_requires': (
         'aiodocker~=0.21.0',
         'aiotools~=1.7.0',
-        """backend.ai-agent==24.03.0rc2
+        """backend.ai-agent==24.03.0rc3
 """,
-        """backend.ai-cli==24.03.0rc2
+        """backend.ai-cli==24.03.0rc3
 """,
-        """backend.ai-common==24.03.0rc2
+        """backend.ai-common==24.03.0rc3
 """,
-        """backend.ai-kernel-binary==24.03.0rc2
+        """backend.ai-kernel-binary==24.03.0rc3
 """,
-        """backend.ai-kernel-helper==24.03.0rc2
+        """backend.ai-kernel-helper==24.03.0rc3
 """,
-        """backend.ai-plugin==24.03.0rc2
+        """backend.ai-plugin==24.03.0rc3
 """,
     ),
     'license': 'LGPLv3',
     'long_description': """Backend.AI Accelerator Plugin for CUDA
 ======================================
 
 Just install this along with Backend.AI agents, using the same virtual environment.
@@ -84,13 +84,13 @@
     'packages': (
         'ai.backend.accelerator.cuda_open',
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

