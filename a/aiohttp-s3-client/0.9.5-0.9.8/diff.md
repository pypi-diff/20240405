# Comparing `tmp/aiohttp_s3_client-0.9.5.tar.gz` & `tmp/aiohttp_s3_client-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_s3_client-0.9.5.tar", max compression
+gzip compressed data, was "aiohttp_s3_client-0.9.8.tar", max compression
```

## Comparing `aiohttp_s3_client-0.9.5.tar` & `aiohttp_s3_client-0.9.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11358 2024-01-11 08:59:55.852390 aiohttp_s3_client-0.9.5/LICENSE
--rw-r--r--   0        0        0    10495 2024-01-11 08:59:55.852390 aiohttp_s3_client-0.9.5/LICENSE.md
--rw-r--r--   0        0        0     8471 2024-01-11 08:59:55.852390 aiohttp_s3_client-0.9.5/README.md
--rw-r--r--   0        0        0      199 2024-01-11 08:59:55.852390 aiohttp_s3_client-0.9.5/aiohttp_s3_client/__init__.py
--rw-r--r--   0        0        0    25424 2024-01-11 08:59:55.852390 aiohttp_s3_client-0.9.5/aiohttp_s3_client/client.py
--rw-r--r--   0        0        0     9902 2024-01-11 08:59:55.852390 aiohttp_s3_client-0.9.5/aiohttp_s3_client/credentials.py
--rw-r--r--   0        0        0        0 2024-01-11 08:59:55.852390 aiohttp_s3_client-0.9.5/aiohttp_s3_client/py.typed
--rw-r--r--   0        0        0      152 2024-01-11 09:00:18.404627 aiohttp_s3_client-0.9.5/aiohttp_s3_client/version.py
--rw-r--r--   0        0        0     2575 2024-01-11 08:59:55.852390 aiohttp_s3_client-0.9.5/aiohttp_s3_client/xml.py
--rw-r--r--   0        0        0     2549 2024-01-11 09:00:18.404627 aiohttp_s3_client-0.9.5/pyproject.toml
--rw-r--r--   0        0        0    10257 1970-01-01 00:00:00.000000 aiohttp_s3_client-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-05 13:21:19.335776 aiohttp_s3_client-0.9.8/LICENSE
+-rw-r--r--   0        0        0    10495 2024-04-05 13:21:19.335776 aiohttp_s3_client-0.9.8/LICENSE.md
+-rw-r--r--   0        0        0     8535 2024-04-05 13:21:19.335776 aiohttp_s3_client-0.9.8/README.md
+-rw-r--r--   0        0        0      199 2024-04-05 13:21:19.335776 aiohttp_s3_client-0.9.8/aiohttp_s3_client/__init__.py
+-rw-r--r--   0        0        0    25459 2024-04-05 13:21:19.335776 aiohttp_s3_client-0.9.8/aiohttp_s3_client/client.py
+-rw-r--r--   0        0        0     9902 2024-04-05 13:21:19.335776 aiohttp_s3_client-0.9.8/aiohttp_s3_client/credentials.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:21:19.335776 aiohttp_s3_client-0.9.8/aiohttp_s3_client/py.typed
+-rw-r--r--   0        0        0      152 2024-04-05 13:21:38.975894 aiohttp_s3_client-0.9.8/aiohttp_s3_client/version.py
+-rw-r--r--   0        0        0     2727 2024-04-05 13:21:19.335776 aiohttp_s3_client-0.9.8/aiohttp_s3_client/xml.py
+-rw-r--r--   0        0        0     2549 2024-04-05 13:21:38.975894 aiohttp_s3_client-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0    10321 1970-01-01 00:00:00.000000 aiohttp_s3_client-0.9.8/PKG-INFO
```

### Comparing `aiohttp_s3_client-0.9.5/LICENSE` & `aiohttp_s3_client-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_s3_client-0.9.5/LICENSE.md` & `aiohttp_s3_client-0.9.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiohttp_s3_client-0.9.5/README.md` & `aiohttp_s3_client-0.9.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,18 @@
         data = await resp.read()
 
     # Delete object using bucket+key
     async with client.delete("bucket/key") as resp:
         assert resp == HTTPStatus.NO_CONTENT
 
     # List objects by prefix
-    async for result in client.list_objects_v2("bucket/", prefix="prefix"):
+    async for result, prefixes in client.list_objects_v2("bucket/", prefix="prefix"):
         # Each result is a list of metadata objects representing an object
-        # stored in the bucket.
-        do_work(result)
+        # stored in the bucket.  Each prefixes is a list of common prefixes
+        do_work(result, prefixes)
 ```
 
 Bucket may be specified as subdomain or in object name:
 
 ```python
 import aiohttp
 from aiohttp_s3_client import S3Client
