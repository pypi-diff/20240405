# Comparing `tmp/tanx-connector-2.0.2.tar.gz` & `tmp/tanx-connector-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tanx-connector-2.0.2.tar", last modified: Tue Apr  2 07:55:02 2024, max compression
+gzip compressed data, was "tanx-connector-2.0.3.tar", last modified: Fri Apr  5 06:32:56 2024, max compression
```

## Comparing `tanx-connector-2.0.2.tar` & `tanx-connector-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20390 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.550124 tanx-connector-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/src/tanx_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/src/tanxconnector/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/src/tanxconnector/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/blockchain_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/erc20_abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   102707 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/pedersen_params.json
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/polygon_deposit.json
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)    64164 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/starkex_abi_main.json
--rw-r--r--   0 runner    (1001) docker     (127)    61398 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/starkex_abi_test.json
--rw-r--r--   0 runner    (1001) docker     (127)    28194 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/wsclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    30174 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:32:56.056538 tanx-connector-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22996 2024-04-05 06:32:56.056538 tanx-connector-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20566 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 06:32:56.056538 tanx-connector-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:32:56.048538 tanx-connector-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:32:56.056538 tanx-connector-2.0.3/src/tanx_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22996 2024-04-05 06:32:56.000000 tanx-connector-2.0.3/src/tanx_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-05 06:32:56.000000 tanx-connector-2.0.3/src/tanx_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:32:56.000000 tanx-connector-2.0.3/src/tanx_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-05 06:32:56.000000 tanx-connector-2.0.3/src/tanx_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 06:32:56.000000 tanx-connector-2.0.3/src/tanx_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:32:56.052538 tanx-connector-2.0.3/src/tanxconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:32:56.052538 tanx-connector-2.0.3/src/tanxconnector/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/blockchain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/erc20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102707 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/pedersen_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/polygon_deposit.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64164 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/starkex_abi_main.json
+-rw-r--r--   0 runner    (1001) docker     (127)    61398 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/bin/starkex_abi_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28194 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/src/tanxconnector/wsclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:32:56.052538 tanx-connector-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    30174 2024-04-05 06:32:49.000000 tanx-connector-2.0.3/tests/test_client.py
```

### Comparing `tanx-connector-2.0.2/LICENSE` & `tanx-connector-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/PKG-INFO` & `tanx-connector-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanx-connector
-Version: 2.0.2
+Version: 2.0.3
 Summary: The official Python connector for Tanx's API
 Author: tanX
 License: MIT License
         
         Copyright (c) 2023 Tanx Fi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -134,31 +134,33 @@
 
 ## Quickstart
 
 Make sure that tanxconnector is [installed](#installation) and up-to-date.
 Also make sure you have an account on the [mainnet](https://trade.tanx.fi/) or [testnet](https://testnet.tanx.fi/) website.
 
 To get quickly started, try running the simple example for creating and fetching the order once logged in.
+For the `stark_private_key`, kindly see the [L2 Key Pair](#l2-key-pair) section of the documentation.
 
 ```python
 from tanxconnector import Client
 
 ETH_ADDRESS = "(your eth wallet address)"
-PRIVATE_KEY = "(your wallet's private key)"
+ETH_WALLET_PRIVATE_KEY = "(your wallet's private key)"
+STARK_PRIVATE_KEY = "(stark private key from the L2 Key Pair)"
 
 client = Client()
 
 # login to the network
 login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY)
 
 # create an order nonce
 nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005}
 
 # create the order
-order = client.create_complete_order(nonce, stark_private_key)
+order = client.create_complete_order(nonce, STARK_PRIVATE_KEY)
 print(order)
 
 # fetch the details of the order just created
 order_id = order['payload']['id']
 fetch_order = client.get_order(order_id)
 print(fetch_order)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tanx-connector Version: 2.0.2 Summary: The official
+Metadata-Version: 2.1 Name: tanx-connector Version: 2.0.3 Summary: The official
 Python connector for Tanx's API Author: tanX License: MIT License Copyright (c)
 2023 Tanx Fi Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
@@ -59,35 +59,37 @@
 [Available Methods](#available-methods) ## Installation First go to the [tanX
 Website](https://www.tanx.fi/) and create an account with your wallet. Install
 the package using pip. ```python pip install tanx-connector ``` ## Quickstart
 Make sure that tanxconnector is [installed](#installation) and up-to-date. Also
 make sure you have an account on the [mainnet](https://trade.tanx.fi/) or
 [testnet](https://testnet.tanx.fi/) website. To get quickly started, try
 running the simple example for creating and fetching the order once logged in.
-```python from tanxconnector import Client ETH_ADDRESS = "(your eth wallet
-address)" PRIVATE_KEY = "(your wallet's private key)" client = Client() # login
-to the network login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # create
-an order nonce nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':
-'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005} # create the
-order order = client.create_complete_order(nonce, stark_private_key) print
-(order) # fetch the details of the order just created order_id = order
-['payload']['id'] fetch_order = client.get_order(order_id) print(fetch_order)
-``` ## Getting Started The default base url for mainnet is https://api.tanx.fi
-and testnet is https://api-testnet.tanx.fi. You can choose between mainnet and
-testnet by providing it through the constructor. The default is mainnet. All
-REST apis, WebSockets are handled by Client, WsClient classes respectively. ###
-Workflow Check out the [example files](./example) to see an example workflow.
-### L2 Key Pair L2 Key Pair generation isn't currently available in the TanX
-Python SDK. To get the L2 Key Pair, follow any of the two steps: 1. Get the Key
-Pair from the [TanX official website](https://trade.tanx.fi/)'s Account
-Settings Tab once wallet is connected. Refer to the image below for more
-reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to
-get the keys. Copy these keys and store it securely. [https://
-raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-
-key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
+For the `stark_private_key`, kindly see the [L2 Key Pair](#l2-key-pair) section
+of the documentation. ```python from tanxconnector import Client ETH_ADDRESS =
+"(your eth wallet address)" ETH_WALLET_PRIVATE_KEY = "(your wallet's private
+key)" STARK_PRIVATE_KEY = "(stark private key from the L2 Key Pair)" client =
+Client() # login to the network login = client.complete_login(ETH_ADDRESS,
+PRIVATE_KEY) # create an order nonce nonce: CreateOrderNonceBody = {'market':
+'ethusdc', 'ord_type':'market', 'price': 29580.51, 'side': 'sell', 'volume':
+0.0005} # create the order order = client.create_complete_order(nonce,
+STARK_PRIVATE_KEY) print(order) # fetch the details of the order just created
+order_id = order['payload']['id'] fetch_order = client.get_order(order_id)
+print(fetch_order) ``` ## Getting Started The default base url for mainnet is
+https://api.tanx.fi and testnet is https://api-testnet.tanx.fi. You can choose
+between mainnet and testnet by providing it through the constructor. The
+default is mainnet. All REST apis, WebSockets are handled by Client, WsClient
+classes respectively. ### Workflow Check out the [example files](./example) to
+see an example workflow. ### L2 Key Pair L2 Key Pair generation isn't currently
+available in the TanX Python SDK. To get the L2 Key Pair, follow any of the two
+steps: 1. Get the Key Pair from the [TanX official website](https://
+trade.tanx.fi/)'s Account Settings Tab once wallet is connected. Refer to the
+image below for more reference. Click on `Settings -> tanX key -> Show Keys`
+and Sign the request to get the keys. Copy these keys and store it securely.
+[https://raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/
+tanx-key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
 github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK,
 refer to [this section](https://github.com/tanx-libs/tanx-connector-
 nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK. ### Rest
 Client Import the REST Client ```py from tanxconnector import Client ``` Create
 a new instance ```python client = Client() # or client = Client('testnet') #
 default is mainnet, can pass explicitly as well ``` ### General Endpoints ####
 Test connectivity `GET /sapi/v1/health/` ```python client.test_connection() ```
```

