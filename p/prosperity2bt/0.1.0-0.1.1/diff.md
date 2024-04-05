# Comparing `tmp/prosperity2bt-0.1.0.tar.gz` & `tmp/prosperity2bt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.1.0.tar", last modified: Fri Apr  5 21:10:03 2024, max compression
+gzip compressed data, was "prosperity2bt-0.1.1.tar", last modified: Fri Apr  5 21:20:24 2024, max compression
```

## Comparing `prosperity2bt-0.1.0.tar` & `prosperity2bt-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:10:03.210351 prosperity2bt-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-05 21:10:03.210351 prosperity2bt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:10:03.206351 prosperity2bt-0.1.0/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:10:03.210351 prosperity2bt-0.1.0/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:10:03.210351 prosperity2bt-0.1.0/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-05 21:09:59.000000 prosperity2bt-0.1.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:10:03.210351 prosperity2bt-0.1.0/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-05 21:10:03.000000 prosperity2bt-0.1.0/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 21:10:03.000000 prosperity2bt-0.1.0/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:10:03.000000 prosperity2bt-0.1.0/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 21:10:03.000000 prosperity2bt-0.1.0/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 21:10:03.000000 prosperity2bt-0.1.0/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 21:10:03.000000 prosperity2bt-0.1.0/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-05 21:10:01.000000 prosperity2bt-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:10:03.210351 prosperity2bt-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.522469 prosperity2bt-0.1.1/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-05 21:20:20.000000 prosperity2bt-0.1.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 21:20:24.000000 prosperity2bt-0.1.1/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-05 21:20:22.000000 prosperity2bt-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:20:24.526469 prosperity2bt-0.1.1/setup.cfg
```

### Comparing `prosperity2bt-0.1.0/LICENSE` & `prosperity2bt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.0/PKG-INFO` & `prosperity2bt-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,16 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsonpickle
 
 # IMC Prosperity 2 Backtester
 
-[![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)  
+[![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
 
 This repository contains a backtester [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. The output it generates closely matches the format of the output generated by the official submission environment and is therefore compatible with my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (assuming your code contains the visualizer's required prerequisites as explained on the visualizer's homepage).
 
 ## Usage
 
 Basic usage:
 ```sh
```

### Comparing `prosperity2bt-0.1.0/README.md` & `prosperity2bt-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # IMC Prosperity 2 Backtester
 
-[![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)  
+[![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
 
 This repository contains a backtester [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. The output it generates closely matches the format of the output generated by the official submission environment and is therefore compatible with my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (assuming your code contains the visualizer's required prerequisites as explained on the visualizer's homepage).
 
 ## Usage
 
 Basic usage:
 ```sh
```

### Comparing `prosperity2bt-0.1.0/prosperity2bt/core.py` & `prosperity2bt-0.1.1/prosperity2bt/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,16 +212,16 @@
     listings = {product: {
         "symbol": product,
         "product": product,
         "denomination": 1,
     } for product in tradable_products}
 
     own_positions = defaultdict(int)
-    own_trades = {}
-    market_trades = {}
+    own_trades = defaultdict(list)
+    market_trades = defaultdict(list)
 
     profit_loss_by_product = defaultdict(float)
 
     for timestamp in sorted(prices_by_timestamp.keys()):
         order_depths = {}
         for product in tradable_products:
             row = prices_by_timestamp[timestamp][product]
```

### Comparing `prosperity2bt-0.1.0/prosperity2bt/data.py` & `prosperity2bt-0.1.1/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.0/prosperity2bt/datamodel.py` & `prosperity2bt-0.1.1/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.0/prosperity2bt/main.py` & `prosperity2bt-0.1.1/prosperity2bt/main.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.1.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.1.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.0/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.1.1/prosperity2bt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,16 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsonpickle
 
 # IMC Prosperity 2 Backtester
 
-[![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)  
+[![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
 
 This repository contains a backtester [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. The output it generates closely matches the format of the output generated by the official submission environment and is therefore compatible with my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (assuming your code contains the visualizer's required prerequisites as explained on the visualizer's homepage).
 
 ## Usage
 
 Basic usage:
 ```sh
```

### Comparing `prosperity2bt-0.1.0/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.1.1/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.0/pyproject.toml` & `prosperity2bt-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

