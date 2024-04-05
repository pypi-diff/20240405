# Comparing `tmp/trustauthx-0.7.2.tar.gz` & `tmp/trustauthx-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustauthx-0.7.2.tar", last modified: Wed Apr  3 23:29:32 2024, max compression
+gzip compressed data, was "trustauthx-0.7.3.tar", last modified: Fri Apr  5 17:58:18 2024, max compression
```

## Comparing `trustauthx-0.7.2.tar` & `trustauthx-0.7.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:29:32.036739 trustauthx-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 23:29:23.000000 trustauthx-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 23:29:32.036739 trustauthx-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 23:29:23.000000 trustauthx-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:29:32.036739 trustauthx-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 23:29:23.000000 trustauthx-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:29:32.032739 trustauthx-0.7.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 23:29:23.000000 trustauthx-0.7.2/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:29:32.036739 trustauthx-0.7.2/trustauthx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 23:29:23.000000 trustauthx-0.7.2/trustauthx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33412 2024-04-03 23:29:23.000000 trustauthx-0.7.2/trustauthx/authlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 23:29:23.000000 trustauthx-0.7.2/trustauthx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 23:29:23.000000 trustauthx-0.7.2/trustauthx/llmai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-03 23:29:23.000000 trustauthx-0.7.2/trustauthx/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:29:32.036739 trustauthx-0.7.2/trustauthx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 23:29:32.000000 trustauthx-0.7.2/trustauthx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 23:29:32.000000 trustauthx-0.7.2/trustauthx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:29:32.000000 trustauthx-0.7.2/trustauthx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 23:29:32.000000 trustauthx-0.7.2/trustauthx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 23:29:32.000000 trustauthx-0.7.2/trustauthx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 23:29:32.000000 trustauthx-0.7.2/trustauthx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:18.140673 trustauthx-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 17:58:09.000000 trustauthx-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-05 17:58:18.140673 trustauthx-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-05 17:58:09.000000 trustauthx-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:58:18.140673 trustauthx-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-05 17:58:09.000000 trustauthx-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:18.136673 trustauthx-0.7.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-05 17:58:09.000000 trustauthx-0.7.3/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:18.140673 trustauthx-0.7.3/trustauthx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41319 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/authlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/llmai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:18.140673 trustauthx-0.7.3/trustauthx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/top_level.txt
```

### Comparing `trustauthx-0.7.2/LICENSE` & `trustauthx-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.2/PKG-INFO` & `trustauthx-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.7.2
+Version: 0.7.3
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trustauthx-0.7.2/README.md` & `trustauthx-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.2/trustauthx/authlite.py` & `trustauthx-0.7.3/trustauthx/authlite.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-import requests
-from requests.exceptions import HTTPError
-from jose import JWTError, jwt
-from jose.constants import ALGORITHMS
 import json
 import sqlite3
-from .scheme import *
-from functools import wraps
 import threading
 from dataclasses import asdict
+from functools import wraps
+from lib2to3.pgen2.parse import ParseError
+
+import requests
+from jose import JWTError, jwt
+from jose.constants import ALGORITHMS
+from requests.exceptions import HTTPError
+
+from .scheme import *
+
 
 class _EdgeDBRoleQuery:
     """
     A class for querying and managing roles and permissions.
 
     Attributes:
         in_memory (bool): Flag indicating whether to store the roles in-memory or in a SQLite database.
@@ -28,40 +32,48 @@
 
         validate(self, role_id, permission_key, permission_val):
             Validates a permission value for a given role ID and permission key.
 
         count_roles(self):
             Returns the number of roles stored.
     """
+
     total_roles = 0
     roles = None
 
     def __init__(self, roles, in_memory=True):
         """
         Initializes the _EdgeDBRoleQuery instance.
 
         Args:
             roles (List[Dict[str, Dict[str, str]]]): A list of dictionaries representing roles and their permissions.
             in_memory (bool, optional): Flag indicating whether to store the roles in-memory or in a SQLite database. Defaults to True.
         """
         self.in_memory = in_memory
         if self.in_memory:
-            self.__class__.roles = {role['rol_id']: role['permissions'][0] for role in roles}
+            self.__class__.roles = {
+                role["rol_id"]: role["permissions"][0] for role in roles
+            }
         else:
-            self.conn = sqlite3.connect(':memory:')  # replace ':memory:' with your database path
+            # replace ':memory:' with your database path
+            self.conn = sqlite3.connect(":memory:")
             self.cursor = self.conn.cursor()
-            self.cursor.execute("""
+            self.cursor.execute(
+                """
                 CREATE TABLE IF NOT EXISTS roles (
                     role_id TEXT PRIMARY KEY,
                     permissions TEXT
                 )
-            """)
+            """
+            )
             for role in roles:
                 for role_id, permissions in role.items():
-                    self.cursor.execute("INSERT INTO roles VALUES (?, ?)", (role_id, permissions))
+                    self.cursor.execute(
+                        "INSERT INTO roles VALUES (?, ?)", (role_id, permissions)
+                    )
             self.conn.commit()
         self.count_roles()
 
     def query(self, role_id=None, permission_key=None):
         """
         Queries the roles and permissions based on the provided role ID and/or permission key.
 
@@ -74,29 +86,41 @@
         """
         if self.in_memory:
             if role_id and permission_key:
                 return self.__class__.roles.get(role_id, {}).get(permission_key, None)
             elif role_id:
                 return self.__class__.roles.get(role_id, None)
             elif permission_key:
-                return {role_id: permissions[permission_key] for role_id, permissions in self.__class__.roles.items() if permission_key in permissions}
+                return {
+                    role_id: permissions[permission_key]
+                    for role_id, permissions in self.__class__.roles.items()
+                    if permission_key in permissions
+                }
             else:
                 return self.__class__.roles
         else:
             if role_id and permission_key:
