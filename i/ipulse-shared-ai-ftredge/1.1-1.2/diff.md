# Comparing `tmp/ipulse_shared_ai_ftredge-1.1.tar.gz` & `tmp/ipulse_shared_ai_ftredge-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipulse_shared_ai_ftredge-1.1.tar", last modified: Thu Apr  4 14:40:07 2024, max compression
+gzip compressed data, was "ipulse_shared_ai_ftredge-1.2.tar", last modified: Fri Apr  5 13:33:48 2024, max compression
```

## Comparing `ipulse_shared_ai_ftredge-1.1.tar` & `ipulse_shared_ai_ftredge-1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:07.436316 ipulse_shared_ai_ftredge-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-04 14:40:07.436316 ipulse_shared_ai_ftredge-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:40:07.436316 ipulse_shared_ai_ftredge-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:07.432316 ipulse_shared_ai_ftredge-1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:07.432316 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:07.436316 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/mlmodel_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/mlmodel_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/mlmodel_specification_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/po_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/po_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-04 14:39:58.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/po_series_abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:07.436316 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-04 14:40:07.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-04 14:40:07.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:40:07.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-04 14:40:07.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 14:40:07.000000 ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.271037 ipulse_shared_ai_ftredge-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 13:33:48.271037 ipulse_shared_ai_ftredge-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:33:48.271037 ipulse_shared_ai_ftredge-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.267037 ipulse_shared_ai_ftredge-1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.267037 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.267037 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/mlmodel_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/mlmodel_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/mlmodel_specification_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-05 13:33:22.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_series_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:33:48.267037 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:33:48.000000 ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/top_level.txt
```

### Comparing `ipulse_shared_ai_ftredge-1.1/LICENCE` & `ipulse_shared_ai_ftredge-1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.1/setup.py` & `ipulse_shared_ai_ftredge-1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ipulse_shared_ai_ftredge',
-    version='1.01',
+    version='1.2',
     package_dir={'': 'src'},  # Specify the source directory
     packages=find_packages(where='src'),  # Look for packages in 'src'
     install_requires=[
         # List your dependencies here
         'pydantic[email]~=2.5',
         'python-dateutil~=2.8',
         'pytest~=7.1',
```

### Comparing `ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/common_utils.py` & `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/common_utils.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/mlmodel_specification_registry.py` & `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/mlmodel_specification_registry.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/po_abstract.py` & `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_abstract.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/po_series.py` & `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_series.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from pydantic import BaseModel,validator, model_validator, Field, field_serializer
+from pydantic import BaseModel,validator, model_validator, Field   #, field_serializer, AwareDatetime
 from typing import Optional, Dict, Any, List, Union
 from datetime import datetime, timezone
 import pandas as pd
 import uuid
 import re
 import pytz
 #  I want you to add methods which will allow for adding, updating or deleting  series to series_registry, with keys being interval to which series relates to such as "5m" , "10m" etc. . When adding a series an origin must be added to series_origin_sources , 
 
 CLASS_ORIGIN_AUTHOR="Russlan Ramdowar;russlan@ftredge.com"
 CLASS_ORGIN_DATE=datetime(2024, 3, 26, 18, 00)
 
 CLASS_VERSION = 2.01
 CLASS_REVISION_AUTHOR="Russlan Ramdowar;russlan@ftredge.com"
-IMPORTANT_MODIFICATIONS_LOG={datetime(2024, 3, 26, 18, 00):"Modified fields in a way to not require POSeriesAbstract"}
+LAST_MODIFICATIONS=["Fixed creat and udpate datestimes ","Modified fields in a way to not require POSeriesAbstract"]
 
 MAXIMUM_SERIES_CHUNK_SIZE=2000
 class POSeries(BaseModel):
    
     name: str #apple
     @validator('name')
     def validate_name(cls, value):
@@ -122,24 +122,17 @@
     uid:Optional[str] = None #stocks_apple_5min_c_202403310905_202403311705_yahoo"
     
     @model_validator(mode='after') # This validator now has priority 1 and will run before add_uid
     def calculate_derived_attributes(self):
         if self.series:  # Checks if the series dictionary is not empty
             
             datetime_keys = [datetime.fromisoformat(k) for k in self.series.keys()]
-            # datetime_keys = [datetime.fromisoformat(k).replace(tzinfo=pytz.UTC) for k in self.series.keys()] 
-            # Now, datetime_keys contains all the keys as datetime objects
             self.start_datetime = min(datetime_keys)
             self.end_datetime = max(datetime_keys)
             self.total_intervals_count = len(self.series)
-            
-            # datetime_keys = list(self.series.keys())
-            # self.start_datetime = min(datetime_keys)
-            # self.end_datetime = max(datetime_keys)
-            # self.total_intervals_count = len(self.series)
         else:
             # Handle case where series is empty
             self.start_datetime = None
             self.end_datetime = None
             self.total_intervals_count = 0
         return self
     
@@ -162,14 +155,17 @@
     @staticmethod
     def from_dict_series_chunk(series_dict: Dict[str, float], **kwargs) -> "POSeries":
         kwargs['series'] = series_dict
         return POSeries(**kwargs)
 
     class Config:
         arbitrary_types_allowed = True
+        # json_encoders = {
+        #     datetime: lambda v: v.isoformat(),
+        # }
 
 def convert_pandasseries_to_dictseries(series: pd.Series) -> Dict[str, float]:
     return {index.isoformat(): value for index, value in series.items()}
 
 def convert_dictseries_to_pandasseries(dict_series: Dict[str, float]) -> pd.Series:
     series = pd.Series({pd.to_datetime(iso_date): value for iso_date, value in dict_series.items()})
```

### Comparing `ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge/models/po_series_abstract.py` & `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge/models/po_series_abstract.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_ai_ftredge-1.1/src/ipulse_shared_ai_ftredge.egg-info/SOURCES.txt` & `ipulse_shared_ai_ftredge-1.2/src/ipulse_shared_ai_ftredge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

