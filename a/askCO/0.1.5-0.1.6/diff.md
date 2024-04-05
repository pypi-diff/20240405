# Comparing `tmp/askCO-0.1.5.tar.gz` & `tmp/askCO-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.1.5.tar", last modified: Sat Nov 18 04:57:11 2023, max compression
+gzip compressed data, was "askCO-0.1.6.tar", last modified: Fri Apr  5 01:26:18 2024, max compression
```

## Comparing `askCO-0.1.5.tar` & `askCO-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 04:57:11.751973 askCO-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-11-18 04:57:11.751973 askCO-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2023-11-18 04:57:02.000000 askCO-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-11-18 04:57:02.000000 askCO-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-18 04:57:11.751973 askCO-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 04:57:11.751973 askCO-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 04:57:11.751973 askCO-0.1.5/src/askCO/
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2023-11-18 04:57:02.000000 askCO-0.1.5/src/askCO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-11-18 04:57:02.000000 askCO-0.1.5/src/askCO/tryCO.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 04:57:11.751973 askCO-0.1.5/src/askCO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-11-18 04:57:11.000000 askCO-0.1.5/src/askCO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-11-18 04:57:11.000000 askCO-0.1.5/src/askCO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 04:57:11.000000 askCO-0.1.5/src/askCO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-18 04:57:11.000000 askCO-0.1.5/src/askCO.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:26:18.781379 askCO-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-05 01:26:18.781379 askCO-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-05 01:26:12.000000 askCO-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 01:26:12.000000 askCO-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 01:26:18.781379 askCO-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:26:18.777379 askCO-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:26:18.781379 askCO-0.1.6/src/askCO/
+-rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-04-05 01:26:12.000000 askCO-0.1.6/src/askCO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-05 01:26:12.000000 askCO-0.1.6/src/askCO/tryCO.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:26:18.781379 askCO-0.1.6/src/askCO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-05 01:26:18.000000 askCO-0.1.6/src/askCO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-05 01:26:18.000000 askCO-0.1.6/src/askCO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:26:18.000000 askCO-0.1.6/src/askCO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 01:26:18.000000 askCO-0.1.6/src/askCO.egg-info/top_level.txt
```

### Comparing `askCO-0.1.5/PKG-INFO` & `askCO-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `askCO-0.1.5/README.md` & `askCO-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `askCO-0.1.5/pyproject.toml` & `askCO-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "askCO"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
 	{name = "Lucy Schrader", email = "lucy@schrader.nz"},
 ]
 description = "Python interface for Te Papa's collections API"
 readme = "README.md"
 keywords = ["python", "museum", "api"]
 requires-python = ">=3.7"
```

### Comparing `askCO-0.1.5/src/askCO/__init__.py` & `askCO-0.1.6/src/askCO/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from requests import get, post, exceptions
 import json
 import os
+from sys import exit
 import time
 
+
 class Query():
 	# Run a single query to the API to return either a page of results or a single resource
 	# Provide the API key, a method (either GET or POST), and a complete URL and body (if POST)
 	# Redirects cannot be allowed on a scroll POST request
 	def __init__(self, api_key=None, method=None, url=None, data=None, allow_redirects=True, timeout=5, attempts=3, sleep=0.1, quiet=False):
 		auth_key = "x-api-key"
 		headers = {auth_key: api_key, "Content-Type": "application/json", "Accept": "application/json;profiles=tepapa.collections.api.v1"}
@@ -35,14 +37,15 @@
 					if not quiet:
 						print(response.status_code)
 					time.sleep(sleep)
 
 		if self.response == None:
 			print("Query {m} {u} failed".format(m=method, u=url))
 
+
 class Request():
 	def __init__(self, **kwargs):
 		# Functional request settings
 		self.quiet = kwargs.get("quiet")
 		self.sleep = kwargs.get("sleep")
 
 		# Request header settings
@@ -68,16 +71,16 @@
 
 		# Switches to True when a 200, 204, or 404 status is returned
 		# Look at self.status_code to handle retrying in other cases
 		self.complete = False
 
 	def send_query(self):
 		if not self.api_key:
-			# Raise error, stop script
-			pass
+			raise ValueError("No api key found.")
+			exit("No api key found.")
 
 		self.response = Query(
 			api_key=self.api_key,
 			method=self.method,
 			url=self.request_url,
 			data=self.request_body,
 			timeout=self.timeout,
@@ -143,24 +146,26 @@
 			self.record_count = response_text["_metadata"]["resultset"]["count"]
 			if not self.quiet:
 				print("Retrieving {} records".format(self.record_count))
 
 		if response_text.get("results"):
 			self.records.extend([result for result in response_text["results"]])
 
+
 class Search(Request):
 	def __init__(self, **kwargs):
 		Request.__init__(self, **kwargs)
 		# Build a search for a specified page of results
 		self.query_type = "search"
 		self.query = kwargs.get("query")
 		self.fields = kwargs.get("fields")
 		self.sort = kwargs.get("sort")
 		self.start = kwargs.get("start")
 		self.size = kwargs.get("size")
+		# Note that filters with multiple values only work for GET queries at the moment
 		self.filters = kwargs.get("filters")
 		self.exists = kwargs.get("exists")
 
 		self.build_query()
 
 	def build_query(self):
 		if not self.endpoint:
@@ -194,15 +199,19 @@
 			url_parts = []
 			query_parts = []
 
 			if self.query:
 				query_parts.append(self.query)
 			if self.filters:
 				for f in self.filters:
-					query_parts.append("{k}:{v}".format(k=f["field"], v=f["keyword"]))
+					if isinstance(f["keyword"], list):
+						filter_value = "(" + " OR ".join(f["keyword"]) + ")"
+					else:
+						filter_value = f["keyword"]
+					query_parts.append("{k}:{v}".format(k=f["field"], v=filter_value))
 			if self.exists:
 				query_parts.append("_exists_:{}".format(self.exists))
 
 			query_string = " AND ".join(query_parts)
 			url_parts.append(query_string)
 			
 			if self.fields:
@@ -221,14 +230,15 @@
 		
 	def _singleValueFormatter(self, param_name, value):
 		return {param_name: value}
 
 	def _multiValueFormatter(self, param_name, values):
 		return {param_name: ",".join(values)}
 
+
 class Scroll(Request):
 	# Continually call all matching records until done
 	def __init__(self, **kwargs):
 		Request.__init__(self, **kwargs)
 		self.query_type = "scroll"
 		self.allow_redirects = False
 
@@ -287,14 +297,15 @@
 					break
 
 			self.method = "GET"
 			self.request_url = "{b}{l}".format(b=self.base_url, l=self.response.headers["Location"])
 			self.send_query()
 			time.sleep(self.sleep)
 
+
 class Resource(Request):
 	# Resource object to build a query and hold a returned resource
 	def __init__(self, **kwargs):
 		Request.__init__(self, **kwargs)
 		self.query_type = "resource"
 		self.method = "GET"
 		self.irn = kwargs.get("irn")
@@ -318,8 +329,8 @@
 				self.request_url += "size={}".format(size)
 			if self.size and self.types:
 				self.request_url += "&"
 			if self.types:
 				self.request_url += "types={}".format(types)
 
 	def save_record(self):
-		self.response_text = json.loads(self.response.text)
+		self.response_text = json.loads(self.response.text)
```

### Comparing `askCO-0.1.5/src/askCO/tryCO.py` & `askCO-0.1.6/src/askCO/tryCO.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 quiet = False
 sleep = 0.1
 timeout = 5
 attempts = 3
 
 def try_search():
 	# Set the search request parameters
-	# No endpoint specified - will search all records
+	# Can only use multiple terms on a single filter for a GET query with a specified endpoint
 	query = "Myosotis"
-	filters = [{"field": "type", "keyword": "Specimen"}, {"field": "collection", "keyword": "Plants"}]
+	endpoint = "object"
+	filters = [{"field": "type", "keyword": "Specimen"}, {"field": "collection", "keyword": ["Plants", "LandMammals"]}]
 	fields = None
 	size = 100
 	start = 0
 
 	# Create the query object
 	request = Search(api_key=api_key,
 		query=query,
+		endpoint=endpoint,
 		filters=filters,
 		fields=fields,
 		size=size,
 		start=start,
 		timeout=timeout,
 		attempts=attempts,
 		sleep=sleep,
@@ -97,10 +99,10 @@
 	request.save_record()
 
 	# See what you got
 	print("Received record for {e}/{i}".format(e=endpoint, i=irn))
 	if request.response_text:
 		print(request.response_text)
 
-#try_search()
-try_scroll()
+try_search()
+#try_scroll()
 #try_resource()
```

### Comparing `askCO-0.1.5/src/askCO.egg-info/PKG-INFO` & `askCO-0.1.6/src/askCO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

