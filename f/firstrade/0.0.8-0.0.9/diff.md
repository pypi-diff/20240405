# Comparing `tmp/firstrade-0.0.8.tar.gz` & `tmp/firstrade-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firstrade-0.0.8.tar", last modified: Mon Nov  6 15:12:57 2023, max compression
+gzip compressed data, was "firstrade-0.0.9.tar", last modified: Mon Nov  6 15:53:53 2023, max compression
```

## Comparing `firstrade-0.0.8.tar` & `firstrade-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:12:57.538850 firstrade-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-11-06 15:12:44.000000 firstrade-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2023-11-06 15:12:57.538850 firstrade-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-11-06 15:12:44.000000 firstrade-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:12:57.538850 firstrade-0.0.8/firstrade/
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2023-11-06 15:12:44.000000 firstrade-0.0.8/firstrade/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2023-11-06 15:12:44.000000 firstrade-0.0.8/firstrade/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-11-06 15:12:44.000000 firstrade-0.0.8/firstrade/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-11-06 15:12:44.000000 firstrade-0.0.8/firstrade/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:12:57.538850 firstrade-0.0.8/firstrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2023-11-06 15:12:57.000000 firstrade-0.0.8/firstrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-11-06 15:12:57.000000 firstrade-0.0.8/firstrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 15:12:57.000000 firstrade-0.0.8/firstrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-06 15:12:57.000000 firstrade-0.0.8/firstrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-06 15:12:57.000000 firstrade-0.0.8/firstrade.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 15:12:57.538850 firstrade-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-11-06 15:12:44.000000 firstrade-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:53:53.894771 firstrade-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-11-06 15:53:41.000000 firstrade-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2023-11-06 15:53:53.894771 firstrade-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2023-11-06 15:53:41.000000 firstrade-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:53:53.890771 firstrade-0.0.9/firstrade/
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2023-11-06 15:53:41.000000 firstrade-0.0.9/firstrade/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2023-11-06 15:53:41.000000 firstrade-0.0.9/firstrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2023-11-06 15:53:41.000000 firstrade-0.0.9/firstrade/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-11-06 15:53:41.000000 firstrade-0.0.9/firstrade/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:53:53.894771 firstrade-0.0.9/firstrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2023-11-06 15:53:53.000000 firstrade-0.0.9/firstrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-11-06 15:53:53.000000 firstrade-0.0.9/firstrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 15:53:53.000000 firstrade-0.0.9/firstrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-06 15:53:53.000000 firstrade-0.0.9/firstrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-06 15:53:53.000000 firstrade-0.0.9/firstrade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 15:53:53.894771 firstrade-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-11-06 15:53:41.000000 firstrade-0.0.9/setup.py
```

### Comparing `firstrade-0.0.8/LICENSE` & `firstrade-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firstrade-0.0.8/PKG-INFO` & `firstrade-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: firstrade
-Version: 0.0.8
+Version: 0.0.9
 Summary: An unofficial API for Firstrade
 Home-page: https://github.com/MaxxRK/firstrade-api
-Download-URL: https://github.com/MaxxRK/firstrade-api/archive/refs/tags/008.tar.gz
+Download-URL: https://github.com/MaxxRK/firstrade-api/archive/refs/tags/009.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: FIRSTRADE,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
@@ -91,15 +91,16 @@
 # Create an order object.   
 ft_order = order.Order(ft_ss)
 
 # Place order and print out order confirmation data.
 ft_order.place_order(
     ft_accounts.account_numbers[0],
     symbol='INTC',
-    order_type=order.PriceType.MARKET,
+    price_type=order.PriceType.MARKET,
+    order_type=order.OrderType.BUY,
     quantity=1,
     duration=order.Duration.DAY,
     dry_run=True
 )
 
 # Print Order data Dict
 print(ft_order.order_confirmation)
