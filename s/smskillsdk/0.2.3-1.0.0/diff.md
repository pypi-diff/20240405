# Comparing `tmp/smskillsdk-0.2.3.tar.gz` & `tmp/smskillsdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smskillsdk-0.2.3.tar", last modified: Tue Jun  7 00:03:59 2022, max compression
+gzip compressed data, was "smskillsdk-1.0.0.tar", last modified: Fri Apr  5 14:29:34 2024, max compression
```

## Comparing `smskillsdk-0.2.3.tar` & `smskillsdk-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.593738 smskillsdk-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.589738 smskillsdk-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.589738 smskillsdk-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8933 2022-06-07 00:03:59.593738 smskillsdk-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8178 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.589738 smskillsdk-0.2.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/scripts/build.ps1
--rwxr-xr-x   0 runner    (1001) docker     (121)       43 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/scripts/build.sh
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/scripts/generate_models.ps1
--rwxr-xr-x   0 runner    (1001) docker     (121)      174 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/scripts/generate_models.sh
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/scripts/run_tests.ps1
--rwxr-xr-x   0 runner    (1001) docker     (121)       46 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/scripts/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-06-07 00:03:59.593738 smskillsdk-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.589738 smskillsdk-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.589738 smskillsdk-0.2.3/src/smskillsdk/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/src/smskillsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.593738 smskillsdk-0.2.3/src/smskillsdk/models/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/src/smskillsdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6068 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/src/smskillsdk/models/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.593738 smskillsdk-0.2.3/src/smskillsdk/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/src/smskillsdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/src/smskillsdk/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3486 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/src/smskillsdk/utils/memory_values.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.593738 smskillsdk-0.2.3/src/smskillsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8933 2022-06-07 00:03:59.000000 smskillsdk-0.2.3/src/smskillsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-06-07 00:03:59.000000 smskillsdk-0.2.3/src/smskillsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 00:03:59.000000 smskillsdk-0.2.3/src/smskillsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 00:03:57.000000 smskillsdk-0.2.3/src/smskillsdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 00:03:59.000000 smskillsdk-0.2.3/src/smskillsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-07 00:03:59.000000 smskillsdk-0.2.3/src/smskillsdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 00:03:59.593738 smskillsdk-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8111 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/tests/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-06-07 00:03:34.000000 smskillsdk-0.2.3/tests/test_memory_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.592486 smskillsdk-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.580486 smskillsdk-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.584486 smskillsdk-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-05 14:29:34.592486 smskillsdk-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.588487 smskillsdk-1.0.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1546 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/scripts/add_license.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/scripts/build.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)       43 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/scripts/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/scripts/generate_models.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/scripts/generate_models.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/scripts/run_tests.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/scripts/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-05 14:29:34.592486 smskillsdk-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.588487 smskillsdk-1.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.588487 smskillsdk-1.0.0/src/smskillsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/smskillsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.588487 smskillsdk-1.0.0/src/smskillsdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/smskillsdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/smskillsdk/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/smskillsdk/models/api_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/smskillsdk/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.592486 smskillsdk-1.0.0/src/smskillsdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/smskillsdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/smskillsdk/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/src/smskillsdk/utils/memory_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.592486 smskillsdk-1.0.0/src/smskillsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-05 14:29:34.000000 smskillsdk-1.0.0/src/smskillsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-05 14:29:34.000000 smskillsdk-1.0.0/src/smskillsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:29:34.000000 smskillsdk-1.0.0/src/smskillsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:29:34.000000 smskillsdk-1.0.0/src/smskillsdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 14:29:34.000000 smskillsdk-1.0.0/src/smskillsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 14:29:34.000000 smskillsdk-1.0.0/src/smskillsdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:29:34.592486 smskillsdk-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-05 14:29:14.000000 smskillsdk-1.0.0/tests/test_memory_values.py
```

### Comparing `smskillsdk-0.2.3/.github/workflows/ci.yml` & `smskillsdk-1.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `smskillsdk-0.2.3/.github/workflows/codeql-analysis.yml` & `smskillsdk-1.0.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `smskillsdk-0.2.3/.github/workflows/release.yml` & `smskillsdk-1.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `smskillsdk-0.2.3/.gitignore` & `smskillsdk-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `smskillsdk-0.2.3/CONTRIBUTING.md` & `smskillsdk-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `smskillsdk-0.2.3/LICENSE` & `smskillsdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smskillsdk-0.2.3/PKG-INFO` & `smskillsdk-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smskillsdk
-Version: 0.2.3
+Version: 1.0.0
 Summary: A Python package to assist with developing services conforming to the Soul Machines Skill REST API.
 Home-page: https://docs.soulmachines.com
 Author: Soul Machines Ltd
 License: Apache 2.0
 Project-URL: Documentation, https://docs.soulmachines.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic>=1.8.2
 
 # smskillsdk (Python)
 
 The Skills Python SDK package contains data types for the session and execute endpoints specified within the Skills REST API, along with a range of utility functions for working with the memory data structure.
 
 ## Installation
```

