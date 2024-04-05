# Comparing `tmp/heaobject-1.1.1.tar.gz` & `tmp/heaobject-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.1.1.tar", last modified: Mon Apr  1 23:31:21 2024, max compression
+gzip compressed data, was "heaobject-1.2.0.tar", last modified: Fri Apr  5 17:59:40 2024, max compression
```

## Comparing `heaobject-1.1.1.tar` & `heaobject-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 23:31:21.578748 heaobject-1.1.1/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4251 2024-04-01 23:31:21.577748 heaobject-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2789 2024-03-29 22:37:21.000000 heaobject-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 23:31:21.578748 heaobject-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2550 2024-04-01 23:29:58.000000 heaobject-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:31:21.521659 heaobject-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 23:31:21.568697 heaobject-1.1.1/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15432 2024-01-04 00:00:42.000000 heaobject-1.1.1/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7499 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9306 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/error.py
--rw-rw-rw-   0        0        0    21224 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4482 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     6790 2024-03-30 04:52:01.000000 heaobject-1.1.1/src/heaobject/organization.py
--rw-rw-rw-   0        0        0     7609 2024-03-26 22:41:59.000000 heaobject-1.1.1/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5045 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      130 2022-03-11 01:28:08.000000 heaobject-1.1.1/src/heaobject/record.py
--rw-rw-rw-   0        0        0    24503 2024-03-19 23:51:31.000000 heaobject-1.1.1/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    73318 2024-03-29 00:46:01.000000 heaobject-1.1.1/src/heaobject/root.py
--rw-rw-rw-   0        0        0      505 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.1.1/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     3994 2023-12-22 03:29:41.000000 heaobject-1.1.1/src/heaobject/storage.py
--rw-rw-rw-   0        0        0     9591 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.1.1/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/util.py
--rw-rw-rw-   0        0        0     5802 2023-12-16 22:23:08.000000 heaobject-1.1.1/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:31:21.576748 heaobject-1.1.1/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     4251 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-01 23:31:21.000000 heaobject-1.1.1/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 17:59:40.159804 heaobject-1.2.0/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4456 2024-04-05 17:59:40.159804 heaobject-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2994 2024-04-05 17:58:45.000000 heaobject-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 17:59:40.160805 heaobject-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2550 2024-04-05 17:58:39.000000 heaobject-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:59:40.108804 heaobject-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 17:59:40.150804 heaobject-1.2.0/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0     4882 2024-04-04 18:28:19.000000 heaobject-1.2.0/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15432 2024-01-04 00:00:42.000000 heaobject-1.2.0/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7499 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9306 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    21224 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4482 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     9023 2024-04-04 19:03:32.000000 heaobject-1.2.0/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0     7609 2024-03-26 22:41:59.000000 heaobject-1.2.0/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5045 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      130 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    24503 2024-03-19 23:51:31.000000 heaobject-1.2.0/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    76293 2024-04-04 20:22:49.000000 heaobject-1.2.0/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      505 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.2.0/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     3994 2023-12-22 03:29:41.000000 heaobject-1.2.0/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0     9591 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.2.0/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     6347 2024-04-04 20:08:02.000000 heaobject-1.2.0/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:59:40.157804 heaobject-1.2.0/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     4456 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.1.1/LICENSE` & `heaobject-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/PKG-INFO` & `heaobject-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.1.1
+Version: 1.2.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -32,14 +32,18 @@
 Requires-Dist: python-dateutil~=2.8.2
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.2.0
+* Created AbstractAssociation base class for complex associations between desktop objects.
+* Used it for the association between organizations and accounts, and volumes and accounts.
+
 ## Version 1.1.1
 * Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
 should replace CHECK_DYNAMIC with any dynamically computed permissions).
 
 ## Version 1.1.0
 * Added APIs for generating Person objects representing system users.
 * Added system|aws user.
```

### Comparing `heaobject-1.1.1/README.md` & `heaobject-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.2.0
+* Created AbstractAssociation base class for complex associations between desktop objects.
+* Used it for the association between organizations and accounts, and volumes and accounts.
+
 ## Version 1.1.1
 * Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
 should replace CHECK_DYNAMIC with any dynamically computed permissions).
 
 ## Version 1.1.0
 * Added APIs for generating Person objects representing system users.
 * Added system|aws user.