-                self.cursor.execute("SELECT permissions FROM roles WHERE role_id = ?", (role_id,))
+                self.cursor.execute(
+                    "SELECT permissions FROM roles WHERE role_id = ?", (role_id,)
+                )
                 permissions = self.cursor.fetchone()
                 if permissions:
                     return permissions[0].get(permission_key, None)
             elif role_id:
-                self.cursor.execute("SELECT permissions FROM roles WHERE role_id = ?", (role_id,))
+                self.cursor.execute(
+                    "SELECT permissions FROM roles WHERE role_id = ?", (role_id,)
+                )
                 return self.cursor.fetchone()
             elif permission_key:
                 self.cursor.execute("SELECT * FROM roles")
-                return {role_id: permissions[permission_key] for role_id, permissions in self.cursor.fetchall() if permission_key in permissions}
+                return {
+                    role_id: permissions[permission_key]
+                    for role_id, permissions in self.cursor.fetchall()
+                    if permission_key in permissions
+                }
             else:
                 self.cursor.execute("SELECT * FROM roles")
                 return self.cursor.fetchall()
 
     def validate(self, role_id, permission_key, permission_val):
         """
         Validates a permission value for a given role ID and permission key.
@@ -106,17 +130,22 @@
             permission_key (str): The permission key to validate.
             permission_val (str): The expected permission value to validate.
 
         Returns:
             bool: True if the permission value matches the expected value, False otherwise.
         """
         if self.in_memory:
-            return self.__class__.roles.get(role_id, {}).get(permission_key, None) == permission_val
+            return (
+                self.__class__.roles.get(role_id, {}).get(permission_key, None)
+                == permission_val
+            )
         else:
-            self.cursor.execute("SELECT permissions FROM roles WHERE role_id = ?", (role_id,))
+            self.cursor.execute(
+                "SELECT permissions FROM roles WHERE role_id = ?", (role_id,)
+            )
             permissions = self.cursor.fetchone()
             if permissions:
                 return permissions[0].get(permission_key, None) == permission_val
 
     def count_roles(self):
         """
         Returns the number of roles stored.
@@ -134,42 +163,48 @@
             _EdgeDBRoleQuery.total_roles = r
             return r
 
     @classmethod
     def reinitialize_all(foreground=True):
         if foreground:
             for instance in AuthLiteClient.instances:
-                instance:AuthLiteClient = instance
+                instance: AuthLiteClient = instance
                 instance._re_init_roles()
         else:
+
             def target():
                 for instance in AuthLiteClient.instances:
-                    instance:AuthLiteClient = instance
+                    instance: AuthLiteClient = instance
                     instance._re_init_roles()
+
             thread = threading.Thread(target=target)
             thread.start()
 
     @staticmethod
     def _EDGE_Wrapper(func):
+
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Call the function
             response = func(*args, **kwargs)
             # Check for "X-EDGE"
             x_edge = response.headers.get("X-EDGE")
             if x_edge:
                 if int(x_edge) != _EdgeDBRoleQuery.total_roles:
-                    _EdgeDBRoleQuery.reinitialize_all() # Add data
+                    _EdgeDBRoleQuery.reinitialize_all()  # Add data
             return response
+
         return wrapper
 
+
 requests.get = _EdgeDBRoleQuery._EDGE_Wrapper(requests.get)
 requests.post = _EdgeDBRoleQuery._EDGE_Wrapper(requests.post)
 requests.delete = _EdgeDBRoleQuery._EDGE_Wrapper(requests.delete)
 
+
 class _Roles(_EdgeDBRoleQuery):
     """
     A class for managing roles and permissions in the EdgeDB system.
 
     Attributes:
         org_id (str): The organization ID associated with the roles.
         api_key (str): The API key for authentication.
@@ -190,17 +225,27 @@
 
         add_permission(self, rol_id, **Permission_):
             Adds a new permission to a role with the specified role ID.
 
         delete_permission(self, rol_id, **Permission_):
             Deletes a permission from a role with the specified role ID.
     """
+
     instances = []
 
-    def __init__(self, roles, org_id, api_key, signed_key, secret_key, API_BASE_URL, InMemory=True):
+    def __init__(
+        self,
+        roles,
+        org_id,
+        api_key,
+        signed_key,
+        secret_key,
+        API_BASE_URL,
+        InMemory=True,
+    ):
         """
         Initializes the _Roles instance.
 
         Args:
             roles (List[Dict[str, Dict[str, str]]]): A list of dictionaries representing roles and their permissions.
             org_id (str): The organization ID associated with the roles.
             api_key (str): The API key for authentication.
@@ -221,15 +266,15 @@
     def get_all_roles(self) -> GetAllRolesResponse:
         """
         Retrieves all roles and their permissions from the API.
 
         Returns:
             roles_list = List[Role]: A list of Role objects representing the roles and their permissions.roles
             roles_json_list = List[dict]: A list of dict representing the roles and their permissions
-        
+
         demo response ==> [
           {
             "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
             "rol_id": "rol_gCD_ebc6f7715bb14554",
             "name": "string",
             "permissions": [
               {
@@ -256,36 +301,38 @@
               },
               {
                 "maintainer": "administration"
               }
             ]
           }
         ]"""
-        url = f'{self.API_BASE_URL}/rbac/role'
-        headers = {'accept': 'application/json'}
+        url = f"{self.API_BASE_URL}/rbac/role"
+        headers = {"accept": "application/json"}
         params = {
-            'org_id': f'{self.org_id}',
-            'api_key': f'{self._api_key}',
-            'signed_key': f'{self._signed_key}'
+            "org_id": f"{self.org_id}",
+            "api_key": f"{self._api_key}",
+            "signed_key": f"{self._signed_key}",
         }
         response = requests.get(url, headers=headers, params=params)
         roles = [Role(**role_data) for role_data in response.json()]
