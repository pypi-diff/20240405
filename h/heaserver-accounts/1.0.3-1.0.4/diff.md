# Comparing `tmp/heaserver-accounts-1.0.3.tar.gz` & `tmp/heaserver-accounts-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-accounts-1.0.3.tar", last modified: Wed Mar 27 00:05:55 2024, max compression
+gzip compressed data, was "heaserver-accounts-1.0.4.tar", last modified: Fri Apr  5 19:50:15 2024, max compression
```

## Comparing `heaserver-accounts-1.0.3.tar` & `heaserver-accounts-1.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.834125 heaserver-accounts-1.0.3/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/.gitignore
--rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5411 2024-03-27 00:05:55.833126 heaserver-accounts-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4103 2024-03-27 00:05:15.000000 heaserver-accounts-1.0.3/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/RELEASING.md
--rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.704903 heaserver-accounts-1.0.3/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.704903 heaserver-accounts-1.0.3/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.771124 heaserver-accounts-1.0.3/integrationtests/heaserver/accountintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/integrationtests/heaserver/accountintegrationtest/__init__.py
--rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/integrationtests/heaserver/accountintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7748 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.3/integrationtests/heaserver/accountintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/requirements_dev.txt
--rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-03-27 00:05:55.834125 heaserver-accounts-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-03-27 00:04:26.000000 heaserver-accounts-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.706902 heaserver-accounts-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.705903 heaserver-accounts-1.0.3/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.783124 heaserver-accounts-1.0.3/src/heaserver/account/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/src/heaserver/account/__init__.py
--rw-rw-rw-   0        0        0    44562 2024-01-20 03:20:59.000000 heaserver-accounts-1.0.3/src/heaserver/account/service.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.790127 heaserver-accounts-1.0.3/src/heaserver/account/wstl/
--rw-rw-rw-   0        0        0    11424 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.3/src/heaserver/account/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.832125 heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/
--rw-rw-rw-   0        0        0     5411 2024-03-27 00:05:55.000000 heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-03-27 00:05:55.000000 heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 00:05:55.000000 heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-03-27 00:05:55.000000 heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-03-27 00:05:55.000000 heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-27 00:05:55.000000 heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.706902 heaserver-accounts-1.0.3/tests/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.707903 heaserver-accounts-1.0.3/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:05:55.830125 heaserver-accounts-1.0.3/tests/heaserver/accounttest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.3/tests/heaserver/accounttest/__init__.py
--rw-rw-rw-   0        0        0     7408 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.3/tests/heaserver/accounttest/test_all.py
--rw-rw-rw-   0        0        0     5146 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.3/tests/heaserver/accounttest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.100082 heaserver-accounts-1.0.4/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/.gitignore
+-rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5504 2024-04-05 19:50:15.099005 heaserver-accounts-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4196 2024-04-05 19:01:13.000000 heaserver-accounts-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/RELEASING.md
+-rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.922949 heaserver-accounts-1.0.4/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.923977 heaserver-accounts-1.0.4/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.015649 heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     7748 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 19:50:15.100082 heaserver-accounts-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-04-05 19:48:53.000000 heaserver-accounts-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.926044 heaserver-accounts-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.925003 heaserver-accounts-1.0.4/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.032575 heaserver-accounts-1.0.4/src/heaserver/account/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/src/heaserver/account/__init__.py
+-rw-rw-rw-   0        0        0    45036 2024-04-05 18:57:12.000000 heaserver-accounts-1.0.4/src/heaserver/account/service.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.042306 heaserver-accounts-1.0.4/src/heaserver/account/wstl/
+-rw-rw-rw-   0        0        0    11424 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.4/src/heaserver/account/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.097822 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/
+-rw-rw-rw-   0        0        0     5504 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.927113 heaserver-accounts-1.0.4/tests/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.927113 heaserver-accounts-1.0.4/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.095821 heaserver-accounts-1.0.4/tests/heaserver/accounttest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/tests/heaserver/accounttest/__init__.py
+-rw-rw-rw-   0        0        0     7466 2024-04-01 23:50:21.000000 heaserver-accounts-1.0.4/tests/heaserver/accounttest/test_all.py
+-rw-rw-rw-   0        0        0     5146 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.4/tests/heaserver/accounttest/testcase.py
```

### Comparing `heaserver-accounts-1.0.3/Dockerfile` & `heaserver-accounts-1.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.3/LICENSE` & `heaserver-accounts-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.3/PKG-INFO` & `heaserver-accounts-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.3
+Version: 1.0.4
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,28 +21,32 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.1
+Requires-Dist: heaserver~=1.2.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.4
+* Corrected caching issue.
+
 ## Version 1.0.3
 * Improved error handling when the user lacks authorization for some AWS account information.
 
 ## Version 1.0.2
 * Avoid a 500 error when retrieving accounts when attempting to access a suspended account.
 * AWS account info requests return more complete information.
+* Omit shares from the properties template.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
 Initial release.
```

### Comparing `heaserver-accounts-1.0.3/README.md` & `heaserver-accounts-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.4
+* Corrected caching issue.
+
 ## Version 1.0.3
 * Improved error handling when the user lacks authorization for some AWS account information.
 
 ## Version 1.0.2
 * Avoid a 500 error when retrieving accounts when attempting to access a suspended account.
 * AWS account info requests return more complete information.
+* Omit shares from the properties template.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
 Initial release.
