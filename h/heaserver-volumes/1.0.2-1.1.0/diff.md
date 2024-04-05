# Comparing `tmp/heaserver-volumes-1.0.2.tar.gz` & `tmp/heaserver-volumes-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-volumes-1.0.2.tar", last modified: Thu Mar 21 23:45:20 2024, max compression
+gzip compressed data, was "heaserver-volumes-1.1.0.tar", last modified: Fri Apr  5 20:01:11 2024, max compression
```

## Comparing `heaserver-volumes-1.0.2.tar` & `heaserver-volumes-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.908263 heaserver-volumes-1.0.2/
--rw-rw-rw-   0        0        0      261 2022-03-20 02:03:35.000000 heaserver-volumes-1.0.2/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/.gitignore
--rw-rw-rw-   0        0        0     1689 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-20 02:03:35.000000 heaserver-volumes-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4933 2024-03-21 23:45:20.906647 heaserver-volumes-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3631 2024-03-21 23:42:04.000000 heaserver-volumes-1.0.2/README.md
--rw-rw-rw-   0        0        0     1737 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/RELEASING.md
--rw-rw-rw-   0        0        0      408 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.802773 heaserver-volumes-1.0.2/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.802773 heaserver-volumes-1.0.2/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.857553 heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     6897 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0     8935 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     3703 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0    10676 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/requirements_dev.txt
--rw-rw-rw-   0        0        0     4637 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-03-21 23:45:20.908263 heaserver-volumes-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1799 2024-03-21 23:44:15.000000 heaserver-volumes-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.804819 heaserver-volumes-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.803797 heaserver-volumes-1.0.2/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.870621 heaserver-volumes-1.0.2/src/heaserver/volume/
--rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.0.2/src/heaserver/volume/__init__.py
--rw-rw-rw-   0        0        0    34166 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/src/heaserver/volume/service.py
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.872388 heaserver-volumes-1.0.2/src/heaserver/volume/wstl/
--rw-rw-rw-   0        0        0    14506 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/src/heaserver/volume/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.905630 heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/
--rw-rw-rw-   0        0        0     4933 2024-03-21 23:45:20.000000 heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1093 2024-03-21 23:45:20.000000 heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 23:45:20.000000 heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-03-21 23:45:20.000000 heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-03-21 23:45:20.000000 heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 23:45:20.000000 heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.805859 heaserver-volumes-1.0.2/tests/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.805859 heaserver-volumes-1.0.2/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:45:20.904612 heaserver-volumes-1.0.2/tests/heaserver/volumetest/
--rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.0.2/tests/heaserver/volumetest/__init__.py
--rw-rw-rw-   0        0        0     6704 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/tests/heaserver/volumetest/permissionstestcase.py
--rw-rw-rw-   0        0        0     8648 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/tests/heaserver/volumetest/test_all.py
--rw-rw-rw-   0        0        0     3681 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/tests/heaserver/volumetest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     7549 2023-12-18 23:36:40.000000 heaserver-volumes-1.0.2/tests/heaserver/volumetest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.543153 heaserver-volumes-1.1.0/
+-rw-rw-rw-   0        0        0      261 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1689 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4933 2024-04-05 20:01:11.542115 heaserver-volumes-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3631 2024-03-21 23:46:04.000000 heaserver-volumes-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1737 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/RELEASING.md
+-rw-rw-rw-   0        0        0      408 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.358392 heaserver-volumes-1.1.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.358392 heaserver-volumes-1.1.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.455568 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     6953 2024-04-04 20:56:23.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     8935 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     3703 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0    10728 2024-04-04 20:56:14.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4637 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 20:01:11.543153 heaserver-volumes-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1799 2024-04-05 20:00:40.000000 heaserver-volumes-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.360478 heaserver-volumes-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.359455 heaserver-volumes-1.1.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.468851 heaserver-volumes-1.1.0/src/heaserver/volume/
+-rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/src/heaserver/volume/__init__.py
+-rw-rw-rw-   0        0        0    35524 2024-04-05 05:05:11.000000 heaserver-volumes-1.1.0/src/heaserver/volume/service.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.476743 heaserver-volumes-1.1.0/src/heaserver/volume/wstl/
+-rw-rw-rw-   0        0        0    14506 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/src/heaserver/volume/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.541060 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/
+-rw-rw-rw-   0        0        0     4933 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1093 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.361508 heaserver-volumes-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.361508 heaserver-volumes-1.1.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.538950 heaserver-volumes-1.1.0/tests/heaserver/volumetest/
+-rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/__init__.py
+-rw-rw-rw-   0        0        0     6760 2024-04-04 20:56:06.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     8648 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/test_all.py
+-rw-rw-rw-   0        0        0     3681 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     7601 2024-04-04 20:55:52.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/testcase.py
```

### Comparing `heaserver-volumes-1.0.2/Dockerfile` & `heaserver-volumes-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/LICENSE` & `heaserver-volumes-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/PKG-INFO` & `heaserver-volumes-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-volumes
-Version: 1.0.2
+Version: 1.1.0
 Summary: The HEA volumes service
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-volumes,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.8
+Requires-Dist: heaserver~=1.2.0
 
 # HEA Volumes Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Volumes Microservice The HEA volumes service.
