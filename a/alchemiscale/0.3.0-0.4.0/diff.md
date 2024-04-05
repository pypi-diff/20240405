# Comparing `tmp/alchemiscale-0.3.0.tar.gz` & `tmp/alchemiscale-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemiscale-0.3.0.tar", last modified: Fri Jan 19 18:31:11 2024, max compression
+gzip compressed data, was "alchemiscale-0.4.0.tar", last modified: Fri Apr  5 05:09:54 2024, max compression
```

## Comparing `alchemiscale-0.3.0.tar` & `alchemiscale-0.4.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.447470 alchemiscale-0.3.0/
--rw-r--r--   0 david     (1001) david     (1001)     1084 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/LICENSE
--rw-r--r--   0 david     (1001) david     (1001)     1356 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/PKG-INFO
--rw-r--r--   0 david     (1001) david     (1001)      639 2023-09-30 17:52:16.000000 alchemiscale-0.3.0/README.md
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.440803 alchemiscale-0.3.0/alchemiscale/
--rw-r--r--   0 david     (1001) david     (1001)      158 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/__init__.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/alchemiscale/base/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/base/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     8073 2024-01-19 18:29:50.000000 alchemiscale-0.3.0/alchemiscale/base/api.py
--rw-r--r--   0 david     (1001) david     (1001)    17610 2024-01-09 16:12:34.000000 alchemiscale-0.3.0/alchemiscale/base/client.py
--rw-r--r--   0 david     (1001) david     (1001)    17259 2023-09-30 17:52:16.000000 alchemiscale-0.3.0/alchemiscale/cli.py
--rw-r--r--   0 david     (1001) david     (1001)      929 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/cli_utils.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/alchemiscale/compute/
--rw-r--r--   0 david     (1001) david     (1001)       46 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/compute/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     8039 2024-01-09 16:12:34.000000 alchemiscale-0.3.0/alchemiscale/compute/api.py
--rw-r--r--   0 david     (1001) david     (1001)     3697 2023-09-30 17:52:16.000000 alchemiscale-0.3.0/alchemiscale/compute/client.py
--rw-r--r--   0 david     (1001) david     (1001)    17317 2023-10-06 18:26:01.000000 alchemiscale-0.3.0/alchemiscale/compute/service.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/alchemiscale/interface/
--rw-r--r--   0 david     (1001) david     (1001)       39 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/interface/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)    25661 2024-01-19 18:29:50.000000 alchemiscale-0.3.0/alchemiscale/interface/api.py
--rw-r--r--   0 david     (1001) david     (1001)    49547 2024-01-19 18:29:50.000000 alchemiscale-0.3.0/alchemiscale/interface/client.py
--rw-r--r--   0 david     (1001) david     (1001)     2754 2024-01-19 18:29:50.000000 alchemiscale-0.3.0/alchemiscale/keyedchain.py
--rw-r--r--   0 david     (1001) david     (1001)     6152 2024-01-09 16:12:34.000000 alchemiscale-0.3.0/alchemiscale/models.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/alchemiscale/security/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/security/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     2051 2024-01-09 16:12:32.000000 alchemiscale-0.3.0/alchemiscale/security/auth.py
--rw-r--r--   0 david     (1001) david     (1001)     1565 2024-01-09 16:12:32.000000 alchemiscale-0.3.0/alchemiscale/security/models.py
--rw-r--r--   0 david     (1001) david     (1001)     2552 2024-01-09 16:12:32.000000 alchemiscale-0.3.0/alchemiscale/settings.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/alchemiscale/storage/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/storage/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     7000 2024-01-09 16:12:32.000000 alchemiscale-0.3.0/alchemiscale/storage/models.py
--rw-r--r--   0 david     (1001) david     (1001)     9796 2023-09-30 17:52:16.000000 alchemiscale-0.3.0/alchemiscale/storage/objectstore.py
--rw-r--r--   0 david     (1001) david     (1001)    81831 2024-01-09 16:12:34.000000 alchemiscale-0.3.0/alchemiscale/storage/statestore.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/alchemiscale/strategies/
--rw-r--r--   0 david     (1001) david     (1001)       27 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/strategies/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)      369 2023-09-30 17:52:16.000000 alchemiscale-0.3.0/alchemiscale/strategies/base.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/alchemiscale/strategist/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-08-16 17:56:36.000000 alchemiscale-0.3.0/alchemiscale/strategist/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)      133 2023-09-30 17:52:16.000000 alchemiscale-0.3.0/alchemiscale/strategist/service.py
--rw-r--r--   0 david     (1001) david     (1001)     3398 2024-01-19 18:29:50.000000 alchemiscale-0.3.0/alchemiscale/utils.py
--rw-r--r--   0 david     (1001) david     (1001)      818 2023-10-06 23:05:37.000000 alchemiscale-0.3.0/alchemiscale/validators.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-01-19 18:31:11.444137 alchemiscale-0.3.0/alchemiscale.egg-info/
--rw-r--r--   0 david     (1001) david     (1001)     1356 2024-01-19 18:31:11.000000 alchemiscale-0.3.0/alchemiscale.egg-info/PKG-INFO
--rw-r--r--   0 david     (1001) david     (1001)     1155 2024-01-19 18:31:11.000000 alchemiscale-0.3.0/alchemiscale.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1001) david     (1001)        1 2024-01-19 18:31:11.000000 alchemiscale-0.3.0/alchemiscale.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1001) david     (1001)       54 2024-01-19 18:31:11.000000 alchemiscale-0.3.0/alchemiscale.egg-info/entry_points.txt
--rw-r--r--   0 david     (1001) david     (1001)        1 2023-08-22 01:18:23.000000 alchemiscale-0.3.0/alchemiscale.egg-info/not-zip-safe
--rw-r--r--   0 david     (1001) david     (1001)       28 2024-01-19 18:31:11.000000 alchemiscale-0.3.0/alchemiscale.egg-info/requires.txt
--rw-r--r--   0 david     (1001) david     (1001)       13 2024-01-19 18:31:11.000000 alchemiscale-0.3.0/alchemiscale.egg-info/top_level.txt
--rw-r--r--   0 david     (1001) david     (1001)     1710 2023-09-30 17:52:16.000000 alchemiscale-0.3.0/pyproject.toml
--rw-r--r--   0 david     (1001) david     (1001)       38 2024-01-19 18:31:11.447470 alchemiscale-0.3.0/setup.cfg
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.647961 alchemiscale-0.4.0/
+-rw-r--r--   0 david     (1001) david     (1001)     1084 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/LICENSE
+-rw-r--r--   0 david     (1001) david     (1001)     2118 2024-04-05 05:09:54.647961 alchemiscale-0.4.0/PKG-INFO
+-rw-r--r--   0 david     (1001) david     (1001)     1401 2024-04-03 18:28:03.000000 alchemiscale-0.4.0/README.md
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.641294 alchemiscale-0.4.0/alchemiscale/
+-rw-r--r--   0 david     (1001) david     (1001)      158 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/__init__.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.644627 alchemiscale-0.4.0/alchemiscale/base/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/base/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     8127 2024-02-22 17:40:50.000000 alchemiscale-0.4.0/alchemiscale/base/api.py
+-rw-r--r--   0 david     (1001) david     (1001)    17606 2024-02-21 06:53:56.000000 alchemiscale-0.4.0/alchemiscale/base/client.py
+-rw-r--r--   0 david     (1001) david     (1001)    17958 2024-04-03 18:28:03.000000 alchemiscale-0.4.0/alchemiscale/cli.py
+-rw-r--r--   0 david     (1001) david     (1001)      929 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/cli_utils.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.644627 alchemiscale-0.4.0/alchemiscale/compute/
+-rw-r--r--   0 david     (1001) david     (1001)       46 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/compute/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     8016 2024-02-22 17:40:50.000000 alchemiscale-0.4.0/alchemiscale/compute/api.py
+-rw-r--r--   0 david     (1001) david     (1001)     3693 2024-02-21 06:53:56.000000 alchemiscale-0.4.0/alchemiscale/compute/client.py
+-rw-r--r--   0 david     (1001) david     (1001)    17397 2024-04-05 05:04:35.000000 alchemiscale-0.4.0/alchemiscale/compute/service.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.644627 alchemiscale-0.4.0/alchemiscale/interface/
+-rw-r--r--   0 david     (1001) david     (1001)       39 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/interface/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)    30810 2024-04-03 18:28:03.000000 alchemiscale-0.4.0/alchemiscale/interface/api.py
+-rw-r--r--   0 david     (1001) david     (1001)    63217 2024-04-03 18:28:03.000000 alchemiscale-0.4.0/alchemiscale/interface/client.py
+-rw-r--r--   0 david     (1001) david     (1001)     2754 2024-01-19 18:29:50.000000 alchemiscale-0.4.0/alchemiscale/keyedchain.py
+-rw-r--r--   0 david     (1001) david     (1001)     6149 2024-02-21 06:53:56.000000 alchemiscale-0.4.0/alchemiscale/models.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.644627 alchemiscale-0.4.0/alchemiscale/security/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/security/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     2047 2024-02-21 06:53:56.000000 alchemiscale-0.4.0/alchemiscale/security/auth.py
+-rw-r--r--   0 david     (1001) david     (1001)     1557 2024-02-21 06:53:56.000000 alchemiscale-0.4.0/alchemiscale/security/models.py
+-rw-r--r--   0 david     (1001) david     (1001)     2548 2024-02-21 06:53:56.000000 alchemiscale-0.4.0/alchemiscale/settings.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.644627 alchemiscale-0.4.0/alchemiscale/storage/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/storage/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)      688 2024-04-03 18:28:03.000000 alchemiscale-0.4.0/alchemiscale/storage/cypher.py
+-rw-r--r--   0 david     (1001) david     (1001)     8828 2024-04-03 18:28:03.000000 alchemiscale-0.4.0/alchemiscale/storage/models.py
+-rw-r--r--   0 david     (1001) david     (1001)     9792 2024-02-21 06:53:56.000000 alchemiscale-0.4.0/alchemiscale/storage/objectstore.py
+-rw-r--r--   0 david     (1001) david     (1001)    96750 2024-04-03 18:28:03.000000 alchemiscale-0.4.0/alchemiscale/storage/statestore.py
+-rw-r--r--   0 david     (1001) david     (1001)     4949 2024-02-22 17:40:50.000000 alchemiscale-0.4.0/alchemiscale/storage/subgraph.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.644627 alchemiscale-0.4.0/alchemiscale/strategies/
+-rw-r--r--   0 david     (1001) david     (1001)       27 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/strategies/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)      345 2024-02-21 06:53:56.000000 alchemiscale-0.4.0/alchemiscale/strategies/base.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.647961 alchemiscale-0.4.0/alchemiscale/strategist/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-08-16 17:56:36.000000 alchemiscale-0.4.0/alchemiscale/strategist/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)      133 2023-09-30 17:52:16.000000 alchemiscale-0.4.0/alchemiscale/strategist/service.py
+-rw-r--r--   0 david     (1001) david     (1001)     3398 2024-01-19 18:29:50.000000 alchemiscale-0.4.0/alchemiscale/utils.py
+-rw-r--r--   0 david     (1001) david     (1001)      818 2023-10-06 23:05:37.000000 alchemiscale-0.4.0/alchemiscale/validators.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2024-04-05 05:09:54.647961 alchemiscale-0.4.0/alchemiscale.egg-info/
+-rw-r--r--   0 david     (1001) david     (1001)     2118 2024-04-05 05:09:54.000000 alchemiscale-0.4.0/alchemiscale.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1001) david     (1001)     1219 2024-04-05 05:09:54.000000 alchemiscale-0.4.0/alchemiscale.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1001) david     (1001)        1 2024-04-05 05:09:54.000000 alchemiscale-0.4.0/alchemiscale.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1001) david     (1001)       54 2024-04-05 05:09:54.000000 alchemiscale-0.4.0/alchemiscale.egg-info/entry_points.txt
+-rw-r--r--   0 david     (1001) david     (1001)        1 2024-04-05 05:09:54.000000 alchemiscale-0.4.0/alchemiscale.egg-info/not-zip-safe
+-rw-r--r--   0 david     (1001) david     (1001)       28 2024-04-05 05:09:54.000000 alchemiscale-0.4.0/alchemiscale.egg-info/requires.txt
+-rw-r--r--   0 david     (1001) david     (1001)       13 2024-04-05 05:09:54.000000 alchemiscale-0.4.0/alchemiscale.egg-info/top_level.txt
+-rw-r--r--   0 david     (1001) david     (1001)     1710 2023-09-30 17:52:16.000000 alchemiscale-0.4.0/pyproject.toml
+-rw-r--r--   0 david     (1001) david     (1001)       38 2024-04-05 05:09:54.647961 alchemiscale-0.4.0/setup.cfg
```

### Comparing `alchemiscale-0.3.0/LICENSE` & `alchemiscale-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.3.0/alchemiscale/base/api.py` & `alchemiscale-0.4.0/alchemiscale/base/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from functools import lru_cache
 from typing import Any, Union, List, Callable
 import json
 import gzip
 
 from starlette.responses import JSONResponse
-from fastapi import APIRouter, Depends, HTTPException, status, Request, Response
+from fastapi import APIRouter, Depends, HTTPException, Request, Response
+from fastapi import status as http_status
 from fastapi.routing import APIRoute
 from fastapi.security import OAuth2PasswordRequestForm
 from gufe.tokenization import JSON_HANDLER, GufeTokenizable
 
 from ..settings import (
     JWTSettings,
     Neo4jStoreSettings,
@@ -41,15 +42,15 @@
     if not isinstance(scope, Scope):
         raise ValueError("`scope` must be a `Scope` object to ensure validity")
 
     scope_in_token = any([Scope.from_str(ts).is_superset(scope) for ts in token.scopes])
 
     if not scope_in_token:
         raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
+            status_code=http_status.HTTP_401_UNAUTHORIZED,
             detail=(
                 f"Targeted scope '{scope}' not accessible via scopes for this identity: {token.scopes}."
             ),
             headers={"WWW-Authenticate": "Bearer"},
         )
 
 
@@ -168,15 +169,15 @@
 
 
 def scope_params(org: str = None, campaign: str = None, project: str = None):
     try:
         return Scope(org=org, campaign=campaign, project=project)
     except (AttributeError, ValueError):
         raise HTTPException(
-            status_code=status.HTTP_400_BAD_REQUEST,
+            status_code=http_status.HTTP_400_BAD_REQUEST,
             detail=(
                 f"Requested Scope cannot be processed as a 3-object tuple of form"
                 f'"X-Y-Z" and cast to string. Alpha numerical values (a-z A-Z 0-9) and "*" are accepted for '
                 f'parameter "scope"'
             ),
             headers={"WWW-Authenticate": "Bearer"},
         )
@@ -188,15 +189,15 @@
     neo4jreachable = n4js._store_check()
     # check if s3 object store is reachable
     s3reachable = s3os._store_check()
 
     if not neo4jreachable or not s3reachable:
         detail = f"Attempt to reach services failed, Neo4j reachable: {neo4jreachable}, S3 reachable: {s3reachable}"
         raise HTTPException(
-            status_code=status.HTTP_503_SERVICE_UNAVAILABLE, detail=detail
+            status_code=http_status.HTTP_503_SERVICE_UNAVAILABLE, detail=detail
         )
     else:
         return True
 
 
 def get_token_data_depends(
     token: str = Depends(oauth2_scheme),
@@ -237,15 +238,15 @@
     n4js: Neo4jStore = Depends(get_n4js_depends),
     cred_cls: CredentialedEntity = Depends(get_cred_entity),
 ):
     entity = authenticate(n4js, cred_cls, form_data.username, form_data.password)
 
     if entity is None:
         raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
