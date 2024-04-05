# Comparing `tmp/deribit_wrapper-0.2.7.tar.gz` & `tmp/deribit_wrapper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deribit_wrapper-0.2.7.tar", last modified: Thu Apr  4 14:32:20 2024, max compression
+gzip compressed data, was "deribit_wrapper-0.3.0.tar", last modified: Fri Apr  5 18:05:37 2024, max compression
```

## Comparing `deribit_wrapper-0.2.7.tar` & `deribit_wrapper-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/deribit_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/market_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.657101 deribit_wrapper-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-05 18:05:37.657101 deribit_wrapper-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.653102 deribit_wrapper-0.3.0/deribit_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.653102 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.653102 deribit_wrapper-0.3.0/dev_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/config_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/debug_account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/debug_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/utilities_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:05:37.657101 deribit_wrapper-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.657101 deribit_wrapper-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/tests/test_base.py
```

### Comparing `deribit_wrapper-0.2.7/LICENSE` & `deribit_wrapper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.7/PKG-INFO` & `deribit_wrapper-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit_wrapper
-Version: 0.2.7
+Version: 0.3.0
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.2.7/README.md` & `deribit_wrapper-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.7/deribit_wrapper/base.py` & `deribit_wrapper-0.3.0/deribit_wrapper/base.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.7/deribit_wrapper/core.py` & `deribit_wrapper-0.3.0/deribit_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.7/deribit_wrapper/market_data.py` & `deribit_wrapper-0.3.0/deribit_wrapper/market_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,17 @@
     def get_currencies(self) -> list[dict]:
         ret = self._request(self.__GET_CURRENCY_URI, {})
         return ret
 
     @property
     def currencies(self) -> list[str]:
         df = pd.DataFrame(self.get_currencies())
-        currency = list(df['currency'])
-        return currency
+        currency_list = list(df['currency'])
+        sorted_currency_list = sorted(currency_list)
+        return sorted_currency_list
 
     def get_complete_market_book(self) -> pd.DataFrame:
         uri = self.__GET_BOOK_BY_CURRENCY_URI
         params = {'currency': ''}
         currencies = self.currencies
         ret = pd.DataFrame()
         for currency in currencies:
```

### Comparing `deribit_wrapper-0.2.7/deribit_wrapper/trading.py` & `deribit_wrapper-0.3.0/deribit_wrapper/trading.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.7/deribit_wrapper/utilities.py` & `deribit_wrapper-0.3.0/deribit_wrapper/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from __future__ import absolute_import, annotations
 
 from datetime import datetime
-from typing import List, Literal, Tuple, Union
+from typing import List, Literal, Tuple, Union, get_args
 
 import numpy as np
 import pandas as pd
 
+ParamsType = dict[str, Union[str, int, float]]
+
 MarketOrderType = Tuple[str, float]
 LimitOrderType = Tuple[str, float, float]
 OrdersType = List[Union[MarketOrderType, LimitOrderType]]
 DatetimeType = Union[datetime, str, float]
 StrikeType = Union[str, float]
 
 ScopeType = Literal['read', 'read_write', 'none']
+SCOPES = list(get_args(ScopeType))
+
+MarginModelType = Literal['cross_pm', 'cross_sm', 'segregated_pm', 'segregated_sm']
+MARGIN_MODELS = list(get_args(MarginModelType))
 
 DEFAULT_START = '2000-01-01'
 DEFAULT_END = 'now'
 
 
 def from_ts_to_dt(timestamp: int | float, milliseconds: bool = True) -> datetime:
     ts = timestamp * 1e9
@@ -29,7 +35,13 @@
 
 def from_dt_to_ts(date: str | datetime, milliseconds: bool = True) -> int:
     dt = pd.to_datetime(date)
     ts = int(datetime.timestamp(dt))
     if milliseconds:
         ts *= int(1e3)
     return ts
+
+
+def seconds_to_hms(seconds: int) -> str:
+    h, r = divmod(seconds, 3600)
+    m, s = divmod(r, 60)
+    return f'{h}h {m:02d}m {s:02d}s'
```

### Comparing `deribit_wrapper-0.2.7/deribit_wrapper.egg-info/PKG-INFO` & `deribit_wrapper-0.3.0/deribit_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit-wrapper
-Version: 0.2.7
+Version: 0.3.0
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.2.7/setup.py` & `deribit_wrapper-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='deribit_wrapper',
-    version='0.2.7',
+    version='0.3.0',
     packages=find_packages(),
     description='A Python wrapper for seamless integration with Deribit\'s trading API, offering easy access to '
                 'market data, account management, and trading operations.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
```

### Comparing `deribit_wrapper-0.2.7/tests/test_authentication.py` & `deribit_wrapper-0.3.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.7/tests/test_base.py` & `deribit_wrapper-0.3.0/tests/test_base.py`

 * *Files identical despite different names*