-        return GetAllRolesResponse(roles_list=roles, roles_json_list=[asdict(role) for role in roles])
+        return GetAllRolesResponse(
+            roles_list=roles, roles_json_list=[asdict(role) for role in roles]
+        )
 
-    def add_role(self, name, **Permission_)->AddRoleResponse:
+    def add_role(self, name, **Permission_) -> AddRoleResponse:
         """
         Adds a new role with the specified name and permissions.
 
         Args:
             name (str): The name of the new role.
             **Permission_: Keyword arguments representing the permissions to be added to the new role.
 
         Returns:
             AddRoleResponse: An AddRoleResponse object representing the newly created role.
-            
+
         demo response ==> {
           "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
           "rol_id": "rol_rce_474ae9e59b3d49ce",
           "name": "string",
           "permissions": [
             {
               "user": "administration"
@@ -294,51 +341,45 @@
               "viewer": "administration"
             },
             {
               "maintainer": "administration"
             }
           ]
         }"""
-        url = f'{self.API_BASE_URL}/rbac/role'
-        headers = {
-            'accept': 'application/json',
-            'Content-Type': 'application/json'
-        }
+        url = f"{self.API_BASE_URL}/rbac/role"
+        headers = {"accept": "application/json", "Content-Type": "application/json"}
         params = {
-            'org_id': f'{self.org_id}',
-            'api_key': f'{self._api_key}',
-            'signed_key': f'{self._signed_key}'
+            "org_id": f"{self.org_id}",
+            "api_key": f"{self._api_key}",
+            "signed_key": f"{self._signed_key}",
         }
         permissions = [{k: v} for k, v in Permission_.items()]
-        data = {
-            "org_id": f'{self.org_id}',
-            "name": name,
-            "permissions": permissions
-        }
-        response = requests.post(url, headers=headers, params=params, data=json.dumps(data))
+        data = {"org_id": f"{self.org_id}", "name": name, "permissions": permissions}
+        response = requests.post(
+            url, headers=headers, params=params, data=json.dumps(data)
+        )
         role_data = response.json()
         permissions = [Permission(**p) for p in role_data.get("permissions", [])]
         return AddRoleResponse(
             org_id=role_data.get("org_id"),
             rol_id=role_data.get("rol_id"),
             name=role_data.get("name"),
-            permissions=[p.__dict__ for p in permissions]
+            permissions=[p.__dict__ for p in permissions],
         )
 
     def delete_role(self, rol_id) -> DeleteRoleResponse:
-
         """
         Deletes a role with the specified role ID.
 
         Args:
             rol_id (str): The ID of the role to be deleted.
 
         Returns:
             DeleteRoleResponse: A DeleteRoleResponse object representing the deleted role.
-        
+
         demo response ==> {
           "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
           "rol_id": "rol_YHV_78ae9006bcaa4c77",
           "name": "string",
           "permissions": [
             {
               "user": "administration"
@@ -347,133 +388,131 @@
               "viewer": "administration"
             },
             {
               "maintainer": "administration"
             }
           ]
         }"""
-        url = f'{self.API_BASE_URL}/rbac/role'
-        headers = {
-            'accept': 'application/json',
-            'Content-Type': 'application/json'
-        }
+        url = f"{self.API_BASE_URL}/rbac/role"
+        headers = {"accept": "application/json", "Content-Type": "application/json"}
         params = {
-            'org_id': f'{self.org_id}',
-            'api_key': f'{self._api_key}',
-            'signed_key': f'{self._signed_key}'
-        }
-        data = {
-            "org_id": f'{self.org_id}',
-            "rol_id": rol_id
+            "org_id": f"{self.org_id}",
+            "api_key": f"{self._api_key}",
+            "signed_key": f"{self._signed_key}",
         }
-        response = requests.delete(url, headers=headers, params=params, data=json.dumps(data))
+        data = {"org_id": f"{self.org_id}", "rol_id": rol_id}
+        response = requests.delete(
+            url, headers=headers, params=params, data=json.dumps(data)
+        )
         role_data = response.json()
         permissions = [Permission(**p) for p in role_data.get("permissions", [])]
         return DeleteRoleResponse(
             org_id=role_data.get("org_id"),
             rol_id=role_data.get("rol_id"),
             name=role_data.get("name"),
-            permissions=[p.__dict__ for p in permissions]
+            permissions=[p.__dict__ for p in permissions],
         )
 
-    def add_permission(self, rol_id, foreground=False, **Permission_) -> AddPermissionResponse:
+    def add_permission(
+        self, rol_id, foreground=False, **Permission_
+    ) -> AddPermissionResponse:
         """
         Adds a new permission to a role with the specified role ID.
 
         Args:
             rol_id (str): The ID of the role to which the permission should be added.
             **Permission_: Keyword arguments representing the permissions to be added.
 
         Returns:
             AddPermissionResponse: An AddPermissionResponse object representing the added permission.
-              
+
         demo response ==> {
           "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
           "rol_id": "rol_rce_474ae9e59b3d49ce",
           "permissions": [
             {
               "any": "view" ##only return added content
             }
           ]
         }"""
-        url = f'{self.API_BASE_URL}/rbac/permission'
-        headers = {
-            'accept': 'application/json',
-            'Content-Type': 'application/json'
-        }
+        url = f"{self.API_BASE_URL}/rbac/permission"
+        headers = {"accept": "application/json", "Content-Type": "application/json"}
         params = {
-            'org_id': f'{self.org_id}',
-            'api_key': f'{self._api_key}',
-            'signed_key': f'{self._signed_key}'
+            "org_id": f"{self.org_id}",
+            "api_key": f"{self._api_key}",
+            "signed_key": f"{self._signed_key}",
         }
         permissions = [{k: v} for k, v in Permission_.items()]
         data = {
-            "org_id": f'{self.org_id}',
+            "org_id": f"{self.org_id}",
             "rol_id": rol_id,
-            "permissions": permissions
+            "permissions": permissions,
         }
