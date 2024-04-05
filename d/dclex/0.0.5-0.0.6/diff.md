# Comparing `tmp/dclex-0.0.5.tar.gz` & `tmp/dclex-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dclex-0.0.5.tar", last modified: Tue Mar  5 12:03:40 2024, max compression
+gzip compressed data, was "dclex-0.0.6.tar", last modified: Fri Apr  5 14:10:04 2024, max compression
```

## Comparing `dclex-0.0.5.tar` & `dclex-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-03-05 12:03:40.614270 dclex-0.0.5/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     8250 2024-01-31 17:39:20.000000 dclex-0.0.5/LICENSE
--rw-r--r--   0 clouds    (1001) clouds    (1001)     9779 2024-03-05 12:03:40.614270 dclex-0.0.5/PKG-INFO
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      385 2024-02-20 12:18:10.000000 dclex-0.0.5/README.md
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      739 2024-03-05 11:51:46.000000 dclex-0.0.5/pyproject.toml
--rw-rw-r--   0 clouds    (1001) clouds    (1001)       38 2024-03-05 12:03:40.614270 dclex-0.0.5/setup.cfg
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-03-05 12:03:40.606270 dclex-0.0.5/src/
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-03-05 12:03:40.610270 dclex-0.0.5/src/dclex/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      208 2024-03-04 19:14:07.000000 dclex-0.0.5/src/dclex/__init__.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    11377 2024-03-04 19:14:07.000000 dclex-0.0.5/src/dclex/dclex.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    12712 2024-03-04 16:55:10.000000 dclex-0.0.5/src/dclex/dclex_client.py
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-03-05 12:03:40.610270 dclex-0.0.5/src/dclex/resources/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    19297 2024-02-02 17:33:59.000000 dclex-0.0.5/src/dclex/resources/digital_identity_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    15662 2024-02-02 17:33:59.000000 dclex-0.0.5/src/dclex/resources/factory_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6200 2024-02-02 17:33:59.000000 dclex-0.0.5/src/dclex/resources/usdc_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     9883 2024-02-02 17:33:59.000000 dclex-0.0.5/src/dclex/resources/vault_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1188 2024-03-01 16:20:01.000000 dclex-0.0.5/src/dclex/settings.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     2285 2024-03-01 16:30:00.000000 dclex-0.0.5/src/dclex/types.py
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-03-05 12:03:40.610270 dclex-0.0.5/src/dclex.egg-info/
--rw-r--r--   0 clouds    (1001) clouds    (1001)     9779 2024-03-05 12:03:40.000000 dclex-0.0.5/src/dclex.egg-info/PKG-INFO
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      580 2024-03-05 12:03:40.000000 dclex-0.0.5/src/dclex.egg-info/SOURCES.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)        1 2024-03-05 12:03:40.000000 dclex-0.0.5/src/dclex.egg-info/dependency_links.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)       60 2024-03-05 12:03:40.000000 dclex-0.0.5/src/dclex.egg-info/requires.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)        6 2024-03-05 12:03:40.000000 dclex-0.0.5/src/dclex.egg-info/top_level.txt
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-03-05 12:03:40.610270 dclex-0.0.5/tests/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1167 2024-03-04 19:14:07.000000 dclex-0.0.5/tests/test_account.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6062 2024-03-04 19:14:07.000000 dclex-0.0.5/tests/test_orders.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1515 2024-03-04 19:14:07.000000 dclex-0.0.5/tests/test_stocks.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6753 2024-03-04 19:14:07.000000 dclex-0.0.5/tests/test_transfers.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.566264 dclex-0.0.6/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     8250 2024-01-31 17:39:20.000000 dclex-0.0.6/LICENSE
+-rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-04-05 14:10:04.566264 dclex-0.0.6/PKG-INFO
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      450 2024-04-05 14:00:22.000000 dclex-0.0.6/README.md
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      739 2024-04-05 14:05:35.000000 dclex-0.0.6/pyproject.toml
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)       38 2024-04-05 14:10:04.566264 dclex-0.0.6/setup.cfg
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.558265 dclex-0.0.6/src/
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.562265 dclex-0.0.6/src/dclex/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      208 2024-03-04 19:14:07.000000 dclex-0.0.6/src/dclex/__init__.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    11488 2024-04-05 13:54:10.000000 dclex-0.0.6/src/dclex/dclex.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    12964 2024-04-05 13:53:24.000000 dclex-0.0.6/src/dclex/dclex_client.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.562265 dclex-0.0.6/src/dclex/resources/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    19297 2024-02-02 17:33:59.000000 dclex-0.0.6/src/dclex/resources/digital_identity_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    15662 2024-02-02 17:33:59.000000 dclex-0.0.6/src/dclex/resources/factory_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6200 2024-02-02 17:33:59.000000 dclex-0.0.6/src/dclex/resources/usdc_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     9883 2024-02-02 17:33:59.000000 dclex-0.0.6/src/dclex/resources/vault_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1188 2024-03-01 16:20:01.000000 dclex-0.0.6/src/dclex/settings.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     2285 2024-03-01 16:30:00.000000 dclex-0.0.6/src/dclex/types.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.566264 dclex-0.0.6/src/dclex.egg-info/
+-rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/PKG-INFO
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      580 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/SOURCES.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)        1 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/dependency_links.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)       60 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/requires.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)        6 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/top_level.txt
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.566264 dclex-0.0.6/tests/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1167 2024-03-04 19:14:07.000000 dclex-0.0.6/tests/test_account.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6062 2024-03-04 19:14:07.000000 dclex-0.0.6/tests/test_orders.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1534 2024-04-05 13:55:04.000000 dclex-0.0.6/tests/test_stocks.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6753 2024-03-04 19:14:07.000000 dclex-0.0.6/tests/test_transfers.py
```

### Comparing `dclex-0.0.5/LICENSE` & `dclex-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/PKG-INFO` & `dclex-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dclex
-Version: 0.0.5
+Version: 0.0.6
 Summary: DCLEX python library
 License: DCLEX API Non-Commercial License
         
         This DCLEX API Non-Commercial License ("License") is an agreement between DCLEX inc. ("DCLEX") and You, and governs Your use of the API Code. By loging to your DCLEX account programmatically , you acknowledge that You consent to be legally bound by this Agreement.
         
         1. Introduction.
         1.1 DCLEX has developed application program interface ("API") code to permit its customers to use their own internal proprietary software tools in managing their accounts with DCLEX. This License is intended only for users who wish to use the API Code by itself as is, or in connection with or for the development of their own internal proprietary tools to manage their own DCLEX accounts. This License is NOT for anybody who is developing software applications that they wish to: (a) sell to third party users for a fee, or (b) give to third party users to generate an indirect financial benefit (e.g., commissions). If You wish to make a software application for the purposes described in the preceding sentence then please us at info@dclex.com.
