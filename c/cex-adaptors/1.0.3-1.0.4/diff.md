# Comparing `tmp/cex-adaptors-1.0.3.tar.gz` & `tmp/cex-adaptors-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cex-adaptors-1.0.3.tar", last modified: Wed Mar 27 03:39:32 2024, max compression
+gzip compressed data, was "cex-adaptors-1.0.4.tar", last modified: Fri Apr  5 14:30:04 2024, max compression
```

## Comparing `cex-adaptors-1.0.3.tar` & `cex-adaptors-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-03-27 03:39:32.908109 cex-adaptors-1.0.3/
--rw-r--r--   0 davidding   (501) staff       (20)     8252 2024-03-27 03:39:32.907960 cex-adaptors-1.0.3/PKG-INFO
--rw-r--r--   0 davidding   (501) staff       (20)     8155 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/README.md
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-03-27 03:39:32.904286 cex-adaptors-1.0.3/cex_adaptors/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)     6090 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/binance.py
--rw-r--r--   0 davidding   (501) staff       (20)     6355 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/bitget.py
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/bitmex.py
--rw-r--r--   0 davidding   (501) staff       (20)     8292 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/bybit.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-03-27 03:39:32.906432 cex-adaptors-1.0.3/cex_adaptors/exchanges/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)     2945 2024-03-27 02:40:55.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/auth.py
--rw-r--r--   0 davidding   (501) staff       (20)     2098 2024-03-27 02:40:55.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/base.py
--rw-r--r--   0 davidding   (501) staff       (20)     3677 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/binance.py
--rw-r--r--   0 davidding   (501) staff       (20)     2034 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/bitget.py
--rw-r--r--   0 davidding   (501) staff       (20)      129 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/bitmex.py
--rw-r--r--   0 davidding   (501) staff       (20)     2873 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/bybit.py
--rw-r--r--   0 davidding   (501) staff       (20)     2572 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/gateio.py
--rw-r--r--   0 davidding   (501) staff       (20)     3032 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/htx.py
--rw-r--r--   0 davidding   (501) staff       (20)     2284 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/kucoin.py
--rw-r--r--   0 davidding   (501) staff       (20)     6356 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/okx.py
--rw-r--r--   0 davidding   (501) staff       (20)      336 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/exchanges/woo.py
--rw-r--r--   0 davidding   (501) staff       (20)     5101 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/gateio.py
--rw-r--r--   0 davidding   (501) staff       (20)     5986 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/htx.py
--rw-r--r--   0 davidding   (501) staff       (20)     4562 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/kucoin.py
--rw-r--r--   0 davidding   (501) staff       (20)    15548 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/okx.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-03-27 03:39:32.907790 cex-adaptors-1.0.3/cex_adaptors/parsers/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)     4181 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/base.py
--rw-r--r--   0 davidding   (501) staff       (20)     8532 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/binance.py
--rw-r--r--   0 davidding   (501) staff       (20)     8230 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/bitget.py
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/bitmex.py
--rw-r--r--   0 davidding   (501) staff       (20)    10000 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/bybit.py
--rw-r--r--   0 davidding   (501) staff       (20)    10967 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/gateio.py
--rw-r--r--   0 davidding   (501) staff       (20)    15223 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/htx.py
--rw-r--r--   0 davidding   (501) staff       (20)     9404 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/kucoin.py
--rw-r--r--   0 davidding   (501) staff       (20)    16864 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/okx.py
--rw-r--r--   0 davidding   (501) staff       (20)     2464 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/parsers/woo.py
--rw-r--r--   0 davidding   (501) staff       (20)     1532 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/cex_adaptors/utils.py
--rw-r--r--   0 davidding   (501) staff       (20)      441 2024-03-27 03:36:43.000000 cex-adaptors-1.0.3/cex_adaptors/woo.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-03-27 03:39:32.904929 cex-adaptors-1.0.3/cex_adaptors.egg-info/
--rw-r--r--   0 davidding   (501) staff       (20)     8252 2024-03-27 03:39:32.000000 cex-adaptors-1.0.3/cex_adaptors.egg-info/PKG-INFO
--rw-r--r--   0 davidding   (501) staff       (20)     1174 2024-03-27 03:39:32.000000 cex-adaptors-1.0.3/cex_adaptors.egg-info/SOURCES.txt
--rw-r--r--   0 davidding   (501) staff       (20)        1 2024-03-27 03:39:32.000000 cex-adaptors-1.0.3/cex_adaptors.egg-info/dependency_links.txt
--rw-r--r--   0 davidding   (501) staff       (20)      384 2024-03-27 03:39:32.000000 cex-adaptors-1.0.3/cex_adaptors.egg-info/requires.txt
--rw-r--r--   0 davidding   (501) staff       (20)       13 2024-03-27 03:39:32.000000 cex-adaptors-1.0.3/cex_adaptors.egg-info/top_level.txt
--rw-r--r--   0 davidding   (501) staff       (20)      614 2024-03-21 09:58:13.000000 cex-adaptors-1.0.3/pyproject.toml
--rw-r--r--   0 davidding   (501) staff       (20)       38 2024-03-27 03:39:32.908152 cex-adaptors-1.0.3/setup.cfg
--rw-r--r--   0 davidding   (501) staff       (20)      380 2024-03-27 03:37:12.000000 cex-adaptors-1.0.3/setup.py
+drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.675141 cex-adaptors-1.0.4/
+-rw-r--r--   0 davidding   (501) staff       (20)     8252 2024-04-05 14:30:04.674839 cex-adaptors-1.0.4/PKG-INFO
+-rw-r--r--   0 davidding   (501) staff       (20)     8155 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/README.md
+drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.667493 cex-adaptors-1.0.4/cex_adaptors/
+-rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/__init__.py
+-rw-r--r--   0 davidding   (501) staff       (20)     8394 2024-04-05 14:26:43.000000 cex-adaptors-1.0.4/cex_adaptors/binance.py
+-rw-r--r--   0 davidding   (501) staff       (20)     6355 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/bitget.py
+-rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/bitmex.py
+-rw-r--r--   0 davidding   (501) staff       (20)     8292 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/bybit.py
+drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.671153 cex-adaptors-1.0.4/cex_adaptors/exchanges/
+-rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/__init__.py
+-rw-r--r--   0 davidding   (501) staff       (20)     2945 2024-03-27 02:40:55.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/auth.py
+-rw-r--r--   0 davidding   (501) staff       (20)     2098 2024-03-27 02:40:55.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/base.py
+-rw-r--r--   0 davidding   (501) staff       (20)     4656 2024-04-05 14:26:43.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/binance.py
+-rw-r--r--   0 davidding   (501) staff       (20)     2034 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/bitget.py
+-rw-r--r--   0 davidding   (501) staff       (20)      129 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/bitmex.py
+-rw-r--r--   0 davidding   (501) staff       (20)     2873 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/bybit.py
+-rw-r--r--   0 davidding   (501) staff       (20)     2572 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/gateio.py
+-rw-r--r--   0 davidding   (501) staff       (20)     3032 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/htx.py
+-rw-r--r--   0 davidding   (501) staff       (20)     2284 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/kucoin.py
+-rw-r--r--   0 davidding   (501) staff       (20)     6356 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/okx.py
+-rw-r--r--   0 davidding   (501) staff       (20)      336 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/woo.py
+-rw-r--r--   0 davidding   (501) staff       (20)     5101 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/gateio.py
+-rw-r--r--   0 davidding   (501) staff       (20)     5986 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/htx.py
+-rw-r--r--   0 davidding   (501) staff       (20)     4562 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/kucoin.py
+-rw-r--r--   0 davidding   (501) staff       (20)    15548 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/okx.py
+drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.674452 cex-adaptors-1.0.4/cex_adaptors/parsers/
+-rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/__init__.py
+-rw-r--r--   0 davidding   (501) staff       (20)     4457 2024-04-05 14:26:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/base.py
+-rw-r--r--   0 davidding   (501) staff       (20)     9183 2024-04-05 14:26:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/binance.py
+-rw-r--r--   0 davidding   (501) staff       (20)     8230 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/bitget.py
+-rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/bitmex.py
+-rw-r--r--   0 davidding   (501) staff       (20)    10000 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/bybit.py
+-rw-r--r--   0 davidding   (501) staff       (20)    10967 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/gateio.py
+-rw-r--r--   0 davidding   (501) staff       (20)    15223 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/htx.py
+-rw-r--r--   0 davidding   (501) staff       (20)     9404 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/kucoin.py
+-rw-r--r--   0 davidding   (501) staff       (20)    16864 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/okx.py
+-rw-r--r--   0 davidding   (501) staff       (20)     2464 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/woo.py
+-rw-r--r--   0 davidding   (501) staff       (20)     1532 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/utils.py
+-rw-r--r--   0 davidding   (501) staff       (20)      441 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/woo.py
+drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.668383 cex-adaptors-1.0.4/cex_adaptors.egg-info/
+-rw-r--r--   0 davidding   (501) staff       (20)     8252 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/PKG-INFO
+-rw-r--r--   0 davidding   (501) staff       (20)     1174 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/SOURCES.txt
+-rw-r--r--   0 davidding   (501) staff       (20)        1 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/dependency_links.txt
+-rw-r--r--   0 davidding   (501) staff       (20)      384 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/requires.txt
+-rw-r--r--   0 davidding   (501) staff       (20)       13 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/top_level.txt
+-rw-r--r--   0 davidding   (501) staff       (20)      614 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/pyproject.toml
+-rw-r--r--   0 davidding   (501) staff       (20)       38 2024-04-05 14:30:04.675200 cex-adaptors-1.0.4/setup.cfg
+-rw-r--r--   0 davidding   (501) staff       (20)      380 2024-04-05 14:27:29.000000 cex-adaptors-1.0.4/setup.py
```

### Comparing `cex-adaptors-1.0.3/PKG-INFO` & `cex-adaptors-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cex-adaptors
-Version: 1.0.3
+Version: 1.0.4
 Description-Content-Type: text/markdown
 
 # cex_services
 This package is designed for interacting with many crypto centralized exchanges. Currently only support **public API endpoints** in Version `1.0.x`. Will add private API endpoints in version `2.0.x`.
 
 ## Getting started
 use ```pip install cex-adaptor``` to install the package.