-        response = requests.post(url, headers=headers, params=params, data=json.dumps(data))
+        response = requests.post(
+            url, headers=headers, params=params, data=json.dumps(data)
+        )
         response_data = response.json()
         permissions = [Permission(**{k: v}) for k, v in permissions.items()]
         self.reinitialize_all(foreground)
         return AddPermissionResponse(
             org_id=response_data.get("org_id"),
             rol_id=response_data.get("rol_id"),
-            permissions=[p.__dict__ for p in permissions]
+            permissions=[p.__dict__ for p in permissions],
         )
 
-    def delete_permission(self, rol_id, foreground=False, **Permission_) -> DeletePermissionResponse:
+    def delete_permission(
+        self, rol_id, foreground=False, **Permission_
+    ) -> DeletePermissionResponse:
         """
         Deletes a permission from a role with the specified role ID.
 
         Args:
             rol_id (str): The ID of the role from which the permission should be deleted.
             **Permission_: Keyword arguments representing the permissions to be deleted.
 
         Returns:
             DeletePermissionResponse: A DeletePermissionResponse object representing the role with the deleted permission.
-        
+
         demo response ==> {
           "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
           "rol_id": "rol_rce_474ae9e59b3d49ce",
           "permissions": [
             {
               "user": "administration"
             },
             {
               "viewer": "administration"
             },
             {
               "maintainer": "administration"
             }
           ]
-        }""" #return full
-        url = f'{self.API_BASE_URL}/rbac/permission'
-        headers = {
-            'accept': 'application/json',
-            'Content-Type': 'application/json'
-        }
+        }"""  # return full
+        url = f"{self.API_BASE_URL}/rbac/permission"
+        headers = {"accept": "application/json", "Content-Type": "application/json"}
         params = {
-            'org_id': f'{self.org_id}',
-            'api_key': f'{self._api_key}',
-            'signed_key': f'{self._signed_key}'
+            "org_id": f"{self.org_id}",
+            "api_key": f"{self._api_key}",
+            "signed_key": f"{self._signed_key}",
         }
         permissions = [{k: v} for k, v in Permission_.items()]
         data = {
-            "org_id": f'{self.org_id}',
+            "org_id": f"{self.org_id}",
             "rol_id": rol_id,
-            "permissions": permissions
+            "permissions": permissions,
         }
-        response = requests.delete(url, headers=headers, params=params, data=json.dumps(data))
+        response = requests.delete(
+            url, headers=headers, params=params, data=json.dumps(data)
+        )
         self.reinitialize_all(foreground)
         return response.json()
-    
-class AuthLiteClient():
-    instances = []
 
+
+class AuthLiteClient:
+    instances = []
     """
     AuthLiteClient is a Python client for the TrustAuthX authentication service.
 
     Attributes:
         api_key (str): The API key used for authentication.
         secret_key (str): The secret key used for JWT encoding.
         org_id (str): The organization ID for generating authentication URLs.
@@ -521,79 +560,100 @@
         TokenCheck is a nested class for representing the state of access and refresh tokens.
 
         Attributes:
             access (str): The access token.
             refresh (str): The refresh token.
             state (bool): The state of the tokens (True if valid, False otherwise).
         """
-        access :str
-        refresh:str
-        state:bool
-
-    def __init__(self, api_key, secret_key, org_id=None, API_BASE_URL="https://api.trustauthx.com", in_memory=True):
-        """
-       Initializes the AuthLiteClient instance.
-
-       Args:
-           api_key (str): The API key used for authentication.
-           secret_key (str): The secret key used for JWT encoding.
-           org_id (str, optional): The organization ID for generating authentication URLs.
-           API_BASE_URL (str, optional): The base URL for the API. Defaults to "https://api.trustauthx.com".
-           in_memory (bool, optional): Flag indicating whether to store the roles in-memory or in a SQLite database. Defaults to True (ie. in-memory).
-       
-       """
-        self.jwt_encode = lambda key, data: jwt.encode(data, key=key, algorithm= ALGORITHMS.HS256)
-        self.jwt_decode = lambda key, data: jwt.decode(str(data), key=key, algorithms=ALGORITHMS.HS256)
+
+        access: str
+        refresh: str
+        state: bool
+
+    def __init__(
+        self,
+        api_key,
+        secret_key,
+        org_id=None,
+        API_BASE_URL="https://api.trustauthx.com",
+        in_memory=True,
+    ):
+        """
+        Initializes the AuthLiteClient instance.
+
+        Args:
+            api_key (str): The API key used for authentication.
+            secret_key (str): The secret key used for JWT encoding.
+            org_id (str, optional): The organization ID for generating authentication URLs.
+            API_BASE_URL (str, optional): The base URL for the API. Defaults to "https://api.trustauthx.com".
+            in_memory (bool, optional): Flag indicating whether to store the roles in-memory or in a SQLite database. Defaults to True (ie. in-memory).
+
+        """
+        self.jwt_encode = lambda key, data: jwt.encode(
+            data, key=key, algorithm=ALGORITHMS.HS256
+        )
+        self.jwt_decode = lambda key, data: jwt.decode(
+            str(data), key=key, algorithms=ALGORITHMS.HS256
+        )
         self._secret_key = secret_key
         self._api_key = api_key
         self.org_id = org_id
-        self._signed_key = self.jwt_encode(key=self._secret_key, data={"api_key":self._api_key})
+        self._signed_key = self.jwt_encode(
+            key=self._secret_key, data={"api_key": self._api_key}
+        )
         self.API_BASE_URL = API_BASE_URL
         self.in_memory = in_memory
-        self.Roles: _Roles = _Roles(roles=self._set_edge_roles(), org_id=self.org_id, 
-                                    api_key=self._api_key, signed_key=self._signed_key, 
-                                    secret_key=self._secret_key, API_BASE_URL=self.API_BASE_URL,
-                                    InMemory=in_memory)
+        self.Roles: _Roles = _Roles(
+            roles=self._set_edge_roles(),
+            org_id=self.org_id,
+            api_key=self._api_key,
+            signed_key=self._signed_key,
+            secret_key=self._secret_key,
+            API_BASE_URL=self.API_BASE_URL,
+            InMemory=in_memory,
+        )
         self.__class__.instances.append(self)
-        
+
     def generate_url(self) -> str:
         """
         Generates an authentication URL for the given organization.
 
         Returns:
             str: The generated authentication URL.
