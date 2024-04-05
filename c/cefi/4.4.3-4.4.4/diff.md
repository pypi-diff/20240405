# Comparing `tmp/cefi-4.4.3.tar.gz` & `tmp/cefi-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.4.3.tar", max compression
+gzip compressed data, was "cefi-4.4.4.tar", max compression
```

## Comparing `cefi-4.4.3.tar` & `cefi-4.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-03-30 05:46:33.024253 cefi-4.4.3/LICENSE
--rw-r--r--   0        0        0     2661 2024-03-30 05:46:33.024253 cefi-4.4.3/README.md
--rw-r--r--   0        0        0       87 2024-03-30 05:47:04.312325 cefi-4.4.3/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/handler/__init__.py
--rw-r--r--   0        0        0     9048 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     4838 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     6972 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8055 2024-03-30 05:46:33.024253 cefi-4.4.3/cefi/main.py
--rw-r--r--   0        0        0     3722 2024-03-30 05:47:04.312325 cefi-4.4.3/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-05 17:33:56.688904 cefi-4.4.4/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-05 17:33:56.688904 cefi-4.4.4/README.md
+-rw-r--r--   0        0        0       87 2024-04-05 17:34:30.189050 cefi-4.4.4/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/handler/__init__.py
+-rw-r--r--   0        0        0     9053 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     4838 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     6972 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8055 2024-04-05 17:33:56.688904 cefi-4.4.4/cefi/main.py
+-rw-r--r--   0        0        0     3724 2024-04-05 17:34:30.189050 cefi-4.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.4/PKG-INFO
```

### Comparing `cefi-4.4.3/LICENSE` & `cefi-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.4.3/README.md` & `cefi-4.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.4.3/cefi/default_settings.toml` & `cefi-4.4.4/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.4.3/cefi/handler/capitalcom.py` & `cefi-4.4.4/cefi/handler/capitalcom.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
         Returns:
             int: The number of decimal places for the instrument.
         """
         instrument_info = self.client.single_market(instrument)
         decimals = instrument_info.get("snapshot", {}).get("decimalPlacesFactor", 0)
         logger.debug("Decimals {}", decimals)
-        return decimals
+        return int(decimals)
 
     async def execute_order(self, order_params):
         """
         Execute order
 
         Args:
             order_params (dict):
```

### Comparing `cefi-4.4.3/cefi/handler/ccxt.py` & `cefi-4.4.4/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.3/cefi/handler/client.py` & `cefi-4.4.4/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.3/cefi/handler/ctrader.py` & `cefi-4.4.4/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.3/cefi/handler/ib_sync.py` & `cefi-4.4.4/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.3/cefi/main.py` & `cefi-4.4.4/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.3/pyproject.toml` & `cefi-4.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.4.3"
+version = "4.4.4"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -140,27 +140,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.4.3/PKG-INFO` & `cefi-4.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.4.3
+Version: 4.4.4
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.4.3 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.4.4 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