@@ -85,10 +85,11 @@
 ```bash
 pip install dclex
 ```
 
 ## 2. Code examples ##
 
 ### 2.1 [Login and logout](./examples/login_and_logout.py) ###
-### 2.2 [Deposit and withdraw](./examples/deposit_and_withdraw.py) ###
-### 2.3 [Buying and selling stocks](./examples/buying_and_selling_stocks.py) ###
-### 2.4 [Portfolio](./examples/portfolio.py) ###
+### 2.2 [Stocks and prices](./examples/stocks_and_prices.py) ###
+### 2.3 [Deposit and withdraw](./examples/deposit_and_withdraw.py) ###
+### 2.4 [Buying and selling stocks](./examples/buying_and_selling_stocks.py) ###
+### 2.5 [Portfolio](./examples/portfolio.py) ###
```

### Comparing `dclex-0.0.5/pyproject.toml` & `dclex-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dclex"
-version = "0.0.5"
+version = "0.0.6"
 description = "DCLEX python library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 classifiers = [
     "Intended Audience :: Financial and Insurance Industry",
     "Programming Language :: Python :: 3.7",
```

### Comparing `dclex-0.0.5/src/dclex/dclex.py` & `dclex-0.0.6/src/dclex/dclex.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,15 +303,16 @@
     def market_prices(self):
         try:
             return self._dclex_client.market_prices()
         except AuthorizationError:
             raise AccountNotVerified()
 
     def prices_stream(self):