-        
+
         Raises:
             ValueError: If org_id is not provided.
         """
         # Generate an authentication url for the given org
-        if self.org_id:return f"https://app.trustauthx.com/widget/login/?org_id={self.org_id}"
-        else:raise ValueError("must provide org_id")
+        if self.org_id:
+            return f"https://app.trustauthx.com/widget/login/?org_id={self.org_id}"
+        else:
+            raise ValueError("must provide org_id")
 
     def generate_edit_user_url(self, access_token, url) -> str:
         """
         Generates an authentication URL for editing user settings.
 
         Args:
             access_token (str): The access token for authentication.
             url (str): The URL to be included in the generated URL.
 
         Returns:
             str: The generated authentication URL.
         """
         # Generate an authentication url for the given org
-        headers = {'accept': 'application/json'}
+        headers = {"accept": "application/json"}
         params = {
-            'AccessToken': access_token,
-            'api_key': self._api_key,
-            'signed_key': self._signed_key,
-            'url':url
-                 }
+            "AccessToken": access_token,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+            "url": url,
+        }
         url = f"{self.API_BASE_URL}/api/user/me/settings/"
-        req = requests.Request('GET', url, params=params, headers=headers).prepare()
+        req = requests.Request("GET", url, params=params, headers=headers).prepare()
         return req.url
 
     def re_auth(self, code):
         """
         Performs re-authentication with a provided code after the user finishes Editing profile.
 
         Args:
@@ -604,66 +664,71 @@
 
         Raises:
             HTTPError: If the request fails with an HTTP error status code.
         """
         url = f"{self.API_BASE_URL}/api/user/me/widget/re-auth/token"
         params = {
             "code": code,
-            'api_key': self._api_key,
-            'signed_key': self._signed_key
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
         }
         headers = {"accept": "application/json"}
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
-            rtn = self.jwt_decode(self._secret_key,response.json())
+            rtn = self.jwt_decode(self._secret_key, response.json())
             sub = json.loads(rtn["sub"])
             rtn.pop("sub")
             rtn["email"] = sub["email"]
             rtn["uid"] = sub["uid"]
             return rtn
-        else:raise HTTPError(
-            'Request failed with status code : {} \n this code contains a msg : {}'.format(
-                                                                            response.status_code, 
-                                                                            response.text)
-                            )
+        else:
+            raise HTTPError(
+                "Request failed with status code : {} \n this code contains a msg : {}".format(
+                    response.status_code, response.text
+                )
+            )
 
-    def get_user(self, token) -> dict:
+    def get_user(self, token, return_class=False) -> User | dict:
         """
         Validates the given authentication token and returns user data.
 
         Args:
             token (str): The authentication token to validate.
 
         Returns:
             dict: A dictionary containing user information.
             returns a dict containing 'access_token', 'refresh_token', 'img', 'sub'
         Raises:
             HTTPError: If the request fails with an HTTP error status code.
         """
         # Validate the given authentication token
-        url = f'{self.API_BASE_URL}/api/user/me/auth/data'
-        headers = {'accept': 'application/json'}
+        url = f"{self.API_BASE_URL}/api/user/me/auth/data"
+        headers = {"accept": "application/json"}
         params = {
-            'UserToken': token,
-            'api_key': self._api_key,
-            'signed_key': self._signed_key
-                 }
+            "UserToken": token,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+        }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
-            rtn = self.jwt_decode(self._secret_key,response.json())
+            rtn = self.jwt_decode(self._secret_key, response.json())
             sub = json.loads(rtn["sub"])
             rtn.pop("sub")
             rtn["email"] = sub["email"]
             rtn["uid"] = sub["uid"]
-            return rtn
-        else:raise HTTPError(
-            'Request failed with status code : {} \n this code contains a msg : {}'.format(
-                                                                            response.status_code, 
-                                                                            response.text)
-                            )
+            if not return_class:
+                return User(rtn).to_dict()
+            else:
+                return User(rtn)
+        else:
+            raise HTTPError(
+                "Request failed with status code : {} \n this code contains a msg : {}".format(
+                    response.status_code, response.text
+                )
+            )
 
     def get_user_data(self, AccessToken) -> dict:
         """
         Retrieves user data using an access token.
 
         Args:
             AccessToken (str): The access token for retrieving user data.
@@ -672,30 +737,31 @@
             dict: A dictionary containing user data.
 
         Raises:
             HTTPError: If the request fails with an HTTP error status code.
         """
         # Validate the given authentication token
         """returns a dict containing 'access_token', 'refresh_token', 'img', 'sub'"""
-        url = f'{self.API_BASE_URL}/api/user/me/data'
-        headers = {'accept': 'application/json'}
+        url = f"{self.API_BASE_URL}/api/user/me/data"
+        headers = {"accept": "application/json"}
         params = {
-            'AccessToken': AccessToken,
-            'api_key': self._api_key,
-            'signed_key': self._signed_key
-                 }
+            "AccessToken": AccessToken,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+        }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
-            rtn = self.jwt_decode(self._secret_key,response.json())
+            rtn = self.jwt_decode(self._secret_key, response.json())
             return rtn
-        else:raise HTTPError(
-            'Request failed with status code : {} \n this code contains a msg : {}'.format(
-                                                                            response.status_code, 
-                                                                            response.text)
-                            )
+        else:
+            raise HTTPError(
+                "Request failed with status code : {} \n this code contains a msg : {}".format(
+                    response.status_code, response.text
+                )
+            )
 
     def get_access_token_from_refresh_token(self, refresh_token):
         """
         Retrieves an access token from a refresh token.
 
         Args:
             refresh_token (str): The refresh token for obtaining a new access token.
