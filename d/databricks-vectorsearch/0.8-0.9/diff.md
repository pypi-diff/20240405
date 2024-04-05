# Comparing `tmp/databricks_vectorsearch-0.8-py3-none-any.whl.zip` & `tmp/databricks_vectorsearch-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7765 bytes, number of entries: 11
+Zip file size: 7870 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Oct-12 17:55 databricks/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Oct-12 17:55 databricks/vector_search/__init__.py
--rw-r--r--  2.0 unx    10588 b- defN 23-Oct-12 18:33 databricks/vector_search/client.py
+-rw-r--r--  2.0 unx    11208 b- defN 23-Oct-12 21:37 databricks/vector_search/client.py
 -rw-r--r--  2.0 unx       50 b- defN 23-Oct-12 17:55 databricks/vector_search/exceptions.py
 -rw-r--r--  2.0 unx     6036 b- defN 23-Oct-12 18:50 databricks/vector_search/index.py
 -rw-r--r--  2.0 unx     2364 b- defN 23-Oct-12 18:33 databricks/vector_search/utils.py
--rw-r--r--  2.0 unx     2414 b- defN 23-Oct-12 18:51 databricks_vectorsearch-0.8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      400 b- defN 23-Oct-12 18:51 databricks_vectorsearch-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-12 18:51 databricks_vectorsearch-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Oct-12 18:51 databricks_vectorsearch-0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      989 b- defN 23-Oct-12 18:51 databricks_vectorsearch-0.8.dist-info/RECORD
-11 files, 22944 bytes uncompressed, 6051 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx     2414 b- defN 23-Oct-12 21:38 databricks_vectorsearch-0.9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      400 b- defN 23-Oct-12 21:38 databricks_vectorsearch-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Oct-12 21:38 databricks_vectorsearch-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Oct-12 21:38 databricks_vectorsearch-0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      989 b- defN 23-Oct-12 21:38 databricks_vectorsearch-0.9.dist-info/RECORD
+11 files, 23564 bytes uncompressed, 6156 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: databricks/vector_search/index.py
 Comment: 
 
 Filename: databricks/vector_search/utils.py
 Comment: 
 
-Filename: databricks_vectorsearch-0.8.dist-info/LICENSE.md
+Filename: databricks_vectorsearch-0.9.dist-info/LICENSE.md
 Comment: 
 
-Filename: databricks_vectorsearch-0.8.dist-info/METADATA
+Filename: databricks_vectorsearch-0.9.dist-info/METADATA
 Comment: 
 
-Filename: databricks_vectorsearch-0.8.dist-info/WHEEL
+Filename: databricks_vectorsearch-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: databricks_vectorsearch-0.8.dist-info/top_level.txt
+Filename: databricks_vectorsearch-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: databricks_vectorsearch-0.8.dist-info/RECORD
+Filename: databricks_vectorsearch-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databricks/vector_search/client.py

```diff
@@ -14,55 +14,63 @@
 class VectorSearchClient:
 
     def __init__(
         self,
         workspace_url=None,
         personal_access_token=None,
         service_principal_client_id=None,
-        service_principal_client_secret=None
+        service_principal_client_secret=None,
+        disable_notice=False
     ):
         self.workspace_url = workspace_url
         self.personal_access_token = personal_access_token
         self.service_principal_client_id = service_principal_client_id
         self.service_principal_client_secret = service_principal_client_secret
+        self._is_notebook_pat = False
         if not (
             self.service_principal_client_id and
             self.service_principal_client_secret
         ):
             if self.workspace_url is None:
                 host_creds = databricks_utils.get_databricks_host_creds()
                 self.workspace_url = host_creds.host
             if self.personal_access_token is None:
+                self._is_notebook_pat = True
                 host_creds = databricks_utils.get_databricks_host_creds()
                 self.personal_access_token = host_creds.token
 
             host_creds = databricks_utils.get_databricks_host_creds()
             self.personal_access_token = host_creds.token
         self._control_plane_oauth_token = None
         self._control_plane_oauth_token_expiry_ts = None
-        self.validate()
+        self.validate(disable_notice=disable_notice)
 
-    def validate(self):
+    def validate(self, disable_notice=False):
         if not (self.personal_access_token or
                 (self.service_principal_client_id and 
                     self.service_principal_client_secret)):
             raise InvalidInputException(
                 "Please specify either personal access token or service principal client ID and secret."
             )
         if (self.service_principal_client_id and
                 self.service_principal_client_secret and
                 not self.workspace_url):
             raise InvalidInputException(
                 "Service Principal auth flow requires workspace url"
             )
-        if self.personal_access_token:
+        if self._is_notebook_pat and not disable_notice:
+            print(
+                """[NOTICE] Using a notebook authentication token. Recommended for development only. For improved performance, please use Service Principal based authentication. To disable this message, pass disable_notice=True to VectorSearchClient()."""
+            )
+        elif self.personal_access_token and not disable_notice:
             print(
-                """[WARNING] Personal access tokens should only be used for development.\nIf you are using vector search in production, please use our Service Principal flow."""
+                """[NOTICE] Using a Personal Authentication Token (PAT). Recommended for development only. For improved performance, please use Service Principal based authentication. To disable this message, pass disable_notice=True to VectorSearchClient()."""
             )
 
+
     def _get_token_for_request(self):
         if self.personal_access_token:
             logging.info("[VectorSearchClient] Using PAT token")
             return self.personal_access_token
         if (
             self._control_plane_oauth_token
             and self._control_plane_oauth_token_expiry_ts
```

## Comparing `databricks_vectorsearch-0.8.dist-info/LICENSE.md` & `databricks_vectorsearch-0.9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `databricks_vectorsearch-0.8.dist-info/RECORD` & `databricks_vectorsearch-0.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 databricks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databricks/vector_search/client.py,sha256=g7u7Zfugx9ErryB2_82LEUz3uWFdl_-qCZNP6CAWTt0,10588
+databricks/vector_search/client.py,sha256=_Zsp7cVM8F9JUzpaXOj6phNkdp-i6tLr1LAV03ezktA,11208
 databricks/vector_search/exceptions.py,sha256=uQDicrJ1_Hv41hI7mvJlRgh3uAZ-u1CCCNlo3zvLflE,50
 databricks/vector_search/index.py,sha256=h1U4WW31euXBJV-pPC3gzL89uZ6nS1d9mMd35OfL2sU,6036
 databricks/vector_search/utils.py,sha256=1ui9NJJdVhdniZTgNGAgVgk2Zb1H2M6KCOzjF4GGxHs,2364
-databricks_vectorsearch-0.8.dist-info/LICENSE.md,sha256=VlYiPV28DtYjKCQz5F3iskOvlNCMSXKQ8l5ggcRt28s,2414
-databricks_vectorsearch-0.8.dist-info/METADATA,sha256=ULRKz9eS0bURARsYER2acCE5KPPapVdgM_A2gahsf4M,400
-databricks_vectorsearch-0.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-databricks_vectorsearch-0.8.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
-databricks_vectorsearch-0.8.dist-info/RECORD,,
+databricks_vectorsearch-0.9.dist-info/LICENSE.md,sha256=VlYiPV28DtYjKCQz5F3iskOvlNCMSXKQ8l5ggcRt28s,2414
+databricks_vectorsearch-0.9.dist-info/METADATA,sha256=t4ksdZOPRO6k-kf4cs5Okl6bGjijr83fjyYBiTj4mHQ,400
+databricks_vectorsearch-0.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+databricks_vectorsearch-0.9.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
+databricks_vectorsearch-0.9.dist-info/RECORD,,
```

