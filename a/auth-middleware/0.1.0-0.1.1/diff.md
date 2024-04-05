# Comparing `tmp/auth_middleware-0.1.0.tar.gz` & `tmp/auth_middleware-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_middleware-0.1.0.tar", max compression
+gzip compressed data, was "auth_middleware-0.1.1.tar", max compression
```

## Comparing `auth_middleware-0.1.0.tar` & `auth_middleware-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1070 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/LICENSE
--rw-r--r--   0        0        0     1483 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/README.md
--rw-r--r--   0        0        0      799 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      536 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/__init__.py
--rw-r--r--   0        0        0       89 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/exceptions.py
--rw-r--r--   0        0        0      823 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/functions.py
--rw-r--r--   0        0        0     1058 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/group_checker.py
--rw-r--r--   0        0        0     3949 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/jwt_auth_middleware.py
--rw-r--r--   0        0        0     1963 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/jwt_auth_provider.py
--rw-r--r--   0        0        0     2904 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/jwt_bearer_manager.py
--rw-r--r--   0        0        0      682 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/logging.py
--rw-r--r--   0        0        0        0 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/providers/cognito/__init__.py
--rw-r--r--   0        0        0     3008 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/providers/cognito/cognito_provider.py
--rw-r--r--   0        0        0      180 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/providers/cognito/exceptions.py
--rw-r--r--   0        0        0     1017 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/providers/cognito/settings.py
--rw-r--r--   0        0        0        0 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/providers/entra_id/__init__.py
--rw-r--r--   0        0        0     4112 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/providers/entra_id/entra_id_provider.py
--rw-r--r--   0        0        0      184 2024-04-03 19:21:55.936961 auth_middleware-0.1.0/src/auth_middleware/providers/entra_id/exceptions.py
--rw-r--r--   0        0        0      780 2024-04-03 19:21:55.940961 auth_middleware-0.1.0/src/auth_middleware/providers/entra_id/settings.py
--rw-r--r--   0        0        0      844 2024-04-03 19:21:55.940961 auth_middleware-0.1.0/src/auth_middleware/settings.py
--rw-r--r--   0        0        0     1375 2024-04-03 19:21:55.940961 auth_middleware-0.1.0/src/auth_middleware/types.py
--rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 auth_middleware-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1904 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/README.md
+-rw-r--r--   0        0        0      799 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/src/auth_middleware/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/src/auth_middleware/exceptions.py
+-rw-r--r--   0        0        0      834 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/functions.py
+-rw-r--r--   0        0        0     1069 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/group_checker.py
+-rw-r--r--   0        0        0     3949 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/jwt_auth_middleware.py
+-rw-r--r--   0        0        0     1963 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/jwt_auth_provider.py
+-rw-r--r--   0        0        0     2915 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/jwt_bearer_manager.py
+-rw-r--r--   0        0        0      762 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/logging.py
+-rw-r--r--   0        0        0        0 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/__init__.py
+-rw-r--r--   0        0        0      141 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/cognito/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/cognito/cognito_provider.py
+-rw-r--r--   0        0        0      180 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/cognito/exceptions.py
+-rw-r--r--   0        0        0     1157 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/cognito/settings.py
+-rw-r--r--   0        0        0      146 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/__init__.py
+-rw-r--r--   0        0        0     4176 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/entra_id_provider.py
+-rw-r--r--   0        0        0      184 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/exceptions.py
+-rw-r--r--   0        0        0      864 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/settings.py
+-rw-r--r--   0        0        0     1007 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/settings.py
+-rw-r--r--   0        0        0     1375 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/types.py
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 auth_middleware-0.1.1/PKG-INFO
```

### Comparing `auth_middleware-0.1.0/LICENSE` & `auth_middleware-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.0/pyproject.toml` & `auth_middleware-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auth-middleware"
-version = "0.1.0"
+version = "0.1.1"
 description = "Async Auth Middleware for FastAPI/Starlette"
 authors = ["impalah <impalah@gmail.com>"]
 readme = "README.md"
 packages = [{include = "auth_middleware", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `auth_middleware-0.1.0/src/auth_middleware/__init__.py` & `auth_middleware-0.1.1/src/auth_middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.0/src/auth_middleware/functions.py` & `auth_middleware-0.1.1/src/auth_middleware/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 
 
 def require_user():
     """Check if the user is authenticated"""
 
     def _user_checker(request: Request):
 
-        if settings.AUTH_DISABLED:
+        if settings.AUTH_MIDDLEWARE_DISABLED:
             return
 
         if not hasattr(request.state, "current_user") or not request.state.current_user:
             raise HTTPException(status_code=401, detail="Authentication required")
 
     return _user_checker
```

### Comparing `auth_middleware-0.1.0/src/auth_middleware/group_checker.py` & `auth_middleware-0.1.1/src/auth_middleware/group_checker.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     __allowed_groups: list = []
 
     def __init__(self, allowed_groups: List):
         self.__allowed_groups = allowed_groups
 
     def __call__(self, request: Request):
 
-        if settings.AUTH_DISABLED:
+        if settings.AUTH_MIDDLEWARE_DISABLED:
             return
 
         if not hasattr(request.state, "current_user") or not request.state.current_user:
             raise HTTPException(status_code=401, detail="Authentication required")
 
         user: User = request.state.current_user
```

### Comparing `auth_middleware-0.1.0/src/auth_middleware/jwt_auth_middleware.py` & `auth_middleware-0.1.1/src/auth_middleware/jwt_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.0/src/auth_middleware/jwt_auth_provider.py` & `auth_middleware-0.1.1/src/auth_middleware/jwt_auth_provider.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.0/src/auth_middleware/jwt_bearer_manager.py` & `auth_middleware-0.1.1/src/auth_middleware/jwt_bearer_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ):
         super().__init__(auto_error=auto_error)
         self.auth_provider = auth_provider
 
     async def get_credentials(
         self, request: Request
     ) -> Optional[JWTAuthorizationCredentials]:
-        if settings.AUTH_DISABLED:
+        if settings.AUTH_MIDDLEWARE_DISABLED:
             return None
 
         try:
             credentials: Optional[HTTPAuthorizationCredentials] = (
                 await super().__call__(request)
             )
         except HTTPException as e:
```

### Comparing `auth_middleware-0.1.0/src/auth_middleware/providers/cognito/cognito_provider.py` & `auth_middleware-0.1.1/src/auth_middleware/providers/cognito/cognito_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 
         Returns:
             JWKS: _description_
         """
 
         # TODO: Control errors
         keys: List[JWK] = requests.get(
-            settings.AWS_COGNITO_JWKS_URL_TEMPLATE.format(
-                settings.AWS_COGNITO_USER_POOL_REGION,
-                settings.AWS_COGNITO_USER_POOL_ID,
+            settings.AUTH_PROVIDER_AWS_COGNITO_JWKS_URL_TEMPLATE.format(
+                settings.AUTH_PROVIDER_AWS_COGNITO_USER_POOL_REGION,
+                settings.AUTH_PROVIDER_AWS_COGNITO_USER_POOL_ID,
             )
         ).json()["keys"]
         timestamp: int = (
-            time_ns() + settings.AUTH_JWKS_CACHE_INTERVAL_MINUTES * 60 * 1000000000
+            time_ns() + settings.AUTH_MIDDLEWARE_JWKS_CACHE_INTERVAL_MINUTES * 60 * 1000000000
         )
-        usage_counter: int = settings.AUTH_JWKS_CACHE_USAGES
+        usage_counter: int = settings.AUTH_MIDDLEWARE_JWKS_CACHE_USAGES
         jks: JWKS = JWKS(keys=keys, timestamp=timestamp, usage_counter=usage_counter)
 
         return jks
 
     def verify_token(self, token: JWTAuthorizationCredentials) -> bool:
 
         hmac_key_candidate = self._get_hmac_key(token)
```

### Comparing `auth_middleware-0.1.0/src/auth_middleware/providers/cognito/settings.py` & `auth_middleware-0.1.1/src/auth_middleware/providers/cognito/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 
 config = Config()
 
 
 class ModuleSettings(Settings):
     """Settings for the module"""
 
-    AWS_COGNITO_USER_POOL_ID: Optional[str] = config(
-        "AWS_COGNITO_USER_POOL_ID",
+    AUTH_PROVIDER_AWS_COGNITO_USER_POOL_ID: Optional[str] = config(
+        "AUTH_PROVIDER_AWS_COGNITO_USER_POOL_ID",
         cast=str,
         default=None,
     )
 
-    AWS_COGNITO_USER_POOL_REGION: Optional[str] = config(
-        "AWS_COGNITO_USER_POOL_REGION",
+    AUTH_PROVIDER_AWS_COGNITO_USER_POOL_REGION: Optional[str] = config(
+        "AUTH_PROVIDER_AWS_COGNITO_USER_POOL_REGION",
         cast=str,
         default=None,
     )
 
-    AWS_COGNITO_JWKS_URL_TEMPLATE: str = config(
-        "AWS_COGNITO_JWKS_URL_TEMPLATE",
+    AUTH_PROVIDER_AWS_COGNITO_JWKS_URL_TEMPLATE: str = config(
+        "AUTH_PROVIDER_AWS_COGNITO_JWKS_URL_TEMPLATE",
         cast=str,
         default="https://cognito-idp.{}.amazonaws.com/{}/.well-known/jwks.json",
     )
 
-    AWS_COGNITO_USER_POOL_CLIENT_ID: Optional[str] = config(
-        "AWS_COGNITO_USER_POOL_CLIENT_ID",
+    AUTH_PROVIDER_AWS_COGNITO_USER_POOL_CLIENT_ID: Optional[str] = config(
+        "AUTH_PROVIDER_AWS_COGNITO_USER_POOL_CLIENT_ID",
         cast=str,
         default=None,
     )
 
-    AWS_COGNITO_USER_POOL_CLIENT_SECRET: Optional[str] = config(
-        "AWS_COGNITO_USER_POOL_CLIENT_SECRET",
+    AUTH_PROVIDER_AWS_COGNITO_USER_POOL_CLIENT_SECRET: Optional[str] = config(
+        "AUTH_PROVIDER_AWS_COGNITO_USER_POOL_CLIENT_SECRET",
         cast=str,
         default=None,
     )
 
 
 settings = ModuleSettings()
```

### Comparing `auth_middleware-0.1.0/src/auth_middleware/providers/entra_id/entra_id_provider.py` & `auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/entra_id_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 
         Returns:
             JWKS: _description_
         """
 
         # TODO: Control errors
         openid_config = requests.get(
-            settings.AZURE_ENTRA_ID_JWKS_URL_TEMPLATE.format(
-                settings.AZURE_ENTRA_ID_TENANT_ID,
+            settings.AUTH_PROVIDER_AZURE_ENTRA_ID_JWKS_URL_TEMPLATE.format(
+                settings.AUTH_PROVIDER_AZURE_ENTRA_ID_TENANT_ID,
             )
         ).json()
         jwks_uri = openid_config["jwks_uri"]
         keys = requests.get(jwks_uri).json()["keys"]
 
         # Convert 'x5c' field in each key from list to string
         for key in keys:
             if "x5c" in key and isinstance(key["x5c"], list):
                 key["x5c"] = "".join(key["x5c"])
 
         timestamp: int = (
-            time_ns() + settings.AUTH_JWKS_CACHE_INTERVAL_MINUTES * 60 * 1000000000
+            time_ns() + settings.AUTH_MIDDLEWARE_JWKS_CACHE_INTERVAL_MINUTES * 60 * 1000000000
         )
-        usage_counter: int = settings.AUTH_JWKS_CACHE_USAGES
+        usage_counter: int = settings.AUTH_MIDDLEWARE_JWKS_CACHE_USAGES
         jks: JWKS = JWKS(keys=keys, timestamp=timestamp, usage_counter=usage_counter)
         return jks
 
     def verify_token(self, token: JWTAuthorizationCredentials) -> bool:
         """Verifiy token signature
 
         Args:
@@ -80,15 +80,15 @@
             }
 
             # Decode jwt token
             payload = jwt.decode(
                 token.jwt_token,
                 rsa_key,
                 algorithms=["RS256"],
-                audience=settings.AZURE_ENTRA_ID_AUDIENCE_ID,
+                audience=settings.AUTH_PROVIDER_AZURE_ENTRA_ID_AUDIENCE_ID,
                 options={"verify_at_hash": False},  # Disable at_hash verification
             )
             return False if payload.get("sub") is None else True
         except JWTError as je:
             logger.error("Error in EntraIDClient: %s", str(je))
             return False
         except Exception as e:
```

### Comparing `auth_middleware-0.1.0/src/auth_middleware/providers/entra_id/settings.py` & `auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 config = Config()
 
 
 class ModuleSettings(Settings):
     """Settings for the module"""
 
-    AZURE_ENTRA_ID_TENANT_ID: Optional[str] = config(
-        "AZURE_ENTRA_ID_TENANT_ID",
+    AUTH_PROVIDER_AZURE_ENTRA_ID_TENANT_ID: Optional[str] = config(
+        "AUTH_PROVIDER_AZURE_ENTRA_ID_TENANT_ID",
         cast=str,
         default=None,
     )
 
     # The audience id is the client id of the application
-    AZURE_ENTRA_ID_AUDIENCE_ID: Optional[str] = config(
-        "AZURE_ENTRA_ID_AUDIENCE_ID",
+    AUTH_PROVIDER_AZURE_ENTRA_ID_AUDIENCE_ID: Optional[str] = config(
+        "AUTH_PROVIDER_AZURE_ENTRA_ID_AUDIENCE_ID",
         cast=str,
         default=None,
     )
 
-    AZURE_ENTRA_ID_JWKS_URL_TEMPLATE: str = config(
-        "AZURE_ENTRA_ID_JWKS_URL_TEMPLATE",
+    AUTH_PROVIDER_AZURE_ENTRA_ID_JWKS_URL_TEMPLATE: str = config(
+        "AUTH_PROVIDER_AZURE_ENTRA_ID_JWKS_URL_TEMPLATE",
         cast=str,
         default="https://login.microsoftonline.com/{}/v2.0/.well-known/openid-configuration",
     )
 
 
 settings = ModuleSettings()
```

### Comparing `auth_middleware-0.1.0/src/auth_middleware/types.py` & `auth_middleware-0.1.1/src/auth_middleware/types.py`

 * *Files identical despite different names*