```

### Comparing `cex-adaptors-1.0.3/README.md` & `cex-adaptors-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/binance.py` & `cex-adaptors-1.0.4/cex_adaptors/htx.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,154 +1,145 @@
-import tracemalloc
-from typing import Literal, Optional
+from .exchanges.htx import HtxFutures, HtxUnified
+from .parsers.htx import HtxParser
+from .utils import query_dict, sort_dict
 
-from .exchanges.binance import BinanceInverse, BinanceLinear, BinanceSpot
-from .parsers.binance import BinanceParser
-from .utils import sort_dict
-
-tracemalloc.start()
-
-
-class Binance(object):
-    name = "binance"
-
-    def __init__(self, api_key: str = None, api_secret: str = None):
-        self.spot = BinanceSpot(api_key=api_key, api_secret=api_secret)
-        self.linear = BinanceLinear()
-        self.inverse = BinanceInverse()
-        self.parser = BinanceParser()
 
+class Htx(object):
+    name = "htx"
+
+    def __init__(self):
+        self.spot = HtxUnified()
+        self.futures = HtxFutures()
+        self.parser = HtxParser()
         self.exchange_info = {}
 
     async def close(self):
         await self.spot.close()
-        await self.linear.close()
-        await self.inverse.close()
+        await self.futures.close()
 
     @classmethod
     async def create(cls):
         instance = cls()
         instance.exchange_info = await instance.get_exchange_info()
         return instance
 
