# Comparing `tmp/praetorian-api-client-0.4.4.tar.gz` & `tmp/praetorian_api_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praetorian-api-client-0.4.4.tar", last modified: Sun May  9 14:14:20 2021, max compression
+gzip compressed data, was "praetorian_api_client-0.5.0.tar", max compression
```

## Comparing `praetorian-api-client-0.4.4.tar` & `praetorian_api_client-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-09 14:14:20.826174 praetorian-api-client-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2021-05-09 14:14:20.826174 praetorian-api-client-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-09 14:14:20.822174 praetorian-api-client-0.4.4/praetorian_api_client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-09 14:14:20.826174 praetorian-api-client-0.4.4/praetorian_api_client/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/resources/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/resources/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/resources/service.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/resources/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/resources/user.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/praetorian_api_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-09 14:14:20.826174 praetorian-api-client-0.4.4/praetorian_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2021-05-09 14:14:20.000000 praetorian-api-client-0.4.4/praetorian_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      798 2021-05-09 14:14:20.000000 praetorian-api-client-0.4.4/praetorian_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-09 14:14:20.000000 praetorian-api-client-0.4.4/praetorian_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-05-09 14:14:20.000000 praetorian-api-client-0.4.4/praetorian_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-09 14:14:20.000000 praetorian-api-client-0.4.4/praetorian_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-09 14:14:20.826174 praetorian-api-client-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2021-05-09 14:14:12.000000 praetorian-api-client-0.4.4/setup.py
+-rw-r--r--   0        0        0     1075 2024-04-04 19:10:01.664197 praetorian_api_client-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1898 2024-04-04 19:10:01.664871 praetorian_api_client-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 13:12:52.434245 praetorian_api_client-0.5.0/praetorian_api_client/__init__.py
+-rw-r--r--   0        0        0     2004 2024-04-04 19:10:01.666526 praetorian_api_client-0.5.0/praetorian_api_client/api_client.py
+-rw-r--r--   0        0        0     1339 2024-04-04 19:10:01.667217 praetorian_api_client-0.5.0/praetorian_api_client/configuration.py
+-rw-r--r--   0        0        0     1323 2023-07-06 13:12:52.434675 praetorian_api_client-0.5.0/praetorian_api_client/errors.py
+-rw-r--r--   0        0        0     1933 2023-07-06 13:12:52.434814 praetorian_api_client-0.5.0/praetorian_api_client/requestor.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:12:52.434957 praetorian_api_client-0.5.0/praetorian_api_client/resources/__init__.py
+-rw-r--r--   0        0        0      881 2023-07-06 13:12:52.435116 praetorian_api_client-0.5.0/praetorian_api_client/resources/base.py
+-rw-r--r--   0        0        0      789 2024-04-04 19:10:01.667807 praetorian_api_client-0.5.0/praetorian_api_client/resources/log.py
+-rw-r--r--   0        0        0      708 2023-07-06 13:12:52.435259 praetorian_api_client-0.5.0/praetorian_api_client/resources/project.py
+-rw-r--r--   0        0        0     1530 2023-07-06 13:12:52.435402 praetorian_api_client-0.5.0/praetorian_api_client/resources/remote.py
+-rw-r--r--   0        0        0     1162 2023-07-06 13:12:52.435534 praetorian_api_client-0.5.0/praetorian_api_client/resources/service.py
+-rw-r--r--   0        0        0      594 2023-07-06 13:12:52.435666 praetorian_api_client-0.5.0/praetorian_api_client/resources/token.py
+-rw-r--r--   0        0        0     1661 2023-07-06 13:12:52.435803 praetorian_api_client-0.5.0/praetorian_api_client/resources/user.py
+-rw-r--r--   0        0        0      514 2023-07-06 13:12:52.435930 praetorian_api_client-0.5.0/praetorian_api_client/utils.py
+-rw-r--r--   0        0        0       22 2024-04-04 19:10:01.668419 praetorian_api_client-0.5.0/praetorian_api_client/version.py
+-rw-r--r--   0        0        0      795 2024-04-05 08:39:02.304626 praetorian_api_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 praetorian_api_client-0.5.0/PKG-INFO
```

### Comparing `praetorian-api-client-0.4.4/LICENSE` & `praetorian_api_client-0.5.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Praetorian-Defence
+Copyright (c) 2023 Praetorian-Defence
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `praetorian-api-client-0.4.4/README.md` & `praetorian_api_client-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -62,9 +62,9 @@
 
 To run tests, you need to run command: `pytest`
 
 Tests require access data to the api. For security reasons, access data is stored in environment variables. To set 
 environment variables, you need to create an `.env` file from the example in the `.env.example` file.
 
 ---
-Developed with 💙 and ☕️ by [Adam Žúrek](https://zurek11.github.io/)
-with the support of [BACKBONE s.r.o.](https://www.backbone.sk/), 2021 (C)
+Developed with 💙 and ☕️ by [Adam Žúrek](https://zurek11.github.io/) & Erik Belák
+with the support of [BACKBONE s.r.o.](https://www.backbone.sk/), 2024 (C)
```

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/api_client.py` & `praetorian_api_client-0.5.0/praetorian_api_client/api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .resources.log import LogResource
 from .resources.project import ProjectResource
 from .resources.remote import RemoteResource
 from .resources.service import ServiceResource
 from .resources.token import TokenResource
 from .resources.user import UserResource
 from .version import __version__
 
