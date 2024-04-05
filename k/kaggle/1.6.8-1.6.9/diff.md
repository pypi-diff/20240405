# Comparing `tmp/kaggle-1.6.8.tar.gz` & `tmp/kaggle-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaggle-1.6.8.tar", last modified: Mon Mar 25 15:49:21 2024, max compression
+gzip compressed data, was "kaggle-1.6.9.tar", last modified: Fri Apr  5 21:16:19 2024, max compression
```

## Comparing `kaggle-1.6.8.tar` & `kaggle-1.6.9.tar`

### file list

```diff
@@ -1,49 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:49:21.951108 kaggle-1.6.8/
--rw-r--r--   0 root         (0) root         (0)    11541 2024-03-25 15:49:17.000000 kaggle-1.6.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-25 15:49:17.000000 kaggle-1.6.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      607 2024-03-25 15:49:21.951108 kaggle-1.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35600 2024-03-25 15:49:17.000000 kaggle-1.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:49:21.943107 kaggle-1.6.8/kaggle/
--rw-r--r--   0 root         (0) root         (0)      799 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:49:21.943107 kaggle-1.6.8/kaggle/api/
--rw-r--r--   0 root         (0) root         (0)      742 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   189890 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/api/kaggle_api.py
--rw-r--r--   0 root         (0) root         (0)   174039 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/api/kaggle_api_extended.py
--rw-r--r--   0 root         (0) root         (0)    25458 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/api_client.py
--rw-r--r--   0 root         (0) root         (0)    75747 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/cli.py
--rw-r--r--   0 root         (0) root         (0)     9163 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:49:21.951108 kaggle-1.6.8/kaggle/models/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/api_blob_type.py
--rw-r--r--   0 root         (0) root         (0)     4851 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/collaborator.py
--rw-r--r--   0 root         (0) root         (0)     5166 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/create_inbox_file_request.py
--rw-r--r--   0 root         (0) root         (0)     7424 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/dataset_column.py
--rw-r--r--   0 root         (0) root         (0)    12569 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/dataset_new_request.py
--rw-r--r--   0 root         (0) root         (0)     9991 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/dataset_new_version_request.py
--rw-r--r--   0 root         (0) root         (0)    10114 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/dataset_update_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     4342 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/error.py
--rw-r--r--   0 root         (0) root         (0)     7791 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/kaggle_models_extended.py
--rw-r--r--   0 root         (0) root         (0)    20199 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/kernel_push_request.py
--rw-r--r--   0 root         (0) root         (0)     4365 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/license.py
--rw-r--r--   0 root         (0) root         (0)     5051 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/model_instance_new_version_request.py
--rw-r--r--   0 root         (0) root         (0)    13721 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/model_instance_update_request.py
--rw-r--r--   0 root         (0) root         (0)    16192 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/model_new_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    10055 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/model_new_request.py
--rw-r--r--   0 root         (0) root         (0)     9096 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/model_update_request.py
--rw-r--r--   0 root         (0) root         (0)     2895 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/result.py
--rw-r--r--   0 root         (0) root         (0)     7844 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/start_blob_upload_request.py
--rw-r--r--   0 root         (0) root         (0)     4826 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/start_blob_upload_response.py
--rw-r--r--   0 root         (0) root         (0)     5439 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/models/upload_file.py
--rw-r--r--   0 root         (0) root         (0)    13927 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:49:21.951108 kaggle-1.6.8/kaggle/test/
--rw-r--r--   0 root         (0) root         (0)      596 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-03-25 15:49:18.000000 kaggle-1.6.8/kaggle/test/test_authenticate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:49:21.943107 kaggle-1.6.8/kaggle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      607 2024-03-25 15:49:21.000000 kaggle-1.6.8/kaggle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1236 2024-03-25 15:49:21.000000 kaggle-1.6.8/kaggle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 15:49:21.000000 kaggle-1.6.8/kaggle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-03-25 15:49:21.000000 kaggle-1.6.8/kaggle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       89 2024-03-25 15:49:21.000000 kaggle-1.6.8/kaggle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-25 15:49:21.000000 kaggle-1.6.8/kaggle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-03-25 15:49:21.951108 kaggle-1.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2024-03-25 15:49:18.000000 kaggle-1.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:16:19.980978 kaggle-1.6.9/
+-rw-r--r--   0 root         (0) root         (0)    11541 2024-04-03 01:15:53.000000 kaggle-1.6.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-03 01:15:53.000000 kaggle-1.6.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15780 2024-04-05 21:16:19.980978 kaggle-1.6.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2336 2024-04-03 01:15:53.000000 kaggle-1.6.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:16:19.976978 kaggle-1.6.9/kaggle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15780 2024-04-05 21:16:19.000000 kaggle-1.6.9/kaggle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-05 21:16:19.000000 kaggle-1.6.9/kaggle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 21:16:19.000000 kaggle-1.6.9/kaggle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-05 21:16:19.000000 kaggle-1.6.9/kaggle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-05 21:16:19.000000 kaggle-1.6.9/kaggle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-05 21:16:19.000000 kaggle-1.6.9/kaggle.egg-info/top_level.txt
+-rw-r-----   0 root         (0) root         (0)     1841 2024-04-05 19:46:07.000000 kaggle-1.6.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-05 21:16:19.980978 kaggle-1.6.9/setup.cfg
+-rw-r-----   0 root         (0) root         (0)     1308 2024-04-05 20:46:41.000000 kaggle-1.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:16:19.976978 kaggle-1.6.9/src/
+-rw-r-----   0 root         (0) root         (0)       23 2024-04-05 20:46:51.000000 kaggle-1.6.9/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:16:19.976978 kaggle-1.6.9/src/kaggle/
+-rw-r--r--   0 root         (0) root         (0)      203 2024-04-05 09:18:26.000000 kaggle-1.6.9/src/kaggle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75151 2024-04-05 09:19:50.000000 kaggle-1.6.9/src/kaggle/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:16:19.980978 kaggle-1.6.9/src/kaggle/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 01:15:53.000000 kaggle-1.6.9/src/kaggle/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-04-05 09:19:50.000000 kaggle-1.6.9/src/kaggle/test/test_authenticate.py
+-rw-r-----   0 root         (0) root         (0)     1308 2024-04-05 20:46:41.000000 kaggle-1.6.9/src/setup.py
```

### Comparing `kaggle-1.6.8/LICENSE` & `kaggle-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.8/kaggle/cli.py` & `kaggle-1.6.9/src/kaggle/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,9 @@
 #!/usr/bin/python
 #