@@ -703,51 +769,58 @@
         Returns:
             dict: A dictionary containing the new access and refresh tokens.
 
         Raises:
             HTTPError: If the request fails with an HTTP error status code.
         """
         # Store the given authentication token
-        url = f'{self.API_BASE_URL}/api/user/me/access/token/'
-        headers = {'accept': 'application/json'}
+        url = f"{self.API_BASE_URL}/api/user/me/access/token/"
+        headers = {"accept": "application/json"}
         params = {
-            'RefreshToken': refresh_token,
-            'api_key': self._api_key,
-            'signed_key': self._signed_key
-                 }
+            "RefreshToken": refresh_token,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+        }
         response = requests.get(url, headers=headers, params=params)
-        if response.status_code == 200:return response.json()
-        else:raise HTTPError(
-            'Request failed with status code : {} \n this code contains a msg : {}'.format(
-                                                                            response.status_code, 
-                                                                            response.text)
-                            )
+        if response.status_code == 200:
+            return response.json()
+        else:
+            raise HTTPError(
+                "Request failed with status code : {} \n this code contains a msg : {}".format(
+                    response.status_code, response.text
+                )
+            )
 
     def validate_access_token(self, access_token) -> bool:
         """
         Validates an access token.
 
         Args:
             access_token (str): The access token to validate.
 
         Returns:
             bool: True if the access token is valid, False otherwise.
         """
         # Store the given authentication token
-        url = f'{self.API_BASE_URL}/api/user/me/auth/validate/token'
-        headers = {'accept': 'application/json'}
+        url = f"{self.API_BASE_URL}/api/user/me/auth/validate/token"
+        headers = {"accept": "application/json"}
         params = {
-            'AccessToken': access_token,
-            'api_key': self._api_key,
-            'signed_key': self._signed_key
-                 }
+            "AccessToken": access_token,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+        }
         response = requests.get(url, headers=headers, params=params)
         return response.status_code == 200
 
-    def revoke_token(self,AccessToken:str=None, RefreshToken:str = None, revoke_all_tokens:bool = False) -> bool:
+    def revoke_token(
+        self,
+        AccessToken: str = None,
+        RefreshToken: str = None,
+        revoke_all_tokens: bool = False,
+    ) -> bool:
         """
         Revokes an access token or refresh token.
 
         Args:
             AccessToken (str, optional): The access token to revoke.
             RefreshToken (str, optional): The refresh token to revoke.
             revoke_all_tokens (bool): Whether to revoke all tokens associated with the user.
@@ -755,30 +828,36 @@
         Returns:
             bool: True if the token(s) were successfully revoked, False otherwise.
 
         Raises:
             HTTPError: If the request fails with an HTTP error status code.
             AttributeError: If neither AccessToken nor RefreshToken is provided.
         """
-        url = f'{self.API_BASE_URL}/api/user/me/token/'
-        headers = {'accept': 'application/json'}
-        if not AccessToken and not RefreshToken:raise AttributeError("must provide either AccessToken or RefreshToken")
-        tt=True if AccessToken else False
+        url = f"{self.API_BASE_URL}/api/user/me/token/"
+        headers = {"accept": "application/json"}
+        if not AccessToken and not RefreshToken:
+            raise AttributeError("must provide either AccessToken or RefreshToken")
+        tt = True if AccessToken else False
         t = AccessToken if AccessToken else RefreshToken
         params = {
-            'Token': t,
-            'api_key': self._api_key,
-            'signed_key': self._signed_key,
-            'AccessToken': tt,
-            'SpecificTokenOnly':not revoke_all_tokens,
-                }
+            "Token": t,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+            "AccessToken": tt,
+            "SpecificTokenOnly": not revoke_all_tokens,
+        }
         response = requests.delete(url, headers=headers, params=params)
-        if response.status_code == 200:return response.json()
-        else:raise HTTPError(
-            'Request failed with status code : {} \n this code contains a msg : {}'.format(response.status_code, response.text))
+        if response.status_code == 200:
+            return response.json()
+        else:
+            raise HTTPError(
+                "Request failed with status code : {} \n this code contains a msg : {}".format(
+                    response.status_code, response.text
+                )
+            )
 
     def validate_token_set(self, access_token, refresh_token) -> TokenCheck:
         """
         Validates a set of access and refresh tokens.
 
         Args:
             access_token (str): The access token to validate.
@@ -793,51 +872,250 @@
         try:
             d = self.TokenCheck()
             is_valid = self.validate_access_token(access_token)
             if not is_valid:
                 if refresh_token:
                     new_tokens = self.get_access_token_from_refresh_token(refresh_token)
                     d.state = False
-                    d.access = new_tokens['access_token']
-                    d.refresh = new_tokens['refresh_token']
+                    d.access = new_tokens["access_token"]
+                    d.refresh = new_tokens["refresh_token"]
                 return d
             else:
                 d.state = True
                 d.access = access_token
                 d.refresh = refresh_token
                 return d
         except:
-            raise HTTPError('both tokens are invalid login again')
-        
+            raise HTTPError("both tokens are invalid login again")
+
     def _set_edge_roles(self) -> list:
         # self.Roles
