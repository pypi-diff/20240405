# Comparing `tmp/trustwise-3.1.3.tar.gz` & `tmp/trustwise-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustwise-3.1.3.tar", last modified: Sun Mar 31 00:25:15 2024, max compression
+gzip compressed data, was "trustwise-3.1.4.tar", last modified: Fri Apr  5 20:19:19 2024, max compression
```

## Comparing `trustwise-3.1.3.tar` & `trustwise-3.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jaisantosh   (501) staff       (20)        0 2024-03-31 00:25:15.992692 trustwise-3.1.3/
--rw-r--r--   0 jaisantosh   (501) staff       (20)     1065 2024-02-08 14:27:51.000000 trustwise-3.1.3/LICENSE
--rw-r--r--   0 jaisantosh   (501) staff       (20)     2439 2024-03-31 00:25:15.992491 trustwise-3.1.3/PKG-INFO
--rw-r--r--   0 jaisantosh   (501) staff       (20)     1841 2024-03-30 22:13:13.000000 trustwise-3.1.3/README.md
--rw-r--r--   0 jaisantosh   (501) staff       (20)       38 2024-03-31 00:25:15.992734 trustwise-3.1.3/setup.cfg
--rw-r--r--   0 jaisantosh   (501) staff       (20)      783 2024-03-31 00:24:32.000000 trustwise-3.1.3/setup.py
-drwxr-xr-x   0 jaisantosh   (501) staff       (20)        0 2024-03-31 00:25:15.991496 trustwise-3.1.3/trustwise/
--rw-r--r--   0 jaisantosh   (501) staff       (20)        0 2024-02-08 14:27:51.000000 trustwise-3.1.3/trustwise/__init__.py
--rw-r--r--   0 jaisantosh   (501) staff       (20)    10249 2024-03-31 00:24:23.000000 trustwise-3.1.3/trustwise/callback.py
--rw-r--r--   0 jaisantosh   (501) staff       (20)      179 2024-03-30 22:13:13.000000 trustwise-3.1.3/trustwise/config.py
--rw-r--r--   0 jaisantosh   (501) staff       (20)      751 2024-03-30 22:30:08.000000 trustwise-3.1.3/trustwise/models.py
--rw-r--r--   0 jaisantosh   (501) staff       (20)     1986 2024-03-30 22:24:45.000000 trustwise-3.1.3/trustwise/request.py
-drwxr-xr-x   0 jaisantosh   (501) staff       (20)        0 2024-03-31 00:25:15.992279 trustwise-3.1.3/trustwise.egg-info/
--rw-r--r--   0 jaisantosh   (501) staff       (20)     2439 2024-03-31 00:25:15.000000 trustwise-3.1.3/trustwise.egg-info/PKG-INFO
--rw-r--r--   0 jaisantosh   (501) staff       (20)      295 2024-03-31 00:25:15.000000 trustwise-3.1.3/trustwise.egg-info/SOURCES.txt
--rw-r--r--   0 jaisantosh   (501) staff       (20)        1 2024-03-31 00:25:15.000000 trustwise-3.1.3/trustwise.egg-info/dependency_links.txt
--rw-r--r--   0 jaisantosh   (501) staff       (20)       53 2024-03-31 00:25:15.000000 trustwise-3.1.3/trustwise.egg-info/requires.txt
--rw-r--r--   0 jaisantosh   (501) staff       (20)       10 2024-03-31 00:25:15.000000 trustwise-3.1.3/trustwise.egg-info/top_level.txt
+drwxr-xr-x   0 jaisantosh   (501) staff       (20)        0 2024-04-05 20:19:19.277791 trustwise-3.1.4/
+-rw-r--r--   0 jaisantosh   (501) staff       (20)     1065 2024-02-08 14:27:51.000000 trustwise-3.1.4/LICENSE
+-rw-r--r--   0 jaisantosh   (501) staff       (20)     2439 2024-04-05 20:19:19.277587 trustwise-3.1.4/PKG-INFO
+-rw-r--r--   0 jaisantosh   (501) staff       (20)     1841 2024-04-05 20:15:38.000000 trustwise-3.1.4/README.md
+-rw-r--r--   0 jaisantosh   (501) staff       (20)       38 2024-04-05 20:19:19.277833 trustwise-3.1.4/setup.cfg
+-rw-r--r--   0 jaisantosh   (501) staff       (20)      783 2024-04-05 20:19:17.000000 trustwise-3.1.4/setup.py
+drwxr-xr-x   0 jaisantosh   (501) staff       (20)        0 2024-04-05 20:19:19.276518 trustwise-3.1.4/trustwise/
+-rw-r--r--   0 jaisantosh   (501) staff       (20)        0 2024-02-08 14:27:51.000000 trustwise-3.1.4/trustwise/__init__.py
+-rw-r--r--   0 jaisantosh   (501) staff       (20)    10249 2024-04-05 20:15:38.000000 trustwise-3.1.4/trustwise/callback.py
+-rw-r--r--   0 jaisantosh   (501) staff       (20)      179 2024-03-30 22:13:13.000000 trustwise-3.1.4/trustwise/config.py
+-rw-r--r--   0 jaisantosh   (501) staff       (20)      751 2024-04-05 20:15:38.000000 trustwise-3.1.4/trustwise/models.py
+-rw-r--r--   0 jaisantosh   (501) staff       (20)     2050 2024-04-05 20:15:38.000000 trustwise-3.1.4/trustwise/request.py
+drwxr-xr-x   0 jaisantosh   (501) staff       (20)        0 2024-04-05 20:19:19.277368 trustwise-3.1.4/trustwise.egg-info/
+-rw-r--r--   0 jaisantosh   (501) staff       (20)     2439 2024-04-05 20:19:19.000000 trustwise-3.1.4/trustwise.egg-info/PKG-INFO
+-rw-r--r--   0 jaisantosh   (501) staff       (20)      295 2024-04-05 20:19:19.000000 trustwise-3.1.4/trustwise.egg-info/SOURCES.txt
+-rw-r--r--   0 jaisantosh   (501) staff       (20)        1 2024-04-05 20:19:19.000000 trustwise-3.1.4/trustwise.egg-info/dependency_links.txt
+-rw-r--r--   0 jaisantosh   (501) staff       (20)       53 2024-04-05 20:19:19.000000 trustwise-3.1.4/trustwise.egg-info/requires.txt
+-rw-r--r--   0 jaisantosh   (501) staff       (20)       10 2024-04-05 20:19:19.000000 trustwise-3.1.4/trustwise.egg-info/top_level.txt
```

### Comparing `trustwise-3.1.3/LICENSE` & `trustwise-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trustwise-3.1.3/PKG-INFO` & `trustwise-3.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustwise
-Version: 3.1.3
+Version: 3.1.4
 Summary: Trustwise PyPi Package
 Home-page: https://github.com/trustwiseai/trustwise
 Author: Trustwise
 Author-email: nihal@trustwise.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `trustwise-3.1.3/README.md` & `trustwise-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `trustwise-3.1.3/setup.py` & `trustwise-3.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="trustwise",
