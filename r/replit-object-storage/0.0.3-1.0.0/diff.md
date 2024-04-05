# Comparing `tmp/replit_object_storage-0.0.3.tar.gz` & `tmp/replit_object_storage-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_object_storage-0.0.3.tar", max compression
+gzip compressed data, was "replit_object_storage-1.0.0.tar", max compression
```

## Comparing `replit_object_storage-0.0.3.tar` & `replit_object_storage-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      583 2024-03-20 11:46:01.856377 replit_object_storage-0.0.3/README.md
--rw-r--r--   0        0        0     1351 2024-03-20 11:46:04.908582 replit_object_storage-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      219 2024-03-20 11:46:01.860377 replit_object_storage-0.0.3/src/replit/object_storage/__init__.py
--rw-r--r--   0        0        0     6778 2024-03-20 11:46:02.160397 replit_object_storage-0.0.3/src/replit/object_storage/client.py
--rw-r--r--   0        0        0      635 2024-03-20 11:46:04.908582 replit_object_storage-0.0.3/src/replit/object_storage/config.py
--rw-r--r--   0        0        0     1933 2024-03-20 11:46:02.160397 replit_object_storage-0.0.3/src/replit/object_storage/errors.py
--rw-r--r--   0        0        0      186 2024-03-20 11:46:02.160397 replit_object_storage-0.0.3/src/replit/object_storage/object.py
--rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 replit_object_storage-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      583 2024-04-05 00:09:42.784934 replit_object_storage-1.0.0/README.md
+-rw-r--r--   0        0        0     1778 2024-04-05 19:42:55.002040 replit_object_storage-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-05 19:42:55.002040 replit_object_storage-1.0.0/src/replit/__init__.py
+-rw-r--r--   0        0        0      219 2024-03-20 11:46:01.860377 replit_object_storage-1.0.0/src/replit/object_storage/__init__.py
+-rw-r--r--   0        0        0      635 2024-04-05 19:42:55.002040 replit_object_storage-1.0.0/src/replit/object_storage/_config.py
+-rw-r--r--   0        0        0     8283 2024-04-05 19:42:55.002040 replit_object_storage-1.0.0/src/replit/object_storage/client.py
+-rw-r--r--   0        0        0     1934 2024-04-05 19:42:55.002040 replit_object_storage-1.0.0/src/replit/object_storage/errors.py
+-rw-r--r--   0        0        0      242 2024-04-05 19:42:55.002040 replit_object_storage-1.0.0/src/replit/object_storage/object.py
+-rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 replit_object_storage-1.0.0/PKG-INFO
```

### Comparing `replit_object_storage-0.0.3/README.md` & `replit_object_storage-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `replit_object_storage-0.0.3/pyproject.toml` & `replit_object_storage-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit.object_storage"
-version = "0.0.3"
+version = "1.0.0"
 description = "A library for interacting with Object Storage on Replit"
 authors = ["Repl.it <contact@repl.it>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/replit/replit-object-storage-python"
 homepage = "https://github.com/replit/replit-object-storage-python"
 classifiers = [
@@ -24,14 +24,33 @@
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.15"
 pytest = "^8.0.0"
 twine = "*"
 pytest-cov = "^4.1.0"
 tox = "^4.13.0"
+pydoc-markdown = "^4.8.2"
+
+[[tool.pydoc-markdown.loaders]]
+type = "python"
+search_path = [ "src" ]
+
+[tool.pydoc-markdown.renderer]
+docs_base_path = "docs"
+relative_output_path = "."
+
+type = "docusaurus"
+
+[tool.pydoc-markdown.renderer.markdown]
+data_code_block = true
+descriptive_class_title = "Class "
+insert_header_anchors = false
+render_page_title = false
+render_module_header_template = ""
+signature_with_decorators = false
 
 [tool.pyright]
 # https://github.com/microsoft/pyright/blob/main/docs/configuration.md
 useLibraryCodeForTypes = true
 exclude = [".cache"]
 
 [tool.ruff]
```