-        url = f'{self.API_BASE_URL}/rbac/role'
-        headers = {'accept': 'application/json'}
+        url = f"{self.API_BASE_URL}/rbac/role"
+        headers = {"accept": "application/json"}
         params = {
-            'org_id': f'{self.org_id}',
-            'api_key': f'{self._api_key}',
-            'signed_key': f'{self._signed_key}'
+            "org_id": f"{self.org_id}",
+            "api_key": f"{self._api_key}",
+            "signed_key": f"{self._signed_key}",
         }
         response = requests.get(url, headers=headers, params=params)
         roles = [Role(**role_data) for role_data in response.json()]
-        roles = GetAllRolesResponse(roles_list=roles, roles_json_list=[asdict(role) for role in roles])
+        roles = GetAllRolesResponse(
+            roles_list=roles, roles_json_list=[asdict(role) for role in roles]
+        )
         # print(roles.roles_json_list)
         return roles.roles_json_list
 
     def _re_init_roles(self) -> _Roles:
-        self.Roles: _Roles = _Roles(roles=self._set_edge_roles(), org_id=self.org_id, 
-                                    api_key=self._api_key, signed_key=self._signed_key, 
-                                    secret_key=self._secret_key, API_BASE_URL=self.API_BASE_URL,
-                                    InMemory=self.in_memory)
+        self.Roles: _Roles = _Roles(
+            roles=self._set_edge_roles(),
+            org_id=self.org_id,
+            api_key=self._api_key,
+            signed_key=self._signed_key,
+            secret_key=self._secret_key,
+            API_BASE_URL=self.API_BASE_URL,
+            InMemory=self.in_memory,
+        )
         return self.Roles
-    
-    def attach_role(self, uid, signoff_session_and_assign, refresh_token, access_token):
-        # add this and test
-        pass
-
-    def remove_role(self, uid, signoff_session_and_assign, refresh_token, access_token):
-        # add this and test
-        pass
-
-    def update_role(self, uid, signoff_session_and_assign, refresh_token, access_token):
-        # add this and test
-        pass
+
+    def attach_role(
+        self,
+        uid: str,
+        rol_ids: str | list,
+        signoff_session_and_assign=False,
+        refresh_token=None,
+        access_token=None,
+        return_class: bool = False,
+    ) -> dict | SignOffSessionReplace:
+        """
+        Attaches a role to a user.
+
+        Args:
+            uid (str): The user ID to attach the role to.
+            rol_ids (str | list): The ID(s) of the role(s) to attach.
+            signoff_session_and_assign (bool, optional): Whether to sign off the session and assign. Default is False.
+            refresh_token (str, optional): The refresh token for authentication.
+            access_token (str, optional): The access token for authentication.
+            return_class (bool, optional): Whether to return a class instance. Default is False.
+
+        Returns:
+            dict | SignOffSessionReplace: The response from the API, or a class instance if return_class is True.
+
+        Raises:
+            ParseError: If signoff_session_and_assign is True but refresh_token or access_token is not provided.
+        """
+        if signoff_session_and_assign:
+            if not refresh_token or not access_token:
+                raise ParseError(
+                    "must parse refresh_token and access_token if signoff_session_and_assign is true"
+                )
+        url = f"{self.API_BASE_URL}/rbac/assign/permission"
+        headers = {
+            "accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        params = {
+            "org_id": self.org_id,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+        }
+        rols = []
+        if isinstance(rol_ids) == str:
+            rols.append(rol_ids)
+        elif isinstance(rol_ids) == list:
+            rols = [i for i in rol_ids]
+        else:
+            raise TypeError()
+        data = {
+            "uid": uid,
+            "rol_id": rol_ids,
+            "inplace": [],
+            "signoff_session_and_assign": signoff_session_and_assign,
+            "AccessToken": access_token,
+            "RefreshToken": refresh_token,
+        }
+        response = requests.post(url, headers=headers, params=params, json=data)
+        if signoff_session_and_assign:
+            return response.json()
+        else:
+            if return_class:
+                return SignOffSessionReplace(response.json())
+            else:
+                return SignOffSessionReplace(response.json()).to_dict()
+
+    def remove_role(
+        self,
+        uid: str,
+        rol_ids: str | list,
+        signoff_session_and_assign=False,
+        refresh_token=None,
+        access_token=None,
+        return_class: bool = False,
+    ) -> dict | SignOffSessionReplace:
+        """
+        Removes a role from a user.
+
+        Args:
+            uid (str): The user ID to remove the role from.
+            rol_ids (str | list): The ID(s) of the role(s) to remove.
+            signoff_session_and_assign (bool, optional): Whether to sign off the session and assign. Default is False.
+            refresh_token (str, optional): The refresh token for authentication.
+            access_token (str, optional): The access token for authentication.
+            return_class (bool, optional): Whether to return a class instance. Default is False.
+
+        Returns:
+            dict | SignOffSessionReplace: The response from the API, or a class instance if return_class is True.
+
+        Raises:
+            ParseError: If signoff_session_and_assign is True but refresh_token or access_token is not provided.
+        """
+        if signoff_session_and_assign:
+            if not refresh_token or not access_token:
+                raise ParseError(
+                    "must parse refresh_token and access_token if signoff_session_and_assign is true"
+                )
+        url = f"{self.API_BASE_URL}/rbac/assign/permission"
+        headers = {
+            "accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        params = {
+            "org_id": self.org_id,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+        }
+        rols = []
+        if isinstance(rol_ids) == str:
+            rols.append(rol_ids)
+        elif isinstance(rol_ids) == list:
+            rols = [i for i in rol_ids]
+        else:
+            raise TypeError()
+        data = {
+            "uid": uid,
+            "rol_id": [],
+            "inplace": rol_ids,
+            "signoff_session_and_assign": signoff_session_and_assign,
+            "AccessToken": access_token,
+            "RefreshToken": refresh_token,
+        }
+        response = requests.post(url, headers=headers, params=params, json=data)
+        if signoff_session_and_assign:
+            return response.json()
+        else:
+            if return_class:
+                return SignOffSessionReplace(response.json())
+            else:
+                return SignOffSessionReplace(response.json()).to_dict()
+
+    def update_role(
+        self,
+        uid: str,
+        rol_ids_to_add: str | list,
+        rol_ids_to_remove: str | list,
+        signoff_session_and_assign=False,
+        refresh_token=None,
+        access_token=None,
+        return_class: bool = False,
+    ) -> dict | SignOffSessionReplace:
+        """
+        Updates a user's roles by adding and/or removing roles.
+
+        Args:
+            uid (str): The user ID to update roles for.
+            rol_ids_to_add (str | list): The ID(s) of the role(s) to add.
+            rol_ids_to_remove (str | list): The ID(s) of the role(s) to remove.
+            signoff_session_and_assign (bool, optional): Whether to sign off the session and assign. Default is False.
+            refresh_token (str, optional): The refresh token for authentication.
+            access_token (str, optional): The access token for authentication.
+            return_class (bool, optional): Whether to return a class instance. Default is False.
+
+        Returns:
+            dict | SignOffSessionReplace: The response from the API, or a class instance if return_class is True.
+
+        Raises:
+            ParseError: If signoff_session_and_assign is True but refresh_token or access_token is not provided.
+        """
+        if signoff_session_and_assign:
+            if not refresh_token or not access_token:
+                raise ParseError(
+                    "must parse refresh_token and access_token if signoff_session_and_assign is true"
+                )
+        url = f"{self.API_BASE_URL}/rbac/assign/permission"
+        headers = {
+            "accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        params = {
+            "org_id": self.org_id,
+            "api_key": self._api_key,
+            "signed_key": self._signed_key,
+        }
+        rols_add = []
+        if isinstance(rol_ids_to_add) == str:
+            rols_add.append(rol_ids_to_add)
+        elif isinstance(rol_ids_to_add) == list:
+            rols_add = [i for i in rol_ids_to_add]
+        else:
+            raise TypeError()
+        rols_rem = []
+        if isinstance(rol_ids_to_remove) == str:
+            rols_rem.append(rol_ids_to_remove)
+        elif isinstance(rol_ids_to_remove) == list:
+            rols_rem = [i for i in rol_ids_to_remove]
+        else:
+            raise TypeError()
+        data = {
+            "uid": uid,
+            "rol_id": rols_add,
+            "inplace": rols_rem,
+            "signoff_session_and_assign": signoff_session_and_assign,
+            "AccessToken": access_token,
+            "RefreshToken": refresh_token,
+        }
+        response = requests.post(url, headers=headers, params=params, json=data)
+        if signoff_session_and_assign:
+            return response.json()
+        else:
+            if return_class:
+                return SignOffSessionReplace(response.json())
+            else:
+                return SignOffSessionReplace(response.json()).to_dict()
```

### Comparing `trustauthx-0.7.2/trustauthx/cli.py` & `trustauthx-0.7.3/trustauthx/cli.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.2/trustauthx/llmai.py` & `trustauthx-0.7.3/trustauthx/llmai.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.2/trustauthx/scheme.py` & `trustauthx-0.7.3/trustauthx/scheme.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,126 @@
-from dataclasses import dataclass, asdict
-from typing import List, Dict, Union
+from dataclasses import asdict, dataclass
+from typing import Dict, List, Union
+
 
 @dataclass
 class Permission:
     """
     A class representing a permission object.
     """
