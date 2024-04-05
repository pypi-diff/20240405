# Comparing `tmp/tutto_api_client-1.0.5.tar.gz` & `tmp/tutto_api_client-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutto_api_client-1.0.5.tar", max compression
+gzip compressed data, was "tutto_api_client-1.0.6.tar", max compression
```

## Comparing `tutto_api_client-1.0.5.tar` & `tutto_api_client-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1252 2024-04-04 18:35:35.726526 tutto_api_client-1.0.5/README.md
--rw-r--r--   0        0        0      318 2024-04-04 18:35:35.726526 tutto_api_client-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      290 2024-04-04 18:35:35.726526 tutto_api_client-1.0.5/tutto_api_client/__init__.py
--rw-r--r--   0        0        0     3597 2024-04-04 18:35:35.726526 tutto_api_client-1.0.5/tutto_api_client/core/endpoints_factory.py
--rw-r--r--   0        0        0     2295 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/helpers/http.py
--rw-r--r--   0        0        0    10319 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/main.py
--rw-r--r--   0        0        0     3541 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/models/authorization.py
--rw-r--r--   0        0        0    14644 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/models/endpoints.py
--rw-r--r--   0        0        0     2502 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/models/entities.py
--rw-r--r--   0        0        0     2113 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/utils/filter_clean_utils.py
--rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 tutto_api_client-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1252 2024-04-04 20:45:39.190287 tutto_api_client-1.0.6/README.md
+-rw-r--r--   0        0        0      318 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      290 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/tutto_api_client/__init__.py
+-rw-r--r--   0        0        0     3579 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/tutto_api_client/core/endpoints_factory.py
+-rw-r--r--   0        0        0     2295 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/tutto_api_client/helpers/http.py
+-rw-r--r--   0        0        0    10319 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/tutto_api_client/main.py
+-rw-r--r--   0        0        0     3541 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/tutto_api_client/models/authorization.py
+-rw-r--r--   0        0        0    14644 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/tutto_api_client/models/endpoints.py
+-rw-r--r--   0        0        0     2502 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/tutto_api_client/models/entities.py
+-rw-r--r--   0        0        0     2053 2024-04-04 20:45:39.194287 tutto_api_client-1.0.6/tutto_api_client/utils/filter_clean_utils.py
+-rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 tutto_api_client-1.0.6/PKG-INFO
```

### Comparing `tutto_api_client-1.0.5/README.md` & `tutto_api_client-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.5/tutto_api_client/core/endpoints_factory.py` & `tutto_api_client-1.0.6/tutto_api_client/core/endpoints_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,14 @@
         if name in self.__setters:
             self.__services[name] = value
         else:
             raise NameError(f"Name '{name}' not accepted in set_services() method")
 
 
 class _EndpointFactory:
-    @staticmethod
     def create_endpoint(
         base_url: str, endpoint: str, authorization: Authorization, **kwargs
     ) -> Endpoint:
         """Factory method to create an endpoint object"""
         # Fill the services catalog with the required services
         http_client = HTTPRequest(base_url=base_url)
         catalog_instance = _EndpointCatalog()
```

### Comparing `tutto_api_client-1.0.5/tutto_api_client/helpers/http.py` & `tutto_api_client-1.0.6/tutto_api_client/helpers/http.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.5/tutto_api_client/main.py` & `tutto_api_client-1.0.6/tutto_api_client/main.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.5/tutto_api_client/models/authorization.py` & `tutto_api_client-1.0.6/tutto_api_client/models/authorization.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.5/tutto_api_client/models/endpoints.py` & `tutto_api_client-1.0.6/tutto_api_client/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.5/tutto_api_client/models/entities.py` & `tutto_api_client-1.0.6/tutto_api_client/models/entities.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.5/tutto_api_client/utils/filter_clean_utils.py` & `tutto_api_client-1.0.6/tutto_api_client/utils/filter_clean_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from typing import List, Literal, Any
 from datetime import date
 from pydoc import locate
 from operator import itemgetter
 
 
-@staticmethod
 def split_str_to_list(
     values: str,
     split_by: str = ",",
     dtype: Literal["int", "str", "float", "dict", "list"] = "str",
 ) -> List[Any]:
     """
     Splits a string into a list of values of the specified data type.
@@ -28,42 +27,39 @@
     data_type = locate(dtype)
     if isinstance(values, str):
         return [data_type(element) for element in values.split(split_by)]
     else:
         return values
 
 
-@staticmethod
 def filter_dict_with_falsy_values(dictionary: dict) -> dict:
     """
     Filters a dictionary by removing key-value pairs where the value is falsy.
 
     Args:
         dictionary (dict): The dictionary to filter.
 
     Returns:
         dict: The filtered dictionary.
     """
     return dict(filter(itemgetter(1), dictionary.items()))
 
 
-@staticmethod
 def convert_dict_dates_to_isoformat(dictionary: dict) -> dict:
     """
     Converts date values in a dictionary to ISO 8601 format.
     Nested dictionaries and lists are supported.
 
     Args:
         dictionary (dict): The dictionary to convert.
 
     Returns:
         dict: The dictionary with date values converted to ISO 8601 format.
     """
 
-    @staticmethod
     def convert_value(value):
         if isinstance(value, date):
             return value.isoformat()
         elif isinstance(value, dict):
             return convert_dict_dates_to_isoformat(value)
         elif isinstance(value, list):
             return [convert_value(item) for item in value]
```

### Comparing `tutto_api_client-1.0.5/PKG-INFO` & `tutto_api_client-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutto-api-client
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: rapha-pereira
 Author-email: raphaelpgomes1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

