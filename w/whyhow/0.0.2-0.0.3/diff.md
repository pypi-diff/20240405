# Comparing `tmp/whyhow-0.0.2.tar.gz` & `tmp/whyhow-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyhow-0.0.2.tar", last modified: Thu Apr  4 07:55:43 2024, max compression
+gzip compressed data, was "whyhow-0.0.3.tar", last modified: Fri Apr  5 04:36:08 2024, max compression
```

## Comparing `whyhow-0.0.2.tar` & `whyhow-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.759480 whyhow-0.0.2/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     5447 2024-04-04 07:55:43.759234 whyhow-0.0.2/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)     4318 2024-04-04 07:54:08.000000 whyhow-0.0.2/README.md
--rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-04-04 07:43:46.000000 whyhow-0.0.2/pyproject.toml
--rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-04-04 07:55:43.759559 whyhow-0.0.2/setup.cfg
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.754414 whyhow-0.0.2/src/
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.755426 whyhow-0.0.2/src/whyhow/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-04-04 07:55:05.000000 whyhow-0.0.2/src/whyhow/__init__.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.756852 whyhow-0.0.2/src/whyhow/apis/
--rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/apis/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.2/src/whyhow/apis/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     3866 2024-04-04 07:11:07.000000 whyhow-0.0.2/src/whyhow/apis/graph.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-04 07:04:26.000000 whyhow-0.0.2/src/whyhow/client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/exceptions.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/py.typed
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.757432 whyhow-0.0.2/src/whyhow/schemas/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/schemas/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/schemas/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     3755 2024-04-04 06:49:03.000000 whyhow-0.0.2/src/whyhow/schemas/common.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1289 2024-04-04 07:02:16.000000 whyhow-0.0.2/src/whyhow/schemas/graph.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.758074 whyhow-0.0.2/src/whyhow.egg-info/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     5447 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/SOURCES.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/dependency_links.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.2/src/whyhow.egg-info/not-zip-safe
--rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/requires.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/top_level.txt
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.757778 whyhow-0.0.2/tests/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1395 2024-04-04 07:15:22.000000 whyhow-0.0.2/tests/test_client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.2/tests/test_dummy.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.732628 whyhow-0.0.3/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5447 2024-04-05 04:36:08.732419 whyhow-0.0.3/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     4318 2024-04-04 07:54:08.000000 whyhow-0.0.3/README.md
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-04-04 07:43:46.000000 whyhow-0.0.3/pyproject.toml
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-04-05 04:36:08.732668 whyhow-0.0.3/setup.cfg
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.726125 whyhow-0.0.3/src/
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.727666 whyhow-0.0.3/src/whyhow/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-04-05 04:26:15.000000 whyhow-0.0.3/src/whyhow/__init__.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.729347 whyhow-0.0.3/src/whyhow/apis/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/apis/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.3/src/whyhow/apis/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     3757 2024-04-05 04:27:59.000000 whyhow-0.0.3/src/whyhow/apis/graph.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-04 07:04:26.000000 whyhow-0.0.3/src/whyhow/client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/exceptions.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/py.typed
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.730506 whyhow-0.0.3/src/whyhow/schemas/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/schemas/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/schemas/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     3755 2024-04-04 06:49:03.000000 whyhow-0.0.3/src/whyhow/schemas/common.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1155 2024-04-05 04:27:51.000000 whyhow-0.0.3/src/whyhow/schemas/graph.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.731292 whyhow-0.0.3/src/whyhow.egg-info/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5447 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/SOURCES.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/dependency_links.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.3/src/whyhow.egg-info/not-zip-safe
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/requires.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/top_level.txt
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.731022 whyhow-0.0.3/tests/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-04-05 04:27:59.000000 whyhow-0.0.3/tests/test_client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.3/tests/test_dummy.py
```

### Comparing `whyhow-0.0.2/PKG-INFO` & `whyhow-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.2
+Version: 0.0.3
 Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `whyhow-0.0.2/README.md` & `whyhow-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.2/pyproject.toml` & `whyhow-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.2/src/whyhow/apis/graph.py` & `whyhow-0.0.3/src/whyhow/apis/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,14 +130,10 @@
             json=request_body.model_dump(),
         )
 
         raw_response.raise_for_status()
 
         response = QueryGraphResponse.model_validate(raw_response.json())
 
-        retval = QueryGraphReturn(
-            answer=response.answer,
-            cypher_query=response.cypher_query,
-            context=response.context,
-        )
+        retval = QueryGraphReturn(answer=response.answer)
 
         return retval
```

### Comparing `whyhow-0.0.2/src/whyhow/client.py` & `whyhow-0.0.3/src/whyhow/client.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.2/src/whyhow/schemas/base.py` & `whyhow-0.0.3/src/whyhow/schemas/base.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.2/src/whyhow/schemas/common.py` & `whyhow-0.0.3/src/whyhow/schemas/common.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.2/src/whyhow/schemas/graph.py` & `whyhow-0.0.3/src/whyhow/schemas/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,19 +40,13 @@
 
 
 class QueryGraphResponse(BaseResponse):
     """Schema for the response body of the query graph endpoint."""
 
     namespace: str
     answer: str
-    # triples: list[Triple]
-    cypher_query: str
-    context: str
 
 
 class QueryGraphReturn(BaseReturn):
     """Schema for the return value of the query graph endpoint."""
 
     answer: str
-    # triples: list[Triple]
-    cypher_query: str
-    context: str
```

### Comparing `whyhow-0.0.2/src/whyhow.egg-info/PKG-INFO` & `whyhow-0.0.3/src/whyhow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.2
+Version: 0.0.3
 Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `whyhow-0.0.2/src/whyhow.egg-info/SOURCES.txt` & `whyhow-0.0.3/src/whyhow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.2/tests/test_client.py` & `whyhow-0.0.3/tests/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,18 @@
             httpx_kwargs=httpx_kwargs,
         )
 
         assert fake_httpx_client_class.call_count == 1
         args, kwargs = fake_httpx_client_class.call_args
 
         assert not args
-        assert kwargs["base_url"] == "https://43nq5c1b4c.execute-api.us-east-2.amazonaws.com"
+        assert (
+            kwargs["base_url"]
+            == "https://43nq5c1b4c.execute-api.us-east-2.amazonaws.com"
+        )
         assert not kwargs["verify"]
 
         assert client.httpx_client is fake_httpx_client_class.return_value
 
     def test_base_url_twice(self):
         with pytest.raises(
             ValueError, match="base_url cannot be set in httpx_kwargs."
```