+
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
 
+    def to_dict(self):
+        return asdict(self)
+
+
 @dataclass
 class Role:
     """
     A class representing a role object.
 
     Attributes:
         org_id (str): The organization ID associated with the role.
         rol_id (str): The unique identifier of the role.
         name (str): The name of the role.
         permissions (List[Permission]): A list of permissions associated with the role.
     """
+
     org_id: str
     rol_id: str
     name: str
     permissions: List[Permission]
 
+    def to_dict(self):
+        return asdict(self)
+
 
 @dataclass
 class GetAllRolesResponse:
     roles_list: List[Role]
     roles_json_list: List[Dict[str, Union[str, List[Dict[str, str]]]]]
 
+    def to_dict(self):
+        return asdict(self)
+
+
 @dataclass
 class AddRoleResponse:
     org_id: str
     rol_id: str
     name: str
     permissions: List[Permission]
 
+    def to_dict(self):
+        return asdict(self)
+
+
 @dataclass
 class DeleteRoleResponse:
     org_id: str
     rol_id: str
     name: str
     permissions: List[Permission]
 
+    def to_dict(self):
+        return asdict(self)
+
+
 @dataclass
 class AddPermissionResponse:
     org_id: str
     rol_id: str
     permissions: List[Dict[str, str]]
 
+    def to_dict(self):
+        return asdict(self)
+
+
 @dataclass
 class DeletePermissionResponse:
     org_id: str
     rol_id: str
     permissions: List[Permission]
 
+    def to_dict(self):
+        return asdict(self)
+
+
+@dataclass
+class User:
+    iss: str
+    jti: str
+    access_token: str
+    type: str
+    exp: float
+    refresh_token: str
+    refresh_exp: int
+    scope: List[str]
+    img: str
+    name: str
+    iat: int
+    email: str
+    uid: str
+
+    def to_dict(self):
+        return asdict(self)
+
+
+@dataclass
+class SignOffSessionReplace:
+    uid: str
+    access_token: str
+    refresh_token: str
+    role: List[str]
+
+    def to_dict(self):
+        return asdict(self)
 
 
 """# Demo data
 demo_get_all_roles_response = GetAllRolesResponse(roles=[
     {
         "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
         "rol_id": "rol_gCD_ebc6f7715bb14554",
```

### Comparing `trustauthx-0.7.2/trustauthx.egg-info/PKG-INFO` & `trustauthx-0.7.3/trustauthx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.7.2
+Version: 0.7.3
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

