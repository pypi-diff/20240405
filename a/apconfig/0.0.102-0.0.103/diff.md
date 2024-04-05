# Comparing `tmp/apconfig-0.0.102.tar.gz` & `tmp/apconfig-0.0.103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apconfig-0.0.102.tar", max compression
+gzip compressed data, was "apconfig-0.0.103.tar", max compression
```

## Comparing `apconfig-0.0.102.tar` & `apconfig-0.0.103.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.102/README.md
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 apconfig-0.0.102/apconfig/__init__.py
--rw-r--r--   0        0        0      112 2024-04-05 06:25:39.273690 apconfig-0.0.102/apconfig/utilities.py
--rw-r--r--   0        0        0      305 2024-04-05 06:25:49.645785 apconfig-0.0.102/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.102/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.103/README.md
+-rw-r--r--   0        0        0     2792 2024-04-05 10:45:32.404147 apconfig-0.0.103/apconfig/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-05 06:25:39.273690 apconfig-0.0.103/apconfig/utilities.py
+-rw-r--r--   0        0        0      305 2024-04-05 10:45:32.416147 apconfig-0.0.103/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.103/PKG-INFO
```

### Comparing `apconfig-0.0.102/apconfig/__init__.py` & `apconfig-0.0.103/apconfig/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     except Exception as e:
         raise
 
 
 setup_data = get_api_setup_data()
 
 # TSO Configuration
-chains = ['coston', 'songbird', 'flare']
+chains = ['coston', 'coston2', 'songbird', 'flare']
 
 # Data Service Streamers and APIs
 WS = 'ws://'
 WSS = 'wss://'
 HTTP = 'http://'
 HTTPS = 'https://'
 
@@ -46,30 +46,30 @@
 algorithm_prepared_data_buffer = 17
 ml_predictions_buffer = 12
 submission_commit_buffer = 7
 
 # Web3 Providers
 web3_provider_list: dict = {}
 web3_websocket_list: dict = {}
-for chain in ['coston', 'songbird', 'flare']:
+for chain in chains:
     try:
         web3_provider_list[chain] = setup_data["chains"][chain]["providers"]["rpc"]
         web3_websocket_list[chain] = setup_data["chains"][chain]["providers"]["ws"]
     except Exception as e:
         print(e)
 
 test_web3_provider_list = [os.getenv("WEB3_PROVIDER")]
 test_web3_websocket_list = [os.getenv("WEB3_WEBSOCKETS")]
 
 # Chain Wallet Configuration
-flare_reward_offers_manager_addresses = {}
-for chain in ['coston', 'songbird', 'flare']:
+ftso_reward_offers_manager_addresses = {}
+for chain in chains:
     try:
-        flare_reward_offers_manager_addresses[chain] \
-            = setup_data["chains"][chain]["flare_reward_offers_manager_address"]
+        ftso_reward_offers_manager_addresses[chain] \
+            = setup_data["chains"][chain]["ftso_reward_offers_manager_address"]
     except Exception as e:
         print(e)
 
 # Database Configuration
 environment = os.getenv("ENVIRONMENT")
 
 assert environment is not None, "Environment not set. "
```