### Comparing `replit_object_storage-0.0.3/src/replit/object_storage/client.py` & `replit_object_storage-1.0.0/src/replit/object_storage/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 """Client for interacting with Object Storage. This is the top-level interface.
 
 Note: this Client is a thin wrapper over the GCS Python Library. As a result,
 many docstrings are borrowed from the underlying library.
 """
 
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import requests
 from google.auth import identity_pool
 from google.cloud import storage
 from google.cloud.exceptions import NotFound
-from replit.object_storage.config import REPLIT_ADC, REPLIT_DEFAULT_BUCKET_URL
+
+from replit.object_storage._config import REPLIT_ADC, REPLIT_DEFAULT_BUCKET_URL
 from replit.object_storage.errors import (
   DefaultBucketError,
   ObjectNotFoundError,
-  google_error_handler,
+  _google_error_handler,
 )
 from replit.object_storage.object import Object
 
 
 class Client:
   """Client manages interactions with Replit Object Storage.
     
   If multiple buckets are used within an application, one Client should be used
-  per bucket.
+  per bucket
+
+  Any method may return one of the following errors:
+  - `BucketNotFoundError`: If the bucket configured for the client could not be found.
+  - `DefaultBucketError`: If no bucket was explicitly configured and an error occurred
+      when resolving the default bucket.
+  - `ForbiddenError`: If access to the requested resource is not allowed.
+  - `TooManyRequestsError`: If rate limiting occurs.
+  - `UnauthorizedError`: If the requested operation is not allowed.
   """
 
   __gcs_client: storage.Client
 
   __bucket_id: Optional[str] = None
   __gcs_bucket_handle: Optional[storage.Bucket] = None
 
@@ -41,86 +50,110 @@
     """
     creds = identity_pool.Credentials(**REPLIT_ADC)
     if bucket_id:
       self.__bucket_id = bucket_id
     self.__gcs_client = storage.Client(credentials=creds, project="")
     self.__gcs_bucket_handle = None
 
-  @google_error_handler
+  @_google_error_handler
   def copy(self, object_name: str, dest_object_name: str) -> None:
     """Copies the specified object within the same bucket.
 
     If an object exists in the same location, it will be overwritten.
 
     Args:
         object_name: The full path of the object to be copied.
         dest_object_name: The full path to copy the object to.
+
+    Raises:
+        ObjectNotFoundError: If the source object could not be found.
     """
     source_object = self.__object(object_name)
     bucket = self.__bucket()
     bucket.copy_blob(
       source_object,
       bucket,
       dest_object_name,
     )
 
-  @google_error_handler
+  @_google_error_handler
   def delete(self, object_name: str, ignore_not_found: bool = False) -> None:
     """Deletes an object from Object Storage.
 
     Args:
         object_name: The name of the object to be deleted.
         ignore_not_found: Whether an error should be raised if the object does not
           exist.
+
+    Raises:
+        ObjectNotFoundError: If the object could not be found.
     """
     try:
       return self.__object(object_name).delete()
     except NotFound as err:
       if ignore_not_found:
         return
       raise ObjectNotFoundError("The requested object could not be found.") from err
 
-  @google_error_handler
+  @_google_error_handler
   def download_as_bytes(self, object_name: str) -> bytes:
     """Download the contents an object as a bytes object.
 
     Args:
         object_name: The name of the object to be downloaded.
+
+    Returns:
+        The raw byte representation of the object's contents.
+
+    Raises:
+        ObjectNotFoundError: If the object could not be found.
     """
     return self.__object(object_name).download_as_bytes()
 
-  @google_error_handler
+  @_google_error_handler
   def download_as_text(self, object_name: str) -> str:
     """Download the contents an object as a string.
 
     Args:
         object_name: The name of the object to be downloaded.
+
+    Returns:
+        The object's contents as a UTF-8 encoded string.
+
+    Raises:
+        ObjectNotFoundError: If the object could not be found.
     """
     return self.__object(object_name).download_as_text()
 