```

### Comparing `heaserver-volumes-1.0.2/README.md` & `heaserver-volumes-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/RELEASING.md` & `heaserver-volumes-1.1.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/permissionstestcase.py` & `heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/permissionstestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         'modified': None,
         'name': 'heaobject.volume.MongoDBFileSystem^DEFAULT_FILE_SYSTEM',
         'owner': NONE_USER,
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.MongoDBFileSystem',
-        'file_system_name': 'DEFAULT_FILE_SYSTEM'
+        'file_system_name': 'DEFAULT_FILE_SYSTEM',
+        'account': None
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -45,15 +46,16 @@
             'modified': None,
             'name': 'luximus',
             'owner': NONE_USER,
             'source': None,
             'source_detail': None,
             'type': 'heaobject.volume.Volume',
             'file_system_type': 'heaobject.volume.AWSFileSystem',
-            'file_system_name': 'DEFAULT_FILE_SYSTEM'
+            'file_system_name': 'DEFAULT_FILE_SYSTEM',
+            'account': None
         }
     ],
     service.MONGODB_FILE_SYSTEM_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

### Comparing `heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/test_all.py` & `heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/test_all_with_bad_permissions.py` & `heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/integrationtests/heaserver/volumeintegrationtest/testcase.py` & `heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.MongoDBFileSystem',
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'folder_id': '666f6f2d6261722d71757578',
         'mime_type': 'application/x.volume',
-        'credential_id': None
+        'credential_id': None,
+        'account': None
     },
     {
         'id': '0123456789ab0123456789ab',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
@@ -46,15 +47,16 @@
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.AWSFileSystem',
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'folder_id': '0123456789ab0123456789ab',
         'mime_type': 'application/x.volume',
-        'credential_id': None
+        'credential_id': None,
+        'account': None
     }],
     service.MONGODB_FILE_SYSTEM_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': 'Access to Amazon Web Services (AWS)',
```

### Comparing `heaserver-volumes-1.0.2/run-swaggerui.py` & `heaserver-volumes-1.1.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/setup.py` & `heaserver-volumes-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-volumes',
-    version='1.0.2',
+    version='1.1.0',
     description="The HEA volumes service",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.volume'],
     package_data={'heaserver.volume': ['wstl/*.json']},
