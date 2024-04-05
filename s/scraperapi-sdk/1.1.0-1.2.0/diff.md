# Comparing `tmp/scraperapi_sdk-1.1.0.tar.gz` & `tmp/scraperapi_sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraperapi_sdk-1.1.0.tar", max compression
+gzip compressed data, was "scraperapi_sdk-1.2.0.tar", max compression
```

## Comparing `scraperapi_sdk-1.1.0.tar` & `scraperapi_sdk-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3670 2024-04-04 06:44:07.242371 scraperapi_sdk-1.1.0/README.md
--rw-r--r--   0        0        0      713 2024-04-03 11:43:14.100373 scraperapi_sdk-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-12-20 08:41:35.662682 scraperapi_sdk-1.1.0/scraperapi_sdk/__init__.py
--rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.1.0/scraperapi_sdk/__version__.py
--rw-r--r--   0        0        0     4346 2024-04-03 14:03:58.665538 scraperapi_sdk-1.1.0/scraperapi_sdk/_client.py
--rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.1.0/scraperapi_sdk/exceptions.py
--rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 scraperapi_sdk-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5247 2024-04-05 08:24:55.206840 scraperapi_sdk-1.2.0/README.md
+-rw-r--r--   0        0        0      713 2024-04-05 08:32:14.894129 scraperapi_sdk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-12-20 08:41:35.662682 scraperapi_sdk-1.2.0/scraperapi_sdk/__init__.py
+-rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.2.0/scraperapi_sdk/__version__.py
+-rw-r--r--   0        0        0     5500 2024-04-05 08:11:39.300584 scraperapi_sdk-1.2.0/scraperapi_sdk/_client.py
+-rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.2.0/scraperapi_sdk/exceptions.py
+-rw-r--r--   0        0        0     5756 1970-01-01 00:00:00.000000 scraperapi_sdk-1.2.0/PKG-INFO
```

### Comparing `scraperapi_sdk-1.1.0/README.md` & `scraperapi_sdk-1.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -18,31 +18,28 @@
 content = client.get('https://amazon.com/', params={'premium': True})
 
 # post request
 content = client.post('https://webhook.site/403e44ce-5835-4ce9-a648-188a51d9395d', headers={'Content-Type': 'application/x-www-form-urlencoded'}, data={'field1': 'data1'})
 
 # put request
 content = client.put('https://webhook.site/403e44ce-5835-4ce9-a648-188a51d9395d', headers={'Content-Type': 'application/json'}, data={'field1': 'data1'})
-
 ```
 
 The `content` variable will contain the scraped page.
 
 If you want to get the `Response` object instead of the content you can use `make_request`.
 
 ```
-
 response = client.make_request(url='https://webhook.site/403e44ce-5835-4ce9-a648-188a51d9395d', headers={'Content-Type': 'application/json'}, data={'field1': 'data1'})
 # response will be <Response [200]>
 ```
 
 ## Exception
 
 ```
-
 from scraperapi_sdk import ScraperAPIClient
 from scraperapi_sdk.exceptions import ScraperAPIException
 
 client = ScraperAPIClient(
     api_key=api_key,
 )
 try:
@@ -57,15 +54,14 @@
 ### Amazon Endpoints
 #### Amazon Product Page API
 
 This method will retrieve product data from an Amazon product page and transform it into usable JSON.
 
 ```
 result = client.amazon.product("<ASIN>")
-
 result = client.amazon.product("<ASIN>", country="us", tld="com")
 ```
 
 Read more in docs: [Amazon Product Page API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/amazon-product-page-api)
 
 #### Amazon Search API
 
