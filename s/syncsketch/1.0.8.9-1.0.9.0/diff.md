# Comparing `tmp/syncsketch-1.0.8.9.tar.gz` & `tmp/syncsketch-1.0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/syncsketch-1.0.8.9.tar", last modified: Thu Sep 30 19:45:05 2021, max compression
+gzip compressed data, was "dist/syncsketch-1.0.9.0.tar", last modified: Tue Mar 21 19:25:19 2023, max compression
```

## Comparing `syncsketch-1.0.8.9.tar` & `syncsketch-1.0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bradyendres   (501) staff       (20)        0 2021-09-30 19:45:05.000000 syncsketch-1.0.8.9/
--rw-r--r--   0 bradyendres   (501) staff       (20)     5680 2021-09-30 19:45:05.000000 syncsketch-1.0.8.9/PKG-INFO
-drwxr-xr-x   0 bradyendres   (501) staff       (20)        0 2021-09-30 19:45:05.000000 syncsketch-1.0.8.9/syncsketch.egg-info/
--rw-r--r--   0 bradyendres   (501) staff       (20)     5680 2021-09-30 19:45:04.000000 syncsketch-1.0.8.9/syncsketch.egg-info/PKG-INFO
--rw-r--r--   0 bradyendres   (501) staff       (20)      235 2021-09-30 19:45:04.000000 syncsketch-1.0.8.9/syncsketch.egg-info/SOURCES.txt
--rw-r--r--   0 bradyendres   (501) staff       (20)       17 2021-09-30 19:45:04.000000 syncsketch-1.0.8.9/syncsketch.egg-info/requires.txt
--rw-r--r--   0 bradyendres   (501) staff       (20)       11 2021-09-30 19:45:04.000000 syncsketch-1.0.8.9/syncsketch.egg-info/top_level.txt
--rw-r--r--   0 bradyendres   (501) staff       (20)        1 2021-09-30 19:45:04.000000 syncsketch-1.0.8.9/syncsketch.egg-info/dependency_links.txt
--rw-r--r--   0 bradyendres   (501) staff       (20)     4181 2021-09-30 19:12:44.000000 syncsketch-1.0.8.9/README.md
--rw-r--r--   0 bradyendres   (501) staff       (20)      682 2021-09-30 18:51:36.000000 syncsketch-1.0.8.9/setup.py
--rw-r--r--   0 bradyendres   (501) staff       (20)       38 2021-09-30 19:45:05.000000 syncsketch-1.0.8.9/setup.cfg
-drwxr-xr-x   0 bradyendres   (501) staff       (20)        0 2021-09-30 19:45:05.000000 syncsketch-1.0.8.9/syncsketch/
--rw-r--r--   0 bradyendres   (501) staff       (20)      341 2021-09-30 18:51:56.000000 syncsketch-1.0.8.9/syncsketch/__init__.py
--rw-r--r--   0 bradyendres   (501) staff       (20)    38375 2021-09-30 19:12:10.000000 syncsketch-1.0.8.9/syncsketch/syncsketch.py
+drwxr-xr-x   0 eric.palakovich.carr   (501) staff       (20)        0 2023-03-21 19:25:19.000000 syncsketch-1.0.9.0/
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)     7958 2023-03-21 19:25:19.000000 syncsketch-1.0.9.0/PKG-INFO
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)     6091 2023-02-02 15:56:35.000000 syncsketch-1.0.9.0/README.md
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)       38 2023-03-21 19:25:19.000000 syncsketch-1.0.9.0/setup.cfg
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)      690 2023-03-21 19:15:20.000000 syncsketch-1.0.9.0/setup.py
+drwxr-xr-x   0 eric.palakovich.carr   (501) staff       (20)        0 2023-03-21 19:25:19.000000 syncsketch-1.0.9.0/syncsketch/
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)      371 2023-03-21 19:16:17.000000 syncsketch-1.0.9.0/syncsketch/__init__.py
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)    43979 2023-03-21 19:16:36.000000 syncsketch-1.0.9.0/syncsketch/syncsketch.py
+drwxr-xr-x   0 eric.palakovich.carr   (501) staff       (20)        0 2023-03-21 19:25:19.000000 syncsketch-1.0.9.0/syncsketch.egg-info/
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)     7958 2023-03-21 19:25:18.000000 syncsketch-1.0.9.0/syncsketch.egg-info/PKG-INFO
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)      235 2023-03-21 19:25:18.000000 syncsketch-1.0.9.0/syncsketch.egg-info/SOURCES.txt
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)        1 2023-03-21 19:25:18.000000 syncsketch-1.0.9.0/syncsketch.egg-info/dependency_links.txt
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)       17 2023-03-21 19:25:18.000000 syncsketch-1.0.9.0/syncsketch.egg-info/requires.txt
+-rw-r--r--   0 eric.palakovich.carr   (501) staff       (20)       11 2023-03-21 19:25:18.000000 syncsketch-1.0.9.0/syncsketch.egg-info/top_level.txt
```

### Comparing `syncsketch-1.0.8.9/PKG-INFO` & `syncsketch-1.0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: syncsketch
-Version: 1.0.8.9
+Version: 1.0.9.0
 Summary: SyncSketch Python API
 Home-page: https://github.com/syncsketch/python-api
 Author: Philip Floetotto
 Author-email: phil@syncsketch.com
 License: LICENSE.txt
 Description: # Syncsketch Python API
         
-        This package provides methods to communicate with the syncsketch servers and wraps CRUD (create, reade, update, delete) methods to interact with Reviews.
+        This package provides methods to communicate with the syncsketch servers and wraps CRUD (create, read, update, delete) methods to interact with Reviews.
         
         # Overview
         
         SyncSketch is a syncronized visual review tool for the Film/TV/Games industry.
         
         API access requires an enterprise level account.  For help or more info reach out to us.
         
@@ -30,44 +30,90 @@
         
         #### Installation
         
         Install using `pip`...
         
             pip install syncsketch
         
+        ### Data hierarchy
+        
+        Within SyncSketch there is a basic data hierarchy that makes it easy to manage your resources
+        
+        - Account (aka Workspace)
+        - Project
+        - Review
+        - ReviewItem (many-to-many connection table)
+        - Item
+        - Frame (aka comment or sketch)
+        
+        Users can be connected to a workspace and/or project, and may have different permissions on each connection.
+        It's important to know which connections and permissions your api user has to ensure you can build your integration.
+        You can find these permissions in the website or ask an admin from your project/workspace.
+        
+        What does this mean?
+        
+        _These depend on the specific permission level_
+        
+        - Account/Workspace connection means you can
+          - Edit settings on the workspace
+          - Invite new workspace level users
+          - Manage projects in the account
+          - Workspace level users also get all the permissions listed below in projects
+        - Project connection means you can
+          - Edit settings on the project
+          - Invite new project level users
+          - Manage reviews in the project
+          - Manage items in the reviews
+          - Manage comments or sketches on items
         
         ### Basic Examples
         
