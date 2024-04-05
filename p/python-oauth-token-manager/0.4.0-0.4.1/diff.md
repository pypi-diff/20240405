# Comparing `tmp/python-oauth-token-manager-0.4.0.tar.gz` & `tmp/python-oauth-token-manager-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-oauth-token-manager-0.4.0.tar", last modified: Thu Oct 12 18:39:38 2023, max compression
+gzip compressed data, was "python-oauth-token-manager-0.4.1.tar", last modified: Fri Apr  5 14:02:43 2024, max compression
```

## Comparing `python-oauth-token-manager-0.4.0.tar` & `python-oauth-token-manager-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-10-12 18:39:38.313086 python-oauth-token-manager-0.4.0/
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.4.0/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3757 2023-10-12 18:39:38.313086 python-oauth-token-manager-0.4.0/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2387 2023-06-14 15:36:29.000000 python-oauth-token-manager-0.4.0/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-10-12 18:39:38.309085 python-oauth-token-manager-0.4.0/auth/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      769 2023-06-15 15:27:37.000000 python-oauth-token-manager-0.4.0/auth/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2023-06-15 15:30:01.000000 python-oauth-token-manager-0.4.0/auth/abstract_datastore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5476 2023-10-12 18:38:39.000000 python-oauth-token-manager-0.4.0/auth/credentials.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.4.0/auth/credentials_helpers.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.4.0/auth/credentials_helpers_test.py
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-10-12 18:39:38.309085 python-oauth-token-manager-0.4.0/auth/datastore/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.4.0/auth/datastore/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5937 2023-06-15 15:27:04.000000 python-oauth-token-manager-0.4.0/auth/datastore/cloud_storage.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.4.0/auth/datastore/cloud_storage_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4702 2023-06-15 15:27:13.000000 python-oauth-token-manager-0.4.0/auth/datastore/firestore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5063 2023-06-15 15:27:18.000000 python-oauth-token-manager-0.4.0/auth/datastore/local_file.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.4.0/auth/datastore/local_file_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6887 2023-10-12 18:02:55.000000 python-oauth-token-manager-0.4.0/auth/datastore/secret_manager.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.4.0/auth/decorators.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.4.0/auth/decorators_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      947 2023-06-21 13:37:58.000000 python-oauth-token-manager-0.4.0/auth/exceptions.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1266 2023-10-12 18:39:30.000000 python-oauth-token-manager-0.4.0/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-10-12 18:39:38.313086 python-oauth-token-manager-0.4.0/python_oauth_token_manager.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3757 2023-10-12 18:39:38.000000 python-oauth-token-manager-0.4.0/python_oauth_token_manager.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      688 2023-10-12 18:39:38.000000 python-oauth-token-manager-0.4.0/python_oauth_token_manager.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-10-12 18:39:38.000000 python-oauth-token-manager-0.4.0/python_oauth_token_manager.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-10-12 18:39:38.000000 python-oauth-token-manager-0.4.0/python_oauth_token_manager.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-10-12 18:39:38.000000 python-oauth-token-manager-0.4.0/python_oauth_token_manager.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-10-12 18:39:38.313086 python-oauth-token-manager-0.4.0/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2024-04-05 14:02:43.449765 python-oauth-token-manager-0.4.1/
+-rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.4.1/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3757 2024-04-05 14:02:43.449765 python-oauth-token-manager-0.4.1/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2387 2023-06-14 15:36:29.000000 python-oauth-token-manager-0.4.1/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2024-04-05 14:02:43.441765 python-oauth-token-manager-0.4.1/auth/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      769 2023-06-15 15:27:37.000000 python-oauth-token-manager-0.4.1/auth/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2023-06-15 15:30:01.000000 python-oauth-token-manager-0.4.1/auth/abstract_datastore.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5545 2024-04-05 14:02:08.000000 python-oauth-token-manager-0.4.1/auth/credentials.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1327 2024-03-21 18:10:20.000000 python-oauth-token-manager-0.4.1/auth/credentials_helpers.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.4.1/auth/credentials_helpers_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2024-04-05 14:02:43.445765 python-oauth-token-manager-0.4.1/auth/datastore/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.4.1/auth/datastore/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5937 2023-06-15 15:27:04.000000 python-oauth-token-manager-0.4.1/auth/datastore/cloud_storage.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.4.1/auth/datastore/cloud_storage_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4702 2023-06-15 15:27:13.000000 python-oauth-token-manager-0.4.1/auth/datastore/firestore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5063 2023-06-15 15:27:18.000000 python-oauth-token-manager-0.4.1/auth/datastore/local_file.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.4.1/auth/datastore/local_file_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     6888 2023-11-17 09:34:13.000000 python-oauth-token-manager-0.4.1/auth/datastore/secret_manager.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.4.1/auth/decorators.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.4.1/auth/decorators_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      965 2023-11-06 19:57:48.000000 python-oauth-token-manager-0.4.1/auth/exceptions.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1266 2024-04-05 14:02:18.000000 python-oauth-token-manager-0.4.1/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2024-04-05 14:02:43.449765 python-oauth-token-manager-0.4.1/python_oauth_token_manager.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3757 2024-04-05 14:02:43.000000 python-oauth-token-manager-0.4.1/python_oauth_token_manager.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      688 2024-04-05 14:02:43.000000 python-oauth-token-manager-0.4.1/python_oauth_token_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2024-04-05 14:02:43.000000 python-oauth-token-manager-0.4.1/python_oauth_token_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2024-04-05 14:02:43.000000 python-oauth-token-manager-0.4.1/python_oauth_token_manager.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2024-04-05 14:02:43.000000 python-oauth-token-manager-0.4.1/python_oauth_token_manager.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2024-04-05 14:02:43.449765 python-oauth-token-manager-0.4.1/setup.cfg
```

### Comparing `python-oauth-token-manager-0.4.0/LICENSE` & `python-oauth-token-manager-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/PKG-INFO` & `python-oauth-token-manager-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.4.0
+Version: 0.4.1
 Summary: API for managing stored OAuth credentials.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
 Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-oauth-token-manager-0.4.0/README.md` & `python-oauth-token-manager-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/__init__.py` & `python-oauth-token-manager-0.4.1/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/abstract_datastore.py` & `python-oauth-token-manager-0.4.1/auth/abstract_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/credentials.py` & `python-oauth-token-manager-0.4.1/auth/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 import pytz
 from dateutil.relativedelta import relativedelta
 from google.auth.transport import requests
 from google.oauth2 import credentials as oauth
 
 from auth import decorators
 