@@ -89,23 +85,59 @@
 
 #### Amazon Reviews API 
 This method will retrieve reviews for a specified product from an Amazon reviews page and transform it into usable JSON.
 
 ```
 result = client.amazon.review("<ASIN>")
 result = client.amazon.offers("<ASIN>", country="us", tld="com")
-
 ```
 Read more in docs: [Amazon Reviews API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/amazon-reviews-api)
 
 #### Amazon Prices API 
 
 This method will retrieve product prices for the given ASINs and transform it into usable JSON.
 
 ```
 result = client.amazon.prices(['<ASIN1>'])
 result = client.amazon.prices(['<ASIN1>', '<ASIN2>'])
 result = client.amazon.prices(['<ASIN1>', '<ASIN2>'], country="us", tld="com")
-
 ```
 Read more in docs: [Amazon Prices API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/amazon-prices-api)
 
+
+### Google API
+#### Google SERP API
+This method will retrieve product data from an Google search result page and transform it into usable JSON.
+
+```
+result = client.google.search('free hosting')
+result = client.google.search('free hosting', country="us", tld="com")
+```
+Read more in docs: [Google SERP API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/google-serp-api)
+#### Google News API
+This method will retrieve news data from an Google news result page and transform it into usable JSON.
+```
+result = client.google.news('tornado')
+result = client.google.news('tornado', country="us", tld="com")
+```
+Read more in docs: [Google News API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/google-news-api)
+
+#### Google Jobs API
+
+This method will retrieve jobs data from an Google jobs result page and transform it into usable JSON.
+
+```
+result = client.google.jobs('Senior Software Developer')
+result = client.google.jobs('Senior Software Developer', country="us", tld="com")
+```
+Read more in docs: [Google Jobs API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/google-jobs-api)
+
+#### Google Shopping API
+This method will retrieve shopping data from an Google shopping result page and transform it into usable JSON.
+```
+result = client.google.shopping('macbook air')
+result = client.google.shopping('macbook air', country="us", tld="com")
+```
+
+Read more in docs: [Google Shopping API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/google-shopping-api)
+
+
```

### Comparing `scraperapi_sdk-1.1.0/pyproject.toml` & `scraperapi_sdk-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scraperapi-sdk"
-version = "1.1.0"
+version = "1.2.0"
 description = "ScraperAPI Python SDK"
 authors = ["ScraperAPI"]
 readme = "README.md"
 
 [project]
 requires-python = ">= 3.8"