```

### Comparing `heaserver-accounts-1.0.3/RELEASING.md` & `heaserver-accounts-1.0.4/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.3/integrationtests/heaserver/accountintegrationtest/testcase.py` & `heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.3/run-swaggerui.py` & `heaserver-accounts-1.0.4/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.3/setup.py` & `heaserver-accounts-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-accounts',
-    version='1.0.3',
+    version='1.0.4',
     description="Manages account information",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.account'],
     package_data={'heaserver.account': ['wstl/*.json']},
     install_requires=[
-        'heaserver~=1.1.1'
+        'heaserver~=1.2.0'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
```

### Comparing `heaserver-accounts-1.0.3/src/heaserver/account/service.py` & `heaserver-accounts-1.0.4/src/heaserver/account/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,35 +183,37 @@
       '200':
         $ref: '#/components/responses/200'
     """
     async with DesktopObjectActionLifecycle(request=request,
                                                 code='hea-get',
                                                 description=f'Getting all AWS accounts',
                                                 activity_cb=publish_desktop_object) as activity:
+        logger = logging.getLogger(__name__)
         sub = request.headers.get(SUB, NONE_USER)
-        if 'volume_id' in request.query:
-            volume_ids = tuple(request.query.getall('volume_id'))
-        else:
-            volume_ids = tuple()
-        if 'account_id' in request.query:
-            account_ids = tuple(request.query.getall('account_id'))
-        else:
-            account_ids = tuple()
-        cache_key = (sub, None, volume_ids, account_ids)
-        account_dicts = request.app[HEA_CACHE].get(cache_key)
+        account_ids_ = request.query.getall('account_id', None)
+        account_ids = tuple(account_ids_) if account_ids_ is not None else None
+        cache_key = (sub, None, account_ids)
+        account_dicts = request.app[HEA_CACHE].get(cache_key) if account_ids is None else None
         if account_dicts is None:
             db = request.app[HEA_DB]
             account_dicts: list[DesktopObjectDict] = []
-            volume_ids = [volume.id async for volume in db.get_volumes(request, AWSFileSystem)]
+            volume_ids = [volume.id async for volume in db.get_volumes(request, AWSFileSystem,
+                                                                       account_ids=account_ids,
+                                                                       account_type_names=[AWSAccount.get_type_name()] * len(account_ids) if account_ids is not None else None)]
+            logger.debug('Checking volumes %s for accounts %s', volume_ids, account_ids)
+            account_id_to_account = {}
             async for aws_account, volume_id in db.get_accounts(request, volume_ids):
                 if not account_ids or aws_account.id in account_ids:
                     account_dict = aws_account.to_dict()
-                    account_dicts.append(account_dict)
+                    account_id_to_account[account_dict['id']] = account_dict
                     request.app[HEA_CACHE][(sub, f'id^{account_dict["id"]}')] = (account_dict, volume_id)
-            request.app[HEA_CACHE][cache_key] = account_dicts
+            account_dicts_ = list(account_id_to_account.values())
+            if account_dicts is None:
+                request.app[HEA_CACHE][cache_key] = account_dicts_
+            account_dicts = account_dicts_
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_object_uri = 'awsaccounts/'
         return await response.get_all(request, account_dicts)
 
 
 @routes.get('/volumes/{volume_id}/awsaccounts/me')
 @action('heaserver-accounts-awsaccount-get-open-choices', rel='hea-opener-choices hea-context-menu',
```

### Comparing `heaserver-accounts-1.0.3/src/heaserver/account/wstl/all.json` & `heaserver-accounts-1.0.4/src/heaserver/account/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/PKG-INFO` & `heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.3
+Version: 1.0.4
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,28 +21,32 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.1
+Requires-Dist: heaserver~=1.2.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.4
+* Corrected caching issue.
+
 ## Version 1.0.3
 * Improved error handling when the user lacks authorization for some AWS account information.
 
 ## Version 1.0.2
 * Avoid a 500 error when retrieving accounts when attempting to access a suspended account.
 * AWS account info requests return more complete information.
+* Omit shares from the properties template.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
 Initial release.
```

### Comparing `heaserver-accounts-1.0.3/src/heaserver_accounts.egg-info/SOURCES.txt` & `heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.3/tests/heaserver/accounttest/test_all.py` & `heaserver-accounts-1.0.4/tests/heaserver/accounttest/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         url = '/volumes/666f6f2d6261722d71757578/awsaccounts/me'
         async with self.client.request('GET', url, headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             self.assertEqual([self.account.to_dict()], await resp.json())
 
     async def test_get_new_bucket_form(self):
         url = '/volumes/666f6f2d6261722d71757578/awsaccounts/me/newbucket/'
         expected = [{'collection': {'version': '1.0',
+                                    'permissions': [[]],
                                     'items': [{'data': [{'name': 'alternate_contact_name', 'value': None, 'prompt': 'alternate_contact_name', 'display': True},
                                                         {'name': 'alternate_email_address', 'value': None, 'prompt': 'alternate_email_address', 'display': True},
                                                         {'name': 'alternate_phone_number', 'value': None, 'prompt': 'alternate_phone_number', 'display': True},
                                                         {'name': 'created', 'value': None, 'prompt': 'created', 'display': True},
                                                         {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
                                                         {'name': 'derived_from', 'value': [], 'prompt': 'derived_from', 'display': True},
                                                         {'name': 'description', 'value': None, 'prompt': 'description', 'display': True},
```

### Comparing `heaserver-accounts-1.0.3/tests/heaserver/accounttest/testcase.py` & `heaserver-accounts-1.0.4/tests/heaserver/accounttest/testcase.py`

 * *Files identical despite different names*