```

### Comparing `aiohttp_s3_client-0.9.5/aiohttp_s3_client/client.py` & `aiohttp_s3_client-0.9.8/aiohttp_s3_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -735,15 +735,15 @@
         object_name: t.Union[str, Path] = "/",
         *,
         bucket: t.Optional[str] = None,
         prefix: t.Optional[t.Union[str, Path]] = None,
         delimiter: t.Optional[str] = None,
         max_keys: t.Optional[int] = None,
         start_after: t.Optional[str] = None,
-    ) -> t.AsyncIterator[t.List[AwsObjectMeta]]:
+    ) -> t.AsyncIterator[t.Tuple[t.List[AwsObjectMeta], t.List[str]]]:
         """
         List objects in bucket.
 
         Returns an iterator over lists of metadata objects, each corresponding
         to an individual response result (typically limited to 1000 keys).
 
         object_name:
@@ -783,14 +783,14 @@
                         resp,
                         (
                             "Got response with wrong status for GET request "
                             f"for {object_name} with prefix '{prefix}'"
                         ),
                     )
                 payload = await resp.read()
-                metadata, continuation_token = parse_list_objects(payload)
-                if not metadata:
+                metadata, prefixes, cont_token = parse_list_objects(payload)
+                if not metadata and not prefixes:
                     break
-                yield metadata
-                if not continuation_token:
+                yield metadata, prefixes
+                if not cont_token:
                     break
-                params["continuation-token"] = continuation_token
+                params["continuation-token"] = cont_token
```

### Comparing `aiohttp_s3_client-0.9.5/aiohttp_s3_client/credentials.py` & `aiohttp_s3_client-0.9.8/aiohttp_s3_client/credentials.py`

 * *Files identical despite different names*

### Comparing `aiohttp_s3_client-0.9.5/aiohttp_s3_client/xml.py` & `aiohttp_s3_client-0.9.8/aiohttp_s3_client/xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,18 +39,23 @@
     return (
         b'<?xml version="1.0" encoding="UTF-8"?>' +
         ET.tostring(root, encoding="UTF-8")
     )
 
 
 def parse_list_objects(payload: bytes) -> Tuple[
-    List[AwsObjectMeta], Optional[str],
+    List[AwsObjectMeta], List[str], Optional[str],
 ]:
     root = ET.fromstring(payload)
     result = []
+    prefixes = [
+        el.text
+        for el in root.findall(f"{{{NS}}}CommonPrefixes/{{{NS}}}Prefix")
+        if el.text
+    ]
     for el in root.findall(f"{{{NS}}}Contents"):
         etag = key = last_modified = size = storage_class = None
         for child in el:
             tag = child.tag[child.tag.rfind("}") + 1:]
             text = child.text
             if text is None:
                 continue
@@ -74,8 +79,8 @@
             size is not None and
             storage_class
         ):
             meta = AwsObjectMeta(etag, key, last_modified, size, storage_class)
             result.append(meta)
     nct_el = root.find(f"{{{NS}}}NextContinuationToken")
     continuation_token = nct_el.text if nct_el is not None else None
-    return result, continuation_token
+    return result, prefixes, continuation_token
```

### Comparing `aiohttp_s3_client-0.9.5/pyproject.toml` & `aiohttp_s3_client-0.9.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "aiohttp-s3-client"
 # Dummy version which will be rewritten with poem-plugins
-version = "0.9.5"
+version = "0.9.8"
 description = "The simple module for putting and getting object from Amazon S3 compatible endpoints"
 authors = [
     "Dmitry Orlov <me@mosquito.su>",
     "Yuri Shikanov <dizballanze@gmail.com>",
     "Alexander Vasin <hi@alvass.in>"
 ]
 license = "Apache Software License"
```

### Comparing `aiohttp_s3_client-0.9.5/PKG-INFO` & `aiohttp_s3_client-0.9.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-s3-client
-Version: 0.9.5
+Version: 0.9.8
 Summary: The simple module for putting and getting object from Amazon S3 compatible endpoints
 Home-page: https://github.com/aiokitchen/aiohttp-s3-client
 License: Apache Software License
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -96,18 +96,18 @@
         data = await resp.read()
 
     # Delete object using bucket+key
     async with client.delete("bucket/key") as resp:
         assert resp == HTTPStatus.NO_CONTENT
 
     # List objects by prefix
-    async for result in client.list_objects_v2("bucket/", prefix="prefix"):
+    async for result, prefixes in client.list_objects_v2("bucket/", prefix="prefix"):
         # Each result is a list of metadata objects representing an object
-        # stored in the bucket.
-        do_work(result)
+        # stored in the bucket.  Each prefixes is a list of common prefixes
+        do_work(result, prefixes)
 ```
 
 Bucket may be specified as subdomain or in object name:
 
 ```python
 import aiohttp
 from aiohttp_s3_client import S3Client
```