```

### Comparing `scraperapi_sdk-1.1.0/scraperapi_sdk/_client.py` & `scraperapi_sdk-1.2.0/scraperapi_sdk/_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
         :param api_key: ScraperAPI api_key
         :param api_endpoint: ScraperAPI endpoint
         """
         self.api_key = api_key
         self._api_endpoint = api_endpoint
         self.amazon = Amazon(client=self)
+        self.google = Google(client=self)
 
     def _get_headers(self, headers=None):
         if headers is None:
             headers = {}
         return headers
 
     def _get_params(self, params=None):
@@ -122,13 +123,47 @@
             params=dict(asin=asin, country=country, tld=tld),
         )
         return response.json()
 
     def prices(self, asins: list | tuple, country=None, tld=None):
         if type(asins) not in (list, tuple):
             raise ValueError("asins must be a list or tuple")
-        asins_string = ','.join(asins)
+        asins_string = ",".join(asins)
         response = self.client.make_request(
             endpoint=f"structured/amazon/prices?asins={asins_string}",
             params=dict(country=country, tld=tld),
         )
         return response.json()
+
+
+class Google:
+    def __init__(self, client):
+        super().__init__()
+        self.client = client
+
+    def search(self, query, country=None, tld=None):
+        response = self.client.make_request(
+            endpoint="structured/google/search",
+            params=dict(query=query, country=country, tld=tld),
+        )
+        return response.json()
+
+    def news(self, query, country=None, tld=None):
+        response = self.client.make_request(
+            endpoint="structured/google/news",
+            params=dict(query=query, country=country, tld=tld),
+        )
+        return response.json()
+
+    def jobs(self, query, country=None, tld=None):
+        response = self.client.make_request(
+            endpoint="structured/google/jobs",
+            params=dict(query=query, country=country, tld=tld),
+        )
+        return response.json()
+
+    def shopping(self, query, country=None, tld=None):
+        response = self.client.make_request(
+            endpoint="structured/google/shopping",
+            params=dict(query=query, country=country, tld=tld),
+        )
+        return response.json()
```

### Comparing `scraperapi_sdk-1.1.0/PKG-INFO` & `scraperapi_sdk-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scraperapi-sdk
-Version: 1.1.0
+Version: 1.2.0
 Summary: ScraperAPI Python SDK
 Author: ScraperAPI
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -33,31 +33,28 @@
 content = client.get('https://amazon.com/', params={'premium': True})
 
 # post request
 content = client.post('https://webhook.site/403e44ce-5835-4ce9-a648-188a51d9395d', headers={'Content-Type': 'application/x-www-form-urlencoded'}, data={'field1': 'data1'})
 
 # put request
 content = client.put('https://webhook.site/403e44ce-5835-4ce9-a648-188a51d9395d', headers={'Content-Type': 'application/json'}, data={'field1': 'data1'})
-
 ```
 
 The `content` variable will contain the scraped page.
 
 If you want to get the `Response` object instead of the content you can use `make_request`.
 
 ```
-
 response = client.make_request(url='https://webhook.site/403e44ce-5835-4ce9-a648-188a51d9395d', headers={'Content-Type': 'application/json'}, data={'field1': 'data1'})
 # response will be <Response [200]>
 ```
 
 ## Exception
 
 ```
-
 from scraperapi_sdk import ScraperAPIClient
 from scraperapi_sdk.exceptions import ScraperAPIException
 
 client = ScraperAPIClient(
     api_key=api_key,
 )
 try:
@@ -72,15 +69,14 @@
 ### Amazon Endpoints
 #### Amazon Product Page API
 
 This method will retrieve product data from an Amazon product page and transform it into usable JSON.
 
 ```
 result = client.amazon.product("<ASIN>")
-
 result = client.amazon.product("<ASIN>", country="us", tld="com")
 ```
 
 Read more in docs: [Amazon Product Page API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/amazon-product-page-api)
 
 #### Amazon Search API
 
@@ -104,24 +100,60 @@
 
 #### Amazon Reviews API 
 This method will retrieve reviews for a specified product from an Amazon reviews page and transform it into usable JSON.
 
 ```
 result = client.amazon.review("<ASIN>")
 result = client.amazon.offers("<ASIN>", country="us", tld="com")
-
 ```
 Read more in docs: [Amazon Reviews API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/amazon-reviews-api)
 
 #### Amazon Prices API 
 
 This method will retrieve product prices for the given ASINs and transform it into usable JSON.
 
 ```
 result = client.amazon.prices(['<ASIN1>'])
 result = client.amazon.prices(['<ASIN1>', '<ASIN2>'])
 result = client.amazon.prices(['<ASIN1>', '<ASIN2>'], country="us", tld="com")
-
 ```
 Read more in docs: [Amazon Prices API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/amazon-prices-api)
 
 
+### Google API
+#### Google SERP API
+This method will retrieve product data from an Google search result page and transform it into usable JSON.
+
+```
+result = client.google.search('free hosting')
+result = client.google.search('free hosting', country="us", tld="com")
+```
+Read more in docs: [Google SERP API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/google-serp-api)
+#### Google News API
+This method will retrieve news data from an Google news result page and transform it into usable JSON.
+```
+result = client.google.news('tornado')
+result = client.google.news('tornado', country="us", tld="com")
+```
+Read more in docs: [Google News API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/google-news-api)
+
+#### Google Jobs API
+
+This method will retrieve jobs data from an Google jobs result page and transform it into usable JSON.
+
+```
+result = client.google.jobs('Senior Software Developer')
+result = client.google.jobs('Senior Software Developer', country="us", tld="com")
+```
+Read more in docs: [Google Jobs API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/google-jobs-api)
+
+#### Google Shopping API
+This method will retrieve shopping data from an Google shopping result page and transform it into usable JSON.
+```
+result = client.google.shopping('macbook air')
+result = client.google.shopping('macbook air', country="us", tld="com")
+```
+
+Read more in docs: [Google Shopping API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/google-shopping-api)
+
+
+
```