```

### Comparing `heaobject-1.1.1/setup.py` & `heaobject-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.1.1',
+                 version='1.2.0',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.1.1/src/heaobject/__init__.py` & `heaobject-1.2.0/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/account.py` & `heaobject-1.2.0/src/heaobject/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 from .data import DataObject, SameMimeType
+from .root import AbstractAssociation
 from abc import ABC
 from email_validator import validate_email, EmailNotValidError  # Leave this here for other modules to use
 from functools import partial
 
 
 class Account(DataObject, ABC):
     """
@@ -105,8 +106,15 @@
 
     @email_address.setter
     def email_address(self, email_address: Optional[str]) -> None:
         """Sets the email address associated with the account"""
         self.__email_address = _validate_email(str(email_address)).email if email_address is not None else None
 
 
+class AccountAssociation(AbstractAssociation):
+    @property
+    def allowed_actual_object_type_names(self) -> list[str]:
+        return [Account.get_type_name(), AWSAccount.get_type_name()]
+
+
+
 _validate_email = partial(validate_email, check_deliverability=False)
```

### Comparing `heaobject-1.1.1/src/heaobject/activity.py` & `heaobject-1.2.0/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/aws.py` & `heaobject-1.2.0/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/awss3key.py` & `heaobject-1.2.0/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/bucket.py` & `heaobject-1.2.0/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/data.py` & `heaobject-1.2.0/src/heaobject/data.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/dataadapter.py` & `heaobject-1.2.0/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/datamodel.py` & `heaobject-1.2.0/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/folder.py` & `heaobject-1.2.0/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/keychain.py` & `heaobject-1.2.0/src/heaobject/keychain.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/organization.py` & `heaobject-1.2.0/src/heaobject/organization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
-from heaobject.root import Permission, ShareImpl
-from heaobject.data import DataObject, SameMimeType
-from collections.abc import Iterable, Iterator
+from .account import AccountAssociation, AWSAccount
+from .root import Permission
+from .data import DataObject, SameMimeType
 from typing import Optional
+from copy import deepcopy
 
 permission_id_dict = {
     'admin_ids': [Permission.COOWNER],
     'manager_ids': [Permission.VIEWER, Permission.EDITOR, Permission.SHARER, Permission.DELETER],
     'member_ids': [Permission.VIEWER, Permission.SHARER]
 }
 
@@ -16,15 +17,15 @@
     """
     Represents a directory in the HEA desktop.
     """
 
     def __init__(self) -> None:
         super().__init__()
         # id is a super field
-        self.__aws_account_ids: list[str] = []  # allow org to have multiple aws accounts
+        self.__accounts: dict[AccountAssociation, None] = {}
         self.__principal_investigator_id: Optional[str] = None  # this would be a people id
         self.__admin_ids: list[str] = []  # list of user ids to be managers
         self.__manager_ids: list[str] = []  # list of user ids to be managers
         self.__member_ids: list[str] = []  # list of user ids to be members
         # super's name and display name would be used as org name(required)
 
     @classmethod
@@ -38,45 +39,92 @@
 
     @property
     def mime_type(self) -> str:
         """Read-only. The mime type for Organization objects, application/x.organization."""
         return type(self).get_mime_type()
 
     @property
+    def accounts(self) -> list[AccountAssociation]:
+        """The list of accounts owned by this organization."""
+        return list(deepcopy(account) for account in self.__accounts)
+
+    @accounts.setter
+    def accounts(self, accounts: list[AccountAssociation]):
+        if accounts is None:
+            self.__accounts.clear()
+        elif isinstance(accounts, AccountAssociation):
+            self.__accounts.clear()
+            self.__accounts[deepcopy(accounts)] = None
+        else:
+            if not all(isinstance(account, AccountAssociation) for account in accounts):
+                raise TypeError('accounts can only contain AccountAssociation objects')
+            self.__accounts.clear()
+            for account in accounts:
+                self.__accounts[deepcopy(account)] = None
+
+    def add_account(self, account: AccountAssociation):
+        if isinstance(account, AccountAssociation):
+            self.__accounts[deepcopy(account)] = None
+        else:
+            raise TypeError('account must be an AccountAssociation')
+
+    def remove_account(self, account: AccountAssociation):
+        try:
+            del self.__accounts[account]
+        except KeyError:
+            raise ValueError(f'Account {account} not found')
+
+    @property
     def aws_account_ids(self) -> list[str]:
         """