-  @google_error_handler
+  @_google_error_handler
   def download_to_filename(self, object_name: str, dest_filename: str) -> None:
     """Download the contents an object into a file on the local disk.
 
     Args:
         object_name: The name of the object to be downloaded.
         dest_filename: The filename of the file on the local disk to be written.
+
+    Raises:
+        ObjectNotFoundError: If the object could not be found.
     """
     return self.__object(object_name).download_to_filename(dest_filename)
 
-  @google_error_handler
+  @_google_error_handler
   def exists(self, object_name: str) -> bool:
     """Checks if an object exist.
 
     Args:
         object_name: The name of the object to be checked.
+
+    Returns:
+        Whether or not the object exists.
     """
     return self.__object(object_name).exists()
 
-  @google_error_handler
+  @_google_error_handler
   def list(
       self,
       end_offset: Optional[str] = None,
       match_glob: Optional[str] = None,
       max_results: Optional[int] = None,
       prefix: Optional[str] = None,
       start_offset: Optional[str] = None,
@@ -136,38 +169,54 @@
         max_results: The maximum number of results that can be returned in the
             response.
         prefix: Filter results to objects who names have the specified prefix.
         start_offset: Filter results to objects whose names are
             lexicographically equal to or after start_offset. If endOffset is
             also set, the objects listed have names between start_offset
             (inclusive) and end_offset (exclusive).
-        
+
+    Returns:
+        A list of objects matching the given query parameters. 
     """
     iter = self.__bucket().list_blobs(
         end_offset=end_offset,
         match_glob=match_glob,
         max_results=max_results,
         prefix=prefix,
         start_offset=start_offset,
     )
     return [Object(name=object.name) for object in iter]
 
-  @google_error_handler
+  @_google_error_handler
   def upload_from_filename(self, dest_object_name: str,
                            src_filename: str) -> None:
     """Upload an object from a file on the local disk.
 
     Args:
         dest_object_name: The name of the object to be uploaded.
         src_filename: The filename of a file on the local disk
     """
     self.__object(dest_object_name).upload_from_filename(src_filename)
 
-  @google_error_handler
-  def upload_from_text(self, dest_object_name: str, src_data: str) -> None:
+  @_google_error_handler
+  def upload_from_bytes(self, dest_object_name: str, src_data: bytes) -> None:
+    """Upload an object from bytes.
+
+    Args:
+        dest_object_name: The name of the object to be uploaded.
+        src_data: The bytes to be uploaded.
+    """
+    self.__object(dest_object_name).upload_from_string(src_data)
+
+  @_google_error_handler
+  def upload_from_text(
+    self,
+    dest_object_name: str,
+    src_data: Union[bytes, str]
+  ) -> None:
     """Upload an object from a string.
 
     Args:
         dest_object_name: The name of the object to be uploaded.
         src_data: The text to be uploaded.
     """
     self.__object(dest_object_name).upload_from_string(src_data)
```

### Comparing `replit_object_storage-0.0.3/src/replit/object_storage/config.py` & `replit_object_storage-1.0.0/src/replit/object_storage/_config.py`

 * *Files identical despite different names*

### Comparing `replit_object_storage-0.0.3/src/replit/object_storage/errors.py` & `replit_object_storage-1.0.0/src/replit/object_storage/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 class UnauthorizedError(Exception):
   """UnauthorizedError may occur if the requested operation is not allowed."""
   pass
 
 
-def google_error_handler(func):
+def _google_error_handler(func):
   """Wraps functions that call GCP APIs and handles common errors.
 
   Common errors are re-raised in more digestable formats, less common errors are passed
   through.
   """
   @wraps(func)
   def wrapper(*args, **kwargs):
```

### Comparing `replit_object_storage-0.0.3/PKG-INFO` & `replit_object_storage-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-object-storage
-Version: 0.0.3
+Version: 1.0.0
 Summary: A library for interacting with Object Storage on Replit
 Home-page: https://github.com/replit/replit-object-storage-python
 License: ISC
 Author: Repl.it
 Author-email: contact@repl.it
 Requires-Python: >=3.8.0,<3.13
 Classifier: License :: OSI Approved
```