### Comparing `tanx-connector-2.0.2/README.md` & `tanx-connector-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,31 +80,33 @@
 
 ## Quickstart
 
 Make sure that tanxconnector is [installed](#installation) and up-to-date.
 Also make sure you have an account on the [mainnet](https://trade.tanx.fi/) or [testnet](https://testnet.tanx.fi/) website.
 
 To get quickly started, try running the simple example for creating and fetching the order once logged in.
+For the `stark_private_key`, kindly see the [L2 Key Pair](#l2-key-pair) section of the documentation.
 
 ```python
 from tanxconnector import Client
 
 ETH_ADDRESS = "(your eth wallet address)"
-PRIVATE_KEY = "(your wallet's private key)"
+ETH_WALLET_PRIVATE_KEY = "(your wallet's private key)"
+STARK_PRIVATE_KEY = "(stark private key from the L2 Key Pair)"
 
 client = Client()
 
 # login to the network
 login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY)
 
 # create an order nonce
 nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005}
 
 # create the order
-order = client.create_complete_order(nonce, stark_private_key)
+order = client.create_complete_order(nonce, STARK_PRIVATE_KEY)
 print(order)
 
 # fetch the details of the order just created
 order_id = order['payload']['id']
 fetch_order = client.get_order(order_id)
 print(fetch_order)
 ```
```

#### html2text {}

```diff
@@ -29,35 +29,37 @@
 [Available Methods](#available-methods) ## Installation First go to the [tanX
 Website](https://www.tanx.fi/) and create an account with your wallet. Install
 the package using pip. ```python pip install tanx-connector ``` ## Quickstart
 Make sure that tanxconnector is [installed](#installation) and up-to-date. Also
 make sure you have an account on the [mainnet](https://trade.tanx.fi/) or
 [testnet](https://testnet.tanx.fi/) website. To get quickly started, try
 running the simple example for creating and fetching the order once logged in.
-```python from tanxconnector import Client ETH_ADDRESS = "(your eth wallet
-address)" PRIVATE_KEY = "(your wallet's private key)" client = Client() # login
-to the network login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # create
-an order nonce nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':
-'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005} # create the
-order order = client.create_complete_order(nonce, stark_private_key) print
-(order) # fetch the details of the order just created order_id = order
-['payload']['id'] fetch_order = client.get_order(order_id) print(fetch_order)
-``` ## Getting Started The default base url for mainnet is https://api.tanx.fi
-and testnet is https://api-testnet.tanx.fi. You can choose between mainnet and
-testnet by providing it through the constructor. The default is mainnet. All
-REST apis, WebSockets are handled by Client, WsClient classes respectively. ###
-Workflow Check out the [example files](./example) to see an example workflow.
-### L2 Key Pair L2 Key Pair generation isn't currently available in the TanX
-Python SDK. To get the L2 Key Pair, follow any of the two steps: 1. Get the Key
-Pair from the [TanX official website](https://trade.tanx.fi/)'s Account
-Settings Tab once wallet is connected. Refer to the image below for more
-reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to
-get the keys. Copy these keys and store it securely. [https://
-raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-
-key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
+For the `stark_private_key`, kindly see the [L2 Key Pair](#l2-key-pair) section
+of the documentation. ```python from tanxconnector import Client ETH_ADDRESS =
+"(your eth wallet address)" ETH_WALLET_PRIVATE_KEY = "(your wallet's private
+key)" STARK_PRIVATE_KEY = "(stark private key from the L2 Key Pair)" client =
+Client() # login to the network login = client.complete_login(ETH_ADDRESS,
+PRIVATE_KEY) # create an order nonce nonce: CreateOrderNonceBody = {'market':
+'ethusdc', 'ord_type':'market', 'price': 29580.51, 'side': 'sell', 'volume':
+0.0005} # create the order order = client.create_complete_order(nonce,
+STARK_PRIVATE_KEY) print(order) # fetch the details of the order just created
+order_id = order['payload']['id'] fetch_order = client.get_order(order_id)
+print(fetch_order) ``` ## Getting Started The default base url for mainnet is
+https://api.tanx.fi and testnet is https://api-testnet.tanx.fi. You can choose
+between mainnet and testnet by providing it through the constructor. The
+default is mainnet. All REST apis, WebSockets are handled by Client, WsClient
+classes respectively. ### Workflow Check out the [example files](./example) to
+see an example workflow. ### L2 Key Pair L2 Key Pair generation isn't currently
+available in the TanX Python SDK. To get the L2 Key Pair, follow any of the two
+steps: 1. Get the Key Pair from the [TanX official website](https://
+trade.tanx.fi/)'s Account Settings Tab once wallet is connected. Refer to the
+image below for more reference. Click on `Settings -> tanX key -> Show Keys`
+and Sign the request to get the keys. Copy these keys and store it securely.
+[https://raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/
+tanx-key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
 github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK,
 refer to [this section](https://github.com/tanx-libs/tanx-connector-
 nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK. ### Rest
 Client Import the REST Client ```py from tanxconnector import Client ``` Create
 a new instance ```python client = Client() # or client = Client('testnet') #
 default is mainnet, can pass explicitly as well ``` ### General Endpoints ####
 Test connectivity `GET /sapi/v1/health/` ```python client.test_connection() ```
```

### Comparing `tanx-connector-2.0.2/pyproject.toml` & `tanx-connector-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "bumpver",
     "build",
     "twine",
     "python-dotenv"
 ]
 
 [tool.bumpver]
-current_version = "2.0.2"
+current_version = "2.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "update version: v{old_version} -> v{new_version}"
 commit = false
 push = false
 
 [tool.setuptools.dynamic]
 version = {attr = "tanxconnector.__version__"}
```

### Comparing `tanx-connector-2.0.2/src/tanx_connector.egg-info/PKG-INFO` & `tanx-connector-2.0.3/src/tanx_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanx-connector
-Version: 2.0.2
+Version: 2.0.3
 Summary: The official Python connector for Tanx's API
 Author: tanX
 License: MIT License
         
         Copyright (c) 2023 Tanx Fi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -134,31 +134,33 @@
 
 ## Quickstart
 
 Make sure that tanxconnector is [installed](#installation) and up-to-date.
 Also make sure you have an account on the [mainnet](https://trade.tanx.fi/) or [testnet](https://testnet.tanx.fi/) website.
 
 To get quickly started, try running the simple example for creating and fetching the order once logged in.
+For the `stark_private_key`, kindly see the [L2 Key Pair](#l2-key-pair) section of the documentation.
 
 ```python
 from tanxconnector import Client
 
 ETH_ADDRESS = "(your eth wallet address)"
-PRIVATE_KEY = "(your wallet's private key)"
+ETH_WALLET_PRIVATE_KEY = "(your wallet's private key)"
+STARK_PRIVATE_KEY = "(stark private key from the L2 Key Pair)"
 
 client = Client()
 
 # login to the network
 login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY)
 
 # create an order nonce
 nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005}
 
 # create the order
-order = client.create_complete_order(nonce, stark_private_key)
+order = client.create_complete_order(nonce, STARK_PRIVATE_KEY)
 print(order)
 
 # fetch the details of the order just created
 order_id = order['payload']['id']
 fetch_order = client.get_order(order_id)
 print(fetch_order)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tanx-connector Version: 2.0.2 Summary: The official
+Metadata-Version: 2.1 Name: tanx-connector Version: 2.0.3 Summary: The official
 Python connector for Tanx's API Author: tanX License: MIT License Copyright (c)
 2023 Tanx Fi Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
@@ -59,35 +59,37 @@
 [Available Methods](#available-methods) ## Installation First go to the [tanX
 Website](https://www.tanx.fi/) and create an account with your wallet. Install
 the package using pip. ```python pip install tanx-connector ``` ## Quickstart
 Make sure that tanxconnector is [installed](#installation) and up-to-date. Also
 make sure you have an account on the [mainnet](https://trade.tanx.fi/) or
 [testnet](https://testnet.tanx.fi/) website. To get quickly started, try
 running the simple example for creating and fetching the order once logged in.
-```python from tanxconnector import Client ETH_ADDRESS = "(your eth wallet
-address)" PRIVATE_KEY = "(your wallet's private key)" client = Client() # login
-to the network login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # create
-an order nonce nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':
-'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005} # create the
-order order = client.create_complete_order(nonce, stark_private_key) print
-(order) # fetch the details of the order just created order_id = order
-['payload']['id'] fetch_order = client.get_order(order_id) print(fetch_order)
-``` ## Getting Started The default base url for mainnet is https://api.tanx.fi
-and testnet is https://api-testnet.tanx.fi. You can choose between mainnet and
-testnet by providing it through the constructor. The default is mainnet. All
-REST apis, WebSockets are handled by Client, WsClient classes respectively. ###
-Workflow Check out the [example files](./example) to see an example workflow.
-### L2 Key Pair L2 Key Pair generation isn't currently available in the TanX
-Python SDK. To get the L2 Key Pair, follow any of the two steps: 1. Get the Key
-Pair from the [TanX official website](https://trade.tanx.fi/)'s Account
-Settings Tab once wallet is connected. Refer to the image below for more
-reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to
-get the keys. Copy these keys and store it securely. [https://
-raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-
-key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
+For the `stark_private_key`, kindly see the [L2 Key Pair](#l2-key-pair) section
+of the documentation. ```python from tanxconnector import Client ETH_ADDRESS =
+"(your eth wallet address)" ETH_WALLET_PRIVATE_KEY = "(your wallet's private
+key)" STARK_PRIVATE_KEY = "(stark private key from the L2 Key Pair)" client =
+Client() # login to the network login = client.complete_login(ETH_ADDRESS,
+PRIVATE_KEY) # create an order nonce nonce: CreateOrderNonceBody = {'market':
+'ethusdc', 'ord_type':'market', 'price': 29580.51, 'side': 'sell', 'volume':
+0.0005} # create the order order = client.create_complete_order(nonce,
+STARK_PRIVATE_KEY) print(order) # fetch the details of the order just created
+order_id = order['payload']['id'] fetch_order = client.get_order(order_id)
+print(fetch_order) ``` ## Getting Started The default base url for mainnet is
+https://api.tanx.fi and testnet is https://api-testnet.tanx.fi. You can choose
+between mainnet and testnet by providing it through the constructor. The
+default is mainnet. All REST apis, WebSockets are handled by Client, WsClient
+classes respectively. ### Workflow Check out the [example files](./example) to
+see an example workflow. ### L2 Key Pair L2 Key Pair generation isn't currently
+available in the TanX Python SDK. To get the L2 Key Pair, follow any of the two
+steps: 1. Get the Key Pair from the [TanX official website](https://
+trade.tanx.fi/)'s Account Settings Tab once wallet is connected. Refer to the
+image below for more reference. Click on `Settings -> tanX key -> Show Keys`
+and Sign the request to get the keys. Copy these keys and store it securely.
+[https://raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/
+tanx-key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
 github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK,
 refer to [this section](https://github.com/tanx-libs/tanx-connector-
 nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK. ### Rest
 Client Import the REST Client ```py from tanxconnector import Client ``` Create
 a new instance ```python client = Client() # or client = Client('testnet') #
 default is mainnet, can pass explicitly as well ``` ### General Endpoints ####
 Test connectivity `GET /sapi/v1/health/` ```python client.test_connection() ```
```

### Comparing `tanx-connector-2.0.2/src/tanx_connector.egg-info/SOURCES.txt` & `tanx-connector-2.0.3/src/tanx_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/bin/blockchain_utils.py` & `tanx-connector-2.0.3/src/tanxconnector/bin/blockchain_utils.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/bin/erc20_abi.json` & `tanx-connector-2.0.3/src/tanxconnector/bin/erc20_abi.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/bin/math_utils.py` & `tanx-connector-2.0.3/src/tanxconnector/bin/math_utils.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/bin/pedersen_params.json` & `tanx-connector-2.0.3/src/tanxconnector/bin/pedersen_params.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/bin/polygon_deposit.json` & `tanx-connector-2.0.3/src/tanxconnector/bin/polygon_deposit.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/bin/signature.py` & `tanx-connector-2.0.3/src/tanxconnector/bin/signature.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/bin/starkex_abi_main.json` & `tanx-connector-2.0.3/src/tanxconnector/bin/starkex_abi_main.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/bin/starkex_abi_test.json` & `tanx-connector-2.0.3/src/tanxconnector/bin/starkex_abi_test.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/client.py` & `tanx-connector-2.0.3/src/tanxconnector/client.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/constants.py` & `tanx-connector-2.0.3/src/tanxconnector/constants.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/exception.py` & `tanx-connector-2.0.3/src/tanxconnector/exception.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/session.py` & `tanx-connector-2.0.3/src/tanxconnector/session.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/typings.py` & `tanx-connector-2.0.3/src/tanxconnector/typings.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/utils.py` & `tanx-connector-2.0.3/src/tanxconnector/utils.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/src/tanxconnector/wsclient.py` & `tanx-connector-2.0.3/src/tanxconnector/wsclient.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.2/tests/test_client.py` & `tanx-connector-2.0.3/tests/test_client.py`

 * *Files identical despite different names*