-from .abstract_datastore import AbstractDatastore
-from .credentials_helpers import encode_key
-from .exceptions import CredentialsError
+from auth.abstract_datastore import AbstractDatastore
+from auth.credentials_helpers import encode_key
+from auth.exceptions import CredentialsError
 
 
 @dataclass
 class ProjectCredentials(object):
   client_id: str
   client_secret: str
 
@@ -136,16 +136,20 @@
     """Fetches the credentials.
 
     Returns:
        (google.oauth2.credentials.Credentials):  the credentials
     """
     expiry = self._to_utc(
         datetime.now().astimezone(pytz.utc) + relativedelta(minutes=30))
+
     if token := self.token_details:
-      creds = oauth.Credentials.from_authorized_user_info(json.loads(token))
+      if isinstance(token, str):
+        token = json.loads(token)
+
+      creds = oauth.Credentials.from_authorized_user_info(token)
 
       if creds.expired:
         creds.expiry = expiry
         self._refresh_credentials(creds=creds)
 
     else:
       creds = None
```

### Comparing `python-oauth-token-manager-0.4.0/auth/credentials_helpers.py` & `python-oauth-token-manager-0.4.1/auth/credentials_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import base64
 
-from .exceptions import KeyEncodingError
+from exceptions import KeyEncodingError
 
 
 def encode_key(key: str) -> str:
   """Creates the key to use in json oauth storage.
 
   Converts an string to a base64 version to use as a key both for security
   (so you can't easily see which credential goes with which key) but also as
@@ -28,12 +28,12 @@
   translated back.
 
   Returns:
       str: base64 representation of the key value.
   """
   try:
     if encoded_key := base64.b64encode(
-      key.encode('utf-8')).decode('utf-8').rstrip('='):
+            key.encode('utf-8')).decode('utf-8').rstrip('='):
       return encoded_key
 
   except:
     raise KeyEncodingError(f'Cannot encode {key}.')