-# Copyright 2024 Kaggle Inc
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-#!/usr/bin/python
-#
 # Copyright 2019 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `kaggle-1.6.8/kaggle/test/test_authenticate.py` & `kaggle-1.6.9/src/kaggle/test/test_authenticate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-#!/usr/bin/python
-#
-# Copyright 2024 Kaggle Inc
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from kaggle.api.kaggle_api_extended import KaggleApi
 
 # python -m unittest tests.test_authenticate
 
 import os
 import unittest
```

### Comparing `kaggle-1.6.8/setup.py` & `kaggle-1.6.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-#!/usr/bin/python
-#
-# Copyright 2024 Kaggle Inc
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 # coding=utf-8
 from setuptools import setup, find_packages
 
+# Note: pyproject.toml seems to be chosen by pip install over setup.py, so this
+# file is likely not being used anymore. We should verify and merge this into
+# pyproject.toml instead of maintaining both flows.
 setup(
     name='kaggle',
-    version='1.6.8',
+    version='1.6.9',
     description='Kaggle API',
     long_description=
     ('Official API for https://www.kaggle.com, accessible using a command line '
      'tool implemented in Python. Beta release - Kaggle reserves the right to '
      'modify the API functionality currently offered.'),
     author='Kaggle',
     author_email='support@kaggle.com',
```