+            status_code=http_status.HTTP_401_UNAUTHORIZED,
             detail="Incorrect identity or key",
             headers={"WWW-Authenticate": "Bearer"},
         )
 
     access_token = create_access_token(
         data={"sub": entity.identifier, "scopes": entity.scopes},
         secret_key=settings.JWT_SECRET_KEY,
```

### Comparing `alchemiscale-0.3.0/alchemiscale/base/client.py` & `alchemiscale-0.4.0/alchemiscale/base/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 
 class AlchemiscaleBaseClientError(Exception):
     def __init__(self, *args, **kwargs):
         self.status_code = kwargs.pop("status_code", None)
         super().__init__(*args, **kwargs)
 
 
-class AlchemiscaleConnectionError(Exception):
-    ...
+class AlchemiscaleConnectionError(Exception): ...
 
 
 def use_session(f):
     async def _wrapper(self, *args, **kwargs):
         self._lock = asyncio.Lock()
         self._session = httpx.AsyncClient(verify=self.verify)
         try:
```

### Comparing `alchemiscale-0.3.0/alchemiscale/cli.py` & `alchemiscale-0.4.0/alchemiscale/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -209,16 +209,15 @@
     gunicorn_app = ApiApplication(
         api_app, workers, bind=f"{host}:{port}", options=options
     )
     gunicorn_app.run()
 
 
 @click.group()
-def cli():
-    ...
+def cli(): ...
 
 
 # reusable parameters to ensure consistent naming and help strings
 
 
 @cli.command(
     name="api",
@@ -279,16 +278,15 @@
         host["ALCHEMISCALE_API_HOST"],
         port["ALCHEMISCALE_API_PORT"],
         options=options,
     )
 
 
 @cli.group(help="Subcommands for compute services")
-def compute():
-    ...
+def compute(): ...
 
 
 @compute.command(help="Start the compute API service.")
 @api_starting_params(
     "ALCHEMISCALE_COMPUTE_API_HOST",
     "ALCHEMISCALE_COMPUTE_API_PORT",
     "ALCHEMISCALE_COMPUTE_API_LOGLEVEL",
@@ -389,16 +387,15 @@
     try:
         service.start(**params_start)
     except KeyboardInterrupt:
         pass
 
 
 @cli.group(help="Subcommands for the database")
-def database():
-    ...
+def database(): ...
 
 
 @database.command()
 @db_params
 def init(url, user, password, dbname):
     """Initialize the Neo4j database.
 
@@ -449,14 +446,41 @@
     cli_values = url | user | password | dbname
     settings = get_settings_from_options(cli_values, Neo4jStoreSettings)
 
     n4js = get_n4js(settings)
     n4js.reset()
 
 
+@database.group(help="Subcommands for database migrations")
+def migrate(): ...
+
+
+@migrate.command()
+@db_params
+def v03_to_v04(url, user, password, dbname):
+    """Perform migration appropriate for transitioning from alchemiscale v0.3
+    to v0.4.
+
+    Note that options here can be set by environment variables, as shown on
+    each option.
+    """
+    from .storage.statestore import get_n4js
+    from .settings import Neo4jStoreSettings
+    from .migrations.v03_to_v04 import migrate
+
+    cli_values = url | user | password | dbname
+    settings = get_settings_from_options(cli_values, Neo4jStoreSettings)
+
+    n4js = get_n4js(settings)
+
+    migrate(n4js)
+
+    click.echo("Migration completed without errors.")
+
+
 def _identity_type_string_to_cls(identity_type: str) -> Type[CredentialedEntity]:
     if identity_type == "user":
         identity_type_cls = CredentialedUserIdentity
     elif identity_type == "compute":
         identity_type_cls = CredentialedComputeIdentity
     else:
         raise RuntimeError(f"Unknown identity type {identity_type}")
@@ -491,16 +515,15 @@
     scope = click.option(
         "--scope", "-s", help="scope", required=True, type=str, multiple=True
     )
     return scope(func)
 
 
 @cli.group(help="Subcommands for managing identities")
-def identity():
-    ...
+def identity(): ...
 
 
 @identity.command()
 @db_params
 @identity_type
 @identifier
 @key
```

### Comparing `alchemiscale-0.3.0/alchemiscale/cli_utils.py` & `alchemiscale-0.4.0/alchemiscale/cli_utils.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.3.0/alchemiscale/compute/api.py` & `alchemiscale-0.4.0/alchemiscale/compute/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from typing import Any, Dict, List, Optional
 import os
 import json
 from datetime import datetime, timedelta
 
-from fastapi import FastAPI, APIRouter, Body, Depends, HTTPException, status
+from fastapi import FastAPI, APIRouter, Body, Depends
 from fastapi.middleware.gzip import GZipMiddleware
 from gufe.tokenization import GufeTokenizable, JSON_HANDLER
 
 from ..base.api import (
     QueryGUFEHandler,
     scope_params,
     get_token_data_depends,
```

### Comparing `alchemiscale-0.3.0/alchemiscale/compute/client.py` & `alchemiscale-0.4.0/alchemiscale/compute/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,15 @@
     AlchemiscaleBaseClientError,
     json_to_gufe,
 )
 from ..models import Scope, ScopedKey
 from ..storage.models import TaskHub, Task, ComputeServiceID, TaskStatusEnum
 
 
-class AlchemiscaleComputeClientError(AlchemiscaleBaseClientError):
-    ...
+class AlchemiscaleComputeClientError(AlchemiscaleBaseClientError): ...
 
 
 class AlchemiscaleComputeClient(AlchemiscaleBaseClient):
     """Client for compute service interaction with compute API service."""
 
     _exception = AlchemiscaleComputeClientError
```

### Comparing `alchemiscale-0.3.0/alchemiscale/compute/service.py` & `alchemiscale-0.4.0/alchemiscale/compute/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,17 +247,22 @@
 
         if len(taskhubs) == 0:
             return []
 
         # claim tasks from taskhubs based on weight; keep going till we hit our
         # total desired task count, or we run out of taskhubs to draw from
         while len(tasks) < count and len(taskhubs) > 0:
+            weights = [th.weight for th in taskhubs.values()]
+
+            if sum(weights) == 0:
+                break
+
             # based on weights, choose taskhub to draw from
             taskhub: List[ScopedKey] = random.choices(
-                list(taskhubs.keys()), weights=[th.weight for th in taskhubs.values()]
+                list(taskhubs.keys()), weights=weights
             )[0]
 
             # claim tasks from the taskhub
             claimed_tasks = self.client.claim_taskhub_tasks(
                 taskhub,
                 compute_service_id=self.compute_service_id,
                 count=(count - len(tasks)),
@@ -501,16 +506,15 @@
 
     def __init__(self, api_url):
         self.scheduler = sched.scheduler(time.monotonic, time.sleep)
         # self.loop = asyncio.get_event_loop()
 
         self._stop = False
 
-    def get_new_tasks(self):
-        ...
+    def get_new_tasks(self): ...
 
     def start(self):
         """Start the service; will keep going until told to stop."""
         while True:
             if self._stop:
                 return
```

### Comparing `alchemiscale-0.3.0/alchemiscale/interface/api.py` & `alchemiscale-0.4.0/alchemiscale/interface/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 """
 
 from typing import Any, Dict, List, Optional, Union
 import os
 import json
 from collections import Counter
 
-from fastapi import FastAPI, APIRouter, Body, Depends, HTTPException, status
+from fastapi import FastAPI, APIRouter, Body, Depends, HTTPException
+from fastapi import status as http_status
 from fastapi.middleware.gzip import GZipMiddleware
 from gufe import AlchemicalNetwork, ChemicalSystem, Transformation
 from gufe.protocols import ProtocolDAGResult
 from gufe.tokenization import GufeTokenizable, JSON_HANDLER
 
 from ..base.api import (
     GufeJSONResponse,
@@ -30,15 +31,15 @@
     gufe_to_json,
     GzipRoute,
 )
 from ..settings import get_api_settings
 from ..settings import get_base_api_settings, get_api_settings
 from ..storage.statestore import Neo4jStore
 from ..storage.objectstore import S3ObjectStore
-from ..storage.models import ProtocolDAGResultRef, TaskStatusEnum
+from ..storage.models import ProtocolDAGResultRef, TaskStatusEnum, NetworkStateEnum
 from ..models import Scope, ScopedKey
 from ..security.auth import get_token_data, oauth2_scheme
 from ..security.models import Token, TokenData, CredentialedUserIdentity
 from ..keyedchain import KeyedChain
 
 
 app = FastAPI(title="AlchemiscaleAPI")
@@ -105,41 +106,80 @@
 
     return n4js.check_existence(scoped_key=sk)
 
 
 @router.post("/networks", response_model=ScopedKey)
 def create_network(
     *,
-    network: List = Body(...),
-    scope: Scope,
+    network: List = Body(embed=True),
+    scope: Scope = Body(embed=True),
+    state: str = Body(embed=True),
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
     validate_scopes(scope, token)
 
     an = KeyedChain(network).to_gufe()
 
     try:
-        an_sk = n4js.create_network(network=an, scope=scope)
+        an_sk, _, _ = n4js.assemble_network(network=an, scope=scope, state=state)
     except ValueError as e:
         raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            status_code=http_status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=e.args[0],
         )
 
-    # create taskhub for this network
-    n4js.create_taskhub(an_sk)
-
     return an_sk
 
 
+@router.post("/bulk/networks/state/set")
+def set_networks_state(
+    *,
+    networks: List[str] = Body(embed=True),
+    states: List[str] = Body(embed=True),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> List[Optional[str]]:
+    network_sks = []
+    for network in networks:
+        network_sk = ScopedKey.from_str(network)
+        validate_scopes(network_sk.scope, token)
+        network_sks.append(network_sk)
+
+    try:
+        results = n4js.set_network_state(network_sks, states)
+    except ValueError as e:
+        raise HTTPException(status_code=http_status.HTTP_400_BAD_REQUEST, detail=str(e))
+
+    return [None if network_sk is None else str(network_sk) for network_sk in results]
+
+
+@router.post("/bulk/networks/state/get")
+def get_networks_state(
+    *,
+    networks: List[str] = Body(embed=True),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> List[Optional[str]]:
+    network_sks = []
+    for network in networks:
+        network_sk = ScopedKey.from_str(network)
+        validate_scopes(network_sk.scope, token)
+        network_sks.append(network_sk)
+
+    results = n4js.get_network_state(network_sks)
+
+    return [None if network_sk is None else str(network_sk) for network_sk in results]
+
+
 @router.get("/networks")
 def query_networks(
     *,
     name: str = None,
+    state: str = None,
     scope: Scope = Depends(scope_params),
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
     # Intersect query scopes with accessible scopes in the token
     query_scopes = validate_scopes_query(scope, token)
 
@@ -147,14 +187,15 @@
     # loop might be removable in the future with a Union like operator on scopes
     results = []
     for single_query_scope in query_scopes:
         results.extend(
             n4js.query_networks(
                 name=name,
                 scope=single_query_scope,
+                state=state,
             )
         )
 
     return [str(sk) for sk in results]
 
 
 @router.get("/transformations")
@@ -193,26 +234,14 @@
     results = []
     for single_query_scope in query_scopes:
         results.extend(n4js.query_chemicalsystems(name=name, scope=single_query_scope))
 
     return [str(sk) for sk in results]
 
 
-@router.get("/networks/{network_scoped_key}/weight")
-def get_network_weight(
-    network_scoped_key,
-    *,
-    n4js: Neo4jStore = Depends(get_n4js_depends),
-    token: TokenData = Depends(get_token_data_depends),
-) -> float:
-    sk = ScopedKey.from_str(network_scoped_key)
-    validate_scopes(sk.scope, token)
-    return n4js.get_taskhub_weight(sk)
-
-
 @router.get("/networks/{network_scoped_key}/transformations")
 def get_network_transformations(
     network_scoped_key,
     *,
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
@@ -333,35 +362,59 @@
     return GufeJSONResponse(chemicalsystem)
 
 
 ### compute
 
 
 @router.post("/networks/{scoped_key}/strategy")
-def set_strategy(scoped_key: str, *, strategy: Dict = Body(...), scope: Scope):
-    ...
+def set_strategy(scoped_key: str, *, strategy: Dict = Body(...), scope: Scope): ...
 
 
 @router.post("/transformations/{transformation_scoped_key}/tasks")
 def create_tasks(
     transformation_scoped_key,
     *,
     extends: Optional[ScopedKey] = None,
     count: int = Body(...),
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ) -> List[str]:
     sk = ScopedKey.from_str(transformation_scoped_key)
     validate_scopes(sk.scope, token)
 
-    task_sks = []
-    for i in range(count):
-        task_sks.append(
-            n4js.create_task(transformation=sk, extends=extends, creator=token.entity)
-        )
+    task_sks = n4js.create_tasks([sk] * count, [extends] * count)
+    return [str(sk) for sk in task_sks]
+
+
+@router.post("/bulk/transformations/tasks/create")
+def create_transformations_tasks(
+    *,
+    transformations: List[str] = Body(embed=True),
+    extends: Optional[List[Optional[str]]] = None,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    transformation_sks = [
+        ScopedKey.from_str(transformation_string)
+        for transformation_string in transformations
+    ]
+
+    for transformation_sk in transformation_sks:
+        validate_scopes(transformation_sk.scope, token)
+
+    if extends is not None:
+        extends = [
+            None if not extends_str else ScopedKey.from_str(extends_str)
+            for extends_str in extends
+        ]
+
+    try:
+        task_sks = n4js.create_tasks(transformation_sks, extends)
+    except ValueError as e:
+        raise HTTPException(status_code=http_status.HTTP_400_BAD_REQUEST, detail=str(e))
 
     return [str(sk) for sk in task_sks]
 
 
 @router.get("/tasks")
 def query_tasks(
     *,
@@ -438,48 +491,68 @@
     elif return_as == "graph":
         return {
             str(sk): str(extends) if extends is not None else None
             for sk, extends in task_sks.items()
         }
     else:
         raise HTTPException(
-            status_code=status.HTTP_400_BAD_REQUEST,
+            status_code=http_status.HTTP_400_BAD_REQUEST,
             detail=f"`return_as` takes 'list' or 'graph', not '{return_as}'",
         )
 
 
 @router.get("/scopes/{scope}/status")
 def get_scope_status(
     scope,
     *,
+    network_state: str = None,
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
     scope = Scope.from_str(scope)
     scope_space = validate_scopes_query(scope, token)
 
     status_counts = Counter()
     for single_scope in scope_space:
-        status_counts.update(n4js.get_scope_status(single_scope))
+        status_counts.update(
+            n4js.get_scope_status(single_scope, network_state=network_state)
+        )
 
     return dict(status_counts)
 
 
 @router.get("/networks/{network_scoped_key}/status")
 def get_network_status(
     network_scoped_key,
     *,
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
     sk = ScopedKey.from_str(network_scoped_key)
     validate_scopes(sk.scope, token)
 
-    status_counts = n4js.get_network_status(network_scoped_key)
+    status_counts = n4js.get_network_status([network_scoped_key])[0]
+
+    return status_counts
+
+
+@router.post("/bulk/networks/status")
+def get_networks_status(
+    *,
+    networks: List[str] = Body(embed=True),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> List[Dict[str, int]]:
 
+    network_sks = [ScopedKey.from_str(sk) for sk in networks]
+
+    for sk in network_sks:
+        validate_scopes(sk.scope, token)
+
+    status_counts = n4js.get_network_status(network_sks)
     return status_counts
 
 
 @router.get("/transformations/{transformation_scoped_key}/status")
 def get_transformation_status(
     transformation_scoped_key,
     *,
@@ -502,22 +575,51 @@
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ) -> Union[Dict[str, float], List[str]]:
     network_sk = ScopedKey.from_str(network_scoped_key)
     validate_scopes(network_sk.scope, token)
 
     taskhub_sk = n4js.get_taskhub(network_sk)
-    task_sks = n4js.get_taskhub_actioned_tasks(taskhub_sk)
+    task_sks = n4js.get_taskhub_actioned_tasks([taskhub_sk])[0]
 
     if task_weights:
         return {str(task_sk): weight for task_sk, weight in task_sks.items()}
 
     return [str(task_sk) for task_sk in task_sks]
 
 
+@router.post("/bulk/networks/tasks/actioned")
+def get_networks_actioned_tasks(
+    *,
+    networks: List[str] = Body(embed=True),
+    task_weights: bool = Body(embed=True),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> List[Union[Dict[str, float], List[str]]]:
+
+    network_sks = [ScopedKey.from_str(network) for network in networks]
+
+    for sk in network_sks:
+        validate_scopes(sk.scope, token)
+
+    taskhub_sks = [n4js.get_taskhub(network_sk) for network_sk in network_sks]
+    grouped_task_sks = n4js.get_taskhub_actioned_tasks(taskhub_sks)
+
+    return_data = []
+    for group in grouped_task_sks:
+        if task_weights:
+            return_data.append(
+                {str(task_sk): weight for task_sk, weight in group.items()}
+            )
+        else:
+            return_data.append([str(task_sk) for task_sk in group])
+
+    return return_data
+
+
 @router.post("/tasks/{task_scoped_key}/networks/actioned")
 def get_task_actioned_networks(
     task_scoped_key,
     *,
     task_weights: bool = Body(embed=True),
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
@@ -551,42 +653,94 @@
     try:
         if isinstance(weight, float):
             n4js.set_task_weights(tasks, taskhub_sk, weight)
         elif isinstance(weight, list):
             if len(weight) != len(tasks):
                 detail = "weight (when in a list) must have the same length as tasks"
                 raise HTTPException(
-                    status_code=status.HTTP_400_BAD_REQUEST,
+                    status_code=http_status.HTTP_400_BAD_REQUEST,
                     detail=detail,
                 )
 
             n4js.set_task_weights(
                 {task: weight for task, weight in zip(tasks, weight)}, taskhub_sk, None
             )
     except ValueError as e:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(e))
+        raise HTTPException(status_code=http_status.HTTP_400_BAD_REQUEST, detail=str(e))
 
     return [str(sk) if sk is not None else None for sk in actioned_sks]
 
 
+@router.get("/networks/{network_scoped_key}/weight")
+def get_network_weight(
+    network_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> float:
+    sk = ScopedKey.from_str(network_scoped_key)
+    validate_scopes(sk.scope, token)
+    return n4js.get_taskhub_weight([sk])[0]
+
+
+@router.post("/bulk/networks/weight/get")
+def get_networks_weight(
+    *,
+    networks: List[str] = Body(embed=True),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> List[float]:
+
+    network_sks = [ScopedKey.from_str(network_str) for network_str in networks]
+
+    for network_sk in network_sks:
+        validate_scopes(network_sk.scope, token)
+
+    return n4js.get_taskhub_weight(network_sks)
+
+
 @router.post("/networks/{network_scoped_key}/weight")
 def set_network_weight(
     network_scoped_key,
     *,
     weight: float = Body(),
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ) -> None:
     sk = ScopedKey.from_str(network_scoped_key)
     validate_scopes(sk.scope, token)
 
     try:
-        n4js.set_taskhub_weight(sk, weight)
+        network_sk = n4js.set_taskhub_weight([sk], [weight])[0]
+        return str(network_sk) if network_sk else None
     except ValueError as e:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(e))
+        raise HTTPException(status_code=http_status.HTTP_400_BAD_REQUEST, detail=str(e))
+
+
+@router.post("/bulk/networks/weight/set")
+def set_networks_weight(
+    *,
+    networks: List[str] = Body(embed=True),
+    weights: List[float] = Body(embed=True),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> None:
+
+    network_sks = [ScopedKey.from_str(network_str) for network_str in networks]
+
+    for network in network_sks:
+        validate_scopes(network.scope, token)
+
+    try:
+        network_sks = n4js.set_taskhub_weight(
+            [ScopedKey.from_str(network) for network in networks], weights
+        )
+        return [str(network_sk) if network_sk else None for network_sk in network_sks]
+    except Exception as e:
+        raise HTTPException(status_code=http_status.HTTP_400_BAD_REQUEST, detail=str(e))
 
 
 @router.post("/networks/{network_scoped_key}/tasks/cancel")
 def cancel_tasks(
     network_scoped_key,
     *,
     tasks: List[ScopedKey] = Body(embed=True),
@@ -637,15 +791,15 @@
             valid_tasks.append(task_sk)
         except HTTPException:
             valid_tasks.append(None)
 
     try:
         tasks_updated = n4js.set_task_priority(valid_tasks, priority)
     except ValueError as e:
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(e))
+        raise HTTPException(status_code=http_status.HTTP_400_BAD_REQUEST, detail=str(e))
 
     return [str(t) if t is not None else None for t in tasks_updated]
 
 
 @router.post("/bulk/tasks/status/get")
 def tasks_status_get(
     *,
@@ -677,15 +831,15 @@
     status = TaskStatusEnum(status)
     if status not in (
         TaskStatusEnum.waiting,
         TaskStatusEnum.invalid,
         TaskStatusEnum.deleted,
     ):
         raise HTTPException(
-            status_code=status.HTTP_400_BAD_REQUEST,
+            status_code=http_status.HTTP_400_BAD_REQUEST,
             detail=f"Cannot set status to '{status}', must be one of 'waiting', 'invalid', 'deleted'",
         )
 
     valid_tasks = []
     for task_sk in tasks:
         try:
             validate_scopes(task_sk.scope, token)
@@ -708,15 +862,15 @@
     status = TaskStatusEnum(status)
     if status not in (
         TaskStatusEnum.waiting,
         TaskStatusEnum.invalid,
         TaskStatusEnum.deleted,
     ):
         raise HTTPException(
-            status_code=status.HTTP_400_BAD_REQUEST,
+            status_code=http_status.HTTP_400_BAD_REQUEST,
             detail=f"Cannot set status to '{status}', must be one of 'waiting', 'invalid', 'deleted'",
         )
     task_sk = ScopedKey.from_str(task_scoped_key)
     validate_scopes(task_sk.scope, token)
     tasks_statused = n4js.set_task_status([task_sk], status)
     return [str(t) if t is not None else None for t in tasks_statused][0]
 
@@ -799,15 +953,15 @@
 ) -> List[str]:
     if route == "results":
         ok = True
     elif route == "failures":
         ok = False
     else:
         raise HTTPException(
-            status_code=status.HTTP_400_BAD_REQUEST,
+            status_code=http_status.HTTP_400_BAD_REQUEST,
             detail=f"`route` takes 'results' or 'failures', not '{route}'",
         )
 
     sk = ScopedKey.from_str(protocoldagresultref_scoped_key)
     transformation_sk = ScopedKey.from_str(transformation_scoped_key)
 
     validate_scopes(sk.scope, token)
```

### Comparing `alchemiscale-0.3.0/alchemiscale/interface/client.py` & `alchemiscale-0.4.0/alchemiscale/interface/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 :mod:`alchemiscale.interface.client` --- client for interacting with user-facing API
 ====================================================================================
 
 """
 
 import asyncio
-from typing import Union, List, Dict, Optional, Tuple, Any
+from typing import Union, List, Dict, Optional, Tuple, Any, Iterable
 import json
 from itertools import chain
 from collections import Counter
 from functools import lru_cache
 
 import httpx
 from async_lru import alru_cache
@@ -22,23 +22,29 @@
 from ..base.client import (
     AlchemiscaleBaseClient,
     AlchemiscaleBaseClientError,
     json_to_gufe,
     use_session,
 )
 from ..models import Scope, ScopedKey
-from ..storage.models import Task, ProtocolDAGResultRef, TaskStatusEnum
+from ..storage.models import (
+    Task,
+    ProtocolDAGResultRef,
+    TaskStatusEnum,
+    NetworkStateEnum,
+)
 from ..strategies import Strategy
 from ..security.models import CredentialedUserIdentity
 from ..validators import validate_network_nonself
 from ..keyedchain import KeyedChain
 
+from warnings import warn
+
 
-class AlchemiscaleClientError(AlchemiscaleBaseClientError):
-    ...
+class AlchemiscaleClientError(AlchemiscaleBaseClientError): ...
 
 
 def _get_transformation_results(client_settings, tf_sk, ok: bool, kwargs):
     client = AlchemiscaleClient(**client_settings)
     if ok:
         return tf_sk, client.get_transformation_results(tf_sk, **kwargs)
     else:
@@ -65,14 +71,26 @@
         """Given any gufe object and a fully-specified Scope, return corresponding ScopedKey.
 
         This method does not check that this ScopedKey is represented in the database.
         It is only a convenience for properly constructing a ScopedKey from a
         gufe object and a Scope.
 
         """
+
+        msg = """`get_scoped_key` will be removed in v0.5.0
+
+        For accurate server-side ScopedKeys, use the relevant methods for the GufeTokenizable of interest.
+        For instance, `get_network_transformations` should be used to get Transformation ScopedKeys for a given AlchemicalNetwork.
+
+        """
+        warn(
+            msg,
+            DeprecationWarning,
+        )
+
         if scope.specific():
             return ScopedKey(gufe_key=obj.key, **scope.dict())
         else:
             raise ValueError(
                 "Scope for a ScopedKey must be specific; it cannot contain wildcards."
             )
 
@@ -80,26 +98,30 @@
         """Returns ``True`` if the given ScopedKey represents an object in the database."""
         return self._get_resource(f"/exists/{scoped_key}")
 
     def create_network(
         self,
         network: AlchemicalNetwork,
         scope: Scope,
+        state: Union[NetworkStateEnum, str] = NetworkStateEnum.active,
         compress: Union[bool, int] = True,
         visualize: bool = True,
     ) -> ScopedKey:
         """Submit an AlchemicalNetwork to a specific Scope.
 
         Parameters
         ----------
         network
             The AlchemicalNetwork to submit.
         scope
             The Scope in which to submit the AlchemicalNetwork.
             This must be a *specific* Scope; it must not contain wildcards.
+        state
+            The starting state of the AlchemicalNetwork in the database.
+            See :meth:`AlchemiscaleClient.set_network_state` for valid states.
         compress
             If ``True``, compress the AlchemicalNetwork client-side before
             shipping to the API service. This can reduce submission time
             depending on the bandwidth of your connection to the API service.
             Set to ``False`` to submit without compressing. This is a
             performance optimization; it has no bearing on the result of this
             method call.
@@ -119,19 +141,21 @@
         if not scope.specific():
             raise ValueError(
                 f"`scope` '{scope}' contains wildcards ('*'); `scope` must be *specific*"
             )
 
         validate_network_nonself(network)
 
-        sk = self.get_scoped_key(network, scope)
+        state = NetworkStateEnum(state)
+
+        sk = ScopedKey(gufe_key=network.key, **scope.dict())
 
         def post():
             keyed_chain = KeyedChain.gufe_to_keyed_chain_rep(network)
-            data = dict(network=keyed_chain, scope=scope.dict())
+            data = dict(network=keyed_chain, scope=scope.dict(), state=state.value)
             return self._post_resource("/networks", data, compress=compress)
 
         if visualize:
             from rich.progress import Progress
 
             with Progress(*self._rich_waiting_columns(), transient=False) as progress:
                 task = progress.add_task(
@@ -142,30 +166,135 @@
                 progress.start_task(task)
                 progress.update(task, total=1, completed=1)
         else:
             scoped_key = post()
 
         return ScopedKey.from_dict(scoped_key)
 
+    def set_network_state(
+        self, network: ScopedKey, state: Union[NetworkStateEnum, str]
+    ) -> Optional[ScopedKey]:
+        """Set the state of an AlchemicalNetwork.
+
+        Parameters
+        ----------
+        network
+            The network whose state will be updated.
+        state
+            The state to set the network to. Valid options include "active",
+            "inactive", "invalid", and "deleted".
+
+        Returns
+        -------
+        Optional[ScopedKey]
+            The ScopedKey of the updated network. If the network was not found, ``None``
+            is returned.
+        """
+        return self.set_networks_state([network], [state])[0]
+
+    def set_networks_state(
+        self, networks: List[ScopedKey], states: List[Union[NetworkStateEnum, str]]
+    ) -> List[Optional[ScopedKey]]:
+        """Set the state of a list of AlchemicalNetworks.
+
+        Parameters
+        ----------
+        networks
+            The networks whose states will be updated.
+        states
+            The states to set the networks to, in the same order as `networks`.
+            Values must be in a list of the same length as the networks
+            parameter. Valid options include "active", "inactive", "invalid",
+            and "deleted".
+
+        Returns
+        -------
+        List[Optional[ScopedKey]]
+            The ScopedKeys of the updated networks. If a network was not found, ``None``
+            is returned at the corresponding index.
+        """
+        data = dict(networks=list(map(str, networks)), states=states)
+        networks_updated = self._post_resource("/bulk/networks/state/set", data=data)
+        return [
+            ScopedKey.from_str(network_sk) if network_sk is not None else None
+            for network_sk in networks_updated
+        ]
+
+    def get_network_state(self, network: ScopedKey) -> Optional[str]:
+        """Get the state of an AlchemicalNetwork.
+
+        Parameters
+        ----------
+        network
+            The ScopedKey of the AlchemicalNetwork to get the state for.
+
+        Returns
+        -------
+        Optional[str]
+            The state of the AlchemicalNetwork. If the network was not found in
+            the database, ``None`` is returned instead.
+        """
+        return self.get_networks_state([network])[0]
+
+    def get_networks_state(self, networks: List[ScopedKey]) -> List[Optional[str]]:
+        """Get the states for a list of AlchemicalNetworks.
+
+        Parameters
+        ----------
+        networks
+            A list of ScopedKeys for the AlchemicalNetworks to get the states
+            of.
+
+        Returns
+        -------
+        List[Optional[str]]
+            A list of network states, in the same order as the specified
+            networks. If a network was not found in the database, the
+            corresponding entry in this list is ``None``.
+        """
+        data = dict(networks=list(map(str, networks)))
+        states = self._post_resource("/bulk/networks/state/get", data=data)
+        return states
+
     def query_networks(
         self,
         name: Optional[str] = None,
         scope: Optional[Scope] = None,
+        state: Optional[Union[NetworkStateEnum, str]] = NetworkStateEnum.active,
     ) -> List[ScopedKey]:
         """Query for AlchemicalNetworks, optionally by name or Scope.
 
         Calling this method with no query arguments will return ScopedKeys for
         all AlchemicalNetworks that are within the Scopes this user has access
         to.
 
+        Parameters
+        ----------
+        name : optional
+            Regex expression for the network names. Defaults to a wildcard.
+        scope : optional
+            A Scope to filter AlchemicalNetworks on.
+        state : optional
+            Regex expression for the network states. Nonexistent state values
+            entered will not raise any warnings. Use ``None`` to get networks
+            regardless of state. Defaults to the "active" state.
+
+        Returns
+        -------
+        List[ScopedKey]
+            A list of ScopedKeys for the networks matching the query
+            parameters.
         """
         if scope is None:
             scope = Scope()
 
-        params = dict(name=name, **scope.dict())
+        if isinstance(state, NetworkStateEnum):
+            state = state.value
+
+        params = dict(name=name, **scope.dict(), state=state)
 
         return self._query_resource("/networks", params=params)
 
     def query_transformations(
         self,
         name: Optional[str] = None,
         scope: Optional[Scope] = None,
@@ -216,15 +345,54 @@
 
         A weight of ``0`` means the AlchemicalNetwork will not receive any
         compute for its actioned Tasks.
 
         """
         return self._get_resource(f"/networks/{network}/weight")
 
-    def set_network_weight(self, network: ScopedKey, weight: float) -> None:
+    async def _get_network_weight(self, networks: List[ScopedKey]) -> List[float]:
+        data = dict(networks=[str(network) for network in networks])
+        weights = await self._post_resource_async(
+            "/bulk/networks/weight/get", data=data
+        )
+        return weights
+
+    def get_networks_weight(
+        self, networks: List[ScopedKey], batch_size: int = 1000
+    ) -> List[float]:
+        """Get the weight of the TaskHubs associated with the given AlchemicalNetworks.
+
+        Compute services perform a weighted selection of the AlchemicalNetworks
+        visible to them before claiming Tasks actioned on those networks.
+        Networks with higher weight are more likely to be selected than those
+        with lower weight, and so will generally get more compute attention
+        over time.
+
+        A weight of ``0`` means the AlchemicalNetwork will not receive any
+        compute for its actioned Tasks.
+
+        Parameters
+        ----------
+        networks
+            A list of AlchemicalNetwork ScopedKeys.
+
+        Returns
+        -------
+        List[float]
+            The weights of the TaskHubs associated with the specified AlchemicalNetworks.
+            If the network was not found in the database, then None is returned in the
+            corresponding index.
+        """
+        return self._batched_attribute_getter(
+            networks, self._get_network_weight, batch_size
+        )
+
+    def set_network_weight(
+        self, network: ScopedKey, weight: float
+    ) -> Optional[ScopedKey]:
         """Set the weight of the TaskHub associated with the given AlchemicalNetwork.
 
         Compute services perform a weighted selection of the AlchemicalNetworks
         visible to them before claiming Tasks actioned on those networks.
         Networks with higher weight are more likely to be selected than those
         with lower weight, and so will generally get more compute attention
         over time.
@@ -236,17 +404,74 @@
         ----------
         network
             The ScopedKey of the AlchemicalNetwork to set the weight for.
         weight
             The weight to set for the network. This must be between 0 and 1
             (inclusive). Setting the value to 0 will effectively disable
             compute on this network without cancelling its actioned Tasks.
-
         """
-        self._post_resource(f"/networks/{network}/weight", weight)
+        network_sk = self._post_resource(f"/networks/{network}/weight", weight)
+        return ScopedKey.from_str(network_sk) if network_sk else None
+
+    async def _set_network_weight(
+        self,
+        items: List[Tuple[ScopedKey, float]],
+    ) -> List[Optional[ScopedKey]]:
+
+        networks = []
+        weights = []
+        for item in items:
+            networks.append(str(item[0]))
+            weights.append(item[1])
+
+        data = dict(networks=networks, weights=weights)
+        return await self._post_resource_async("/bulk/networks/weight/set", data=data)
+
+    def set_networks_weight(
+        self,
+        networks: List[ScopedKey],
+        weights: List[float],
+        batch_size: int = 1000,
+    ) -> List[Optional[ScopedKey]]:
+        """Set the weights of the TaskHubs associated with the given
+        AlchemicalNetworks.
+
+        Compute services perform a weighted selection of the AlchemicalNetworks
+        visible to them before claiming Tasks actioned on those networks.
+        Networks with higher weight are more likely to be selected than those
+        with lower weight, and so will generally get more compute attention
+        over time.
+
+        A weight of ``0`` means the AlchemicalNetwork will not receive any
+        compute for its actioned Tasks.
+
+        Parameters
+        ----------
+        networks
+            The ScopedKeys of the AlchemicalNetworks to set the weights for.
+        weight
+            The weights to set for the `networks`, in the same order. Each must
+            be between 0 and 1 (inclusive). Setting the value to 0 will
+            effectively disable compute on the networks without cancelling its
+            actioned Tasks. Should be a list of the same length as `networks`.
+
+        Returns
+        -------
+        List[Optional[ScopedKey]]
+            The ScopedKeys of the TaskHubs whose weight changed, in the order
+            that the AlchemicalNetworks ScopedKeys were provided. If one of
+            the specified networks could not be found, a None is returned
+            at its corresponding index.
+        """
+        values = self._batched_attribute_setter(
+            [(network, weight) for network, weight in zip(networks, weights)],
+            self._set_network_weight,
+            batch_size=batch_size,
+        )
+        return [ScopedKey.from_str(value) if value else None for value in values]
 
     def get_transformation_networks(self, transformation: ScopedKey) -> List[ScopedKey]:
         """List ScopedKeys for AlchemicalNetworks associated with the given Transformation."""
         return self._query_resource(f"/transformations/{transformation}/networks")
 
     def get_network_chemicalsystems(self, network: ScopedKey) -> List[ScopedKey]:
         """List ScopedKeys for the ChemicalSystems associated with the given AlchemicalNetwork."""
@@ -466,14 +691,72 @@
         if extends:
             extends = extends.dict()
 
         data = dict(extends=extends, count=count)
         task_sks = self._post_resource(f"/transformations/{transformation}/tasks", data)
         return [ScopedKey.from_str(i) for i in task_sks]
 
+    def create_transformations_tasks(
+        self,
+        transformations: List[ScopedKey],
+        extends: Optional[List[Optional[ScopedKey]]] = None,
+    ) -> List[ScopedKey]:
+        """Create Tasks for multiple Transformations.
+
+        Unlike `create_tasks`, this method can create Tasks for many
+        Transformations. This method should be used instead of `create_tasks`
+        whenever creating Tasks for more than one unique Transformation since it
+        minimizes the number of API requests to the alchemiscale server.
+
+        Parameters
+        ----------
+        transformations
+            A list of ScopedKeys of Transformations to create Tasks for. The
+            same ScopedKey can be repeated to create multiple Tasks for the
+            same Transformation.
+        extends
+            A list of ScopedKeys for the Tasks to be extended. When not `None`,
+            `extends` must be a list of the same length as `transformations`. If
+            a transformation in `transformations` should not extend a Task, use
+            a `None` as a placeholder in the `extends` list.
+
+        Returns
+        -------
+        List[ScopedKey]
+            A list giving the ScopedKeys of the new Tasks created.
+
+        Examples
+        --------
+
+        Instead of looping over Transformations and calling `create_tasks`, make
+        one call to `create_transformations_tasks`.
+
+        >>> client.create_transformations_tasks([transformation_1_sk, transformation_2_sk])
+
+        The behavior of the `count` keyword argument from `create_tasks` can be
+        recreated by repeating the same transformation in the list while also
+        allowing the addition of other transformtions.
+
+        >>> client.create_transformations_tasks([transformation_1_sk] * 3 + [transformation_2_sk] * 2)
+
+        """
+
+        data = dict(
+            transformations=[str(transformation) for transformation in transformations],
+            extends=(
+                None
+                if not extends
+                else [
+                    str(task_sk) if task_sk is not None else None for task_sk in extends
+                ]
+            ),
+        )
+        task_sks = self._post_resource("/bulk/transformations/tasks/create", data)
+        return [ScopedKey.from_str(i) for i in task_sks]
+
     def query_tasks(
         self,
         scope: Optional[Scope] = None,
         status: Optional[str] = None,
     ) -> List[ScopedKey]:
         """Query for Tasks, optionally by status or Scope.
 
@@ -567,35 +850,45 @@
 
         rprint(table)
 
     def get_scope_status(
         self,
         scope: Optional[Scope] = None,
         visualize: Optional[bool] = True,
+        network_state: Optional[Union[NetworkStateEnum, str]] = NetworkStateEnum.active,
     ) -> Dict[str, int]:
         """Return status counts for all Tasks within the given Scope.
 
         Parameters
         ----------
         scope
             Scope to use for querying status. Non-specific Scopes are allowed,
             and will give back counts for all Tasks within that this user has
             Scope access to. Defaults to all Scopes.
         visualize
             If ``True``, print a table of status counts.
+        network_state
+            Regex expression for the network states. Nonexistent state values
+            entered will not raise any warnings. Use ``None`` to get networks
+            regardless of state. Defaults to the "active" state.
 
         Returns
         -------
         status_counts
             Dict giving statuses as keys, Task counts as values.
         """
         if scope is None:
             scope = Scope()
 
-        status_counts = self._get_resource(f"/scopes/{scope}/status")
+        if isinstance(network_state, NetworkStateEnum):
+            network_state = network_state.value
+
+        params = dict(network_state=network_state)
+
+        status_counts = self._get_resource(f"/scopes/{scope}/status", params=params)
 
         if visualize:
             self._visualize_status(status_counts, scope)
 
         return status_counts
 
     def get_network_status(
@@ -604,15 +897,15 @@
         visualize: Optional[bool] = True,
     ) -> Dict[str, int]:
         """Return status counts for all Tasks associated with the given AlchemicalNetwork.
 
         Parameters
         ----------
         network
-            ScopedKey for the Alchemicalnetwork to obtain status counts for.
+            ScopedKey for the AlchemicalNetwork to obtain status counts for.
         visualize
             If ``True``, print a table of status counts.
 
         Returns
         -------
         status_counts
             Dict giving statuses as keys, Task counts as values.
@@ -620,14 +913,39 @@
         status_counts = self._get_resource(f"/networks/{network}/status")
 
         if visualize:
             self._visualize_status(status_counts, network)
 
         return status_counts
 
+    def get_networks_status(
+        self,
+        networks: List[ScopedKey],
+    ) -> List[Dict[str, int]]:
+        """Get the status counts of Tasks for a list of AlchemicalNetworks.
+
+        Parameters
+        ----------
+        networks
+            List of AlchemicalNetwork ScopedKeys to obtain status counts for.
+
+        Returns
+        -------
+        List[Dict[str, int]]
+            A list of dictionaries, in the same order as the provided networks,
+            containing the Task status counts for all Tasks in each network.
+            The dictionary keys are the statuses and the values are the number
+            of Tasks with that status. If either no tasks exist for the
+            Transformations in a network, or the network does not exist in the
+            database, a empty dictionary is returned at the corresponding index.
+        """
+        data = {"networks": [str(network) for network in networks]}
+        status_counts = self._post_resource("/bulk/networks/status", data=data)
+        return status_counts
+
     def get_transformation_status(
         self,
         transformation: ScopedKey,
         visualize: Optional[bool] = True,
     ) -> Dict[str, int]:
         """Return status counts for all Tasks associated with the given
         Transformation.
@@ -677,14 +995,52 @@
         tasks = self._post_resource(f"/networks/{network}/tasks/actioned", data)
 
         if task_weights:
             return {ScopedKey.from_str(t): w for t, w in tasks.items()}
 
         return [ScopedKey.from_str(t) for t in tasks]
 
+    def get_networks_actioned_tasks(
+        self,
+        networks: List[ScopedKey],
+        task_weights: bool = False,
+    ) -> List[Union[Dict[ScopedKey, float], List[ScopedKey]]]:
+        """Get all actioned Tasks for a list of AlchemicalNetwork ScopedKeys.
+
+        Parameters
+        ----------
+        networks
+            A list of AlchemicalNetwork ScopedKeys to retrieve actioned
+            Tasks for.
+
+        Returns
+        -------
+        List[Union[Dict[ScopedKey, float], List[ScopedKey]]]
+            If task_weights is True, a list of dictionaries is returned with
+            the same length as the specified network list. The keys and values
+            of the contained dictionaries are the ScopedKeys and weights of
+            the actioned Tasks, respectively.
+
+            If task_weights is False, only a list of actioned Task ScopedKeys
+            is returned for each network in the specified list.
+        """
+        data = dict(
+            networks=[str(network) for network in networks], task_weights=task_weights
+        )
+        grouped_tasks = self._post_resource("/bulk/networks/tasks/actioned", data=data)
+
+        return_data = []
+        for tasks in grouped_tasks:
+            if task_weights:
+                return_data.append({ScopedKey.from_str(t): w for t, w in tasks.items()})
+            else:
+                return_data.append([ScopedKey.from_str(t) for t in tasks])
+
+        return return_data
+
     def get_task_actioned_networks(
         self, task: ScopedKey, task_weights: bool = False
     ) -> Union[Dict[ScopedKey, float], List[ScopedKey]]:
         """Return all AlchemicalNetworks the given Task is actioned on.
 
         Parameters
         ----------
@@ -780,28 +1136,27 @@
 
         """
         data = dict(tasks=[t.dict() for t in tasks])
         canceled_sks = self._post_resource(f"/networks/{network}/tasks/cancel", data)
 
         return [ScopedKey.from_str(i) if i is not None else None for i in canceled_sks]
 
-    def _task_attribute_getter(
-        self, tasks: List[ScopedKey], getter_function, batch_size
+    def _batched_attribute_getter(
+        self,
+        batchables: List[Any],
+        getter_function,
+        batch_size,
     ) -> List[Any]:
-        tasks = [
-            ScopedKey.from_str(task) if isinstance(task, str) else task
-            for task in tasks
-        ]
 
         @use_session
         async def async_request(self):
             values = await asyncio.gather(
                 *[
-                    getter_function(task_batch)
-                    for task_batch in self._batched(tasks, batch_size)
+                    getter_function(batch)
+                    for batch in self._batched(batchables, batch_size)
                 ]
             )
 
             return list(chain.from_iterable(values))
 
         coro = async_request(self)
 
@@ -811,31 +1166,38 @@
             # we use nest_asyncio to support environments where an event loop
             # is already running, such as in a Jupyter notebook
             import nest_asyncio
 
             nest_asyncio.apply()
             return asyncio.run(coro)
 
-    def _task_attribute_setter(
-        self, tasks: List[ScopedKey], setter_function, setter_args, batch_size
+    def _batched_attribute_setter(
+        self,
+        batchables: List[Any],
+        setter_function,
+        setter_args: Iterable[Any] = None,
+        batch_size: int = 1000,
+        should_return=True,
     ) -> List[Optional[ScopedKey]]:
-        tasks = [
-            ScopedKey.from_str(task) if isinstance(task, str) else task
-            for task in tasks
-        ]
+
+        if setter_args is None:
+            setter_args = []
 
         @use_session
         async def async_request(self):
             scoped_keys = await asyncio.gather(
                 *[
-                    setter_function(task_batch, *setter_args)
-                    for task_batch in self._batched(tasks, batch_size)
+                    setter_function(batch, *setter_args)
+                    for batch in self._batched(batchables, batch_size)
                 ]
             )
 
+            if not should_return:
+                return None
+
             return list(chain.from_iterable(scoped_keys))
 
         coro = async_request(self)
 
         try:
             return asyncio.run(coro)
         except RuntimeError:
@@ -884,22 +1246,22 @@
             The ScopedKeys of the Tasks that were updated, in the same order
             as given in `tasks`. If a given Task doesn't exist, ``None`` will
             be returned in its place.
 
         """
         status = TaskStatusEnum(status)
 
-        return self._task_attribute_setter(
+        return self._batched_attribute_setter(
             tasks, self._set_task_status, (status,), batch_size
         )
 
     async def _get_task_status(self, tasks: List[ScopedKey]) -> List[TaskStatusEnum]:
         """Get the statuses for many Tasks"""
         data = dict(tasks=[t.dict() for t in tasks])
-        statuses = await self._post_resource_async(f"/bulk/tasks/status/get", data=data)
+        statuses = await self._post_resource_async("/bulk/tasks/status/get", data=data)
         return statuses
 
     def get_tasks_status(
         self, tasks: List[ScopedKey], batch_size: int = 1000
     ) -> List[str]:
         """Get the status of multiple Tasks.
 
@@ -914,15 +1276,15 @@
         Returns
         -------
         statuses
             The status of each Task in the same order as given in `tasks`. If a
             given Task doesn't exist, ``None`` will be returned in its place.
 
         """
-        return self._task_attribute_getter(tasks, self._get_task_status, batch_size)
+        return self._batched_attribute_getter(tasks, self._get_task_status, batch_size)
 
     async def _set_task_priority(
         self, tasks: List[ScopedKey], priority: int
     ) -> List[Optional[ScopedKey]]:
         data = dict(tasks=[t.dict() for t in tasks], priority=priority)
         tasks_updated = await self._post_resource_async(
             f"/bulk/tasks/priority/set", data=data
@@ -954,15 +1316,15 @@
         Returns
         -------
         updated
             The ScopedKeys of the Tasks that were updated, in the same order
             as given in `tasks`. If a given Task doesn't exist, ``None`` will
             be returned in its place.
         """
-        return self._task_attribute_setter(
+        return self._batched_attribute_setter(
             tasks, self._set_task_priority, (priority,), batch_size
         )
 
     async def _get_task_priority(self, tasks: List[ScopedKey]) -> List[int]:
         """Get the priority for many Tasks"""
         data = dict(tasks=[t.dict() for t in tasks])
         priorities = await self._post_resource_async(
@@ -988,15 +1350,17 @@
         Returns
         -------
         priorities
             The priority of each Task in the same order as given in `tasks`. If a
             given Task doesn't exist, ``None`` will be returned in its place.
 
         """
-        return self._task_attribute_getter(tasks, self._get_task_priority, batch_size)
+        return self._batched_attribute_getter(
+            tasks, self._get_task_priority, batch_size
+        )
 
     ### results
 
     @alru_cache(maxsize=10000)
     async def _async_get_protocoldagresult(
         self, protocoldagresultref, transformation, route, compress
     ):
```

### Comparing `alchemiscale-0.3.0/alchemiscale/keyedchain.py` & `alchemiscale-0.4.0/alchemiscale/keyedchain.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.3.0/alchemiscale/models.py` & `alchemiscale-0.4.0/alchemiscale/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 :mod:`alchemiscale.models` --- common data models
 =================================================
 
 """
+
 from typing import Optional, Union
 from pydantic import BaseModel, Field, validator, root_validator
 from gufe.tokenization import GufeKey
 from re import fullmatch
 
 
 class Scope(BaseModel):
@@ -167,16 +168,15 @@
         return self.dict()
 
     @classmethod
     def from_dict(cls, d):
         return cls(**d)
 
 
-class InvalidScopeError(ValueError):
-    ...
+class InvalidScopeError(ValueError): ...
 
 
 def _is_wildcard(char: Union[str, None]) -> bool:
     return char is None
 
 
 def _find_wildcard(scope_list: list) -> Union[int, None]:
```

### Comparing `alchemiscale-0.3.0/alchemiscale/security/auth.py` & `alchemiscale-0.4.0/alchemiscale/security/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,15 @@
     if entity is None:
         return False
     if not pwd_context.verify(key, entity.hashed_key):
         return False
     return entity
 
 
-class AuthenticationError(Exception):
-    ...
+class AuthenticationError(Exception): ...
 
 
 def hash_key(key):
     return pwd_context.hash(key)
 
 
 def create_access_token(
```

### Comparing `alchemiscale-0.3.0/alchemiscale/security/models.py` & `alchemiscale-0.4.0/alchemiscale/security/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,17 +49,15 @@
 
 
 class UserIdentity(ScopedIdentity):
     email: Optional[str] = None
     full_name: Optional[str] = None
 
 
-class CredentialedUserIdentity(UserIdentity, CredentialedEntity):
-    ...
+class CredentialedUserIdentity(UserIdentity, CredentialedEntity): ...
 
 
 class ComputeIdentity(ScopedIdentity):
     email: Optional[str] = None
 
 
-class CredentialedComputeIdentity(ComputeIdentity, CredentialedEntity):
-    ...
+class CredentialedComputeIdentity(ComputeIdentity, CredentialedEntity): ...
```

### Comparing `alchemiscale-0.3.0/alchemiscale/settings.py` & `alchemiscale-0.4.0/alchemiscale/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,15 @@
     """
 
     JWT_SECRET_KEY: str
     JWT_EXPIRE_SECONDS: int = 1800
     JWT_ALGORITHM: str = "HS256"
 
 
-class BaseAPISettings(Neo4jStoreSettings, S3ObjectStoreSettings, JWTSettings):
-    ...
+class BaseAPISettings(Neo4jStoreSettings, S3ObjectStoreSettings, JWTSettings): ...
 
 
 class APISettings(BaseAPISettings):
     """Automatically populates settings from environment variables where they
     match; case-insensitive.
 
     """
```

### Comparing `alchemiscale-0.3.0/alchemiscale/storage/models.py` & `alchemiscale-0.4.0/alchemiscale/storage/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 :mod:`alchemiscale.storage.models` --- data models for storage components
 =========================================================================
 
 """
 
+from abc import abstractmethod
 from copy import copy
 from datetime import datetime
 from enum import Enum
 from typing import Union, Dict, Optional
 from uuid import uuid4
 import hashlib
 
 
 from pydantic import BaseModel, Field
 from gufe.tokenization import GufeTokenizable, GufeKey
 
 from ..models import ScopedKey, Scope
 
 
-class ComputeServiceID(str):
-    ...
+class ComputeServiceID(str): ...
 
 
 class ComputeServiceRegistration(BaseModel):
     """Registration for AlchemiscaleComputeService instances."""
 
     identifier: ComputeServiceID
     registered: datetime
@@ -187,14 +187,85 @@
         return cls(**d)
 
     @classmethod
     def _defaults(cls):
         return super()._defaults()
 
 
+class Mark(GufeTokenizable):
+
+    def __init__(self, target: ScopedKey):
+        self.target = str(target)
+
+    @abstractmethod
+    def _to_dict(self):
+        raise NotImplementedError
+
+    def _gufe_tokenize(self):
+        hash_string = str(self.target)
+        return hashlib.md5(hash_string.encode(), usedforsecurity=False).hexdigest()
+
+    @classmethod
+    def _from_dict(cls, d):
+        return cls(**d)
+
+    @classmethod
+    def _defaults(cls):
+        return super()._defaults()
+
+
+class NetworkStateEnum(Enum):
+    active = "active"
+    inactive = "inactive"
+    invalid = "invalid"
+    deleted = "deleted"
+
+
+class NetworkMark(Mark):
+    """Mark object for AlchemicalNetworks.
+
+    Attributes
+    ----------
+    network : str
+        ScopedKey of the AlchemicalNetwork this NetworkMark corresponds to.
+        Used to ensure that there is only one NetworkMark for a given
+        AlchemicalNetwork using neo4j constraints.
+
+    state : NetworkStateEnum
+        State of the AlchemicalNetwork, stored on this NetworkMark.
+    """
+
+    network: str
+    state: NetworkStateEnum
+
+    def __init__(
+        self,
+        target: ScopedKey,
+        state: Union[str, NetworkStateEnum] = NetworkStateEnum.active,
+    ):
+        self.state = state
+        super().__init__(target)
+
+    @property
+    def state(self):
+        return self._state
+
+    @state.setter
+    def state(self, state_value):
+        try:
+            self._state = NetworkStateEnum(state_value)
+        except ValueError:
+            valid_states_string = ", ".join(sorted([i.value for i in NetworkStateEnum]))
+            msg = f"`state` = {state_value} must be one of the following: {valid_states_string}"
+            raise ValueError(msg)
+
+    def _to_dict(self):
+        return {"target": self.target, "state": self._state.value}
+
+
 class TaskArchive(GufeTokenizable):
     ...
 
     def _to_dict(self):
         return {}
 
     @classmethod
@@ -256,27 +327,25 @@
 
     def _to_dict(self):
         return {
             "location": self.location,
             "obj_key": str(self.obj_key),
             "scope": str(self.scope),
             "ok": self.ok,
-            "datetime_created": self.datetime_created.isoformat()
-            if self.datetime_created is not None
-            else None,
+            "datetime_created": (
+                self.datetime_created.isoformat()
+                if self.datetime_created is not None
+                else None
+            ),
             "creator": self.creator,
         }
 
     @classmethod
     def _from_dict(cls, d):
         d_ = copy(d)
         d_["datetime_created"] = (
             datetime.fromisoformat(d["datetime_created"])
             if d.get("received") is not None
             else None
         )
 
         return super()._from_dict(d_)
-
-
-class TaskArchive(GufeTokenizable):
-    ...
```

### Comparing `alchemiscale-0.3.0/alchemiscale/storage/objectstore.py` & `alchemiscale-0.4.0/alchemiscale/storage/objectstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         session=session,
         bucket=settings.AWS_S3_BUCKET,
         prefix=settings.AWS_S3_PREFIX,
         endpoint_url=endpoint_url,
     )
 
 
-class S3ObjectStoreError(Exception):
-    ...
+class S3ObjectStoreError(Exception): ...
 
 
 class S3ObjectStore:
     """Object storage for use with AWS S3."""
 
     def __init__(
         self, session: "boto3.Session", bucket: str, prefix: str, endpoint_url=None
```

### Comparing `alchemiscale-0.3.0/alchemiscale/storage/statestore.py` & `alchemiscale-0.4.0/alchemiscale/storage/statestore.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,127 +5,132 @@
 """
 
 import abc
 from datetime import datetime
 from contextlib import contextmanager
 import json
 from functools import lru_cache
-from time import sleep
-from typing import Dict, List, Optional, Union, Tuple, Set
+from typing import Dict, List, Optional, Union, Tuple
 import weakref
 import numpy as np
 
 import networkx as nx
-from gufe import AlchemicalNetwork, Transformation, Settings
+from gufe import AlchemicalNetwork, Transformation, NonTransformation, Settings
 from gufe.tokenization import GufeTokenizable, GufeKey, JSON_HANDLER
-from py2neo import Graph, Node, Relationship, Subgraph
-from py2neo.database import Transaction
-from py2neo.matching import NodeMatcher
-from py2neo.errors import ClientError
+
+from neo4j import Transaction, GraphDatabase, Driver
 
 from .models import (
     ComputeServiceID,
     ComputeServiceRegistration,
+    NetworkMark,
+    NetworkStateEnum,
     Task,
     TaskHub,
-    TaskArchive,
     TaskStatusEnum,
     ProtocolDAGResultRef,
 )
 from ..strategies import Strategy
 from ..models import Scope, ScopedKey
+from .cypher import cypher_list_from_scoped_keys
 
 from ..security.models import CredentialedEntity
-from ..settings import Neo4jStoreSettings, get_neo4jstore_settings
+from ..settings import Neo4jStoreSettings
 from ..validators import validate_network_nonself
 
+from .subgraph import (
+    Node,
+    Relationship,
+    Subgraph,
+    create_subgraph,
+    merge_subgraph,
+    record_data_to_node,
+    subgraph_from_path_record,
+)
+
 
 @lru_cache()
 def get_n4js(settings: Neo4jStoreSettings):
     """Convenience function for getting a Neo4jStore directly from settings."""
-    graph = Graph(
-        settings.NEO4J_URL,
-        auth=(settings.NEO4J_USER, settings.NEO4J_PASS),
-        name=settings.NEO4J_DBNAME,
+
+    graph = GraphDatabase.driver(
+        settings.NEO4J_URL, auth=(settings.NEO4J_USER, settings.NEO4J_PASS)
     )
-    return Neo4jStore(graph)
+    return Neo4jStore(graph, db_name=settings.NEO4J_DBNAME)
 
 
-class Neo4JStoreError(Exception):
-    ...
+class Neo4JStoreError(Exception): ...
 
 
-class AlchemiscaleStateStore(abc.ABC):
-    ...
+class AlchemiscaleStateStore(abc.ABC): ...
 
 
-def _select_task_from_taskpool(taskpool: Subgraph) -> Union[ScopedKey, None]:
-    """
-    Select a Task from a pool of tasks in a neo4j subgraph according to the following scheme:
+def _select_tasks_from_taskpool(taskpool: List[Tuple[str, float]], count) -> List[str]:
+    """Select Tasks from a pool of tasks according to the following scheme:
 
-    PRE: taskpool is a subgraph of Tasks of equal priority with a weight on their ACTIONS relationship.
-    The records in the subgraph are :ACTIONS relationships with two properties: 'task' and 'weight'.
-    1. Randomly select 1 Task from the TaskPool based on weighting
-    2. Return the ScopedKey of the Task.
+    1. Randomly select N=`count` tasks from the TaskPool based on weighting
+    2. Return the string representation of the Task ScopedKeys.
 
     Parameters
     ----------
-    taskpool: 'subgraph'
-        A subgraph of Tasks of equal priority with a weight on their ACTIONS relationship.
+    taskpool: List[Tuple[str, float]]
+        A list of tuples containing Tasks (string represtnation of their ScopedKeys) of
+        equal priority with the weights of their ACTIONS relationships.
 
     Returns
     -------
-    sk: ScopedKey
-        The ScopedKey of the Task selected from the taskpool.
+    sk: List[str]
+        The string representations of the ScopedKeys of the Tasks selected from the taskpool.
     """
-    tasks = []
     weights = []
-    for actions in taskpool.relationships:
-        tasks.append(actions.get("task"))
-        weights.append(actions.get("weight"))
+    tasks = []
+    for t, w in taskpool:
+        tasks.append(t)
+        weights.append(w)
 
-    # normalize weights
     weights = np.array(weights)
-    weights = weights / weights.sum()
+    prob = weights / weights.sum()
 
-    # randomly select a task from the taskpool based on weights without replacement
-    # NOTE: if useful could expand this to select multiple tasks
-    chosen_one = np.random.choice(tasks, 1, p=weights, replace=False)
-    return chosen_one[0]
+    return list(np.random.choice(tasks, count, replace=False, p=prob))
 
 
 def _generate_claim_query(
-    task_sk: ScopedKey, compute_service_id: ComputeServiceID
+    task_sks: List[ScopedKey], compute_service_id: ComputeServiceID
 ) -> str:
-    """
-    Generate a query to claim a single Task.
+    """Generate a query to claim a list of Tasks.
+
     Parameters
     ----------
-    task_sk
-        The ScopedKey of the Task to claim.
+    task_sks
+        A list of ScopedKeys of Tasks to claim.
     compute_service_id
         ComputeServiceID of the claiming service.
 
     Returns
     -------
     query: str
         The Cypher query to claim the Task.
     """
+
+    task_data = cypher_list_from_scoped_keys(task_sks)
+
     query = f"""
     // only match the task if it doesn't have an existing CLAIMS relationship
-    MATCH (t:Task {{_scoped_key: '{task_sk}'}})
+    UNWIND {task_data} AS task_sk
+    MATCH (t:Task {{_scoped_key: task_sk}})
     WHERE NOT (t)<-[:CLAIMS]-(:ComputeServiceRegistration)
-    SET t.status = 'running'
 
     WITH t
 
     // create CLAIMS relationship with given compute service
     MATCH (csreg:ComputeServiceRegistration {{identifier: '{compute_service_id}'}})
     CREATE (t)<-[cl:CLAIMS {{claimed: localdatetime('{datetime.utcnow().isoformat()}')}}]-(csreg)
 
+    SET t.status = '{TaskStatusEnum.running.value}'
+
     RETURN t
     """
     return query
 
 
 class Neo4jStore(AlchemiscaleStateStore):
     # uniqueness constraints applied to the database; key is node label,
@@ -143,61 +148,63 @@
         },
         "ComputeServiceRegistration": {
             "name": "compute_service_registration_identifier",
             "property": "identifier",
         },
     }
 
-    def __init__(self, graph: "py2neo.Graph"):
-        self.graph: Graph = graph
+    def __init__(self, graph: Driver, db_name: str = "neo4j"):
+        self.graph: Driver = graph
+        self.db_name = db_name
         self.gufe_nodes = weakref.WeakValueDictionary()
 
     @contextmanager
-    def transaction(self, readonly=False, ignore_exceptions=False) -> Transaction:
-        """Context manager for a py2neo Transaction."""
-        tx = self.graph.begin(readonly=readonly)
-        try:
-            yield tx
-        except:
-            self.graph.rollback(tx)
-            if not ignore_exceptions:
-                raise
+    def transaction(self, ignore_exceptions=False) -> Transaction:
+        """Context manager for a Neo4j Transaction."""
+        with self.graph.session(database=self.db_name) as session:
+            tx = session.begin_transaction()
+            try:
+                yield tx
+            except:
+                tx.rollback()
+                if not ignore_exceptions:
+                    raise
 
-        else:
-            self.graph.commit(tx)
+            else:
+                tx.commit()
+
+    def execute_query(self, *args, **kwargs):
+        kwargs.update({"database_": self.db_name})
+        return self.graph.execute_query(*args, **kwargs)
 
     def initialize(self):
         """Initialize database.
 
         Ensures that constraints and any other required structures are in place.
         Should be used on any Neo4j database prior to use for Alchemiscale.
 
         """
         for label, values in self.constraints.items():
-            self.graph.run(
+            self.execute_query(
                 f"""
                 CREATE CONSTRAINT {values['name']} IF NOT EXISTS
                 FOR (n:{label}) REQUIRE n.{values['property']} is unique
             """
             )
 
-        # make sure we don't get objects with id 0 by creating at least one
-        # this is a compensating control for a bug in py2neo, where nodes with id 0 are not properly
-        # deduplicated by Subgraph set operations, which we currently rely on
-        # see this PR: https://github.com/py2neo-org/py2neo/pull/951
-        self.graph.run("MERGE (:NOPE)")
-
     def check(self):
         """Check consistency of database.
 
         Will raise `Neo4JStoreError` if any state check fails.
         If no check fails, will return without any exception.
 
         """
-        constraints = {rec["name"]: rec for rec in self.graph.run("show constraints")}
+        constraints = {
+            rec["name"]: rec for rec in self.execute_query("show constraints").records
+        }
 
         if len(constraints) != len(self.constraints):
             raise Neo4JStoreError(
                 f"Number of constraints in database is {len(constraints)}; expected {len(self.constraints)}"
             )
 
         for label, values in self.constraints.items():
@@ -206,37 +213,29 @@
                 constraint["labelsOrTypes"] == [label]
                 and constraint["properties"] == [values["property"]]
             ):
                 raise Neo4JStoreError(
                     f"Constraint {constraint['name']} does not have expected form"
                 )
 
-        nope = self.graph.run("MATCH (n:NOPE) RETURN n").to_subgraph()
-        if nope.identity != 0:
-            raise Neo4JStoreError("Identity of NOPE node is not exactly 0")
-
     def _store_check(self):
         """Check that the database is in a state that can be used by the API."""
         try:
             # just list available functions to see if database is working
-            self.graph.run("SHOW FUNCTIONS YIELD *")
-        except:
+            self.execute_query("SHOW FUNCTIONS YIELD *")
+        except Exception:
             return False
         return True
 
     def reset(self):
         """Remove all data from database; undo all components in `initialize`."""
-        # we'll keep NOPE around to avoid a case where Neo4j doesn't give it id 0
-        # after a series of wipes; appears to happen often enough in tests
-        # can remove this once py2neo#951 merged
-        # self.graph.run("MATCH (n) DETACH DELETE n")
-        self.graph.run("MATCH (n) WHERE NOT n:NOPE DETACH DELETE n")
+        self.execute_query("MATCH (n) DETACH DELETE n")
 
         for label, values in self.constraints.items():
-            self.graph.run(
+            self.execute_query(
                 f"""
                 DROP CONSTRAINT {values['name']} IF EXISTS
             """
             )
 
     ## gufe object handling
 
@@ -488,20 +487,21 @@
             q += """
             RETURN n
             """
 
         nodes = set()
         subgraph = Subgraph()
 
-        for record in self.graph.run(q):
-            nodes.add(record["n"])
+        for record in self.execute_query(q).records:
+            node = record_data_to_node(record["n"])
+            nodes.add(node)
             if return_subgraph and record["p"] is not None:
-                subgraph = subgraph | record["p"]
+                subgraph = subgraph | subgraph_from_path_record(record["p"])
             else:
-                subgraph = record["n"]
+                subgraph = node
 
         if len(nodes) == 0:
             raise KeyError("No such object in database")
         elif len(nodes) > 1:
             raise Neo4JStoreError(
                 "More than one such object in database; this should not be possible"
             )
@@ -556,26 +556,28 @@
             RETURN n,p
             """
         else:
             q += """
             RETURN DISTINCT n
             ORDER BY n._org, n._campaign, n._project, n._gufe_key
             """
+
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q).to_eager_result()
 
         nodes = list()
         subgraph = Subgraph()
 
-        for record in res:
-            nodes.append(record["n"])
+        for record in res.records:
+            node = record_data_to_node(record["n"])
+            nodes.append(node)
             if return_gufe and record["p"] is not None:
-                subgraph = subgraph | record["p"]
+                subgraph = subgraph | subgraph_from_path_record(record["p"])
             else:
-                subgraph = record["n"]
+                subgraph = node
 
         if return_gufe:
             return {
                 ScopedKey.from_str(k["_scoped_key"]): v
                 for k, v in self._subgraph_to_gufe(nodes, subgraph).items()
             }
         else:
@@ -602,33 +604,78 @@
 
         return res[0]
 
     def get_gufe(self, scoped_key: ScopedKey):
         node, subgraph = self._get_node(scoped_key=scoped_key, return_subgraph=True)
         return self._subgraph_to_gufe([node], subgraph)[node]
 
-    def create_network(self, network: AlchemicalNetwork, scope: Scope):
-        """Add an `AlchemicalNetwork` to the target neo4j database, even if
-        some of its components already exist in the database.
+    def assemble_network(
+        self,
+        network: AlchemicalNetwork,
+        scope: Scope,
+        state: Union[NetworkStateEnum, str] = NetworkStateEnum.active,
+    ):
+        """Create all nodes and relationships needed for an AlchemicalNetwork
+        represented in an alchemiscale state store.
+
+        Parameters
+        ----------
+        network
+            The AlchemicalNetwork to submit to the database.
+        scope
+            The Scope where the AlchemicalNetwork resides.
+        state
+            The starting state of the network as marked by the NetworkMark.
+
+        Returns
+        -------
+        A tuple containing the AlchemicalNetwork ScopedKey, the TaskHub
+        ScopedKey, and the NetworkMark ScopedKey.
+        """
+
+        nw_subgraph, nw_node, nw_sk = self.create_network_subgraph(network, scope)
+        th_subgraph, th_node, th_sk = self.create_taskhub_subgraph(nw_node)
+        nm_subgraph, nm_node, nm_sk = self.create_network_mark_subgraph(nw_node, state)
+
+        subgraph = nw_subgraph | th_subgraph | nm_subgraph
+
+        with self.transaction() as tx:
+            merge_subgraph(tx, subgraph, "GufeTokenizable", "_scoped_key")
+
+        return nw_sk, th_sk, nm_sk
+
+    def create_network_subgraph(self, network: AlchemicalNetwork, scope: Scope):
+        """Create a Subgraph for the given AlchemicalNetwork.
+
+        Parameters
+        ----------
+        network
+            An AlchemicalNetwork to generate a Subgraph form of.
+        scope
+            The Scope where the AlchemicalNetwork resides.
 
+        Returns
+        -------
+        A tuple containing the AlchemicalNetwork Subgraph, the specific
+        AlchemicalNetwork Node within the Subgraph, and the ScopedKey of the
+        AlchemicalNetwork.
         """
+
         validate_network_nonself(network)
 
         ndict = network.to_shallow_dict()
 
-        g, n, scoped_key = self._gufe_to_subgraph(
+        subgraph, node, scoped_key = self._gufe_to_subgraph(
             ndict,
             labels=["GufeTokenizable", network.__class__.__name__],
             gufe_key=network.key,
             scope=scope,
         )
-        with self.transaction() as tx:
-            tx.merge(g, "GufeTokenizable", "_scoped_key")
 
-        return scoped_key
+        return subgraph, node, scoped_key
 
     def delete_network(
         self,
         network: ScopedKey,
     ) -> ScopedKey:
         """Delete the given `AlchemicalNetwork` from the database.
 
@@ -654,34 +701,193 @@
         self.delete_taskhub(network)
 
         # then delete the network
         q = f"""
         MATCH (an:AlchemicalNetwork {{_scoped_key: "{network}"}})
         DETACH DELETE an
         """
-        return network
+        raise NotImplementedError
+
+    def get_network_state(self, networks: List[ScopedKey]) -> List[Optional[str]]:
+        """Get the states of a group of networks.
+
+        Parameters
+        ----------
+        networks
+            The list networks to get the states of.
+
+        Returns
+        -------
+        List[Optional[str]]
+            A list containing the states of the given networks, in the same
+            order as they were provided. If a network was not found, ``None``
+            is returned at the corresponding index.
+        """
+
+        q = """
+            UNWIND $networks AS network
+            MATCH (an:AlchemicalNetwork {`_scoped_key`: network})<-[:MARKS]-(nm:NetworkMark)
+            RETURN an._scoped_key as sk, nm.state AS state
+        """
+
+        results = self.execute_query(q, networks=[str(network) for network in networks])
+
+        state_results = {}
+        for record in results.records:
+            sk = record["sk"]
+            state = record["state"]
+
+            state_results[sk] = state
+
+        return [state_results.get(str(network), None) for network in networks]
+
+    def create_network_mark_subgraph(
+        self, network_node: Node, state=NetworkStateEnum.active
+    ):
+        """Create the Subgraph for an AlchemicalNetwork's NetworkMark.
+
+        Parameters
+        ----------
+        network_node
+            A Node representing the target AlchemicalNetwork. This is
+            a returned value from the :py:meth:`create_network_subgraph`
+            method.
+        state
+            The starting state for the AlchemicalNetwork.
+
+        Returns
+        -------
+        A tuple containing the NetworkMark Subgraph, the specific NetworkMark
+        Node within the Subgraph, and the ScopedKey of the NetworkMark.
+        """
+
+        network_sk = ScopedKey.from_str(network_node["_scoped_key"])
+        scope = network_sk.scope
+
+        network_mark = NetworkMark(target=str(network_sk), state=state)
+
+        _, network_mark_node, scoped_key = self._gufe_to_subgraph(
+            network_mark.to_shallow_dict(),
+            labels=["GufeTokenizable", network_mark.__class__.__name__],
+            gufe_key=network_mark.key,
+            scope=scope,
+        )
+
+        subgraph = Relationship.type("MARKS")(
+            network_mark_node,
+            network_node,
+            _org=scope.org,
+            _campaign=scope.campaign,
+            _project=scope.project,
+        )
+
+        return subgraph, network_mark_node, scoped_key
+
+    def set_network_state(
+        self, networks: List[ScopedKey], states: List[str]
+    ) -> List[Optional[ScopedKey]]:
+        """Set the state of a group of AlchemicalNetworks.
+
+        Parameters
+        ----------
+        networks
+            A list networks to set the states for.
+        states
+            A list of states to set the networks to.
+
+        Returns
+        -------
+        List[Optional[ScopedKey]]
+            The list of ScopedKeys for networks that were updated. If the
+            network could not be found in the database, ``None`` is returned at
+            the corresponding index.
+        """
+
+        if len(networks) != len(states):
+            msg = "networks and states must have the same length"
+            raise ValueError(msg)
+
+        for network, state in zip(networks, states):
+            if network.qualname != "AlchemicalNetwork":
+                raise ValueError(
+                    "`network` ScopedKey does not correspond to an `AlchemicalNetwork`"
+                )
+            try:
+                NetworkStateEnum(state)
+            except ValueError:
+                valid_states = [state.value for state in NetworkStateEnum]
+                msg = f"'{state}' is not a valid state. Valid values include: {valid_states}"
+                raise ValueError(msg)
+
+        q = """
+            WITH $inputs AS inputs
+            UNWIND inputs AS x
+            WITH x[0] as network, x[1] as state
+            MATCH (:AlchemicalNetwork {`_scoped_key`: network})<-[:MARKS]-(nm:NetworkMark)
+            SET nm.state = state
+            RETURN network
+        """
+        inputs = [[str(network), state] for network, state in zip(networks, states)]
+
+        results = self.execute_query(q, inputs=inputs)
+
+        network_results = {}
+        for record in results.records:
+            network_sk_str = record["network"]
+            network_results[network_sk_str] = ScopedKey.from_str(network_sk_str)
+
+        return [network_results.get(str(network), None) for network in networks]
 
     def query_networks(
         self,
         *,
         name=None,
         key=None,
         scope: Optional[Scope] = Scope(),
-        return_gufe: bool = False,
-    ):
+        state: Optional[str] = None,
+    ) -> List[ScopedKey]:
         """Query for `AlchemicalNetwork`\s matching given attributes."""
-        additional = {"name": name}
-        return self._query(
-            qualname="AlchemicalNetwork",
-            additional=additional,
-            key=key,
-            scope=scope,
-            return_gufe=return_gufe,
+
+        query_params = dict(
+            name_pattern=name,
+            org_pattern=scope.org,
+            campaign_pattern=scope.campaign,
+            project_pattern=scope.project,
+            state_pattern=state,
+            gufe_key_pattern=None if key is None else str(key),
+        )
+
+        for k, v in query_params.items():
+            if v is None:
+                query_params[k] = ".*"
+
+        q = """
+            MATCH (an:AlchemicalNetwork)<-[:MARKS]-(nm:NetworkMark)
+            WHERE
+                    an.name =~ $name_pattern
+                AND an.`_gufe_key` =~ $gufe_key_pattern
+                AND an.`_org` =~ $org_pattern
+                AND an.`_campaign` =~ $campaign_pattern
+                AND an.`_project` =~ $project_pattern
+                AND nm.state =~ $state_pattern
+            RETURN an._scoped_key as sk
+        """
+
+        results = self.execute_query(
+            q,
+            parameters_=query_params,
         )
 
+        network_sks = []
+        for record in results.records:
+            sk = record["sk"]
+            network_sks.append(ScopedKey.from_str(sk))
+
+        return network_sks
+
     def query_transformations(self, *, name=None, key=None, scope: Scope = Scope()):
         """Query for `Transformation`\s matching given attributes."""
         additional = {"name": name}
         return self._query(
             qualname="Transformation", additional=additional, key=key, scope=scope
         )
 
@@ -850,15 +1056,15 @@
         """
 
         node = Node(
             "ComputeServiceRegistration", **compute_service_registration.to_dict()
         )
 
         with self.transaction() as tx:
-            tx.create(node)
+            create_subgraph(tx, Subgraph() | node)
 
         return compute_service_registration.identifier
 
     def deregister_computeservice(self, compute_service_id: ComputeServiceID):
         """Remove the registration for the given ComputeServiceID from the
         state store.
 
@@ -895,15 +1101,14 @@
         """Update the heartbeat for the given ComputeServiceID."""
 
         q = f"""
         MATCH (n:ComputeServiceRegistration {{identifier: '{compute_service_id}'}})
         SET n.heartbeat = localdatetime('{heartbeat.isoformat()}')
 
         """
-
         with self.transaction() as tx:
             tx.run(q)
 
         return compute_service_id
 
     def expire_registrations(self, expire_time: datetime):
         """Remove all registrations with last heartbeat prior to the given `expire_time`."""
@@ -929,39 +1134,33 @@
             for rec in res:
                 identities.add(rec["ident"])
 
         return [ComputeServiceID(i) for i in identities]
 
     ## task hubs
 
-    def create_taskhub(
-        self,
-        network: ScopedKey,
-    ) -> ScopedKey:
-        """Create a TaskHub for the given AlchemicalNetwork.
-
-        An AlchemicalNetwork can have only one associated TaskHub.
-        A TaskHub is required to action Tasks for a given AlchemicalNetwork.
+    def create_taskhub_subgraph(self, network_node: Node):
+        """Create a Subgraph for an AlchemicalNetwork's TaskHub.
 
-        This method will only create a TaskHub for an AlchemicalNetwork if it
-        doesn't already exist; it will return the scoped key for the TaskHub
-        either way.
+        Parameters
+        ----------
+        network_node
+            A Node representing the target AlchemicalNetwork. This is
+            a returned value from the :py:meth:`create_network_subgraph`
+            method.
 
+        Returns
+        -------
+        A tuple containing the TaskHub Subgraph, the specific TaskHub
+        Node within the Subgraph, and the ScopedKey of the TaskHub.
         """
-        if network.qualname != "AlchemicalNetwork":
-            raise ValueError(
-                "`network` ScopedKey does not correspond to an `AlchemicalNetwork`"
-            )
+        network_sk = ScopedKey.from_str(network_node["_scoped_key"])
+        scope = network_sk.scope
 
-        scope = network.scope
-        network_node = self._get_node(network)
-
-        # create a taskhub for the supplied network
-        # use a PERFORMS relationship
-        taskhub = TaskHub(network=str(network))
+        taskhub = TaskHub(network=str(network_sk))
         _, taskhub_node, scoped_key = self._gufe_to_subgraph(
             taskhub.to_shallow_dict(),
             labels=["GufeTokenizable", taskhub.__class__.__name__],
             gufe_key=taskhub.key,
             scope=scope,
         )
 
@@ -969,20 +1168,15 @@
             taskhub_node,
             network_node,
             _org=scope.org,
             _campaign=scope.campaign,
             _project=scope.project,
         )
 
-        # if the TaskHub already exists, this will rollback transaction
-        # automatically
-        with self.transaction(ignore_exceptions=True) as tx:
-            tx.create(subgraph)
-
-        return scoped_key
+        return subgraph, taskhub_node, scoped_key
 
     def query_taskhubs(
         self, scope: Optional[Scope] = Scope(), return_gufe: bool = False
     ) -> Union[List[ScopedKey], Dict[ScopedKey, TaskHub]]:
         """Query for `TaskHub`\s matching the given criteria.
 
         Parameters
@@ -1007,20 +1201,19 @@
 
         """
         if network.qualname != "AlchemicalNetwork":
             raise ValueError(
                 "`network` ScopedKey does not correspond to an `AlchemicalNetwork`"
             )
 
-        node = self.graph.run(
-            f"""
+        q = f"""
                 match (th:TaskHub {{network: "{network}"}})-[:PERFORMS]->(an:AlchemicalNetwork)
                 return th
                 """
-        ).to_subgraph()
+        node = record_data_to_node(self.execute_query(q).records[0]["th"])
 
         if return_gufe:
             return self._subgraph_to_gufe([node], node)[node]
         else:
             return ScopedKey.from_str(node["_scoped_key"])
 
     def delete_taskhub(
@@ -1036,70 +1229,93 @@
 
         taskhub = self.get_taskhub(network)
 
         q = f"""
         MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}}),
         DETACH DELETE th
         """
-        self.graph.run(q)
+        self.execute_query(q)
 
         return taskhub
 
-    def set_taskhub_weight(self, network: ScopedKey, weight: float):
-        """Set the weight for the TaskHub associated with the given
-        AlchemicalNetwork.
+    def set_taskhub_weight(
+        self, networks: List[ScopedKey], weights: List[float]
+    ) -> List[Optional[ScopedKey]]:
+        """Set the weights for the TaskHubs associated with the given
+        AlchemicalNetworks.
 
         """
 
-        if not 0 <= weight <= 1:
-            raise ValueError("weight must be between 0 and 1 (inclusive)")
+        for weight in weights:
+            if not 0 <= weight <= 1:
+                raise ValueError("all `weights` must be between 0 and 1 (inclusive)")
 
-        if network.qualname != "AlchemicalNetwork":
-            raise ValueError(
-                "`network` ScopedKey does not correspond to an `AlchemicalNetwork`"
-            )
+        for network in networks:
+            if network.qualname != "AlchemicalNetwork":
+                raise ValueError(
+                    "a `networks` ScopedKey does not correspond to an `AlchemicalNetwork`"
+                )
 
-        q = f"""
-        MATCH (th:TaskHub {{network: "{network}"}})
-        SET th.weight = {weight}
-        RETURN th
-        """
-        with self.transaction() as tx:
-            tx.run(q)
+        if len(networks) != len(weights):
+            raise ValueError("length of `networks` and `weights` must be the same")
+
+        q = """
+        WITH $inputs AS inputs
+        UNWIND inputs AS x
+        WITH x[0] as network, x[1] as weight
+        MATCH (th:TaskHub {network: network})
+        SET th.weight = weight
+        RETURN network
+        """
+        inputs = [[str(network), weight] for network, weight in zip(networks, weights)]
+
+        results = self.execute_query(q, inputs=inputs)
+
+        network_results = {}
+        for record in results.records:
+            network_sk_str = record["network"]
+            network_results[network_sk_str] = ScopedKey.from_str(network_sk_str)
+
+        return [network_results.get(str(network), None) for network in networks]
 
     def get_taskhub_actioned_tasks(
         self,
-        taskhub: ScopedKey,
-    ) -> Dict[ScopedKey, float]:
-        """Get the Tasks that a given TaskHub ACTIONS.
+        taskhubs: List[ScopedKey],
+    ) -> List[Dict[ScopedKey, float]]:
+        """Get the Tasks that the given TaskHubs ACTIONS.
 
         Parameters
         ----------
-        taskhub
-            The ScopedKey of the TaskHub to query.
+        taskhubs
+            The ScopedKeys of the TaskHubs to query.
 
         Returns
         -------
         tasks
-            A dict with Task ScopedKeys that are actioned on the given TaskHub
-            as keys, Task weights as values.
+            A list of dicts, one per TaskHub, which contains the Task ScopedKeys that are
+            actioned on the given TaskHub as keys, with their weights as values.
         """
 
-        q = """
-           MATCH (th: TaskHub {_scoped_key: $th_sk})-[a:ACTIONS]->(t:Task)
-           RETURN t._scoped_key, a.weight
+        q = f"""
+           UNWIND {cypher_list_from_scoped_keys(taskhubs)} as th_sk
+           MATCH (th: TaskHub {{_scoped_key: th_sk}})-[a:ACTIONS]->(t:Task)
+           RETURN t._scoped_key, a.weight, th._scoped_key
         """
 
-        with self.transaction() as tx:
-            results = tx.run(q, th_sk=str(taskhub))
+        results = self.execute_query(q)
 
-        return {
-            ScopedKey.from_str(record.get("t._scoped_key")): record.get("a.weight")
-            for record in results
-        }
+        data = {taskhub: {} for taskhub in taskhubs}
+        for record in results.records:
+            th_sk = ScopedKey.from_str(record["th._scoped_key"])
+            t_sk = ScopedKey.from_str(record["t._scoped_key"])
+            weight = record["a.weight"]
+
+            data[th_sk][t_sk] = weight
+
+        return [data[taskhub] for taskhub in taskhubs]
 
     def get_task_actioned_networks(self, task: ScopedKey) -> Dict[ScopedKey, float]:
         """Get all AlchemicalNetwork ScopedKeys whose TaskHub ACTIONS a given Task.
 
         Parameters
         ----------
         task
@@ -1115,40 +1331,48 @@
 
         q = """
            MATCH (an:AlchemicalNetwork)<-[:PERFORMS]-(TaskHub)-[a:ACTIONS]->(Task {_scoped_key: $scoped_key})
            RETURN an._scoped_key, a.weight
         """
 
         with self.transaction() as tx:
-            results = tx.run(q, scoped_key=str(task))
+            results = tx.run(q, scoped_key=str(task)).to_eager_result()
 
         return {
             ScopedKey.from_str(record.get("an._scoped_key")): record.get("a.weight")
-            for record in results
+            for record in results.records
         }
 
-    def get_taskhub_weight(self, network: ScopedKey) -> float:
-        """Get the weight for the TaskHub associated with the given
-        AlchemicalNetwork.
+    def get_taskhub_weight(self, networks: List[ScopedKey]) -> List[float]:
+        """Get the weight for the TaskHubs associated with the given
+        AlchemicalNetworks.
 
         """
 
-        if network.qualname != "AlchemicalNetwork":
-            raise ValueError(
-                "`network` ScopedKey does not correspond to an `AlchemicalNetwork`"
-            )
+        for network in networks:
+            if network.qualname != "AlchemicalNetwork":
+                raise ValueError(
+                    "`network` ScopedKey does not correspond to an `AlchemicalNetwork`"
+                )
 
         q = f"""
-        MATCH (th:TaskHub {{network: "{network}"}})
-        RETURN th.weight
+        UNWIND {cypher_list_from_scoped_keys(networks)} as network
+        MATCH (th:TaskHub {{network: network}})
+        RETURN network, th.weight
         """
-        with self.transaction() as tx:
-            weight = tx.evaluate(q)
 
-        return weight
+        results = self.execute_query(q)
+
+        network_weights = {str(network): None for network in networks}
+        for record in results.records:
+            weight = record["th.weight"]
+            network_sk_str = record["network"]
+            network_weights[network_sk_str] = weight
+
+        return [network_weights[str(network)] for network in networks]
 
     def action_tasks(
         self,
         tasks: List[ScopedKey],
         taskhub: ScopedKey,
     ) -> List[Union[ScopedKey, None]]:
         """Add Tasks to the TaskHub for a given AlchemicalNetwork.
@@ -1159,46 +1383,49 @@
         A given compute task can be represented in any number of
         AlchemicalNetwork TaskHubs, or none at all.
 
         Only Tasks with status 'waiting', 'running', or 'error' can be
         actioned.
 
         """
-        with self.transaction() as tx:
-            actioned_sks = []
-            for t in tasks:
-                q = f"""
-                // get our TaskHub
-                MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})-[:PERFORMS]->(an:AlchemicalNetwork)
+        # since UNWIND doesn't guarantee order, we need to keep track manually
+        # so we can properly return `None` if needed
+        task_map = {str(task): None for task in tasks}
+
+        q = f"""
+        // get our TaskHub
+        UNWIND {cypher_list_from_scoped_keys(tasks)} AS task_sk
+        MATCH (th:TaskHub {{_scoped_key: "{taskhub}"}})-[:PERFORMS]->(an:AlchemicalNetwork)
+
+        // get the task we want to add to the hub; check that it connects to same network
+        MATCH (task:Task {{_scoped_key: task_sk}})-[:PERFORMS]->(tf:Transformation)<-[:DEPENDS_ON]-(an)
+
+        // only proceed for cases where task is not already actioned on hub
+        // and where the task is either in 'waiting', 'running', or 'error' status
+        WITH th, an, task
+        WHERE NOT (th)-[:ACTIONS]->(task)
+          AND task.status IN ['{TaskStatusEnum.waiting.value}', '{TaskStatusEnum.running.value}', '{TaskStatusEnum.error.value}']
+
+        // create the connection
+        CREATE (th)-[ar:ACTIONS {{weight: 0.5}}]->(task)
+
+        // set the task property to the scoped key of the Task
+        // this is a convenience for when we have to loop over relationships in Python
+        SET ar.task = task._scoped_key
 
-                // get the task we want to add to the hub; check that it connects to same network
-                MATCH (task:Task {{_scoped_key: '{t}'}})-[:PERFORMS]->(tf:Transformation)<-[:DEPENDS_ON]-(an)
+        RETURN task
+        """
+        results = self.execute_query(q)
 
-                // only proceed for cases where task is not already actioned on hub
-                // and where the task is either in 'waiting', 'running', or 'error' status
-                WITH th, an, task
-                WHERE NOT (th)-[:ACTIONS]->(task)
-                  AND task.status IN ['waiting', 'running', 'error']
-
-                // create the connection
-                CREATE (th)-[ar:ACTIONS {{weight: 0.5}}]->(task)
-
-                // set the task property to the scoped key of the Task
-                // this is a convenience for when we have to loop over relationships in Python
-                SET ar.task = task._scoped_key
+        # update our map with the results, leaving None for tasks that aren't found
+        for task_record in results.records:
+            sk = task_record["task"]["_scoped_key"]
+            task_map[str(sk)] = ScopedKey.from_str(sk)
 
-                RETURN task
-                """
-                task = tx.run(q).to_subgraph()
-                actioned_sks.append(
-                    ScopedKey.from_str(task["_scoped_key"])
-                    if task is not None
-                    else None
-                )
-        return actioned_sks
+        return [task_map[str(t)] for t in tasks]
 
     def set_task_weights(
         self,
         tasks: Union[Dict[ScopedKey, float], List[ScopedKey]],
         taskhub: ScopedKey,
         weight: Optional[float] = None,
     ) -> List[Union[ScopedKey, None]]:
@@ -1251,36 +1478,37 @@
 
                 for t, w in tasks.items():
                     q = f"""
                     MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})-[ar:ACTIONS]->(task:Task {{_scoped_key: '{t}'}})
                     SET ar.weight = {w}
                     RETURN task, ar
                     """
-                    results.append(tx.run(q))
+                    results.append(tx.run(q).to_eager_result())
 
             elif isinstance(tasks, list):
                 if weight is None:
                     raise ValueError(
                         "Must set `weight` to a scalar if `tasks` is a list"
                     )
 
                 if not 0 <= weight <= 1:
                     raise ValueError("weight must be between 0 and 1 (inclusive)")
 
+                # TODO: remove for loop with an unwind clause
                 for t in tasks:
                     q = f"""
                     MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})-[ar:ACTIONS]->(task:Task {{_scoped_key: '{t}'}})
                     SET ar.weight = {weight}
                     RETURN task, ar
                     """
-                    tx.run(q)
+                    results.append(tx.run(q).to_eager_result())
 
         # return ScopedKeys for Tasks we changed; `None` for tasks we didn't
         for res in results:
-            for record in res:
+            for record in res.records:
                 task = record["task"]
                 tasks_changed.append(
                     ScopedKey.from_str(task["_scoped_key"])
                     if task is not None
                     else None
                 )
 
@@ -1342,41 +1570,42 @@
             for t in tasks:
                 q = f"""
                 // get our task hub, as well as the task :ACTIONS relationship we want to remove
                 MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})-[ar:ACTIONS]->(task:Task {{_scoped_key: '{t}'}})
                 DELETE ar
                 RETURN task
                 """
-                task = tx.run(q).to_subgraph()
-                canceled_sks.append(
-                    ScopedKey.from_str(task["_scoped_key"])
-                    if task is not None
-                    else None
-                )
+                _task = tx.run(q).to_eager_result()
+
+                if _task.records:
+                    sk = _task.records[0].data()["task"]["_scoped_key"]
+                    canceled_sks.append(ScopedKey.from_str(sk))
+                else:
+                    canceled_sks.append(None)
 
         return canceled_sks
 
     def get_taskhub_tasks(
         self, taskhub: ScopedKey, return_gufe=False
     ) -> Union[List[ScopedKey], Dict[ScopedKey, Task]]:
         """Get a list of Tasks on the TaskHub."""
 
         q = f"""
         // get list of all tasks associated with the taskhub
         MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})-[:ACTIONS]->(task:Task)
         RETURN task
         """
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q).to_eager_result()
 
         tasks = []
         subgraph = Subgraph()
-        for record in res:
-            tasks.append(record["task"])
-            subgraph = subgraph | record["task"]
+        for record in res.records:
+            tasks.append(record_data_to_node(record["task"]))
+            subgraph = subgraph | tasks[-1]
 
         if return_gufe:
             return {
                 ScopedKey.from_str(k["_scoped_key"]): v
                 for k, v in self._subgraph_to_gufe(tasks, subgraph).items()
             }
         else:
@@ -1390,21 +1619,22 @@
         q = f"""
         // get list of all unclaimed tasks in the hub
         MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})-[:ACTIONS]->(task:Task)
         WHERE NOT (task)<-[:CLAIMS]-(:ComputeServiceRegistration)
         RETURN task
         """
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q).to_eager_result()
 
         tasks = []
         subgraph = Subgraph()
-        for record in res:
-            tasks.append(record["task"])
-            subgraph = subgraph | record["task"]
+        for record in res.records:
+            node = record_data_to_node(record["task"])
+            tasks.append(node)
+            subgraph = subgraph | node
 
         if return_gufe:
             return {
                 ScopedKey.from_str(k["_scoped_key"]): v
                 for k, v in self._subgraph_to_gufe(tasks, subgraph).items()
             }
         else:
@@ -1430,154 +1660,302 @@
         ----------
         compute_service_id
             Unique identifier for the compute service claiming the Tasks for execution.
         count
             Claim the given number of Tasks in a single transaction.
 
         """
-        taskpool_q = f"""
-        // get list of all eligible 'waiting' tasks in the hub
-        MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})-[actions:ACTIONS]-(task:Task)
-        WHERE task.status = 'waiting'
-        AND actions.weight > 0
-        OPTIONAL MATCH (task)-[:EXTENDS]->(other_task:Task)
-
-        // drop tasks from consideration if they EXTENDS an incomplete task
-        WITH task, other_task, actions
-        WHERE other_task.status = 'complete' OR other_task IS NULL
-
-        // get the highest priority present among these tasks (value nearest to 1)
-        WITH MIN(task.priority) as top_priority
-
-        // match again, this time filtering on highest priority
-        MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})-[actions:ACTIONS]-(task:Task)
-        WHERE task.status = 'waiting'
-        AND actions.weight > 0
-        AND task.priority = top_priority
-        OPTIONAL MATCH (task)-[:EXTENDS]->(other_task:Task)
-
-        // drop tasks from consideration if they EXTENDS an incomplete task
-        WITH task, other_task, actions
-        WHERE other_task.status = 'complete' OR other_task IS NULL
 
-        // return the tasks and actions relationships
-        RETURN task, actions
-        """
+        q = f"""
+            MATCH (th:TaskHub {{`_scoped_key`: '{taskhub}'}})-[actions:ACTIONS]-(task:Task)
+            WHERE task.status = '{TaskStatusEnum.waiting.value}'
+            AND actions.weight > 0
+            OPTIONAL MATCH (task)-[:EXTENDS]->(other_task:Task)
 
-        tasks = []
+            WITH task, other_task, actions
+            WHERE other_task.status = '{TaskStatusEnum.complete.value}' OR other_task IS NULL
+
+            RETURN task.`_scoped_key`, task.priority, actions.weight
+            ORDER BY task.priority ASC
+        """
+        _tasks = {}
         with self.transaction() as tx:
             tx.run(
                 f"""
             MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})
 
             // lock the TaskHub to avoid other queries from changing its state while we claim
             SET th._lock = True
             """
             )
-            for i in range(count):
-                taskpool = tx.run(taskpool_q).to_subgraph()
-                if taskpool is None:
-                    tasks.append(None)
+            _taskpool = tx.run(q)
+
+            def task_count(task_dict: dict):
+                return sum(map(len, task_dict.values()))
+
+            # directly use iterator to avoid pulling more tasks than we need
+            # since we will likely stop early
+            _task_iter = _taskpool.__iter__()
+            while task_count(_tasks) < count:
+                try:
+                    candidate = next(_task_iter)
+                    pr = candidate["task.priority"]
+
+                    # get all tasks and their actions weights at each priority level
+                    # until we've reached or surpassed `count`
+                    _tasks[pr] = []
+                    _tasks[pr].append(
+                        (candidate["task.`_scoped_key`"], candidate["actions.weight"])
+                    )
+                    while True:
+
+                        # if we've run out of tasks, stop immediately
+                        if not (next_task := _taskpool.peek()):
+                            raise StopIteration
+
+                        # if next task has a different (lower) priority, stop consuming
+                        if next_task["task.priority"] != pr:
+                            break
+
+                        candidate = next(_task_iter)
+                        _tasks[candidate["task.priority"]].append(
+                            (
+                                candidate["task.`_scoped_key`"],
+                                candidate["actions.weight"],
+                            )
+                        )
+
+                except StopIteration:
+                    break
+
+            remaining = count
+            tasks = []
+            # for each group of tasks at each priority level
+            for _, taskgroup in sorted(_tasks.items()):
+                # if we want more tasks (or exactly as many tasks) as there are
+                # in the group, just add them all
+                if len(taskgroup) <= remaining:
+                    tasks.extend(map(lambda x: ScopedKey.from_str(x[0]), taskgroup))
+
+                    # immediately stop if we've reached our target count
+                    if not (remaining := count - len(tasks)):
+                        break
+
+                # otherwise, perform a weighted random selection from the tasks
+                # to fill out remaining
                 else:
-                    chosen_one = _select_task_from_taskpool(taskpool)
-                    claim_query = _generate_claim_query(chosen_one, compute_service_id)
-                    tasks.append(tx.run(claim_query).to_subgraph())
+                    tasks.extend(
+                        map(
+                            ScopedKey.from_str,
+                            _select_tasks_from_taskpool(taskgroup, remaining),
+                        )
+                    )
+
+            # if tasks is not empty, proceed with claiming
+            if tasks:
+                q = _generate_claim_query(tasks, compute_service_id)
+                tx.run(q)
 
             tx.run(
                 f"""
             MATCH (th:TaskHub {{_scoped_key: '{taskhub}'}})
 
             // remove lock on the TaskHub now that we're done with it
             SET th._lock = null
             """
             )
 
-        return [
-            ScopedKey.from_str(t["_scoped_key"]) if t is not None else None
-            for t in tasks
-        ]
+        return tasks + [None] * (count - len(tasks))
 
     ## tasks
 
-    def create_task(
+    def _validate_extends_tasks(self, task_list) -> Dict[str, Tuple[Node, str]]:
+
+        if not task_list:
+            return {}
+
+        q = f"""
+            UNWIND {cypher_list_from_scoped_keys(task_list)} as task
+            MATCH (t:Task {{`_scoped_key`: task}})-[PERFORMS]->(tf:Transformation)
+            return t, tf._scoped_key as tf_sk
+        """
+
+        results = self.execute_query(q)
+
+        nodes = {}
+
+        for record in results.records:
+            node = record_data_to_node(record["t"])
+            transformation_sk = record["tf_sk"]
+
+            status = node.get("status")
+
+            if status in ("invalid", "deleted"):
+                invalid_task_scoped_key = node["_scoped_key"]
+                raise ValueError(
+                    f"Cannot extend a `deleted` or `invalid` Task: {invalid_task_scoped_key}"
+                )
+
+            nodes[node["_scoped_key"]] = (node, transformation_sk)
+
+        return nodes
+
+    def create_tasks(
         self,
-        transformation: ScopedKey,
-        extends: Optional[ScopedKey] = None,
+        transformations: List[ScopedKey],
+        extends: Optional[List[Optional[ScopedKey]]] = None,
         creator: Optional[str] = None,
-    ) -> ScopedKey:
-        """Add a compute Task to a Transformation.
+    ) -> List[ScopedKey]:
+        """Create Tasks for the given Transformations.
 
-        Note: this creates a compute Task, but does not add it to any TaskHubs.
+        Note: this creates Tasks; it does not action them.
 
         Parameters
         ----------
-        transformation
-            The Transformation to compute.
-        scope
-            The scope the Transformation is in; ignored if `transformation` is a ScopedKey.
+        transformations
+            The Transformations to create Tasks for.
+            One Task is created for each Transformation ScopedKey given; to
+            create multiple Tasks for a given Transformation, provide its
+            ScopedKey multiple times.
         extends
-            The ScopedKey of the Task to use as a starting point for this Task.
+            The ScopedKeys of the Tasks to use as a starting point for the
+            created Tasks, in the same order as `transformations`. If ``None``
+            given for a given Task, it will not extend any other Task.
             Will use the `ProtocolDAGResult` from the given Task as the
             `extends` input for the Task's eventual call to `Protocol.create`.
-
+        creator (optional)
+            The creator of the Tasks.
         """
-        if transformation.qualname not in ["Transformation", "NonTransformation"]:
+        allowed_types = [Transformation.__qualname__, NonTransformation.__qualname__]
+
+        # reshape data to a standard form
+        if extends is None:
+            extends = [None] * len(transformations)
+        elif len(extends) != len(transformations):
             raise ValueError(
-                "`transformation` ScopedKey does not correspond to a `Transformation`"
+                "`extends` must either be `None` or have the same length as `transformations`"
             )
 
-        if extends is not None and extends.qualname != "Task":
-            raise ValueError("`extends` ScopedKey does not correspond to a `Task`")
-
-        scope = transformation.scope
-        transformation_node = self._get_node(transformation)
+        for i, _extends in enumerate(extends):
+            if _extends is not None:
+                if not (extended_task_qualname := getattr(_extends, "qualname", None)):
+                    raise ValueError(
+                        f"`extends` entry for `Task` {transformations[i]} is not valid"
+                    )
+                if extended_task_qualname != "Task":
+                    raise ValueError(
+                        f"`extends` ScopedKey ({_extends}) does not correspond to a `Task`"
+                    )
 
-        # create a new task for the supplied transformation
-        # use a PERFORMS relationship
-        task = Task(
-            creator=creator, extends=str(extends) if extends is not None else None
-        )
+        transformation_map = {
+            transformation_type: [[], []] for transformation_type in allowed_types
+        }
+        for i, transformation in enumerate(transformations):
+            if transformation.qualname not in allowed_types:
+                raise ValueError(
+                    f"Got an unsupported `Transformation` type: {transformation.qualname}"
+                )
+            transformation_map[transformation.qualname][0].append(transformation)
+            transformation_map[transformation.qualname][1].append(extends[i])
 
-        _, task_node, scoped_key = self._gufe_to_subgraph(
-            task.to_shallow_dict(),
-            labels=["GufeTokenizable", task.__class__.__name__],
-            gufe_key=task.key,
-            scope=scope,
+        extends_nodes = self._validate_extends_tasks(
+            [_extends for _extends in extends if _extends is not None]
         )
 
         subgraph = Subgraph()
 
-        if extends is not None:
-            previous_task_node = self._get_node(extends)
-            stat = previous_task_node.get("status")
-            # do not allow creation of a task that extends an invalid or deleted task.
-            if (stat == "invalid") or (stat == "deleted"):
-                raise ValueError(
-                    f"Cannot extend a `deleted` or `invalid` Task: {previous_task_node}"
+        sks = []
+        # iterate over all allowed types, unpacking the transformations and extends subsets
+        for node_type, (
+            transformation_subset,
+            extends_subset,
+        ) in transformation_map.items():
+
+            if not transformation_subset:
+                continue
+
+            q = f"""
+            UNWIND {cypher_list_from_scoped_keys(transformation_subset)} as sk
+            MATCH (n:{node_type} {{`_scoped_key`: sk}})
+            RETURN n
+            """
+
+            results = self.execute_query(q)
+
+            transformation_nodes = {}
+            for record in results.records:
+                node = record_data_to_node(record["n"])
+                transformation_nodes[node["_scoped_key"]] = node
+
+            for _transformation, _extends in zip(transformation_subset, extends_subset):
+
+                scope = transformation.scope
+
+                _task = Task(
+                    creator=creator,
+                    extends=str(_extends) if _extends is not None else None,
+                )
+                _, task_node, scoped_key = self._gufe_to_subgraph(
+                    _task.to_shallow_dict(),
+                    labels=["GufeTokenizable", _task.__class__.__name__],
+                    gufe_key=_task.key,
+                    scope=scope,
                 )
-            subgraph = subgraph | Relationship.type("EXTENDS")(
-                task_node,
-                previous_task_node,
-                _org=scope.org,
-                _campaign=scope.campaign,
-                _project=scope.project,
-            )
 
-        subgraph = subgraph | Relationship.type("PERFORMS")(
-            task_node,
-            transformation_node,
-            _org=scope.org,
-            _campaign=scope.campaign,
-            _project=scope.project,
-        )
+                sks.append(scoped_key)
+
+                if _extends is not None:
+
+                    extends_task_node, extends_transformation_sk = extends_nodes[
+                        str(_extends)
+                    ]
+
+                    if extends_transformation_sk != str(_transformation):
+                        raise ValueError(
+                            f"{_extends} extends a Transformation other than {_transformation}"
+                        )
+
+                    subgraph |= Relationship.type("EXTENDS")(
+                        task_node,
+                        extends_task_node,
+                        _org=scope.org,
+                        _campaign=scope.campaign,
+                        _project=scope.project,
+                    )
+
+                subgraph |= Relationship.type("PERFORMS")(
+                    task_node,
+                    transformation_nodes[str(_transformation)],
+                    _org=scope.org,
+                    _campaign=scope.campaign,
+                    _project=scope.project,
+                )
 
         with self.transaction() as tx:
-            tx.create(subgraph)
+            merge_subgraph(tx, subgraph, "GufeTokenizable", "_scoped_key")
 
-        return scoped_key
+        return sks
+
+    def create_task(
+        self,
+        transformation: ScopedKey,
+        extends: Optional[ScopedKey] = None,
+        creator: Optional[str] = None,
+    ) -> ScopedKey:
+        """Create a single Task for a Transformation.
+
+        This is a convenience method that wraps around the more general
+        `create_tasks` method.
+
+        """
+        return self.create_tasks(
+            [transformation],
+            extends=[extends] if extends is not None else [None],
+            creator=creator,
+        )[0]
 
     def query_tasks(self, *, status=None, key=None, scope: Scope = Scope()):
         """Query for `Task`\s matching given attributes."""
         additional = {"status": status}
         return self._query(qualname="Task", additional=additional, key=key, scope=scope)
 
     def get_network_tasks(
@@ -1657,32 +2035,34 @@
         if extends:
             q += f"""
             MATCH (trans)<-[:PERFORMS]-(extends:Task {{_scoped_key: '{extends}'}})
             WHERE (task)-[:EXTENDS*]->(extends)
             RETURN task
             """
         else:
-            q += f"""
+            q += """
             RETURN task
             """
 
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q).to_eager_result()
 
         tasks = []
-        for record in res:
+        for record in res.records:
             tasks.append(record["task"])
 
         if return_as == "list":
             return [ScopedKey.from_str(t["_scoped_key"]) for t in tasks]
         elif return_as == "graph":
             return {
-                ScopedKey.from_str(t["_scoped_key"]): ScopedKey.from_str(t["extends"])
-                if t["extends"] is not None
-                else None
+                ScopedKey.from_str(t["_scoped_key"]): (
+                    ScopedKey.from_str(t["extends"])
+                    if t["extends"] is not None
+                    else None
+                )
                 for t in tasks
             }
 
     def get_task_transformation(
         self,
         task: ScopedKey,
         return_gufe=True,
@@ -1701,19 +2081,19 @@
         q = f"""
         MATCH (task:Task {{_scoped_key: "{task}"}})-[:PERFORMS]->(trans:Transformation)
         OPTIONAL MATCH (task)-[:EXTENDS]->(prev:Task)-[:RESULTS_IN]->(result:ProtocolDAGResultRef)
         RETURN trans, result
         """
 
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q).to_eager_result()
 
         transformations = []
         results = []
-        for record in res:
+        for record in res.records:
             transformations.append(record["trans"])
             results.append(record["result"])
 
         if len(transformations) == 0 or len(results) == 0:
             raise KeyError("No such object in database")
         elif len(transformations) > 1 or len(results) > 1:
             raise Neo4JStoreError(
@@ -1727,17 +2107,19 @@
             if results[0] is not None
             else None
         )
 
         if return_gufe:
             return (
                 self.get_gufe(transformation),
-                self.get_gufe(protocoldagresultref)
-                if protocoldagresultref is not None
-                else None,
+                (
+                    self.get_gufe(protocoldagresultref)
+                    if protocoldagresultref is not None
+                    else None
+                ),
             )
 
         return transformation, protocoldagresultref
 
     def set_tasks(
         self,
         transformation: ScopedKey,
@@ -1797,18 +2179,20 @@
             UNWIND batch AS scoped_key
 
             OPTIONAL MATCH (t:Task {_scoped_key: scoped_key})
             SET t.priority = $priority
 
             RETURN scoped_key, t
             """
-            res = tx.run(q, scoped_keys=[str(t) for t in tasks], priority=priority)
+            res = tx.run(
+                q, scoped_keys=[str(t) for t in tasks], priority=priority
+            ).to_eager_result()
 
         task_results = []
-        for record in res:
+        for record in res.records:
             task_i = record["t"]
             scoped_key = record["scoped_key"]
 
             # catch missing tasks
             if task_i is None:
                 task_results.append(None)
             else:
@@ -1852,51 +2236,76 @@
 
         This method is intended for administrator use; generally Tasks should
         instead have their tasks set to 'deleted' and retained.
 
         """
         raise NotImplementedError
 
-    def get_scope_status(self, scope: Scope) -> Dict[str, int]:
-        """Return status counts for all Tasks within the given Scope."""
+    def get_scope_status(
+        self,
+        scope: Scope,
+        network_state: Optional[Union[NetworkStateEnum, str]] = NetworkStateEnum.active,
+    ) -> Dict[str, int]:
+        """Return status counts for all Tasks within the given Scope.
+
+        Parameters
+        ----------
+        scope
+            Scope to get status for; may be non-specific.
+        network_state
+            Network state to restrict status returns for; may be a regex pattern.
+
+        """
 
         properties = {
             "_org": scope.org,
             "_campaign": scope.campaign,
             "_project": scope.project,
         }
 
         prop_string = ", ".join(
             "{}: '{}'".format(key, value)
             for key, value in properties.items()
             if value is not None
         )
 
+        if isinstance(network_state, NetworkStateEnum):
+            network_state = network_state.value
+
+        if network_state is None:
+            network_state = ".*"
+
         q = f"""
-        MATCH (n:Task {{{prop_string}}})
-        RETURN n.status AS status, count(n) as counts
+        MATCH (n:Task {{{prop_string}}})-[:PERFORMS]->(:Transformation)<-[:DEPENDS_ON]-(:AlchemicalNetwork)<-[:MARKS]-(nm:NetworkMark)
+        WHERE nm.state =~ $state_pattern
+        RETURN n.status AS status, count(DISTINCT n) as counts
         """
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q, state_pattern=network_state)
             counts = {rec["status"]: rec["counts"] for rec in res}
 
         return counts
 
-    def get_network_status(self, network: ScopedKey) -> Dict[str, int]:
-        """Return status counts for all Tasks associated with the given AlchemicalNetwork."""
+    def get_network_status(self, networks: List[ScopedKey]) -> List[Dict[str, int]]:
+        """Return status counts for all Tasks associated with the given AlchemicalNetworks."""
         q = f"""
-        MATCH (:AlchemicalNetwork {{_scoped_key: "{network}"}})-[:DEPENDS_ON]->(tf:Transformation),
+        UNWIND {cypher_list_from_scoped_keys(networks)} as network
+        MATCH (an:AlchemicalNetwork {{_scoped_key: network}})-[:DEPENDS_ON]->(tf:Transformation),
               (tf)<-[:PERFORMS]-(t:Task)
-        RETURN t.status AS status, count(t) as counts
+        RETURN an._scoped_key AS sk, t.status AS status, count(t) as counts
         """
-        with self.transaction() as tx:
-            res = tx.run(q)
-            counts = {rec["status"]: rec["counts"] for rec in res}
 
-        return counts
+        network_data = {str(network_sk): {} for network_sk in networks}
+        for rec in self.execute_query(q).records:
+            sk = rec["sk"]
+            status = rec["status"]
+            counts = rec["counts"]
+            network_data[sk][status] = counts
+
+        return [network_data[str(an)] for an in networks]
 
     def get_transformation_status(self, transformation: ScopedKey) -> Dict[str, int]:
         """Return status counts for all Tasks associated with the given Transformation."""
         q = f"""
         MATCH (:Transformation {{_scoped_key: "{transformation}"}})<-[:PERFORMS]-(t:Task)
         RETURN t.status AS status, count(t) as counts
         """
@@ -1929,15 +2338,15 @@
             protocoldagresultref_node,
             _org=scope.org,
             _campaign=scope.campaign,
             _project=scope.project,
         )
 
         with self.transaction() as tx:
-            tx.merge(subgraph, "GufeTokenizable", "_scoped_key")
+            merge_subgraph(tx, subgraph, "GufeTokenizable", "_scoped_key")
 
         return scoped_key
 
     def get_task_results(self, task: ScopedKey) -> List[ProtocolDAGResultRef]:
         # get all task result protocoldagresultrefs corresponding to given task
         # returned in no particular order
         q = """
@@ -2288,31 +2697,31 @@
         If an entity of this type with the same `identifier` already exists,
         then this will overwrite its properties, including credential.
 
         """
         node = Node("CredentialedEntity", entity.__class__.__name__, **entity.dict())
 
         with self.transaction() as tx:
-            tx.merge(
-                node, primary_label=entity.__class__.__name__, primary_key="identifier"
+            merge_subgraph(
+                tx, Subgraph() | node, entity.__class__.__name__, "identifier"
             )
 
     def get_credentialed_entity(self, identifier: str, cls: type[CredentialedEntity]):
         """Get an existing credentialed entity, such as a user or compute identity."""
         q = f"""
         MATCH (n:{cls.__name__} {{identifier: '{identifier}'}})
         RETURN n
         """
 
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q).to_eager_result()
 
         nodes = set()
-        for record in res:
-            nodes.add(record["n"])
+        for record in res.records:
+            nodes.add(record_data_to_node(record["n"]))
 
         if len(nodes) == 0:
             raise KeyError("No such object in database")
         elif len(nodes) > 1:
             raise Neo4JStoreError(
                 "More than one such object in database; this should not be possible"
             )
@@ -2321,21 +2730,20 @@
 
     def list_credentialed_entities(self, cls: type[CredentialedEntity]):
         """Get an existing credentialed entity, such as a user or compute identity."""
         q = f"""
         MATCH (n:{cls.__name__})
         RETURN n
         """
-
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q).to_eager_result()
 
         nodes = set()
-        for record in res:
-            nodes.add(record["n"])
+        for record in res.records:
+            nodes.add(record_data_to_node(record["n"]))
 
         return [node["identifier"] for node in nodes]
 
     def remove_credentialed_identity(
         self, identifier: str, cls: type[CredentialedEntity]
     ):
         """Remove a credentialed entity, such as a user or compute identity."""
@@ -2370,18 +2778,18 @@
         # get the scope properties for the given entity
         q = f"""
         MATCH (n:{cls.__name__} {{identifier: '{identifier}'}})
         RETURN n.scopes as s
         """
 
         with self.transaction() as tx:
-            res = tx.run(q)
+            res = tx.run(q).to_eager_result()
 
         scopes = []
-        for record in res:
+        for record in res.records:
             scope_rec = record["s"]
             for scope_str in scope_rec:
                 scope = Scope.from_str(scope_str)
                 scopes.append(scope)
         return scopes
 
     def remove_scope(
```

### Comparing `alchemiscale-0.3.0/alchemiscale/utils.py` & `alchemiscale-0.4.0/alchemiscale/utils.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.3.0/alchemiscale/validators.py` & `alchemiscale-0.4.0/alchemiscale/validators.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.3.0/alchemiscale.egg-info/SOURCES.txt` & `alchemiscale-0.4.0/alchemiscale.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 alchemiscale/interface/__init__.py
 alchemiscale/interface/api.py
 alchemiscale/interface/client.py
 alchemiscale/security/__init__.py
 alchemiscale/security/auth.py
 alchemiscale/security/models.py
 alchemiscale/storage/__init__.py
+alchemiscale/storage/cypher.py
 alchemiscale/storage/models.py
 alchemiscale/storage/objectstore.py
 alchemiscale/storage/statestore.py
+alchemiscale/storage/subgraph.py
 alchemiscale/strategies/__init__.py
 alchemiscale/strategies/base.py
 alchemiscale/strategist/__init__.py
 alchemiscale/strategist/service.py
```

### Comparing `alchemiscale-0.3.0/pyproject.toml` & `alchemiscale-0.4.0/pyproject.toml`

 * *Files identical despite different names*