+        This page includes simple examples to get you started working with our api, but does not show all the methods or parameters that you can use.
+        We recommend you read the [source code](https://github.com/syncsketch/python-api/blob/master/syncsketch/syncsketch.py) to see all options. 
         
         #### Authentication
-        Before we can start working, we need to get an `API_KEY` which you can obtain from the syncsketch [settings page](https://syncsketch.com/pro/#userProfile/settingsTab). Follow the given link, login and scroll down to the bottom headline `Developer Options` to see your 40 character API-Key.
+        Before we can start working, we need to get an `API_KEY` which you can obtain from the syncsketch [settings page](https://syncsketch.com/pro/#/userProfile/settings). Follow the given link, login and scroll down to the bottom headline `Developer Options` to see your 40 character API-Key.
         
         
         Setting up a connection with your SyncSketch projects is as easy as following. 
         
             from syncsketch import SyncSketchAPI
             
             username = "username"
             api_key = "api-key-123"
             
             s = SyncSketchAPI(username, api_key)
             
+            # Verify your credentials work
             s.is_connected()
         
+            # Display your current user data
+            s.get_current_user()
+        
         If you got a `200` response, you successfully connected to the syncsketch server! You can proceed with the next examples. We will skip the setup code for the next examples and the snippets will rely on each other, so make sure you run them one by one.
         
         
         ##### 1) Choose your account
         
-        Before we can create/read/update/delete reviews, we need to select an account
+        Before we can create/read/update/delete projects and/or reviews, we need to select an Account (internal api name for Workspace)
         
+            # Get a list of workspaces your user has access to
             accounts = s.get_accounts()
             first_account = accounts["objects"][0]
         
-        ##### 2) Create a project
+        IMPORTANT: You may not see anything in the array returned from `s.get_accounts()`.
+        This means your user is connected directly to the project(s) and not an account.
+        If so you can skip this and proceed to fetching `s.get_projects()`.
+        
+        ##### 2) Interact with Projects
+        
+        Projects are nested under an Account/Workspace
+        
+            # List projects your user has access to
+            s.get_projects()
         
         Let's create a project with the selected account
         
             project = s.create_project(first_account["id"], 'DEV Example Project', 'DEV API Testing')
         
         This creates a new Project called `Dev Example Project` with the description `DEV API Testing`
         
@@ -90,15 +136,15 @@
         You can upload a file to the created review with the review id, we provided one example file in this repo under `examples/test.webm` for testing.
         
             item_data = s.add_media(review['id'],'examples/test.webm')
         
         
         If all steps were successful, you should see the following in the web-app. 
         
-        ![alt text](https://github.com/syncsketch/python-api/blob/documentation/examples/ressources/exampleResult.jpg?raw=true)
+        ![alt text](https://github.com/syncsketch/python-api/blob/documentation/examples/resources/exampleResult.jpg?raw=true)
         
         ### Additional Examples
         
         ##### Adding a user to the project
             addedUsers = s.add_users_to_project(
                 project_id,
                 [
```

### Comparing `syncsketch-1.0.8.9/syncsketch.egg-info/PKG-INFO` & `syncsketch-1.0.9.0/syncsketch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: syncsketch
-Version: 1.0.8.9
+Version: 1.0.9.0
 Summary: SyncSketch Python API
 Home-page: https://github.com/syncsketch/python-api
 Author: Philip Floetotto
 Author-email: phil@syncsketch.com
 License: LICENSE.txt
 Description: # Syncsketch Python API
         
-        This package provides methods to communicate with the syncsketch servers and wraps CRUD (create, reade, update, delete) methods to interact with Reviews.
+        This package provides methods to communicate with the syncsketch servers and wraps CRUD (create, read, update, delete) methods to interact with Reviews.
         
         # Overview
         
         SyncSketch is a syncronized visual review tool for the Film/TV/Games industry.
         
         API access requires an enterprise level account.  For help or more info reach out to us.
         
@@ -30,44 +30,90 @@
         
         #### Installation
         
         Install using `pip`...
         
             pip install syncsketch
         
+        ### Data hierarchy
+        
+        Within SyncSketch there is a basic data hierarchy that makes it easy to manage your resources
+        
+        - Account (aka Workspace)
+        - Project
+        - Review
+        - ReviewItem (many-to-many connection table)
+        - Item
+        - Frame (aka comment or sketch)
+        
+        Users can be connected to a workspace and/or project, and may have different permissions on each connection.
+        It's important to know which connections and permissions your api user has to ensure you can build your integration.
+        You can find these permissions in the website or ask an admin from your project/workspace.
+        
+        What does this mean?
+        
+        _These depend on the specific permission level_
+        
+        - Account/Workspace connection means you can
+          - Edit settings on the workspace
+          - Invite new workspace level users
+          - Manage projects in the account
+          - Workspace level users also get all the permissions listed below in projects
+        - Project connection means you can
+          - Edit settings on the project
+          - Invite new project level users
+          - Manage reviews in the project
+          - Manage items in the reviews
+          - Manage comments or sketches on items
         
         ### Basic Examples
         
+        This page includes simple examples to get you started working with our api, but does not show all the methods or parameters that you can use.
+        We recommend you read the [source code](https://github.com/syncsketch/python-api/blob/master/syncsketch/syncsketch.py) to see all options. 
         
         #### Authentication
-        Before we can start working, we need to get an `API_KEY` which you can obtain from the syncsketch [settings page](https://syncsketch.com/pro/#userProfile/settingsTab). Follow the given link, login and scroll down to the bottom headline `Developer Options` to see your 40 character API-Key.
+        Before we can start working, we need to get an `API_KEY` which you can obtain from the syncsketch [settings page](https://syncsketch.com/pro/#/userProfile/settings). Follow the given link, login and scroll down to the bottom headline `Developer Options` to see your 40 character API-Key.
         
         
         Setting up a connection with your SyncSketch projects is as easy as following. 
         
             from syncsketch import SyncSketchAPI
             
             username = "username"
             api_key = "api-key-123"
             
             s = SyncSketchAPI(username, api_key)
             
+            # Verify your credentials work
             s.is_connected()
         
+            # Display your current user data
+            s.get_current_user()
+        
         If you got a `200` response, you successfully connected to the syncsketch server! You can proceed with the next examples. We will skip the setup code for the next examples and the snippets will rely on each other, so make sure you run them one by one.
         
         
         ##### 1) Choose your account
         
-        Before we can create/read/update/delete reviews, we need to select an account
+        Before we can create/read/update/delete projects and/or reviews, we need to select an Account (internal api name for Workspace)
         
+            # Get a list of workspaces your user has access to
             accounts = s.get_accounts()
             first_account = accounts["objects"][0]
         
-        ##### 2) Create a project
+        IMPORTANT: You may not see anything in the array returned from `s.get_accounts()`.
+        This means your user is connected directly to the project(s) and not an account.
+        If so you can skip this and proceed to fetching `s.get_projects()`.
+        
+        ##### 2) Interact with Projects
+        
+        Projects are nested under an Account/Workspace
+        
+            # List projects your user has access to
+            s.get_projects()
         
         Let's create a project with the selected account
         
             project = s.create_project(first_account["id"], 'DEV Example Project', 'DEV API Testing')
         
         This creates a new Project called `Dev Example Project` with the description `DEV API Testing`
         
@@ -90,15 +136,15 @@
         You can upload a file to the created review with the review id, we provided one example file in this repo under `examples/test.webm` for testing.
         
             item_data = s.add_media(review['id'],'examples/test.webm')
         
         
         If all steps were successful, you should see the following in the web-app. 
         
-        ![alt text](https://github.com/syncsketch/python-api/blob/documentation/examples/ressources/exampleResult.jpg?raw=true)
+        ![alt text](https://github.com/syncsketch/python-api/blob/documentation/examples/resources/exampleResult.jpg?raw=true)
         
         ### Additional Examples
         
         ##### Adding a user to the project
             addedUsers = s.add_users_to_project(
                 project_id,
                 [
```

### Comparing `syncsketch-1.0.8.9/README.md` & `syncsketch-1.0.9.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Syncsketch Python API
 
-This package provides methods to communicate with the syncsketch servers and wraps CRUD (create, reade, update, delete) methods to interact with Reviews.
+This package provides methods to communicate with the syncsketch servers and wraps CRUD (create, read, update, delete) methods to interact with Reviews.
 
 # Overview
 
 SyncSketch is a syncronized visual review tool for the Film/TV/Games industry.
 
 API access requires an enterprise level account.  For help or more info reach out to us.
 
@@ -22,44 +22,90 @@
 
 #### Installation
 
 Install using `pip`...
 
     pip install syncsketch
 
+### Data hierarchy
+
+Within SyncSketch there is a basic data hierarchy that makes it easy to manage your resources
+
+- Account (aka Workspace)
+- Project
+- Review
+- ReviewItem (many-to-many connection table)
+- Item
+- Frame (aka comment or sketch)
+
+Users can be connected to a workspace and/or project, and may have different permissions on each connection.
+It's important to know which connections and permissions your api user has to ensure you can build your integration.
+You can find these permissions in the website or ask an admin from your project/workspace.
+
+What does this mean?
+
+_These depend on the specific permission level_
+
+- Account/Workspace connection means you can
+  - Edit settings on the workspace
+  - Invite new workspace level users
+  - Manage projects in the account
+  - Workspace level users also get all the permissions listed below in projects
+- Project connection means you can
+  - Edit settings on the project
+  - Invite new project level users
+  - Manage reviews in the project
+  - Manage items in the reviews
+  - Manage comments or sketches on items
 
 ### Basic Examples
 
+This page includes simple examples to get you started working with our api, but does not show all the methods or parameters that you can use.
+We recommend you read the [source code](https://github.com/syncsketch/python-api/blob/master/syncsketch/syncsketch.py) to see all options. 
 
 #### Authentication
-Before we can start working, we need to get an `API_KEY` which you can obtain from the syncsketch [settings page](https://syncsketch.com/pro/#userProfile/settingsTab). Follow the given link, login and scroll down to the bottom headline `Developer Options` to see your 40 character API-Key.
+Before we can start working, we need to get an `API_KEY` which you can obtain from the syncsketch [settings page](https://syncsketch.com/pro/#/userProfile/settings). Follow the given link, login and scroll down to the bottom headline `Developer Options` to see your 40 character API-Key.
 
 
 Setting up a connection with your SyncSketch projects is as easy as following. 
 
     from syncsketch import SyncSketchAPI
     
     username = "username"
     api_key = "api-key-123"
     
     s = SyncSketchAPI(username, api_key)
     
+    # Verify your credentials work
     s.is_connected()
 
+    # Display your current user data
+    s.get_current_user()
+
 If you got a `200` response, you successfully connected to the syncsketch server! You can proceed with the next examples. We will skip the setup code for the next examples and the snippets will rely on each other, so make sure you run them one by one.
 
 
 ##### 1) Choose your account
 
-Before we can create/read/update/delete reviews, we need to select an account
+Before we can create/read/update/delete projects and/or reviews, we need to select an Account (internal api name for Workspace)
 
+    # Get a list of workspaces your user has access to
     accounts = s.get_accounts()
     first_account = accounts["objects"][0]
 
-##### 2) Create a project
+IMPORTANT: You may not see anything in the array returned from `s.get_accounts()`.
+This means your user is connected directly to the project(s) and not an account.
+If so you can skip this and proceed to fetching `s.get_projects()`.
+
+##### 2) Interact with Projects
+
+Projects are nested under an Account/Workspace
+
+    # List projects your user has access to
+    s.get_projects()
 
 Let's create a project with the selected account
 
     project = s.create_project(first_account["id"], 'DEV Example Project', 'DEV API Testing')
 
 This creates a new Project called `Dev Example Project` with the description `DEV API Testing`
 
@@ -82,15 +128,15 @@
 You can upload a file to the created review with the review id, we provided one example file in this repo under `examples/test.webm` for testing.
 
     item_data = s.add_media(review['id'],'examples/test.webm')
 
 
 If all steps were successful, you should see the following in the web-app. 
 
-![alt text](https://github.com/syncsketch/python-api/blob/documentation/examples/ressources/exampleResult.jpg?raw=true)
+![alt text](https://github.com/syncsketch/python-api/blob/documentation/examples/resources/exampleResult.jpg?raw=true)
 
 ### Additional Examples
 
 ##### Adding a user to the project
     addedUsers = s.add_users_to_project(
         project_id,
         [
```

### Comparing `syncsketch-1.0.8.9/setup.py` & `syncsketch-1.0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # @Author: yafes
 # @Date:   2018-11-20 17:36:16
-# @Last Modified by:   Brady Endres
-# @Last Modified time: 2021-08-30
+# @Last Modified by:   Eric Palakovich Carr
+# @Last Modified time: 2023-03-21
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme_text = f.read()
 
 setup(
     name="syncsketch",
-    version="1.0.8.9",
+    version="1.0.9.0",
     description="SyncSketch Python API",
     author="Philip Floetotto",
     author_email="phil@syncsketch.com",
     long_description=readme_text,
     long_description_content_type="text/markdown",
     url="https://github.com/syncsketch/python-api",
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
```

### Comparing `syncsketch-1.0.8.9/syncsketch/syncsketch.py` & `syncsketch-1.0.9.0/syncsketch/syncsketch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 """Summary"""
 # @Author: floepi
 # @Date:   2015-06-04 17:42:44
-# @Last Modified by:   Brady Endres
-# @Last Modified time: 2021-08-30
+# @Last Modified by:   Eric Palakovich Carr
+# @Last Modified time: 2023-03-21
 #!/usr/local/bin/python
 
 from __future__ import absolute_import, division, print_function
 
-import os
 import json
+import mimetypes
+import os
 import time
+from io import open
 
 import requests
 
 try:
     # Python 2
     from urllib import urlencode
 except:
@@ -74,32 +76,59 @@
             self.api_params = {"api_key": self.api_key, "username": self.user_auth}
 
         self.api_version = api_version
         self.debug = debug
         self.HOST = host
 
     def get_api_base_url(self, api_version=None):
-        return self.HOST + "/api/{}/".format(api_version or self.api_version)
+        return self.join_url_path(self.HOST, "/api/{}/".format(api_version or self.api_version))
+
+    @staticmethod
+    def join_url_path(base, *path_segments):
+        """Takes one more more strings and returns a properly terminated url path. Handles strings regardless
+        of whether they are "/" prefixed/terminated or not.
+
+        >>> SyncSketchAPI.join_url_path("abc")
+        "abc/"
+        >>> SyncSketchAPI.join_url_path("abc", "123")
+        "abc/123/"
+        >>> SyncSketchAPI.join_url_path("abc", "123", "/xyz/")
+        "abc/123/xyz/"
+
+        :param str base: The "base" path to append to.
+        :param path_segments: Additional strings to be appened to the path.
+        :type path_segments: List[str]
+
+        :returns: A "/" terminated string containing base and path_segments delimited by "/".
+        """
+        # remove preceeding "/" from entries to avoid absolute path behavior with os.path.join
+        # and append an empty string so that os.path.join will add a terminating "/" if needed
+        path_segments = [
+            path_segment[1:] if path_segment.startswith("/") else path_segment
+            for path_segment in path_segments
+        ] + [""]
+        return os.path.join(
+            base, *path_segments
+        )
+
+    def _get_unversioned_api_url(self, path):
+        return self.join_url_path(self.HOST, path)
 
     def _get_json_response(
         self,
         url,
         method=None,
         getData=None,
         postData=None,
         patchData=None,
         putData=None,
-        api_version=None,
         content_type="application/json",
         raw_response=False,
     ):
-        url = self.get_api_base_url(api_version) + url
-
-        if not url.endswith("/"):
-            url += "/"
+        url = self._get_unversioned_api_url(url)
 
         params = self.api_params.copy()
 
         # Update headers with custom content-type
         headers = self.headers.copy()
         headers["Content-Type"] = content_type
 
@@ -137,15 +166,15 @@
     def is_connected(self):
         """
         Convenience function to check if the API is connected to SyncSketch
         Will check against Status Code 200 and return False if not which most likely would be
         and authorization error
         :return:
         """
-        url = "person/connected"
+        url = "/api/v1/person/connected/"
         params = self.api_params.copy()
 
         if self.debug:
             print("URL: %s, params: %s" % (url, params))
 
         r = self._get_json_response(url, raw_response=True)
         return r.status_code == 200
@@ -153,28 +182,28 @@
     def get_tree(self, withItems=False):
         """
             get nested tree of account, projects, reviews and optionally items for the current user
         :param withItems:
         :return:
         """
         get_params = {"fetchItems": 1} if withItems else {}
-        return self._get_json_response("person/tree", getData=get_params)
+        return self._get_json_response("/api/v1/person/tree/", getData=get_params)
 
     """
     Accounts
     """
 
     def get_accounts(self):
         """Summary
 
         Returns:
             TYPE: Account
         """
         get_params = {"active": 1}
-        return self._get_json_response("account", getData=get_params)
+        return self._get_json_response("/api/v1/account/", getData=get_params)
 
     def update_account(self, account_id, data):
         """
         Update a project
 
         Args:
             account_id (TYPE): the id of the item
@@ -183,39 +212,42 @@
         Returns:
             TYPE: item
         """
         if not isinstance(data, dict):
             print("Please make sure you pass a dict as data")
             return False
 
-        return self._get_json_response("account/%s" % account_id, patchData=data)
+        return self._get_json_response("/api/v1/account/%s/" % account_id, patchData=data)
 
     """
     Projects
     """
 
-    def create_project(self, account_id, name, description="", data={}):
+    def create_project(self, account_id, name, description="", data=None):
         """
         Add a project to your account. Please make sure to pass the accountId which you can query using the getAccounts command.
 
         :param account_id: Number - id of the account to connect with
         :param name: String
         :param description: String
         :param data: Dict with additional information e.g is_public. Find out more about available fields at /api/v1/project/schema/.
         :return:
         """
+        if data is None:
+            data = {}
+
         post_data = {
             "name": name,
             "description": description,
             "account_id": account_id,
         }
 
         post_data.update(data)
 
-        return self._get_json_response("project", postData=post_data)
+        return self._get_json_response("/api/v1/project/", postData=post_data)
 
     def get_projects(
         self,
         include_deleted=False,
         include_archived=False,
         include_tags=False,
         include_connections=False,
@@ -249,41 +281,41 @@
         if include_archived:
             del get_params["active"]
             del get_params["is_archived"]
 
         if include_tags:
             get_params["include_tags"] = 1
 
-        return self._get_json_response("project", getData=get_params)
+        return self._get_json_response("/api/v1/project/", getData=get_params)
 
     def get_projects_by_name(self, name):
         """
         Get a project by name regardless of status
 
         Returns:
             TYPE: Dict with meta information and an array of found projects
         """
-        get_params = {"name": name}
-        return self._get_json_response("project", getData=get_params)
+        get_params = {"name__istartswith": name}
+        return self._get_json_response("/api/v1/project/", getData=get_params)
 
     def get_project_by_id(self, project_id):
         """
         Get single project by id
         :param project_id: Number
         :return:
         """
-        return self._get_json_response("project/%s" % project_id)
+        return self._get_json_response("/api/v1/project/%s/" % project_id)
 
     def get_project_storage(self, project_id):
         """
         Get project storage usage in bytes
         :param project_id: Number
         :return:
         """
-        return self._get_json_response("project/%s/storage" % project_id, api_version="v2")
+        return self._get_json_response("/api/v2/project/%s/storage/" % project_id)
 
     def update_project(self, project_id, data):
         """
         Update a project
 
         Args:
             project_id (TYPE): the id of the item
@@ -292,23 +324,23 @@
         Returns:
             TYPE: item
         """
         if not isinstance(data, dict):
             print("Please make sure you pass a dict as data")
             return False
 
-        return self._get_json_response("project/%s" % project_id, patchData=data)
+        return self._get_json_response("/api/v1/project/%s/" % project_id, patchData=data)
 
     def delete_project(self, project_id):
         """
         Get single project by id.
         :param project_id: Number
         :return:
         """
-        return self._get_json_response("project/%s" % project_id, patchData=dict(active=0))
+        return self._get_json_response("/api/v1/project/%s/" % project_id, patchData=dict(active=False))
 
     def duplicate_project(self, project_id, name=None, copy_reviews=False, copy_users=False, copy_settings=False):
         """
         Create a new project from an existing project
 
         :param project_id: Int
         :param name: Str
@@ -322,93 +354,96 @@
             reviews=copy_reviews,
             users=copy_users,
             settings=copy_settings,
         )
         if name:
             config["name"] = name
 
-        return self._get_json_response("project/%s/duplicate/" % project_id, api_version="v2", postData=config)
+        return self._get_json_response("/api/v2/project/%s/duplicate/" % project_id, postData=config)
 
     def archive_project(self, project_id):
         """
         Archive a project
 
         Args:
             project_id (TYPE): the id of the item
 
         Returns:
             TYPE: item
         """
 
-        return self._get_json_response("project/%s" % project_id, patchData=dict(is_archived=1))
+        return self._get_json_response("/api/v1/project/%s/" % project_id, patchData=dict(is_archived=True))
 
     def restore_project(self, project_id):
         """
         Restore (unarchive) a project
 
         Args:
             project_id (TYPE): the id of the item
             data (dict): normal dict with data for item
 
         Returns:
             TYPE: item
         """
 
-        return self._get_json_response("project/%s" % project_id, patchData=dict(is_archived=0))
+        return self._get_json_response("/api/v1/project/%s/" % project_id, patchData=dict(is_archived=False))
 
     """
     Reviews
     """
 
-    def create_review(self, project_id, name, description="", data={}):
+    def create_review(self, project_id, name, description="", data=None):
+        if data is None:
+            data = {}
+
         postData = {
             "project": "/api/%s/project/%s/" % (self.api_version, project_id),
             "name": name,
             "description": description,
         }
 
         postData.update(data)
 
-        return self._get_json_response("review", postData=postData)
+        return self._get_json_response("/api/v1/review/", postData=postData)
 
     def get_reviews_by_project_id(self, project_id, limit=100, offset=0):
         """
         Get list of reviews by project id.
         :param project_id: Number
         :return: Dict with meta information and an array of found projects
         """
         get_params = {
             "project__id": project_id, "project__active": 1, "project__is_archived": 0, "limit": limit, "offset": offset
         }
-        return self._get_json_response("review", getData=get_params)
+        return self._get_json_response("/api/v1/review/", getData=get_params)
 
     def get_review_by_name(self, name):
         """
         Get reviews by name using a case insensitive startswith query
         :param name: String - Name of the review
         :return: Dict with meta information and an array of found projects
         """
         get_params = {"name__istartswith": name}
-        return self._get_json_response("review", getData=get_params)
+        return self._get_json_response("/api/v1/review/", getData=get_params)
 
     def get_review_by_id(self, review_id):
         """
         Get single review by id.
         :param review_id: Number
         :return: Review Dict
         """
-        return self._get_json_response("review/%s" % review_id)
+        return self._get_json_response("/api/v1/review/%s/" % review_id)
 
     def get_review_storage(self, review_id):
         """
         Get review storage usage in bytes
         :param review_id: Number
         :return:
         """
-        return self._get_json_response("review/%s/storage" % review_id, api_version="v2")
+        return self._get_json_response("/api/v2/review/%s/storage/" % review_id)
 
     def update_review(self, review_id, data):
         """
         Update a review
 
         Args:
             review_id (TYPE): the id of the item
@@ -417,15 +452,15 @@
         Returns:
             TYPE: item
         """
         if not isinstance(data, dict):
             print("Please make sure you pass a dict as data")
             return False
 
-        return self._get_json_response("review/%s" % review_id, patchData=data)
+        return self._get_json_response("/api/v1/review/%s/" % review_id, patchData=data)
 
     def sort_review_items(self, review_id, items):
         """
         Update a review
 
         Args:
             review_id (TYPE): the id of the item
@@ -442,30 +477,30 @@
             TYPE: dict
                 { "updated_items": int }  # number of successful items sort updated
         """
         if not isinstance(items, list):
             print("Please make sure you pass a list as data")
             return False
 
-        return self._get_json_response("review/%s/sort_items" % review_id, putData=dict(items=items), api_version="v2")
+        return self._get_json_response("/api/v2/review/%s/sort_items/" % review_id, putData=dict(items=items))
 
     def delete_review(self, review_id):
         """
         Get single review by id.
         :param review_id: Int
         :return:
         """
-        return self._get_json_response("review/%s" % review_id, patchData=dict(active=0))
+        return self._get_json_response("/api/v1/review/%s/" % review_id, patchData=dict(active=False))
 
     """
     Items
     """
 
-    def get_item(self, item_id):
-        return self._get_json_response("item/{}".format(item_id))
+    def get_item(self, item_id, data=None):
+        return self._get_json_response("/api/v1/item/{}/".format(item_id), getData=data)
 
     def update_item(self, item_id, data):
         """Summary
 
         Args:
             item_id (TYPE): the id of the item
             data (dict): normal dict with data for item
@@ -473,15 +508,15 @@
         Returns:
             TYPE: item
         """
         if not isinstance(data, dict):
             print("Please make sure you pass a dict as data")
             return False
 
-        return self._get_json_response("item/%s" % item_id, patchData=data)
+        return self._get_json_response("/api/v1/item/%s/" % item_id, patchData=data)
 
     def add_item(self, review_id, name, fps, additional_data):
         """
         create a media item record and connect it to a review. This should be used in case you want to add items with externaly hosted
         media by passing in the external_url and external_thumbnail_url to the additionalData dict e.g
 
         additionalData = {
@@ -509,34 +544,35 @@
             }
 
         Returns:
             TYPE: Item
         """
 
         postData = {
-            "reviews": ["/api/%s/review/%s/" % (self.api_version, review_id)],
+            "reviewId": review_id,
             "status": "done",
             "fps": fps,
             "name": name,
         }
 
         postData.update(additional_data)
 
-        return self._get_json_response("item", postData=postData)
+        return self._get_json_response("/api/v1/item/", postData=postData)
 
-    def add_media(self, review_id, filepath, artist_name="", noConvertFlag=False, itemParentId=False):
+    def add_media(self, review_id, filepath, artist_name="", file_name="", noConvertFlag=False, itemParentId=False):
         """
             Convenience function to upload a file to a review. It will automatically create
             an Item and attach it to the review. NOTE - if you are hosting your own media, please
             use the addItem function and pass in the external_url and external_thumbnail_url
 
         Args:
             review_id (int): Required review_id
             filepath (string): path for the file on disk e.g /tmp/movie.webm
             artist_name (string): The name of the artist you want associated with this media file
+            file_name (string): The name of the file. Please make sure to pass the correct file extension
             noConvertFlag (bool): the video you are uploading is already in a browser compatible format
             itemParentId (int): set when you want to add a new version of an item.
                                 itemParentId is the id of the item you want to upload a new version for
 
         Returns:
             TYPE: Description
         """
@@ -547,15 +583,15 @@
 
         if itemParentId:
             get_params.update({"itemParentId": itemParentId})
 
         uploadURL = "%s/items/uploadToReview/%s/?%s" % (self.HOST, review_id, urlencode(get_params))
 
         files = {"reviewFile": open(filepath, "rb")}
-        r = requests.post(uploadURL, files=files, data=dict(artist=artist_name), headers=self.headers)
+        r = requests.post(uploadURL, files=files, data=dict(artist=artist_name, name=file_name), headers=self.headers)
 
         try:
             return json.loads(r.text)
         except Exception:
             print(r.text)
 
     def add_media_by_url(self, review_id, media_url, artist_name="", noConvertFlag=False):
@@ -586,14 +622,97 @@
         r = requests.post(upload_url, {"media_url": media_url, "artist": artist_name}, headers=self.headers)
 
         try:
             return json.loads(r.text)
         except Exception:
             print(r.text)
 
+    def add_media_v2(self, review_id, filepath, file_name="", item_uuid=None, noConvertFlag=False):
+        """ Similar to add_media method, but uploads the media file directly to SyncSketche's internal S3 instead of to
+        the SyncSketch server. In some cases, using this method over add_media can improve upload performance and
+        stability. Unlike add_media this method does not return as much data about the created item.
+
+        :param int review_id: Required review_id.
+        :param str filepath: path for the file on disk e.g /tmp/movie.webm.
+        :param str file_name: The name of the file. Please make sure to pass the correct file extension.
+        :param bool noConvertFlag: the video you are uploading is already in a browser compatible format.
+
+        :return: A dict, containing "item_id" and "uuid" or None on failure.
+        :rtype: Optional[dict]
+        """
+        if not self.headers:
+            print("add_media_via_s3 failed. use_header_auth must be set to true.")
+            return None
+
+        content_length = os.stat(filepath).st_size
+
+        # for media > 5gb use v1 upload api
+        if content_length > 5 * 1000 * 1000:
+            result = self.add_media_v1(
+                review_id=review_id,
+                filepath=filepath,
+                file_name=file_name,
+                noConvertFlag=noConvertFlag,
+            )
+            return {"id": result["id"], "uuid": result["uuid"]}
+
+
+        content_type = mimetypes.guess_type(filepath, strict=False)[0]
+
+        url_response = self._get_s3_signed_url(
+            review_id=review_id,
+            item_name=file_name,
+            content_length=content_length,
+            content_type=content_type,
+            no_convert=noConvertFlag,
+        )
+
+        if not url_response.ok:
+            print("Failed to generate signed S3 url.\nAPI response:\n{}".format(url_response.text))
+            return None
+
+        url_response_data = url_response.json()
+        url = url_response_data["url"]
+        fields = url_response_data["fields"]
+
+        with open(filepath, "rb") as file:
+            upload_response = requests.post(url, data=fields, files={"file": file})
+
+        if not upload_response.ok:
+            print("Upload process failed while uploading file to S3.\nS3 response:\n{}".format(upload_response.text))
+            return None
+
+        return {"id": fields["x-amz-meta-item-id"], "uuid": fields["x-amz-meta-item-uuid"]}
+
+    def _get_s3_signed_url(self, review_id, item_name, item_uuid=None, content_type=None, content_length=None, no_convert=False):
+        """
+        Internal method. Use to retrieve s3 signed url for file upload in `add_media_via_s3`.
+        """
+        request_data = self.api_params.copy()
+        additional_request_data = {
+            "review_id": review_id,
+            "item_name": item_name,
+            "item_data": {
+                "uuid": item_uuid,
+                "content_type": content_type,
+                "content_length": content_length,
+                "noConvertFlag": no_convert,
+            },
+        }
+        request_data.update(additional_request_data)
+
+        request_url = "/uploads/get-s3-signed-url/".format(host=self.HOST)
+
+        return self._get_json_response(
+            url=request_url,
+            postData=request_data,
+            raw_response=True,
+        )
+
+
     def get_media(self, searchCriteria):
         """
         This is a general search function. You can search media items by
 
         'id'
         'name'
         'status'
@@ -623,46 +742,45 @@
         Args:
             searchCriteria (dict): dictionary
 
         Returns:
             dict: search results
         """
 
-        return self._get_json_response("item", getData=searchCriteria)
+        return self._get_json_response("/api/v1/item/", getData=searchCriteria)
 
     def get_media_by_review_id(self, review_id):
         """Summary
 
         Args:
             review_id (TYPE): Description
 
         Returns:
             TYPE: Description
         """
         get_params = {"reviews__id": review_id, "active": 1}
-        return self._get_json_response("item", getData=get_params)
+        return self._get_json_response("/api/v1/item/", getData=get_params)
 
     def delete_item(self, item_id):
         """
         Get single item by id.
         :param item_id: Int
         :return:
         """
-        return self._get_json_response("item/%s" % item_id, patchData=dict(active=0))
+        return self._get_json_response("/api/v1/item/%s/" % item_id, patchData=dict(active=False))
 
     def bulk_delete_items(self, item_ids):
         """
         Delete multiple items by id.
         :param item_ids: Array[Int}
         """
         return self._get_json_response(
-            "bulk-delete-items/",
+            "/api/v2/bulk-delete-items/",
             postData=dict(item_ids=item_ids),
             method="post",
-            api_version="v2",
             raw_response=True,
         )
 
     def connect_item_to_review(self, item_id, review_id):
         print("DEPRECATED.")
         print("A new improved method for this will be added soon.")
         return "Deprecated"
@@ -676,59 +794,61 @@
 
         :param new_review_id: int
         :param item_data: list [ dict { review_id: int, item_id: int} ]
         :return:
         """
 
         return self._get_json_response(
-            "move-review-items/",
+            "/api/v2/move-review-items/",
             method="post",
-            api_version="v2",
             postData={"new_review_id": new_review_id, "item_data": item_data},
             raw_response=True,
         )
 
     """
     Frames (Sketches / Comments)
     """
 
-    def add_comment(self, item_id, text, frame=0):
-        item = self.getItem(item_id)
+    def add_comment(self, item_id, text, review_id, frame=0):
+        item = self.get_item(item_id, data={"review_id": review_id})
 
         # Ugly method of getting revision id from item data, should fix this with api v2
-        revisions = item.get("revisions")
-        if not revisions:
+        revision_id = item.get("revision_id")
+        if not revision_id:
             return "error"
-        revision_id = revisions[0].get("id")
 
         post_data = dict(
             item="/api/v1/item/{}/".format(item_id),
             frame=frame,
             revision="/api/v1/revision/{}/".format(revision_id),
             type="comment",
             text=text
         )
 
-        return self._get_json_response("frame", method="post", postData=post_data)
+        return self._get_json_response("/api/v1/frame/", method="post", postData=post_data)
 
-    def get_annotations(self, item_id, revisionId=False):
+    def get_annotations(self, item_id, revisionId=False, review_id=False):
         """
         Get sketches and comments for an item. Frames have a revision id which signifies a "set of notes".
         When querying an item you'll get the available revisions for this item. If you wish to get only the latest
         revision, please get the revisionId for the latest revision.
         :param item_id: id of the media item you are querying.
         :param (number) revisionId: Optional revisionId to narrow down the results
+        :param (number) review_id: RECOMMENDED - retrieve annotations for a specific review only.
         :return: dict
         """
         get_params = {"item__id": item_id, "active": 1}
 
         if revisionId:
             get_params["revision__id"] = revisionId
 
-        return self._get_json_response("frame", getData=get_params)
+        if review_id:
+            get_params["revision__review_id"] = review_id
+
+        return self._get_json_response("/api/v1/frame/", getData=get_params)
 
     def get_flattened_annotations(self, review_id, item_id, with_tracing_paper=False, return_as_base64=False):
         """
         Returns a list of sketches either as signed urls from s3 or base64 encoded strings.
         The sketches are composited over the background frame of the item.
 
         :param syncsketch_review_id: <int>
@@ -739,17 +859,17 @@
         getData = {
             "include_data": 1,
             "tracingpaper": 1 if with_tracing_paper else 0,
             "base64": 1 if return_as_base64 else 0,
             "async": 0
         }
 
-        url = "downloads/flattenedSketches/{}/{}".format(review_id, item_id)
+        url = "/api/v2/downloads/flattenedSketches/{}/{}/".format(review_id, item_id)
 
-        return self._get_json_response(url, method="post", api_version="v2", getData = getData)
+        return self._get_json_response(url, method="post", getData = getData)
 
     def get_grease_pencil_overlays(self, review_id, item_id, homedir=None):
         """Download overlay sketches for Maya Greasepencil.
 
             Download overlay sketches for Maya Greasepencil. Function will download
             a zip file which contains an XML and the sketches as png files. Maya
             can load the zip file to overlay the sketches over the 3D model!
@@ -813,42 +933,50 @@
 
         return self.add_users_to_project(project_id=project_id, users=users)
 
     def get_users_by_name(self, name):
         """
         Name is a combined search and will search in first_name, last_name and email
         """
-        return self._get_json_response("simpleperson", getData={"name": name})
+        return self._get_json_response("/api/v1/simpleperson/", getData={"name": name})
 
     def get_user_by_email(self, email):
         """
         Get user by email
         """
-        response = self._get_json_response("simpleperson", getData={"email": email}, raw_response=True)
+        response = self._get_json_response("/api/v1/simpleperson/", getData={"email__iexact": email}, raw_response=True)
 
         try:
             data = response.json()
             return data.get("objects")[0]
         except:
             return None
 
     def get_users_by_project_id(self, project_id):
-        return self._get_json_response("all-project-users/{}".format(project_id), api_version="v2")
+        return self._get_json_response("/api/v2/all-project-users/{}/".format(project_id))
 
-    def get_connections_by_user_id(self, user_id, account_id):
+    def get_connections_by_user_id(self, user_id, account_id, include_inactive=None, include_archived=None):
         """
         Get all project and account connections for a user. Good for checking access for a user that might have left...
         """
-        return self._get_json_response("user/{}/connections/account/{}".format(user_id, account_id), api_version="v2")
+        data = {}
+        if include_inactive is not None:
+            data["include_inactive"] = "true" if include_inactive else "false"
+        if include_archived is not None:
+            data["include_archived"] = "true" if include_archived else "false"
+        return self._get_json_response(
+            "/api/v2/user/{}/connections/account/{}/".format(user_id, account_id),
+            getData=data,
+        )
 
     def get_user_by_id(self, userId):
-        return self._get_json_response("simpleperson/%s" % userId)
+        return self._get_json_response("/api/v1/simpleperson/%s/" % userId)
 
     def get_current_user(self):
-        return self._get_json_response("simpleperson/currentUser")
+        return self._get_json_response("/api/v1/simpleperson/currentUser/")
 
     def add_users_to_workspace(self, workspace_id, users, note = ''):
         """Add Users to Workspace
 
         Args:
             workspace_id (Number): id of the workspace
             users (List): list with dicts e.g users=[{"email":"test@test.de","permission":"admin"}] - possible permissions "admin"
@@ -866,15 +994,15 @@
         post_data = {
             "which": "account",
             "entity_id": workspace_id,
             "note": note,
             "users": json.dumps(users)
         }
 
-        return self._get_json_response("add-users", postData=post_data, api_version="v2")
+        return self._get_json_response("/api/v2/add-users/", postData=post_data)
 
     def remove_users_from_workspace(self, workspace_id, users):
         """Remove a list of users from a workspace
 
         Args:
             workspace_id (Number): id of the workspace
             users (List): list with dicts e.g users=[{"email":"test@test.de"}, {"id":12345}] - either remove by user email or id
@@ -888,15 +1016,15 @@
 
         post_data = {
             "which": "account",
             "entity_id": workspace_id,
             "users": json.dumps(users)
         }
 
-        return self._get_json_response("remove-users", postData=post_data, api_version="v2")
+        return self._get_json_response("/api/v2/remove-users/", postData=post_data)
 
     def add_users_to_project(self, project_id, users, note=''):
         """Add Users to Project
 
         Args:
             project_id (Number): id of the project
             users (List): list with dicts e.g users=[{"email":"test@test.de","permission":"viewer"}] - possible permissions "admin, member, viewer or reviewer"
@@ -914,15 +1042,15 @@
         post_data = {
             "which": "project",
             "entity_id": project_id,
             "note": note,
             "users": json.dumps(users)
         }
 
-        return self._get_json_response("add-users", postData=post_data, api_version="v2",)
+        return self._get_json_response("/api/v2/add-users/", postData=post_data)
 
     def remove_users_from_project(self, project_id, users):
         """Remove a list of users from a project
 
         Args:
             project_id (Number): id of the project
             users (List): list with dicts e.g users=[{"email":"test@test.de"}, {"id":12345}] - either remove by user email or id
@@ -936,15 +1064,15 @@
 
         post_data = {
             "which": "project",
             "entity_id": project_id,
             "users": json.dumps(users)
         }
 
-        return self._get_json_response("remove-users", postData=post_data, api_version="v2")
+        return self._get_json_response("/api/v2/remove-users/", postData=post_data)
 
     """
     Shotgun API
     """
 
     def shotgun_get_projects(self, syncsketch_project_id):
         """
@@ -965,20 +1093,20 @@
         :param syncsketch_project_id: <int>
         :param shotgun_project_id: <int> (optional)
 
         If the syncsketch project is directly linked to a shotgun by the workspace admin, the
         param shotgun_project_id will be ignored and can be omitted during the function call
 
         """
-        url = "shotgun/playlists/{}".format(syncsketch_account_id)
+        url = "/api/v2/shotgun/playlists/{}/".format(syncsketch_account_id)
         if syncsketch_project_id:
-            url += "/{}".format(syncsketch_project_id)
+            url = self.join_url_path(url, "/{}/".format(syncsketch_project_id))
 
         data = {"shotgun_project_id": shotgun_project_id}
-        return self._get_json_response(url, method="get", getData=data, api_version="v2")
+        return self._get_json_response(url, method="get", getData=data)
 
     def shotgun_sync_review_notes(self, review_id):
         """
         Sync notes from SyncSketch review to the original shotgun playlist
         Returns task id to use in get_shotgun_sync_review_notes_progress to get progress
 
         :param review_id: <int>
@@ -987,17 +1115,17 @@
             status=<STR> processing/done/failed
             progress_url=<STR> Full url to call for progress/results
             task_id=<STR> task_ids *pass this value to the get_shotgun_sync_review_items_progress function
             percent_complete=<INT> 0-100 value of percent complete
             total_items=<INT> number of items being synced from shotgun
             remaining_items=<INT> number of items not yet pulled from shotgun
         """
-        url = "shotgun/sync-review-notes/review/{}".format(review_id)
+        url = "/api/v2/shotgun/sync-review-notes/review/{}/".format(review_id)
 
-        return self._get_json_response(url, method="post", api_version="v2")
+        return self._get_json_response(url, method="post")
 
     def get_shotgun_sync_review_notes_progress(self, task_id):
         """
         Returns status of review notes sync for the task id provided in shotgun_sync_review_notes
 
         :param task_id: <str/uuid>
         :returns <dict>
@@ -1005,17 +1133,17 @@
             status=<STR> processing/done/failed
             progress_url=<STR> Full url to call for progress/results
             task_id=<STR> task_ids *pass this value to the get_shotgun_sync_review_items_progress function
             percent_complete=<INT> 0-100 value of percent complete
             total_items=<INT> number of items being synced from shotgun
             remaining_items=<INT> number of items not yet pulled from shotgun
         """
-        url = "shotgun/sync-review-notes/{}".format(task_id)
+        url = "/api/v2/shotgun/sync-review-notes/{}/".format(task_id)
 
-        return self._get_json_response(url, method="get", api_version="v2")
+        return self._get_json_response(url, method="get")
 
     def shotgun_sync_review_items(self, syncsketch_project_id, playlist_code, playlist_id, review_id=None):
         """
         Create or update SyncSketch review with shotgun playlist items
         Returns task id to use in get_shotgun_sync_review_items_progress to get progress
 
         :param syncsketch_project_id
@@ -1031,34 +1159,33 @@
             total_items=<INT> number of items being synced from shotgun,
             remaining_items=<INT> number of items not yet pulled from shotgun,
             data=<dict>
                 review_id=<INT> review.id,
                 review_link=<STR> url link to the syncsketch player with the review pulled from shotgun,
         )
         """
-        url = "shotgun/sync-items/project/{}/".format(syncsketch_project_id)
+        url = "/api/v2/shotgun/sync-items/project/{}/".format(syncsketch_project_id)
         if review_id:
-            url += "review/{}/check".format(review_id)
+            url = self.join_url_path(url, "/review/{}/check/".format(review_id))
         else:
-            url += "check"
+            url = self.join_url_path(url, "/check/")
 
         data = {"playlist_code": playlist_code, "playlist_id": playlist_id}
 
-        response = self._get_json_response(url, method="post", postData=data, api_version="v2")
+        response = self._get_json_response(url, method="post", postData=data)
         if self.debug:
             print(response)
 
         result = dict(review_id=response["review_id"], items=[], status="done", total_items=len(response["items"]))
 
         if "items" in response:
             for item in response["items"]:
-                item_id = item["id"]
-                data = {"playlist_item_json": {"id": item_id}}
-                item_sync_url = "shotgun/sync-items/project/{}/review/{}/".format(syncsketch_project_id, response["review_id"])
-                item_data = self._get_json_response(item_sync_url, method="post", postData=data, api_version="v2")
+                data = {"playlist_item_json": json.dumps(item)}
+                item_sync_url = "/api/v2/shotgun/sync-items/project/{}/review/{}/".format(syncsketch_project_id, response["review_id"])
+                item_data = self._get_json_response(item_sync_url, method="post", postData=data)
                 result["items"].append(item_data["id"])
 
                 if self.debug:
                     print(item_data)
         return result
 
     def get_shotgun_sync_review_items_progress(self, task_id):
@@ -1074,14 +1201,16 @@
             percent_complete=<INT> 0-100 value of percent complete,
             total_items=<INT> number of items being synced from shotgun,
             remaining_items=<INT> number of items not yet pulled from shotgun,
         )
         """
         print("Deprecated.  Response is printed in the shotgun_sync_review_items() function")
 
+    # alias methods to <name>_v1 if they have a v2
+    add_media_v1 = add_media
     # Keep old names for backwards compatibility
     isConnected = is_connected
     getAccounts = get_accounts
     getProjects = get_projects
     getProjectsByName = get_projects_by_name
     getProjectById = get_project_by_id
     addProject = create_project
```