-    install_requires=['heaserver~=1.0.8'],
+    install_requires=['heaserver~=1.2.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-volumes-1.0.2/src/heaserver/volume/service.py` & `heaserver-volumes-1.1.0/src/heaserver/volume/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 The HEA Volumes Microservice provides ...
 """
+import logging
+
 from heaobject.folder import Folder, Item
 from heaserver.service import client, response, appproperty
 from heaserver.service.appproperty import HEA_DB, HEA_CACHE
 from heaserver.service.runner import init_cmd_line, routes, start, web
 from heaserver.service.db import mongo, mongoservicelib
 from heaserver.service.wstl import builder_factory, action
 from heaserver.service.heaobjectsupport import type_to_resource_url
@@ -165,15 +167,25 @@
     summary: All volumes.
     tags:
         - heaserver-volumes-get-all-volumes
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
-    return await mongoservicelib.get_all(request, MONGODB_VOLUME_COLLECTION)
+    account_ids = request.query.getall('account_id', None)
+    account_type_names = request.query.getall('account_type_name', None)
+    if account_ids is not None and len(account_ids) != len(account_type_names):
+        return response.status_bad_request('Every account_id must have a corresponding account_type_name')
+    if account_ids:
+        mongoattributes = {'$or': [{'$and': [{'account.actual_object_id': account_id,
+                                              'account.actual_object_type_name': account_type_names[i]
+                                              }]} for i, account_id in enumerate(account_ids)]}
+    else:
+        mongoattributes = None
+    return await mongoservicelib.get_all(request, MONGODB_VOLUME_COLLECTION, mongoattributes=mongoattributes)
 
 
 @routes.get('/volumes/{id}/duplicator')
 @action(name='heaserver-volumes-volume-duplicate-form', path='volumes/{id}')
 async def get_volume_duplicate_form(request: web.Request) -> web.Response:
     """
     Gets a form template for duplicating the requested volume.
@@ -565,26 +577,35 @@
               value: heaobject.volume.MongoDBFileSystem
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
     type_ = request.match_info['type']
     sub = request.headers.get(SUB, NONE_USER)
+    account_ids = request.query.getall('account_id', None)
     cache_key = (sub, MONGODB_VOLUME_COLLECTION, None, f'file_system_type^{type_}', f'file_system_name^DEFAULT_FILE_SYSTEM')
-    objs = request.app[HEA_CACHE].get(cache_key)
+    objs = request.app[HEA_CACHE].get(cache_key) if account_ids is None else None
     if objs is None:
+        account_type_names = request.query.getall('account_type_name', None)
+        if account_ids is not None and len(account_ids) != len(account_type_names):
+            return response.status_bad_request('Every account_id must have a corresponding account_type_name')
+        if account_ids:
+            mongoattributes = {'$or': [{'$and': [{'account.actual_object_id': account_id,
+                                                  'account.actual_object_type_name': account_type_names[i]
+                                                  }]} for i, account_id in enumerate(account_ids)]}
+        else:
+            mongoattributes = {}
+        mongoattributes.update({'file_system_type': {'$eq': request.match_info['type']},
+                                'file_system_name': {'$eq': 'DEFAULT_FILE_SYSTEM'}})
         objs = []
-        async for obj in request.app[appproperty.HEA_DB].get_all(request,
-                                                        MONGODB_VOLUME_COLLECTION,
-                                                        mongoattributes={
-                                                            'file_system_type': {'$eq': request.match_info['type']},
-                                                            'file_system_name': {'$eq': 'DEFAULT_FILE_SYSTEM'}
-                                                        }, sub=sub):
+        async for obj in request.app[appproperty.HEA_DB].get_all(request, MONGODB_VOLUME_COLLECTION,
+                                                                 mongoattributes=mongoattributes, sub=sub):
             objs.append(obj)
-        request.app[HEA_CACHE][cache_key] = objs
+        if account_ids is None:
+            request.app[HEA_CACHE][cache_key] = objs
     return await response.get_all(request, objs)
 
 
 @routes.get('/filesystems/{id}')
 @action('heaserver-volumes-file-system-get-properties', rel='hea-properties')
 @action('heaserver-volumes-file-system-duplicate', rel='hea-duplicator', path='filesystems/{id}/duplicator')
 async def get_file_system(request: web.Request) -> web.Response:
```

### Comparing `heaserver-volumes-1.0.2/src/heaserver/volume/wstl/all.json` & `heaserver-volumes-1.1.0/src/heaserver/volume/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/PKG-INFO` & `heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-volumes
-Version: 1.0.2
+Version: 1.1.0
 Summary: The HEA volumes service
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-volumes,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.8
+Requires-Dist: heaserver~=1.2.0
 
 # HEA Volumes Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Volumes Microservice The HEA volumes service.
```

### Comparing `heaserver-volumes-1.0.2/src/heaserver_volumes.egg-info/SOURCES.txt` & `heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/tests/heaserver/volumetest/permissionstestcase.py` & `heaserver-volumes-1.1.0/tests/heaserver/volumetest/permissionstestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         'modified': None,
         'name': 'heaobject.volume.MongoDBFileSystem^DEFAULT_FILE_SYSTEM',
         'owner': NONE_USER,
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.MongoDBFileSystem',
-        'file_system_name': 'DEFAULT_FILE_SYSTEM'
+        'file_system_name': 'DEFAULT_FILE_SYSTEM',
+        'account': None
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -44,15 +45,16 @@
             'modified': None,
             'name': 'heaobject.volume.AWSFileSystem^DEFAULT_FILE_SYSTEM',
             'owner': NONE_USER,
             'source': None,
             'source_detail': None,
             'type': 'heaobject.volume.Volume',
             'file_system_type': 'heaobject.volume.AWSFileSystem',
-            'file_system_name': 'DEFAULT_FILE_SYSTEM'
+            'file_system_name': 'DEFAULT_FILE_SYSTEM',
+            'account': None
         }],
     service.MONGODB_FILE_SYSTEM_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': 'Access to Amazon Web Services (AWS)',
```

### Comparing `heaserver-volumes-1.0.2/tests/heaserver/volumetest/test_all.py` & `heaserver-volumes-1.1.0/tests/heaserver/volumetest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/tests/heaserver/volumetest/test_all_with_bad_permissions.py` & `heaserver-volumes-1.1.0/tests/heaserver/volumetest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.2/tests/heaserver/volumetest/testcase.py` & `heaserver-volumes-1.1.0/tests/heaserver/volumetest/testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.MongoDBFileSystem',
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'folder_id': None,
         'mime_type': 'application/x.volume',
-        'credential_id': None
+        'credential_id': None,
+        'account': None
     },
     {
         'id': '0123456789ab0123456789ab',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
@@ -45,15 +46,16 @@
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.AWSFileSystem',
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'folder_id': None,
         'mime_type': 'application/x.volume',
-        'credential_id': None
+        'credential_id': None,
+        'account': None
     }],
     service.MONGODB_FILE_SYSTEM_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': 'Access to Amazon Web Services (AWS)',
```