### Comparing `smskillsdk-0.2.3/README.md` & `smskillsdk-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `smskillsdk-0.2.3/setup.cfg` & `smskillsdk-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smskillsdk
-version = 0.2.3
+version = 1.0.0
 url = https://docs.soulmachines.com
 project_urls = 
 	Documentation = https://docs.soulmachines.com
 author = Soul Machines Ltd
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
```

### Comparing `smskillsdk-0.2.3/src/smskillsdk/__init__.py` & `smskillsdk-1.0.0/src/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Soul Machines Ltd
+# Copyright 2024 Soul Machines Ltd
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `smskillsdk-0.2.3/src/smskillsdk/models/__init__.py` & `smskillsdk-1.0.0/src/smskillsdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Soul Machines Ltd
+# Copyright 2024 Soul Machines Ltd
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `smskillsdk-0.2.3/src/smskillsdk/utils/__init__.py` & `smskillsdk-1.0.0/src/smskillsdk/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Soul Machines Ltd
+# Copyright 2024 Soul Machines Ltd
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `smskillsdk-0.2.3/src/smskillsdk/utils/memory.py` & `smskillsdk-1.0.0/src/smskillsdk/utils/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Soul Machines Ltd
+# Copyright 2024 Soul Machines Ltd
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utility functions for working with memory arrays"""
 from typing import Any, Dict, List, Tuple, Union
 
-from smskillsdk.models.api import Memory, MemoryScope
+from smskillsdk.models.common import Memory, MemoryScope
 
 
 def _has_valid_session_id_and_scope(
     memory: Memory,
     session_id: Union[str, None],
     scope: Union[MemoryScope, None],
     strict_session_id_match: bool = False,
```

### Comparing `smskillsdk-0.2.3/src/smskillsdk/utils/memory_values.py` & `smskillsdk-1.0.0/src/smskillsdk/utils/memory_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Soul Machines Ltd
+# Copyright 2024 Soul Machines Ltd
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Utility functions for accessing common memory values"""
 from typing import List, Optional
 
 from pydantic import BaseModel
 
-from ..models.api import Memory, MemoryScope
+from ..models.common import Memory, MemoryScope
 from .memory import get_memory_value, set_memory_value
 
 
 class UserIdentity(BaseModel):
     firstName: Optional[str] = None
     lastName: Optional[str] = None
     preferredName: Optional[str] = None
```

### Comparing `smskillsdk-0.2.3/src/smskillsdk.egg-info/PKG-INFO` & `smskillsdk-1.0.0/src/smskillsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smskillsdk
-Version: 0.2.3
+Version: 1.0.0
 Summary: A Python package to assist with developing services conforming to the Soul Machines Skill REST API.
 Home-page: https://docs.soulmachines.com
 Author: Soul Machines Ltd
 License: Apache 2.0
 Project-URL: Documentation, https://docs.soulmachines.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic>=1.8.2
 
 # smskillsdk (Python)
 
 The Skills Python SDK package contains data types for the session and execute endpoints specified within the Skills REST API, along with a range of utility functions for working with the memory data structure.
 
 ## Installation
```

### Comparing `smskillsdk-0.2.3/src/smskillsdk.egg-info/SOURCES.txt` & `smskillsdk-1.0.0/src/smskillsdk.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 pyproject.toml
 requirements-dev.txt
 setup.cfg
 setup.py
 .github/workflows/ci.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/release.yml
+scripts/add_license.sh
 scripts/build.ps1
 scripts/build.sh
 scripts/generate_models.ps1
 scripts/generate_models.sh
 scripts/run_tests.ps1
 scripts/run_tests.sh
+src/LICENSE.txt
 src/smskillsdk/__init__.py
 src/smskillsdk.egg-info/PKG-INFO
 src/smskillsdk.egg-info/SOURCES.txt
 src/smskillsdk.egg-info/dependency_links.txt
 src/smskillsdk.egg-info/not-zip-safe
 src/smskillsdk.egg-info/requires.txt
 src/smskillsdk.egg-info/top_level.txt
 src/smskillsdk/models/__init__.py
 src/smskillsdk/models/api.py
+src/smskillsdk/models/api_async.py
+src/smskillsdk/models/common.py
 src/smskillsdk/utils/__init__.py
 src/smskillsdk/utils/memory.py
 src/smskillsdk/utils/memory_values.py
 tests/__init__.py
 tests/test_memory.py
 tests/test_memory_values.py
```

### Comparing `smskillsdk-0.2.3/tests/__init__.py` & `smskillsdk-1.0.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Soul Machines Ltd
+# Copyright 2024 Soul Machines Ltd
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `smskillsdk-0.2.3/tests/test_memory.py` & `smskillsdk-1.0.0/tests/test_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Soul Machines Ltd
+# Copyright 2024 Soul Machines Ltd
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 from typing import List
 
-from smskillsdk.models.api import Memory, MemoryScope
+from smskillsdk.models.common import Memory, MemoryScope
 from smskillsdk.utils import memory
 
 
 class TestMemoryUtils(unittest.TestCase):
     def test_serialize(self):
         memory_dict = {
             "key1": "value1",
```

### Comparing `smskillsdk-0.2.3/tests/test_memory_values.py` & `smskillsdk-1.0.0/tests/test_memory_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Soul Machines Ltd
+# Copyright 2024 Soul Machines Ltd
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,19 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 from typing import List
 
-from smskillsdk.models.api import Memory, MemoryScope
-from smskillsdk.utils.memory_values import (get_user_identity,
-                                            get_user_location,
-                                            set_user_identity,
-                                            set_user_location)
+from smskillsdk.models.common import Memory, MemoryScope
+from smskillsdk.utils.memory_values import (
+    get_user_identity,
+    get_user_location,
+    set_user_identity,
+    set_user_location,
+)
 
 
 class TestMemoryUtils(unittest.TestCase):
     def test_user_identity(self):
         memories: List[Memory] = list()
 
         set_user_identity(memories, first_name="Joe", preferred_name="Bob")
```

