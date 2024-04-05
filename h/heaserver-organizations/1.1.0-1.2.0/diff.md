# Comparing `tmp/heaserver-organizations-1.1.0.tar.gz` & `tmp/heaserver-organizations-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-organizations-1.1.0.tar", last modified: Tue Apr  2 21:16:58 2024, max compression
+gzip compressed data, was "heaserver-organizations-1.2.0.tar", last modified: Fri Apr  5 18:48:23 2024, max compression
```

## Comparing `heaserver-organizations-1.1.0.tar` & `heaserver-organizations-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.433461 heaserver-organizations-1.1.0/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4812 2024-04-02 21:16:58.432460 heaserver-organizations-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3422 2024-04-02 21:14:43.000000 heaserver-organizations-1.1.0/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/RELEASING.md
--rw-rw-rw-   0        0        0      404 2024-03-20 04:10:28.000000 heaserver-organizations-1.1.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.249726 heaserver-organizations-1.1.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.250314 heaserver-organizations-1.1.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.354195 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10600 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      402 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    14644 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-02 21:16:58.433461 heaserver-organizations-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1911 2024-04-02 21:15:46.000000 heaserver-organizations-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.252311 heaserver-organizations-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.251312 heaserver-organizations-1.1.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.366250 heaserver-organizations-1.1.0/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    29224 2024-03-28 18:53:37.000000 heaserver-organizations-1.1.0/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.379253 heaserver-organizations-1.1.0/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    22622 2024-03-28 17:02:30.000000 heaserver-organizations-1.1.0/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.431460 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     4812 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-02 21:16:58.000000 heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.252311 heaserver-organizations-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.253311 heaserver-organizations-1.1.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-02 21:16:58.429459 heaserver-organizations-1.1.0/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.1.0/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     6736 2023-12-18 21:21:27.000000 heaserver-organizations-1.1.0/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.120495 heaserver-organizations-1.2.0/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5120 2024-04-05 18:48:23.119495 heaserver-organizations-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3730 2024-04-05 18:45:22.000000 heaserver-organizations-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/RELEASING.md
+-rw-rw-rw-   0        0        0      404 2024-03-20 04:10:28.000000 heaserver-organizations-1.2.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.016844 heaserver-organizations-1.2.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.016844 heaserver-organizations-1.2.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.086496 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10658 2024-04-05 02:18:47.000000 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      402 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    14702 2024-04-05 02:18:40.000000 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 18:48:23.121496 heaserver-organizations-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1911 2024-04-05 18:47:37.000000 heaserver-organizations-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.018843 heaserver-organizations-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.017844 heaserver-organizations-1.2.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.088497 heaserver-organizations-1.2.0/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    28882 2024-04-04 23:11:21.000000 heaserver-organizations-1.2.0/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.089497 heaserver-organizations-1.2.0/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    22819 2024-04-04 16:00:27.000000 heaserver-organizations-1.2.0/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.118495 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     5120 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-04-05 18:48:23.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.019843 heaserver-organizations-1.2.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.019843 heaserver-organizations-1.2.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.117495 heaserver-organizations-1.2.0/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     1783 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     6794 2024-04-05 02:18:18.000000 heaserver-organizations-1.2.0/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver-organizations-1.1.0/Dockerfile` & `heaserver-organizations-1.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.1.0/LICENSE` & `heaserver-organizations-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.1.0/PKG-INFO` & `heaserver-organizations-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.1.0
+Version: 1.2.0
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,27 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.2
+Requires-Dist: heaserver~=1.2.0
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.2.0
+* Improved performance accessing an organization's AWS accounts.
+* heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
+aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
+
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
 
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
```

### Comparing `heaserver-organizations-1.1.0/README.md` & `heaserver-organizations-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.2.0
+* Improved performance accessing an organization's AWS accounts.
+* heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
+aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
+
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
 
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
```

### Comparing `heaserver-organizations-1.1.0/RELEASING.md` & `heaserver-organizations-1.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
             "derived_from": [],
             "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
-            'version': None
+            'version': None,
+            'accounts': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -53,15 +54,16 @@
             "derived_from": [],
             "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": [],
             "member_ids": ['0123456789ab0123456789ab'],
             'type': 'heaobject.organization.Organization',