-    async def sync_exchange_info(self) -> None:
-        self.exchange_info = await self.get_exchange_info()
-
-    async def get_exchange_info(self, market_type: Optional[Literal["spot", "margin", "futures", "perp"]] = None):
+    async def get_exchange_info(self, market_type: str = None):
         spot = self.parser.parse_exchange_info(
             await self.spot._get_exchange_info(), self.parser.spot_exchange_info_parser
         )
         linear = self.parser.parse_exchange_info(
-            await self.linear._get_exchange_info(), self.parser.futures_exchange_info_parser("linear")
+            await self.futures._get_linear_contract_info(), self.parser.linear_exchange_info_parser
         )
-        inverse = self.parser.parse_exchange_info(
-            await self.inverse._get_exchange_info(), self.parser.futures_exchange_info_parser("inverse")
+        inverse_futures = self.parser.parse_exchange_info(
+            await self.futures._get_inverse_futures_info(), self.parser.inverse_futures_exchange_info_parser
+        )
+        inverse_perp = self.parser.parse_exchange_info(
+            await self.futures._get_inverse_perp_info(), self.parser.inverse_perp_exchange_info_parser
         )
-        result = {**spot, **linear, **inverse}
-        return result if not market_type else self.parser.query_dict(result, {f"is_{market_type}": True})
-
-    async def get_ticker(self, instrument_id: str):
-        _symbol = self.exchange_info[instrument_id]["raw_data"]["symbol"]
-        info = self.exchange_info[instrument_id]
-        market_type = self.parser.get_market_type(info)
 
-        if market_type == "spot":
-            return {instrument_id: self.parser.parse_ticker(await self.spot._get_ticker(_symbol), info)}
-        elif market_type == "linear":
-            return {instrument_id: self.parser.parse_ticker(await self.linear._get_ticker(_symbol), info)}
-        elif market_type == "inverse":
-            return {instrument_id: self.parser.parse_ticker(await self.inverse._get_ticker(_symbol), info)}
+        return {**spot, **linear, **inverse_futures, **inverse_perp}
 
-    async def get_tickers(self, market_type: Optional[Literal["spot", "margin", "futures", "perp"]] = None) -> dict:
-        results = {}
-
-        tickers = [(self.spot, "spot"), (self.linear, "linear"), (self.inverse, "inverse")]
+    async def get_tickers(self, market_type: str = None):
+        # get_all tickers then filter by market_type
+        if market_type:
+            if market_type == "spot":
+                return self.parser.parse_tickers(await self.spot._get_tickers(), self.exchange_info, "spot")
+            else:
+                linear = self.parser.parse_tickers(
+                    await self.futures._get_linear_contract_tickers(), self.exchange_info, "linear"
+                )
+                inverse_perp = self.parser.parse_tickers(
+                    await self.futures._get_inverse_perp_tickers(), self.exchange_info, "inverse_perp"
+                )
 
-        for exchange, _market_type in tickers:
-            parsed_tickers = self.parser.parse_tickers(await exchange._get_tickers(), _market_type, self.exchange_info)
-            results.update(parsed_tickers)
+                inverse_futures = self.parser.parse_tickers(
+                    await self.futures._get_inverse_futures_tickers(), self.exchange_info, "inverse_futures"
+                )
+                results = {**linear, **inverse_perp, **inverse_futures}
 
-        if market_type:
-            ids = list(self.parser.query_dict(self.exchange_info, {f"is_{market_type}": True}).keys())
-            return self.parser.query_dict_by_keys(results, ids)
+                instrument_id = list(query_dict(self.exchange_info, f"is_{market_type} == True").keys())
+                return {k: v for k, v in results.items() if k in instrument_id}
         else:
-            return results
+            spot = self.parser.parse_tickers(await self.spot._get_tickers(), self.exchange_info, "spot")
 
-    async def get_klines(self, instrument_id: str, interval: str, start: int = None, end: int = None, num: int = 500):
-        _symbol = self.exchange_info[instrument_id]["raw_data"]["symbol"]
-        _interval = self.parser.get_interval(interval)
-        limit = 1000
-        market_type = self.parser.get_market_type(self.exchange_info[instrument_id])
+            linear = self.parser.parse_tickers(
+                await self.futures._get_linear_contract_tickers(), self.exchange_info, "linear"
+            )
+            inverse_perp = self.parser.parse_tickers(
+                await self.futures._get_inverse_perp_tickers(), self.exchange_info, "inverse_perp"
+            )
+            inverse_futures = self.parser.parse_tickers(
+                await self.futures._get_inverse_futures_tickers(), self.exchange_info, "inverse_futures"
+            )
+            return {**spot, **linear, **inverse_perp, **inverse_futures}
+
+    async def get_klines(self, instrument_id: str, interval: str, start: int = None, end: int = None, num: int = None):
+        if instrument_id not in self.exchange_info:
+            raise ValueError(f"{instrument_id} not in exchange_info")
 
-        params = {
-            "symbol": _symbol,
-            "interval": _interval,
-            "limit": limit,
+        info = self.exchange_info[instrument_id]
+        market_type = self.parser.get_market_type(info)
+        _interval = self.parser.get_interval(interval, market_type)
+
+        symbol_map = {
+            "spot": "sc",
+            "linear": "contract_code",
+            "inverse_futures": "symbol",
+            "inverse_perp": "contract_code",
         }
 
         method_map = {
             "spot": self.spot._get_klines,
-            "linear": self.linear._get_klines,
-            "inverse": self.inverse._get_klines,
+            "linear": self.futures._get_linear_contract_klines,
+            "inverse_futures": self.futures._get_inverse_futures_klines,
+            "inverse_perp": self.futures._get_inverse_perp_klines,
         }
 
-        query_end = None
+        limit_map = {
+            "spot": 2000,
+            "linear": 2000,
+            "inverse_futures": 2000,
+            "inverse_perp": 2000,
+        }
 
+        params = {
+            "symbol": info["raw_data"][symbol_map[market_type]]
+            if market_type != "inverse_futures"
+            else self.parser.parse_inverse_futures_symbol(info["raw_data"]),
+            "period": _interval,
+            "limit": limit_map[market_type],
+        }
         results = {}
-        if start and end:
+        query_end = None
+        if start and end and market_type != "spot":
             query_end = end
             while True:
-                params["endTime"] = query_end
-                klines = self.parser.parse_klines(await method_map[market_type](**params), market_type)
-                if not klines:
+                params["end"] = str(query_end)[:10]
+                result = self.parser.parse_klines(await method_map[market_type](**params), market_type, info)
+                results.update(result)
+
+                temp_end = str(sorted(list(result.keys()))[0])[:10]
+                if len(result) < limit_map[market_type] or temp_end == query_end:
                     break
 
-                results.update(klines)
-                query_end = sorted(list(klines.keys()))[0]
-                if len(klines) < limit or query_end <= start:
+                query_end = temp_end  # get the earliest timestamp in 10 digits
+                if query_end <= start:
                     break
-                continue
-            return sort_dict({k: v for k, v in results.items() if end >= k >= start}, ascending=True)
+            return {k: v for k, v in results.items() if start <= int(k) <= end}
 
         elif num:
             while True:
-                params.update({"endTime": query_end} if query_end else {})
-                klines = self.parser.parse_klines(
-                    await method_map[market_type](**params),
-                    market_type,
-                )
-                results.update(klines)
-                if len(klines) < limit or len(results) >= num:
+                params.update({"end": query_end} if query_end else {})
+                result = self.parser.parse_klines(await method_map[market_type](**params), market_type, info)
+                results.update(result)
+
+                temp_end = str(sorted(list(result.keys()))[0])[:10]
+                if len(result) < limit_map[market_type] or temp_end == query_end:
                     break
-                query_end = sorted(list(klines.keys()))[0]
-                continue
 
+                query_end = temp_end  # get the earliest timestamp in 10 digits
+                if len(results) >= num:
+                    break
             return sort_dict(results, ascending=True, num=num)
 
-    # Private function
-    async def get_spot_account_info(self) -> dict:
-        return self.parser.parse_spot_account_info(await self.spot._get_account_info())
-
-    async def get_margin_account_info(self) -> dict:
-        return self.parser.parse_margin_account_info(await self.spot._get_margin_account_info())
-
-    async def get_margin_balance(self, currency: str = None) -> dict:
-        return self.parser.parse_margin_balance(await self.spot._get_margin_account_info(), currency=currency)
-
-    async def get_margin_account_value(self, in_currency: str = None):
-        info = await self.get_margin_account_info()
-
-        net_btc_value = self.parser.parse_str(info["raw_data"]["totalNetAssetOfBtc"], float)
-
-        instrument_id = "BTC/USDT:USDT"
-        ticker = await self.get_ticker(instrument_id)
-        btc_price = ticker[instrument_id]["last_price"]
-
-        if in_currency:
-            instrument_id = f"{in_currency}/USDT:USDT"
-            ccy_ticker = await self.get_ticker(instrument_id)
-            ccy_price = ccy_ticker[instrument_id]["last_price"]
-
-            return net_btc_value * btc_price / ccy_price
-
         else:
-            return net_btc_value * btc_price
+            raise ValueError("(start, end) or num must be provided")
```

### Comparing `cex-adaptors-1.0.3/cex_adaptors/bitget.py` & `cex-adaptors-1.0.4/cex_adaptors/bitget.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/bybit.py` & `cex-adaptors-1.0.4/cex_adaptors/bybit.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/exchanges/auth.py` & `cex-adaptors-1.0.4/cex_adaptors/exchanges/auth.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/exchanges/base.py` & `cex-adaptors-1.0.4/cex_adaptors/exchanges/base.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/exchanges/binance.py` & `cex-adaptors-1.0.4/cex_adaptors/exchanges/kucoin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,67 @@
 from .base import BaseClient
 
 
-class BinanceSpot(BaseClient):
-    BASE_ENDPOINT = "https://api{}.binance.com"
-    name = "binance"
+class KucoinSpot(BaseClient):
+    BASE_ENDPOINT = "https://api.kucoin.com"
 
-    def __init__(self, api_key: str, api_secret: str, api_version: int = 3):
+    def __init__(self) -> None:
         super().__init__()
-        self.base_endpoint = self.BASE_ENDPOINT.format(api_version)
+        self.spot_base_endpoint = self.BASE_ENDPOINT
 
-        self.auth_data = {
-            "api_key": api_key,
-            "api_secret": api_secret,
-        }
+    async def _get_currency_list(self):
+        return await self._get(self.spot_base_endpoint + "/api/v3/currencies")
 
-    async def _get_exchange_info(self):
-        return await self._get(self.base_endpoint + "/api/v3/exchangeInfo")
-
-    async def _get_ticker(self, symbol: str):
-        return await self._get(self.base_endpoint + "/api/v3/ticker/24hr", params={"symbol": symbol})
+    async def _get_symbol_list(self):
+        return await self._get(self.spot_base_endpoint + "/api/v2/symbols")
 
     async def _get_tickers(self):
-        return await self._get(self.base_endpoint + "/api/v3/ticker/24hr")
-
-    async def _get_klines(
-        self,
-        symbol: str,
-        interval: str,
-        startTime: int = None,
-        endTime: int = None,
-        limit: int = 500,
-        timeZone: str = "0",
-    ):
-        params = {"symbol": symbol, "interval": interval, "limit": limit, "timeZone": timeZone}
-        if startTime:
-            params["startTime"] = startTime
-        if endTime:
-            params["endTime"] = endTime
-        return await self._get(self.base_endpoint + "/api/v3/klines", params=params)
-
-    # Private endpoint
-    async def _get_account_info(self):
-        return await self._get(self.base_endpoint + "/api/v3/account", auth_data=self.auth_data)
+        return await self._get(self.spot_base_endpoint + "/api/v1/market/allTickers")
 
-    async def _get_margin_account_info(self):
-        return await self._get(self.base_endpoint + "/sapi/v1/margin/account", auth_data=self.auth_data)
-
-
-class BinanceLinear(BaseClient):
-    BASE_ENDPOINT = "https://fapi.binance.com"
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.linear_base_endpoint = self.BASE_ENDPOINT
+    async def _get_ticker(self, symbol: str):
+        return await self._get(self.spot_base_endpoint + f" /api/v1/market/orderbook/level1?symbol={symbol}")
 
-    async def _get_exchange_info(self):
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/exchangeInfo")
+    async def _get_24hr_stats(self, symbol: str):
+        return await self._get(self.spot_base_endpoint + f"/api/v1/market/stats?symbol={symbol}")
 
-    async def _get_ticker(self, symbol: str):
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/ticker/24hr", params={"symbol": symbol})
+    async def _get_klines(self, symbol: str, type: str, start: int = None, end: int = None):
+        params = {
+            "symbol": symbol,
+            "type": type,
+        }
+        if start:
+            params["startAt"] = start
 
-    async def _get_tickers(self):
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/ticker/24hr")
+        if end:
+            params["endAt"] = end
 
-    async def _get_klines(
-        self, symbol: str, interval: str, startTime: int = None, endTime: int = None, limit: int = 500
-    ):
-        params = {"symbol": symbol, "interval": interval, "limit": limit}
-        if startTime:
-            params["startTime"] = startTime
-        if endTime:
-            params["endTime"] = endTime
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/klines", params=params)
+        return await self._get(self.spot_base_endpoint + "/api/v1/market/candles", params=params)
 
 
-class BinanceInverse(BaseClient):
-    BASE_ENDPOINT = "https://dapi.binance.com"
+class KucoinFutures(BaseClient):
+    BASE_ENDPOINT = "https://api-futures.kucoin.com"
 
     def __init__(self) -> None:
         super().__init__()
-        self.inverse_base_endpoint = self.BASE_ENDPOINT
+        self.futures_base_endpoint = self.BASE_ENDPOINT
 
-    async def _get_exchange_info(self):
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/exchangeInfo")
+    async def _get_symbol_list(self):
+        return await self._get(self.futures_base_endpoint + "/api/v1/contracts/active")
 
     async def _get_ticker(self, symbol: str):
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/ticker/24hr", params={"symbol": symbol})
+        return await self._get(self.futures_base_endpoint + f"/api/v1/ticker?symbol={symbol}")
 
-    async def _get_tickers(self):
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/ticker/24hr")
+    async def _get_contract_info(self, symbol: str):
+        return await self._get(self.futures_base_endpoint + f"/api/v1/contracts/{symbol}")
+
+    async def _get_klines(self, symbol: str, granularity: int, start: int = None, end: int = None):
+
+        params = {
+            "symbol": symbol,
+            "granularity": granularity,
+        }
+        if start:
+            params["from"] = start
+        if end:
+            params["to"] = end
 
-    async def _get_klines(
-        self, symbol: str, interval: str, startTime: int = None, endTime: int = None, limit: int = 500
-    ):
-        params = {"symbol": symbol, "interval": interval, "limit": limit}
-        if startTime:
-            params["startTime"] = startTime
-        if endTime:
-            params["endTime"] = endTime
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/klines", params=params)
+        return await self._get(self.futures_base_endpoint + "/api/v1/kline/query", params=params)
```

### Comparing `cex-adaptors-1.0.3/cex_adaptors/exchanges/bitget.py` & `cex-adaptors-1.0.4/cex_adaptors/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/exchanges/bybit.py` & `cex-adaptors-1.0.4/cex_adaptors/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/exchanges/gateio.py` & `cex-adaptors-1.0.4/cex_adaptors/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/exchanges/htx.py` & `cex-adaptors-1.0.4/cex_adaptors/exchanges/htx.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/exchanges/okx.py` & `cex-adaptors-1.0.4/cex_adaptors/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/gateio.py` & `cex-adaptors-1.0.4/cex_adaptors/gateio.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/kucoin.py` & `cex-adaptors-1.0.4/cex_adaptors/kucoin.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/okx.py` & `cex-adaptors-1.0.4/cex_adaptors/okx.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/base.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,24 @@
 
         multiplier = info["multiplier"]
         return f"{multiplier if multiplier != 1 and multiplier else ''}{instrument_id}"
 
     def parse_unified_symbol(self, base: str, quote: str) -> str:
         return f"{base}/{quote}"
 
+    def parse_unified_market_type(self, info: dict) -> str:
+        if info["is_spot"]:
+            return "spot"
+        elif info["is_futures"]:
+            return "futures"
+        elif info["is_perp"]:
+            return "perp"
+        else:
+            return "unknown"
+
     def parse_base_currency(self, base: str) -> str:
         for i in self.MULTIPLIER:
             if i in base:
                 return base.replace(i, "")
         return base
 
     def parse_multiplier(self, base: str) -> int:
```

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/binance.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/binance.py`

 * *Files 6% similar despite different names*

```diff
@@ -193,14 +193,31 @@
                 "available": self.parse_str(data["free"], float),
                 "raw_data": data,
             }
             currency = result["currency"]
             results[currency] = result
         return results if not query_currency else {query_currency: results[query_currency]}
 
+    def parse_history_funding_rate(self, response: dict, info: dict) -> list:
+        response = self.check_response(response)
+        datas = response["data"]
+
+        results = []
+        for data in datas:
+            result = {
+                "timestamp": self.parse_str(data["fundingTime"], int),
+                "instrument_id": self.parse_unified_id(info),
+                "market": self.parse_unified_market_type(info),
+                "funding_rate": self.parse_str(data["fundingRate"], float),
+                "realized_rate": None,
+                "raw_data": data,
+            }
+            results.append(result)
+        return results
+
     def get_symbol(self, info: dict) -> str:
         return f'{info["base"]}{info["quote"]}'
 
     def get_interval(self, interval: str) -> str:
         return interval
 
     def get_market_type(self, info: dict):
```

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/bitget.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/bitget.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/bybit.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/bybit.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/gateio.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/gateio.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/htx.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/htx.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/kucoin.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/kucoin.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/okx.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/okx.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/parsers/woo.py` & `cex-adaptors-1.0.4/cex_adaptors/parsers/woo.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors/utils.py` & `cex-adaptors-1.0.4/cex_adaptors/utils.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/cex_adaptors.egg-info/PKG-INFO` & `cex-adaptors-1.0.4/cex_adaptors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cex-adaptors
-Version: 1.0.3
+Version: 1.0.4
 Description-Content-Type: text/markdown
 
 # cex_services
 This package is designed for interacting with many crypto centralized exchanges. Currently only support **public API endpoints** in Version `1.0.x`. Will add private API endpoints in version `2.0.x`.
 
 ## Getting started
 use ```pip install cex-adaptor``` to install the package.
```

### Comparing `cex-adaptors-1.0.3/cex_adaptors.egg-info/SOURCES.txt` & `cex-adaptors-1.0.4/cex_adaptors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.3/pyproject.toml` & `cex-adaptors-1.0.4/pyproject.toml`

 * *Files identical despite different names*