@@ -14,14 +15,15 @@
         self._configuration = configuration
         self._requestor = Requestor(configuration)
 
         self._user = UserResource(self._requestor, self._configuration)
         self._project = ProjectResource(self._requestor, self._configuration)
         self._remote = RemoteResource(self._requestor, self._configuration)
         self._service = ServiceResource(self._requestor, self._configuration)
+        self._log = LogResource(self._requestor, self._configuration)
 
     @classmethod
     def create_from_auth(cls, configuration: Configuration, username: str, password: str) -> 'ApiClient':
         token_resource = TokenResource(Requestor(configuration), configuration)
         token_obj = token_resource.auth(username, password)
         configuration.set_token(str(token_obj.token))
 
@@ -51,9 +53,13 @@
     def remote(self) -> RemoteResource:
         return self._remote
 
     @property
     def service(self) -> ServiceResource:
         return self._service
 
+    @property
+    def log(self) -> LogResource:
+        return self._log
+
     def __str__(self) -> str:
         return f"{self.requestor}"
```

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/configuration.py` & `praetorian_api_client-0.5.0/praetorian_api_client/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-import os
-
-from dotenv import load_dotenv
-
-
 class Environment(object):
     def __init__(self, name: str, api_url: str, read_only: bool = True):
         self._name = name
         self._api_url = api_url
         self._read_only = read_only
 
     @property
```

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/errors.py` & `praetorian_api_client-0.5.0/praetorian_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/requestor.py` & `praetorian_api_client-0.5.0/praetorian_api_client/requestor.py`

 * *Files identical despite different names*

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/resources/base.py` & `praetorian_api_client-0.5.0/praetorian_api_client/resources/base.py`

 * *Files identical despite different names*

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/resources/project.py` & `praetorian_api_client-0.5.0/praetorian_api_client/resources/project.py`

 * *Files identical despite different names*

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/resources/remote.py` & `praetorian_api_client-0.5.0/praetorian_api_client/resources/remote.py`

 * *Files identical despite different names*

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/resources/service.py` & `praetorian_api_client-0.5.0/praetorian_api_client/resources/service.py`

 * *Files identical despite different names*

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/resources/token.py` & `praetorian_api_client-0.5.0/praetorian_api_client/resources/token.py`

 * *Files identical despite different names*

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/resources/user.py` & `praetorian_api_client-0.5.0/praetorian_api_client/resources/user.py`

 * *Files identical despite different names*

### Comparing `praetorian-api-client-0.4.4/praetorian_api_client/utils.py` & `praetorian_api_client-0.5.0/praetorian_api_client/utils.py`

 * *Files identical despite different names*

