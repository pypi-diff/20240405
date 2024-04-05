# Comparing `tmp/MarketTime-1.1.0.tar.gz` & `tmp/MarketTime-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarketTime-1.1.0.tar", last modified: Sun Mar 31 12:48:13 2024, max compression
+gzip compressed data, was "MarketTime-1.1.2.tar", last modified: Fri Apr  5 08:18:20 2024, max compression
```

## Comparing `MarketTime-1.1.0.tar` & `MarketTime-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-31 12:48:13.904769 MarketTime-1.1.0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    35149 2024-02-27 11:30:54.000000 MarketTime-1.1.0/LICENSE
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-31 12:48:13.900769 MarketTime-1.1.0/MarketTime/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       96 2024-03-31 10:44:46.000000 MarketTime-1.1.0/MarketTime/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6937 2024-03-31 12:44:44.000000 MarketTime-1.1.0/MarketTime/future_market_time.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2026 2024-03-31 09:43:58.000000 MarketTime-1.1.0/MarketTime/market_time.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2301 2024-02-27 13:46:57.000000 MarketTime-1.1.0/MarketTime/stock_market_time.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-31 12:48:13.900769 MarketTime-1.1.0/MarketTime.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1409 2024-03-31 12:48:13.000000 MarketTime-1.1.0/MarketTime.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      309 2024-03-31 12:48:13.000000 MarketTime-1.1.0/MarketTime.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-03-31 12:48:13.000000 MarketTime-1.1.0/MarketTime.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        9 2024-03-31 12:48:13.000000 MarketTime-1.1.0/MarketTime.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       11 2024-03-31 12:48:13.000000 MarketTime-1.1.0/MarketTime.egg-info/top_level.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1409 2024-03-31 12:48:13.900769 MarketTime-1.1.0/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1075 2024-02-27 14:09:14.000000 MarketTime-1.1.0/README.md
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2024-03-31 12:48:13.904769 MarketTime-1.1.0/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1014 2024-03-31 12:47:01.000000 MarketTime-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:18:20.877856 MarketTime-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 08:18:13.000000 MarketTime-1.1.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:18:20.877856 MarketTime-1.1.2/MarketTime/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 08:18:13.000000 MarketTime-1.1.2/MarketTime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-05 08:18:13.000000 MarketTime-1.1.2/MarketTime/future_market_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-05 08:18:13.000000 MarketTime-1.1.2/MarketTime/market_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-05 08:18:13.000000 MarketTime-1.1.2/MarketTime/stock_market_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:18:20.877856 MarketTime-1.1.2/MarketTime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 08:18:20.000000 MarketTime-1.1.2/MarketTime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-05 08:18:20.877856 MarketTime-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-05 08:18:13.000000 MarketTime-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:18:20.877856 MarketTime-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-05 08:18:13.000000 MarketTime-1.1.2/setup.py
```

### Comparing `MarketTime-1.1.0/LICENSE` & `MarketTime-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MarketTime-1.1.0/MarketTime/future_market_time.py` & `MarketTime-1.1.2/MarketTime/future_market_time.py`

 * *Files identical despite different names*

### Comparing `MarketTime-1.1.0/MarketTime/market_time.py` & `MarketTime-1.1.2/MarketTime/market_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class MarketTime:
     close_date_set = set()
 
     @staticmethod
     def init_close_date_set(close_date_list: Sequence[str] = None):
-        """Init the market close date set.\n
+        """Init the market close date set.
         The date string format should be 'YYYY-mm-dd'"""
         if close_date_list is None:
             return
         for date_str in close_date_list:
             date_date = datetime.strptime(date_str, "%Y-%m-%d").date()
             MarketTime.close_date_set.add(date_date)
```

### Comparing `MarketTime-1.1.0/MarketTime/stock_market_time.py` & `MarketTime-1.1.2/MarketTime/stock_market_time.py`

 * *Files identical despite different names*

### Comparing `MarketTime-1.1.0/MarketTime.egg-info/PKG-INFO` & `MarketTime-1.1.2/MarketTime.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: MarketTime
-Version: 1.1.0
+Version: 1.1.2
 Summary: This is a tool to check the time in the market
 Home-page: https://github.com/Liaou3/MarketTime
 Download-URL: 
 Author: VincentLiao
 Author-email: vincent932693@gmail.com
 License: GPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datetime
 
 # MarketTime
 ## Description
 This is a tool to help you to check the market time.
 
 For example:
  - Check if the time is in market open time
```

### Comparing `MarketTime-1.1.0/PKG-INFO` & `MarketTime-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: MarketTime
-Version: 1.1.0
+Version: 1.1.2
 Summary: This is a tool to check the time in the market
 Home-page: https://github.com/Liaou3/MarketTime
 Download-URL: 
 Author: VincentLiao
 Author-email: vincent932693@gmail.com
 License: GPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datetime
 
 # MarketTime
 ## Description
 This is a tool to help you to check the market time.
 
 For example:
  - Check if the time is in market open time
```

### Comparing `MarketTime-1.1.0/README.md` & `MarketTime-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `MarketTime-1.1.0/setup.py` & `MarketTime-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 PACKAGE_NAME = "MarketTime"
 AUTHOR = "VincentLiao"
 AUTHOR_EMAIL = "vincent932693@gmail.com"
 URL = "https://github.com/Liaou3/MarketTime"
 DOWNLOAD_URL = ""
 
 LICENSE = "GPLv3"
-VERSION = "1.1.0"
+VERSION = "1.1.2"
 DESCRIPTION = "This is a tool to check the time in the market"
 LONG_DESCRIPTION = (HERE/"README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 INSTALL_REQUIRES = ["datetime"]
 EXTRAS_REQUIRE = {}
 CLASSIFIERS = []
 PYTHON_REQUIRES = ">=3.10"
```