```

### Comparing `firstrade-0.0.8/README.md` & `firstrade-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 # Create an order object.   
 ft_order = order.Order(ft_ss)
 
 # Place order and print out order confirmation data.
 ft_order.place_order(
     ft_accounts.account_numbers[0],
     symbol='INTC',
-    order_type=order.PriceType.MARKET,
+    price_type=order.PriceType.MARKET,
+    order_type=order.OrderType.BUY,
     quantity=1,
     duration=order.Duration.DAY,
     dry_run=True
 )
 
 # Print Order data Dict
 print(ft_order.order_confirmation)
```

### Comparing `firstrade-0.0.8/firstrade/account.py` & `firstrade-0.0.9/firstrade/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import pickle
 import re
 import os
+from time import sleep
 from bs4 import BeautifulSoup
 from firstrade import urls
 
 
 class FTSession:
     """
     Class creating a session for Firstrade.
@@ -158,14 +159,15 @@
                 url=urls.get_xml(), 
                 headers=urls.session_headers(), 
                 cookies=self.session.cookies,
                 data=data,
                 ).text, 'xml')
             balance = account_soup.find('total_account_value').text
             self.account_balances.append(balance)
+            sleep(2)
             data = { 'req': 'get_status'}
             account_status = self.session.post(
                 url=urls.status(),
                 headers=urls.session_headers(),
                 cookies=self.session.cookies,
                 data=data
             ).json()
```

### Comparing `firstrade-0.0.8/firstrade/order.py` & `firstrade-0.0.9/firstrade/order.py`

 * *Files identical despite different names*

### Comparing `firstrade-0.0.8/firstrade/symbols.py` & `firstrade-0.0.9/firstrade/symbols.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,10 +43,12 @@
         self.last = float(quote.find('last').text)
         self.change = float(quote.find('change').text)
         if quote.find('high').text == 'N/A':
             self.high = None
         else:
             self.high = float(quote.find('high').text)
         if quote.find('low').text == 'N/A':
-            self.low = None
+            self.low = 'None'
+        else:
+            self.low = float(quote.find('low').text)
         self.volume = quote.find('vol').text
         self.company_name = quote.find('companyname').text
```

### Comparing `firstrade-0.0.8/firstrade/urls.py` & `firstrade-0.0.9/firstrade/urls.py`

 * *Files identical despite different names*

### Comparing `firstrade-0.0.8/firstrade.egg-info/PKG-INFO` & `firstrade-0.0.9/firstrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: firstrade
-Version: 0.0.8
+Version: 0.0.9
 Summary: An unofficial API for Firstrade
 Home-page: https://github.com/MaxxRK/firstrade-api
-Download-URL: https://github.com/MaxxRK/firstrade-api/archive/refs/tags/008.tar.gz
+Download-URL: https://github.com/MaxxRK/firstrade-api/archive/refs/tags/009.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: FIRSTRADE,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
@@ -91,15 +91,16 @@
 # Create an order object.   
 ft_order = order.Order(ft_ss)
 
 # Place order and print out order confirmation data.
 ft_order.place_order(
     ft_accounts.account_numbers[0],
     symbol='INTC',
-    order_type=order.PriceType.MARKET,
+    price_type=order.PriceType.MARKET,
+    order_type=order.OrderType.BUY,
     quantity=1,
     duration=order.Duration.DAY,
     dry_run=True
 )
 
 # Print Order data Dict
 print(ft_order.order_confirmation)
```

### Comparing `firstrade-0.0.8/setup.py` & `firstrade-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="firstrade",
-    version="0.0.8",
+    version="0.0.9",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Firstrade",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url='https://github.com/MaxxRK/firstrade-api',
-    download_url='https://github.com/MaxxRK/firstrade-api/archive/refs/tags/008.tar.gz',
+    download_url='https://github.com/MaxxRK/firstrade-api/archive/refs/tags/009.tar.gz',
     keywords=['FIRSTRADE', 'API'],
     install_requires=['requests', 'beautifulsoup4', 'lxml'],
     packages=['firstrade'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Internet :: WWW/HTTP :: Session',
```

