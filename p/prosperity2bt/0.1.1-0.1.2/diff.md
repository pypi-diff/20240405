# Comparing `tmp/prosperity2bt-0.1.1.tar.gz` & `tmp/prosperity2bt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.1.1.tar", last modified: Fri Apr  5 21:20:24 2024, max compression
+gzip compressed data, was "prosperity2bt-0.1.2.tar", last modified: Fri Apr  5 21:52:43 2024, max compression
```

## Comparing `prosperity2bt-0.1.1.tar` & `prosperity2bt-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.522469 prosperity2bt-0.1.1/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-05 21:20:22.000000 prosperity2bt-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:52:43.203278 prosperity2bt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-05 21:52:43.203278 prosperity2bt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:52:43.199278 prosperity2bt-0.1.2/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:52:43.199278 prosperity2bt-0.1.2/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:52:43.203278 prosperity2bt-0.1.2/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-05 21:52:38.000000 prosperity2bt-0.1.2/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:52:43.203278 prosperity2bt-0.1.2/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-05 21:52:43.000000 prosperity2bt-0.1.2/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 21:52:43.000000 prosperity2bt-0.1.2/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:52:43.000000 prosperity2bt-0.1.2/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 21:52:43.000000 prosperity2bt-0.1.2/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 21:52:43.000000 prosperity2bt-0.1.2/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 21:52:43.000000 prosperity2bt-0.1.2/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-05 21:52:40.000000 prosperity2bt-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:52:43.203278 prosperity2bt-0.1.2/setup.cfg
```

### Comparing `prosperity2bt-0.1.1/LICENSE` & `prosperity2bt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.1/PKG-INFO` & `prosperity2bt-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,14 +88,14 @@
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
 ```
 
 ## Order Matching
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for $10 but there is non-zero ask volume at $9, your order is (possibly partially) filled at $9. Similarly, if you place a sell order for $10 but there is non-zero bid volume at $11, your order is (possibly partially) filled at $11.
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prosperity2bt-0.1.1/README.md` & `prosperity2bt-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,14 @@
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
 ```
 
 ## Order Matching
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for $10 but there is non-zero ask volume at $9, your order is (possibly partially) filled at $9. Similarly, if you place a sell order for $10 but there is non-zero bid volume at $11, your order is (possibly partially) filled at $11.
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prosperity2bt-0.1.1/prosperity2bt/core.py` & `prosperity2bt-0.1.2/prosperity2bt/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,14 +123,16 @@
     profit_loss_by_product: dict[Symbol, float],
 ) -> list[Trade]:
     order_depth = order_depths[order.symbol]
     if order.quantity > 0:
         return process_buy_order(timestamp, order, order_depth, own_trades, own_positions, profit_loss_by_product)
     elif order.quantity < 0:
         return process_sell_order(timestamp, order, order_depth, own_trades, own_positions, profit_loss_by_product)
+    else:
+        return []
 
 def trade_to_dict(trade: Trade) -> dict[str, Any]:
     return {
         "timestamp": trade.timestamp,
         "buyer": trade.buyer,
         "seller": trade.seller,
         "symbol": trade.symbol,
```

### Comparing `prosperity2bt-0.1.1/prosperity2bt/data.py` & `prosperity2bt-0.1.2/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.1/prosperity2bt/datamodel.py` & `prosperity2bt-0.1.2/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.1/prosperity2bt/main.py` & `prosperity2bt-0.1.2/prosperity2bt/main.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.1.2/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.1.2/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.1/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.1.2/prosperity2bt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,14 +88,14 @@
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
 ```
 
 ## Order Matching
 
-Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for $10 but there is non-zero ask volume at $9, your order is (possibly partially) filled at $9. Similarly, if you place a sell order for $10 but there is non-zero bid volume at $11, your order is (possibly partially) filled at $11.
+Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prosperity2bt-0.1.1/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.1.2/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.1/pyproject.toml` & `prosperity2bt-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