-            'version': None
+            'version': None,
+            'accounts': []
         }
     ],
     'filesystems': [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

### Comparing `heaserver-organizations-1.1.0/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
             "derived_from": [],
             "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": ['666f6f2d6261722d71757578'],
             "member_ids": ['0123456789ab0123456789ab'],
             'type': 'heaobject.organization.Organization',
-            'mime_type': 'application/x.organization'
+            'mime_type': 'application/x.organization',
+            'accounts': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -57,15 +58,16 @@
             "derived_from": [],
             "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": ["11234867890b0123a56789ab"],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
-            'mime_type': 'application/x.organization'
+            'mime_type': 'application/x.organization',
+            'accounts': []
         }
     ],
     CollectionKey(name='filesystems', db_manager_cls=MockDockerMongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

### Comparing `heaserver-organizations-1.1.0/run-swaggerui.py` & `heaserver-organizations-1.2.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.1.0/setup.py` & `heaserver-organizations-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.1.0',
+    version='1.2.0',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.organization'],
     package_data={'heaserver.organization': ['wstl/*.json']},
-    install_requires=['heaserver~=1.1.2'],
+    install_requires=['heaserver~=1.2.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-organizations-1.1.0/src/heaserver/organization/service.py` & `heaserver-organizations-1.2.0/src/heaserver/organization/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -674,36 +674,29 @@
         - heaserver-organizations-organization-get-aws-accounts
     parameters:
         - $ref: '#/components/parameters/id'
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
-    sub = request.headers.get(SUB)
+    sub = request.headers.get(SUB, NONE_USER)
     org_dict = await request.app[HEA_DB].get(request, MONGODB_ORGANIZATION_COLLECTION, var_parts='id', sub=sub)
     if org_dict is None:
         return response.status_not_found()
     org = Organization()
     org.from_dict(org_dict)
     headers = {SUB: sub or '',
                hdrs.AUTHORIZATION: request.headers.get(hdrs.AUTHORIZATION, '')} if SUB in request.headers else None
 
-    volume_url = await type_to_resource_url(request, Volume)
-    if volume_url is None:
-        raise ValueError('No Volume service registered')
-    get_volumes_url = URL(volume_url) / 'byfilesystemtype' / AWSFileSystem.get_type_name()
-
     aws_account_url = await type_to_resource_url(request, AWSAccount, file_system_type_or_type_name=AWSFileSystem)
     if aws_account_url is None:
         raise ValueError('No AWSAccount service registered')
-
-    query = [('volume_id', volume.id) async for volume in client.get_all(request.app, get_volumes_url, Volume, headers=headers)]
-    for account_id in org.aws_account_ids:
-        query.append(('account_id', account_id))
-    if org.aws_account_ids:
+    aws_account_ids = org.aws_account_ids
+    query = [('account_id', account_id) for account_id in aws_account_ids]
+    if aws_account_ids:
         result = [a.to_dict() async for a in client.get_all(request.app, URL(aws_account_url).with_path('awsaccounts').with_query(query), AWSAccount, headers=headers)]
     else:
         result = []
     return await response.get_all(request, result)
 
 
 @routes.get('/organizations/{id}/members')
```

### Comparing `heaserver-organizations-1.1.0/src/heaserver/organization/wstl/all.json` & `heaserver-organizations-1.2.0/src/heaserver/organization/wstl/all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999751984126983%*

 * *Differences: {"'wstl'": "{'actions': {7: {'inputs': {14: {'readOnly': True, 'value': 'Internal', 'hea': "*

 * *           "OrderedDict([('display', False)])}}}}}"}*

```diff
@@ -191,16 +191,21 @@
                             "type": "datetime"
                         },
                         "name": "modified",
                         "prompt": "Modified",
                         "readOnly": true
                     },
                     {
+                        "hea": {
+                            "display": false
+                        },
                         "name": "source",
-                        "prompt": "Source"
+                        "prompt": "Source",
+                        "readOnly": true,
+                        "value": "Internal"
                     },
                     {
                         "hea": {
                             "display": false,
                             "optionsFromUrl": {
                                 "path": "people/",
                                 "text": "display_name",
```

### Comparing `heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.1.0
+Version: 1.2.0
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,27 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.2
+Requires-Dist: heaserver~=1.2.0
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.2.0
+* Improved performance accessing an organization's AWS accounts.
+* heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
+aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
+
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
 
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
```

### Comparing `heaserver-organizations-1.1.0/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.1.0/tests/heaserver/organizationtest/test_all.py` & `heaserver-organizations-1.2.0/tests/heaserver/organizationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.1.0/tests/heaserver/organizationtest/testcase.py` & `heaserver-organizations-1.2.0/tests/heaserver/organizationtest/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             "admin_ids": [],
             'type': 'heaobject.organization.Organization',
-            'mime_type': 'application/x.organization'
+            'mime_type': 'application/x.organization',
+            'accounts': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             'source_detail': None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -48,15 +49,16 @@
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": ["11234867890b0123a56789ab"],
             "member_ids": [],
             "admin_ids": [],
             'type': 'heaobject.organization.Organization',
-            'mime_type': 'application/x.organization'
+            'mime_type': 'application/x.organization',
+            'accounts': []
         }
     ],
     'people': [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

