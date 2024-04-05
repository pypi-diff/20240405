# Comparing `tmp/pyaqueduct-0.0.5.tar.gz` & `tmp/pyaqueduct-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaqueduct-0.0.5.tar", max compression
+gzip compressed data, was "pyaqueduct-0.0.6.tar", max compression
```

## Comparing `pyaqueduct-0.0.5.tar` & `pyaqueduct-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2024-02-19 15:06:33.856889 pyaqueduct-0.0.5/LICENSE
--rw-r--r--   0        0        0     2331 2024-02-19 15:06:33.856889 pyaqueduct-0.0.5/README.md
--rw-r--r--   0        0        0      145 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/__init__.py
--rw-r--r--   0        0        0     2996 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/api.py
--rw-r--r--   0        0        0      292 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/client/__init__.py
--rw-r--r--   0        0        0    12799 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/client/client.py
--rw-r--r--   0        0        0     2175 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/client/types.py
--rw-r--r--   0        0        0      929 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/exceptions.py
--rw-r--r--   0        0        0     3283 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/experiment.py
--rw-r--r--   0        0        0        0 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/schemas/__init__.py
--rw-r--r--   0        0        0     2463 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/schemas/mutations.py
--rw-r--r--   0        0        0     1696 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyaqueduct/schemas/queries.py
--rw-r--r--   0        0        0     1110 2024-02-19 15:06:33.860889 pyaqueduct-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 pyaqueduct-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2331 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/README.md
+-rw-r--r--   0        0        0      145 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/__init__.py
+-rw-r--r--   0        0        0     2996 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/api.py
+-rw-r--r--   0        0        0      292 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/client/__init__.py
+-rw-r--r--   0        0        0    12834 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/client/client.py
+-rw-r--r--   0        0        0     2175 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/client/types.py
+-rw-r--r--   0        0        0      929 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/exceptions.py
+-rw-r--r--   0        0        0     3283 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/experiment.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/schemas/__init__.py
+-rw-r--r--   0        0        0     2463 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/schemas/mutations.py
+-rw-r--r--   0        0        0     1696 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/schemas/queries.py
+-rw-r--r--   0        0        0     1129 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 pyaqueduct-0.0.6/PKG-INFO
```

### Comparing `pyaqueduct-0.0.5/LICENSE` & `pyaqueduct-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.5/README.md` & `pyaqueduct-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.5/pyaqueduct/api.py` & `pyaqueduct-0.0.6/pyaqueduct/api.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.5/pyaqueduct/client/client.py` & `pyaqueduct-0.0.6/pyaqueduct/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,19 @@
     def __init__(self, url: str, timeout: float):
         """
         Args:
             url: URL of the Aqueduct server endpoint.
             timeout: Response timeout in seconds.
 
         """
-        super().__init__(url=HttpUrl(url), timeout=timeout)
+        super().__init__(url=url, timeout=timeout)
 
-        self._gql_client = Client(transport=HTTPXTransport(url=f"{url}/graphql"))
+        self._gql_client = Client(
+            transport=HTTPXTransport(url=f"{url}/graphql", timeout=self.timeout)
+        )
         self.connect()
 
     def connect(self):
         """Connect to GraphQL connect"""
         self._session = self._gql_client.connect_sync()  # type: ignore
 
     def close(self):
```

### Comparing `pyaqueduct-0.0.5/pyaqueduct/client/types.py` & `pyaqueduct-0.0.6/pyaqueduct/client/types.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.5/pyaqueduct/exceptions.py` & `pyaqueduct-0.0.6/pyaqueduct/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.5/pyaqueduct/experiment.py` & `pyaqueduct-0.0.6/pyaqueduct/experiment.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.5/pyaqueduct/schemas/mutations.py` & `pyaqueduct-0.0.6/pyaqueduct/schemas/mutations.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.5/pyaqueduct/schemas/queries.py` & `pyaqueduct-0.0.6/pyaqueduct/schemas/queries.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.5/pyproject.toml` & `pyaqueduct-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "pyaqueduct"
-version = "0.0.5"
+version = "0.0.6"
 description = "Aqueduct Python Client Library"
 authors = ["Aqueduct Team <aqueduct@riverlane.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://aqueducthub.github.io/pyaqueduct"
 documentation = "https://aqueducthub.github.io/pyaqueduct"
 repository = "https://github.com/AqueductHub/pyaqueduct"
 
 [tool.poetry.dependencies]
 python = ">= 3.8,< 3.12"
 requests = "^2.31"
 tqdm = "^4.66"
-httpx = "^0.25"
+httpx = ">=0.15,<0.25"
 types-tqdm = "^4.66"
-pydantic = "^2.5"
+pydantic = ">=1.10.13,<3.0.0"
 gql = {extras = ["httpx"], version = "^3.5"}
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4"
 pylint = "^2.17"
 yapf = "^0.40"
```

### Comparing `pyaqueduct-0.0.5/PKG-INFO` & `pyaqueduct-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyaqueduct
-Version: 0.0.5
+Version: 0.0.6
 Summary: Aqueduct Python Client Library
 Home-page: https://aqueducthub.github.io/pyaqueduct
 License: MIT
 Author: Aqueduct Team
 Author-email: aqueduct@riverlane.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gql[httpx] (>=3.5,<4.0)
-Requires-Dist: httpx (>=0.25,<0.26)
-Requires-Dist: pydantic (>=2.5,<3.0)
+Requires-Dist: httpx (>=0.15,<0.25)
+Requires-Dist: pydantic (>=1.10.13,<3.0.0)
 Requires-Dist: requests (>=2.31,<3.0)
 Requires-Dist: tqdm (>=4.66,<5.0)
 Requires-Dist: types-tqdm (>=4.66,<5.0)
 Project-URL: Documentation, https://aqueducthub.github.io/pyaqueduct
 Project-URL: Issues, https://github.com/AqueductHub/pyaqueduct/issues
 Project-URL: Repository, https://github.com/AqueductHub/pyaqueduct
 Description-Content-Type: text/markdown
```