-    version="3.1.3",
+    version="3.1.4",
     description="Trustwise PyPi Package",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="Trustwise",
     author_email="nihal@trustwise.ai",
     url="https://github.com/trustwiseai/trustwise",
     packages=find_packages(),
```

### Comparing `trustwise-3.1.3/trustwise/callback.py` & `trustwise-3.1.4/trustwise/callback.py`

 * *Files identical despite different names*

### Comparing `trustwise-3.1.3/trustwise/models.py` & `trustwise-3.1.4/trustwise/models.py`

 * *Files identical despite different names*

### Comparing `trustwise-3.1.3/trustwise/request.py` & `trustwise-3.1.4/trustwise/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 
 
 # later on...
 
 
 def evaluate(user_id: str, scan_id: str, scan_name: str, query: str, response: PydanticResponse,
              api_key: Optional[str] = None,
-             project_id: Optional[str] = None) -> Any:
+             project_id: Optional[str] = None,
+             llm_name: Optional[str] = None) -> Any:
     context = []  # Context chunks to be logged in the record with text, score and node id.
 
     for node in response.source_nodes:
         node_text = node.text
         node_score = node.score
         node_id = node.id_
 
         chunk = Chunk(node_text=node_text, node_score=node_score, node_id=node_id)
         context.append(chunk)
 
     # Data to be uploaded to the endpoint for the evaluations to run
     data = UploadData(user_id=user_id, scan_id=scan_id, scan_name=scan_name, project_id=project_id, query=query,
                       context=context,
-                      response=response.response, api_key=api_key)
+                      response=response.response, api_key=api_key, llm_name=llm_name)
 
     try:
         data_dict = data.model_dump()  # Convert to dict for JSON serialization
         response_object = requests.post(url=TW_EVALUATION_URL, json=data_dict, timeout=600)
         response_object.raise_for_status()  # Check for HTTP errors
 
         # Check if the response has a valid JSON content type
```

### Comparing `trustwise-3.1.3/trustwise.egg-info/PKG-INFO` & `trustwise-3.1.4/trustwise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustwise
-Version: 3.1.3
+Version: 3.1.4
 Summary: Trustwise PyPi Package
 Home-page: https://github.com/trustwiseai/trustwise
 Author: Trustwise
 Author-email: nihal@trustwise.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