-        The list of REST aws account ids that are served by this organization. The property's setter accepts a list of
-        strings.
+        The list of aws account ids owned by this organization.
         """
-        return [i for i in self.__aws_account_ids]
+        return [account.actual_object_id for account in self.__accounts
+                if account.actual_object_type_name == AWSAccount.get_type_name()]
 
     @aws_account_ids.setter
     def aws_account_ids(self, value: list[str]) -> None:
+        aws_account_type_name = AWSAccount.get_type_name()
+        keys_to_remove = (account for account in self.__accounts if
+                          account.actual_object_type_name != aws_account_type_name)
+        for key in keys_to_remove:
+            del self.__accounts[key]
         if value is None:
-            self.__aws_account_ids = []
-        elif not isinstance(value, str):
-            self.__aws_account_ids = [str(i) for i in value]
+            pass
+        elif isinstance(value, str):
+            self.add_aws_account_id(value)
         else:
-            self.__aws_account_ids = [str(value)]
+            for account_id in value:
+                self.add_aws_account_id(account_id)
 
     def add_aws_account_id(self, value: str) -> None:
         """
         Adds a REST resource to the list of resources that are served by this component.
         :param value: a Resource object.
         """
-
-        self.__aws_account_ids.append(str(value))
+        account = AccountAssociation()
+        account.actual_object_id = value
+        account.actual_object_type_name = AWSAccount.get_type_name()
+        self.__accounts[deepcopy(account)] = None
 
     def remove_aws_account_id(self, value: str) -> None:
         """
         Removes a REST aws_account_id from the list of ids that are served by this organization. Ignores None values.
         :param value: str representing the aws account id.
+        :raises ValueError: if the value is not among this organization's AWS account ids.
         """
-
-        self.__aws_account_ids.remove(str(value))
+        account_to_remove: AccountAssociation | None = None
+        for account in self.__accounts:
+            if account.actual_object_type_name == AWSAccount.get_type_name() and account.actual_object_id == value:
+                account_to_remove = account
+                break
+        if account_to_remove is not None:
+            del self.__accounts[account_to_remove]
+        else:
+            raise ValueError(f'AWS account id {value} not found')
 
     @property
     def principal_investigator_id(self) -> Optional[str]:
         """
         The principal investigator People ID.
         """
         return self.__principal_investigator_id
```

### Comparing `heaobject-1.1.1/src/heaobject/person.py` & `heaobject-1.2.0/src/heaobject/person.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/project.py` & `heaobject-1.2.0/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/registry.py` & `heaobject-1.2.0/src/heaobject/registry.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/root.py` & `heaobject-1.2.0/src/heaobject/root.py`

 * *Files 2% similar despite different names*

```diff
@@ -1486,14 +1486,90 @@
             return self.__actual_object_uri
 
     @actual_object_uri.setter
     def actual_object_uri(self, actual_object_uri: str | None) -> None:
         self.__actual_object_uri = str(actual_object_uri) if actual_object_uri is not None else None
 
 
+class AbstractAssociation(AbstractMemberObject):
+    """
+    Abstract base class for creating associations between desktop objects. Unlike most other classes in heaobject, this
+    class overrides __eq__ and __hash__ so that objects of the same type and that have the same values for its
+    attributes are equal.
+    """
+    def __init__(self):
+        super().__init__()
+        self.__actual_object_type_name: str | None = None
+        self.__actual_object_id: str | None = None
+        self.__name: str | None = None
+
+    @property
+    @abc.abstractmethod
+    def allowed_actual_object_type_names(self) -> list[str]:
+        """
+        The permitted types for this association as a list of type names.
+        """
+        pass
+
+    @property
+    def actual_object_type_name(self) -> str | None:
+        """The name of the type of the associated object."""
+        return self.__actual_object_type_name
+
+    @actual_object_type_name.setter
+    def actual_object_type_name(self, actual_object_type_name: str | None):
+        if actual_object_type_name is not None and actual_object_type_name not in self.allowed_actual_object_type_names:
+            raise ValueError(f'{actual_object_type_name} not an allowed type')
+        self.__actual_object_type_name = str(actual_object_type_name) if actual_object_type_name is not None else None
+
+    @property
+    def actual_object_id(self) -> str | None:
+        """The id string of the associated object."""
+        return self.__actual_object_id
+
+    @actual_object_id.setter
+    def actual_object_id(self, actual_object_id: str | None):
+        self.__actual_object_id = str(actual_object_id) if actual_object_id is not None else None
+
+    @property
+    def name(self) -> str | None:
+        """A name for the association, like hasA."""
+        return self.__name
+
+    @name.setter
+    def name(self, name: str | None):
+        self.__name = str(name) if name is not None else None
+
+    def __eq__(self, other):
+        """
+        Overrides the default equality implementation. Objects of the same type and that have the same values for the
+        actual_object_type_name, actual_object_id, and name attributes are equal.
+        """
+        if self is not type(other):
+            return False
+        if self.actual_object_type_name != other.actual_object_type_name:
+            return False
+        if self.actual_object_id != other.actual_object_id:
+            return False
+        if self.name != other.name:
+            return False
+        return True
+
+    def __hash__(self):
+        """
+        Overrides the default hash code implementation. It computes the hash code from the actual_object_type_name,
+        actual_object_id, and name attributes.
+        """
+        val = 17
+        val += 37 * hash(self.actual_object_type_name)
+        val += 37 * hash(self.actual_object_id)
+        val += 37 * hash(self.name)
+        return val
+
+
 class HasSize:
     """
     Size mixin for use in desktop objects with content.
     """
     @property
     def size(self) -> Optional[int]:
         """Size of the item in bytes"""
```

### Comparing `heaobject-1.1.1/src/heaobject/source2target.py` & `heaobject-1.2.0/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/storage.py` & `heaobject-1.2.0/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/trash.py` & `heaobject-1.2.0/src/heaobject/trash.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/user.py` & `heaobject-1.2.0/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.1.1/src/heaobject/volume.py` & `heaobject-1.2.0/src/heaobject/volume.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 microservice supports it, create a volume with the file_system_name set to DEFAULT_FILE_SYSTEM or None. Or use variants
 of the microservice's REST API calls that do not require passing in a volume id.
 
 """
 from abc import ABC
 from typing import Optional, TypeVar
 from . import root