-        return self._dclex_client.prices_stream()
+        prices_stream_access_token = self._dclex_client.prices_stream_access_token()
+        return self._dclex_client.prices_stream(prices_stream_access_token)
 
     def _build_and_send_transaction(self, contract_function: ContractFunction) -> str:
         transaction = contract_function.build_transaction(
             {
                 "from": self._account.address,
                 "gasPrice": self._web3.eth.gas_price,
                 "nonce": self._web3.eth.get_transaction_count(
```

### Comparing `dclex-0.0.5/src/dclex/dclex_client.py` & `dclex-0.0.6/src/dclex/dclex_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,16 +293,20 @@
                 last_price=Decimal(stock["price"]["price"]),
                 timestamp=self._parse_timestamp(stock["price"]["timestamp"]),
                 percentage_change=Decimal(stock["price"]["percentageChange"]),
             )
             for stock in prices_data
         }
 
-    def prices_stream(self):
-        for sse_message in SSEClient(f"{DCLEX_BASE_URL}/prices-stream/"):
+    def prices_stream_access_token(self) -> str:
+        response = self._authorized_get("/prices-stream-access-token/")
+        return response["pricesStreamAccessToken"]
+
+    def prices_stream(self, prices_stream_access_token: str):
+        for sse_message in SSEClient(f"{DCLEX_BASE_URL}/prices-stream/", params={"token": prices_stream_access_token}):
             price_data = json.loads(sse_message.data)
             yield Price(
                 symbol=price_data["symbol"],
                 last_price=Decimal(price_data["price"]),
                 timestamp=self._parse_timestamp(price_data["timestamp"]),
                 percentage_change=Decimal(price_data["percentageChange"]),
             )
```

### Comparing `dclex-0.0.5/src/dclex/resources/digital_identity_contract_abi.json` & `dclex-0.0.6/src/dclex/resources/digital_identity_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/src/dclex/resources/factory_contract_abi.json` & `dclex-0.0.6/src/dclex/resources/factory_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/src/dclex/resources/usdc_contract_abi.json` & `dclex-0.0.6/src/dclex/resources/usdc_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/src/dclex/resources/vault_contract_abi.json` & `dclex-0.0.6/src/dclex/resources/vault_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/src/dclex/settings.py` & `dclex-0.0.6/src/dclex/settings.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/src/dclex/types.py` & `dclex-0.0.6/src/dclex/types.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/src/dclex.egg-info/PKG-INFO` & `dclex-0.0.6/src/dclex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dclex
-Version: 0.0.5
+Version: 0.0.6
 Summary: DCLEX python library
 License: DCLEX API Non-Commercial License
         
         This DCLEX API Non-Commercial License ("License") is an agreement between DCLEX inc. ("DCLEX") and You, and governs Your use of the API Code. By loging to your DCLEX account programmatically , you acknowledge that You consent to be legally bound by this Agreement.
         
         1. Introduction.
         1.1 DCLEX has developed application program interface ("API") code to permit its customers to use their own internal proprietary software tools in managing their accounts with DCLEX. This License is intended only for users who wish to use the API Code by itself as is, or in connection with or for the development of their own internal proprietary tools to manage their own DCLEX accounts. This License is NOT for anybody who is developing software applications that they wish to: (a) sell to third party users for a fee, or (b) give to third party users to generate an indirect financial benefit (e.g., commissions). If You wish to make a software application for the purposes described in the preceding sentence then please us at info@dclex.com.
@@ -85,10 +85,11 @@
 ```bash
 pip install dclex
 ```
 
 ## 2. Code examples ##
 
 ### 2.1 [Login and logout](./examples/login_and_logout.py) ###
-### 2.2 [Deposit and withdraw](./examples/deposit_and_withdraw.py) ###
-### 2.3 [Buying and selling stocks](./examples/buying_and_selling_stocks.py) ###
-### 2.4 [Portfolio](./examples/portfolio.py) ###
+### 2.2 [Stocks and prices](./examples/stocks_and_prices.py) ###
+### 2.3 [Deposit and withdraw](./examples/deposit_and_withdraw.py) ###
+### 2.4 [Buying and selling stocks](./examples/buying_and_selling_stocks.py) ###
+### 2.5 [Portfolio](./examples/portfolio.py) ###
```

### Comparing `dclex-0.0.5/src/dclex.egg-info/SOURCES.txt` & `dclex-0.0.6/src/dclex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/tests/test_account.py` & `dclex-0.0.6/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/tests/test_orders.py` & `dclex-0.0.6/tests/test_orders.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.5/tests/test_stocks.py` & `dclex-0.0.6/tests/test_stocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 def test_market_prices_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
         dclex_unverified.market_prices()
 
 
 def test_prices_stream(dclex):
+    dclex.login()
+
     prices_stream = dclex.prices_stream()
 
     price = next(prices_stream)
     assert isinstance(price.symbol, str)
     assert isinstance(price.last_price, Decimal)
     assert price.last_price > 0
     assert isinstance(price.timestamp, datetime)
```

### Comparing `dclex-0.0.5/tests/test_transfers.py` & `dclex-0.0.6/tests/test_transfers.py`

 * *Files identical despite different names*