```

### Comparing `python-oauth-token-manager-0.4.0/auth/credentials_helpers_test.py` & `python-oauth-token-manager-0.4.1/auth/credentials_helpers_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/datastore/__init__.py` & `python-oauth-token-manager-0.4.1/auth/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/datastore/cloud_storage.py` & `python-oauth-token-manager-0.4.1/auth/datastore/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/datastore/cloud_storage_test.py` & `python-oauth-token-manager-0.4.1/auth/datastore/cloud_storage_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/datastore/firestore.py` & `python-oauth-token-manager-0.4.1/auth/datastore/firestore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/datastore/local_file.py` & `python-oauth-token-manager-0.4.1/auth/datastore/local_file.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/datastore/local_file_test.py` & `python-oauth-token-manager-0.4.1/auth/datastore/local_file_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/datastore/secret_manager.py` & `python-oauth-token-manager-0.4.1/auth/datastore/secret_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         id=id, type=type, document=new_data)
 
     latest = self._get_latest(id)
 
     # Destroy other versions
     request = secretmanager_v1.ListSecretVersionsRequest(
         parent=self.client.secret_path(project=self._project, secret=id),
-        filter=f'state:enabled' # AND name!="{latest.name}"'
+        filter=f'state:enabled'  # AND name!="{latest.name}"'
     )
     version_list = self.client.list_secret_versions(request=request)
     for page in version_list.pages:
       for version in page.versions:
         # Only delete older versions
         if version.create_time < new_version.create_time:
           self.client.destroy_secret_version(
```

### Comparing `python-oauth-token-manager-0.4.0/auth/decorators.py` & `python-oauth-token-manager-0.4.1/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/decorators_test.py` & `python-oauth-token-manager-0.4.1/auth/decorators_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.4.0/auth/exceptions.py` & `python-oauth-token-manager-0.4.1/auth/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 
-class OAuthException(Exception): ...
+class OAuthException(Exception):
+  ...
+
 
 class CredentialsError(OAuthException):
-  def __init__(self, *args: object, message: str | None = ..., email: str | None) -> None: ...
+  def __init__(self, *args: object, message: str |
+               None = ..., email: str | None) -> None: ...
   message: str | None
 
+
 class KeyEncodingError(OAuthException):
   def __init__(self, *args: object, message: str | None = ...) -> None: ...
   message: str | None
-
```

### Comparing `python-oauth-token-manager-0.4.0/pyproject.toml` & `python-oauth-token-manager-0.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "python-oauth-token-manager"
-version = "0.4.0"
+version = "0.4.1"
 authors = [{ name = "David Harcombe", email = "david.harcombe@gmail.com" }]
 description = "API for managing stored OAuth credentials."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
```

### Comparing `python-oauth-token-manager-0.4.0/python_oauth_token_manager.egg-info/PKG-INFO` & `python-oauth-token-manager-0.4.1/python_oauth_token_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.4.0
+Version: 0.4.1
 Summary: API for managing stored OAuth credentials.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
 Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-oauth-token-manager-0.4.0/python_oauth_token_manager.egg-info/SOURCES.txt` & `python-oauth-token-manager-0.4.1/python_oauth_token_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