+from .account import AccountAssociation
 from .data import DataObject, SameMimeType
+from copy import deepcopy
 
 
 class FileSystem(root.AbstractDesktopObject, ABC):
     """
     Represents a filesystem, which controls how data is stored and retrieved. In HEA, all filesystems are either
     databases or network storage.
 
@@ -87,14 +89,15 @@
 
     def __init__(self) -> None:
         super().__init__()
         self.__file_system_name = DEFAULT_FILE_SYSTEM
         self.__file_system_type = MongoDBFileSystem.get_type_name()
         self.__credential_id: Optional[str] = None
         self.__folder_id: Optional[str] = None
+        self.__account: AccountAssociation | None = None
 
     @property
     def mime_type(self) -> str:
         return type(self).get_mime_type()
 
     @property  # type: ignore
     def folder_id(self) -> Optional[str]:
@@ -138,9 +141,18 @@
         """
         return self.__credential_id
 
     @credential_id.setter  # type: ignore
     def credential_id(self, credentials_id: Optional[str]) -> None:
         self.__credential_id = str(credentials_id) if credentials_id is not None else None
 
+    @property
+    def account(self) -> AccountAssociation | None:
+        return deepcopy(self.__account)
+
+    @account.setter
+    def account(self, account: AccountAssociation | None):
+        if account is not None and not isinstance(account, AccountAssociation):
+            raise TypeError('account must be a AccountAssociation')
+        self.__account = deepcopy(account) if account is not None else None
 
 DEFAULT_FILE_SYSTEM = 'DEFAULT_FILE_SYSTEM'
```

### Comparing `heaobject-1.1.1/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.2.0/src/heaobject.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.1.1
+Version: 1.2.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -32,14 +32,18 @@
 Requires-Dist: python-dateutil~=2.8.2
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.2.0
+* Created AbstractAssociation base class for complex associations between desktop objects.
+* Used it for the association between organizations and accounts, and volumes and accounts.
+
 ## Version 1.1.1
 * Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
 should replace CHECK_DYNAMIC with any dynamically computed permissions).
 
 ## Version 1.1.0
 * Added APIs for generating Person objects representing system users.
 * Added system|aws user.
```

### Comparing `heaobject-1.1.1/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.2.0/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

