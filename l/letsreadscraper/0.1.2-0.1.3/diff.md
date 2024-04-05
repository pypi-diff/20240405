# Comparing `tmp/letsreadscraper-0.1.2.tar.gz` & `tmp/letsreadscraper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsreadscraper-0.1.2.tar", max compression
+gzip compressed data, was "letsreadscraper-0.1.3.tar", max compression
```

## Comparing `letsreadscraper-0.1.2.tar` & `letsreadscraper-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      123 2024-04-04 18:58:20.368834 letsreadscraper-0.1.2/letsreadscraper/__init__.py
--rw-r--r--   0        0        0     1607 2024-04-04 19:19:54.425323 letsreadscraper-0.1.2/letsreadscraper/scraper.py
--rw-r--r--   0        0        0      950 2024-04-04 18:22:12.550219 letsreadscraper-0.1.2/letsreadscraper/utilities.py
--rw-r--r--   0        0        0      736 2024-04-04 19:15:32.376765 letsreadscraper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 18:15:34.197043 letsreadscraper-0.1.2/README.md
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 letsreadscraper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-04-04 18:58:20.368834 letsreadscraper-0.1.3/letsreadscraper/__init__.py
+-rw-r--r--   0        0        0     1602 2024-04-04 19:41:24.879446 letsreadscraper-0.1.3/letsreadscraper/scraper.py
+-rw-r--r--   0        0        0      950 2024-04-04 18:22:12.550219 letsreadscraper-0.1.3/letsreadscraper/utilities.py
+-rw-r--r--   0        0        0      736 2024-04-04 19:42:20.351363 letsreadscraper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 18:15:34.197043 letsreadscraper-0.1.3/README.md
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 letsreadscraper-0.1.3/PKG-INFO
```

### Comparing `letsreadscraper-0.1.2/letsreadscraper/scraper.py` & `letsreadscraper-0.1.3/letsreadscraper/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,25 @@
     response = requests.get('https://letsreadasia.org/api/language')
     results = [item for item in response.json()]
 
     df = pd.json_normalize(results).sort_values(by=['country'])
     df['name'] = df['name'].str.lower()
     return df
 
-def scrape_by_language(language, limit):
+def scrape_by_language(language, limit=10):
     """_summary_
 
     Args:
         language (str): Enter the language of the books that you are interested to gather information about
         limit (int, optional): Enter number of books to gather information
 
     Returns:
         DataFrame: Returns a dataframe with book details based on the parameters provided
     """    
-    df_language = scrape_language_details(limit=10)
+    df_language = scrape_language_details()
     language_value = language
     lId_value = lrs.utilities.xlookup(lookup_value=language_value, lookup_array=df_language["name"], return_array=df_language["id"])
     limit_value = int(limit)
 
     params = {
     'searchText': '',
     'lId': lId_value,
```

### Comparing `letsreadscraper-0.1.2/letsreadscraper/utilities.py` & `letsreadscraper-0.1.3/letsreadscraper/utilities.py`

 * *Files identical despite different names*

### Comparing `letsreadscraper-0.1.2/pyproject.toml` & `letsreadscraper-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "letsreadscraper"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python package to scrape Let's Read Website"
 authors = ["Mohit Shrestha <contact@mohitshrestha.com.np>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "letsreadscraper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `letsreadscraper-0.1.2/PKG-INFO` & `letsreadscraper-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsreadscraper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package to scrape Let's Read Website
 License: MIT
 Author: Mohit Shrestha
 Author-email: contact@mohitshrestha.com.np
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

