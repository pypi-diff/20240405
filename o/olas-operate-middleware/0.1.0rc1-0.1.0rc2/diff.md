# Comparing `tmp/olas_operate_middleware-0.1.0rc1.tar.gz` & `tmp/olas_operate_middleware-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olas_operate_middleware-0.1.0rc1.tar", max compression
+gzip compressed data, was "olas_operate_middleware-0.1.0rc2.tar", max compression
```

## Comparing `olas_operate_middleware-0.1.0rc1.tar` & `olas_operate_middleware-0.1.0rc2.tar`

### file list

```diff
@@ -1,31 +1,37 @@
--rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc1/README.md
--rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc1/operate/__init__.py
--rw-r--r--   0        0        0    11036 2024-03-28 15:25:41.778980 olas_operate_middleware-0.1.0rc1/operate/cli.py
--rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc1/operate/constants.py
--rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc1/operate/data/__init__.py
--rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc1/operate/data/contracts/__init__.py
--rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc1/operate/data/contracts/service_staking_token/__init__.py
--rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc1/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
--rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc1/operate/data/contracts/service_staking_token/contract.py
--rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc1/operate/data/contracts/service_staking_token/contract.yaml
--rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc1/operate/data/contracts/uniswap_v2_erc20/__init__.py
--rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc1/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
--rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc1/operate/data/contracts/uniswap_v2_erc20/contract.py
--rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc1/operate/data/contracts/uniswap_v2_erc20/contract.yaml
--rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc1/operate/http/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc1/operate/http/exceptions.py
--rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc1/operate/keys.py
--rw-r--r--   0        0        0     2481 2024-03-28 15:25:41.779569 olas_operate_middleware-0.1.0rc1/operate/ledger/__init__.py
--rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc1/operate/ledger/base.py
--rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc1/operate/ledger/ethereum.py
--rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc1/operate/ledger/profiles.py
--rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc1/operate/ledger/solana.py
--rw-r--r--   0        0        0     3861 2024-03-28 15:25:41.780238 olas_operate_middleware-0.1.0rc1/operate/resource.py
--rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc1/operate/services/__init__.py
--rw-r--r--   0        0        0    14457 2024-03-28 15:25:41.782863 olas_operate_middleware-0.1.0rc1/operate/services/manage.py
--rw-r--r--   0        0        0    23913 2024-03-28 15:25:41.783808 olas_operate_middleware-0.1.0rc1/operate/services/protocol.py
--rw-r--r--   0        0        0    13179 2024-03-28 09:54:27.542688 olas_operate_middleware-0.1.0rc1/operate/services/service.py
--rw-r--r--   0        0        0     4918 2024-03-28 15:25:41.784895 olas_operate_middleware-0.1.0rc1/operate/types.py
--rw-r--r--   0        0        0      808 2024-03-28 15:38:26.043386 olas_operate_middleware-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc2/LICENSE
+-rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc2/README.md
+-rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc2/operate/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc2/operate/account/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc2/operate/account/user.py
+-rw-r--r--   0        0        0    17459 2024-04-05 14:54:43.349665 olas_operate_middleware-0.1.0rc2/operate/cli.py
+-rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc2/operate/constants.py
+-rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc2/operate/data/__init__.py
+-rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc2/operate/data/contracts/__init__.py
+-rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/__init__.py
+-rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
+-rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/contract.py
+-rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/contract.yaml
+-rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/__init__.py
+-rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/contract.py
+-rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/contract.yaml
+-rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc2/operate/http/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc2/operate/http/exceptions.py
+-rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc2/operate/keys.py
+-rw-r--r--   0        0        0     2849 2024-04-05 14:54:43.350001 olas_operate_middleware-0.1.0rc2/operate/ledger/__init__.py
+-rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc2/operate/ledger/base.py
+-rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc2/operate/ledger/ethereum.py
+-rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc2/operate/ledger/profiles.py
+-rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc2/operate/ledger/solana.py
+-rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc2/operate/resource.py
+-rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc2/operate/services/__init__.py
+-rw-r--r--   0        0        0    16022 2024-04-05 14:54:43.350907 olas_operate_middleware-0.1.0rc2/operate/services/manage.py
+-rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc2/operate/services/protocol.py
+-rw-r--r--   0        0        0    13179 2024-03-28 09:54:27.542688 olas_operate_middleware-0.1.0rc2/operate/services/service.py
+-rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc2/operate/types.py
+-rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc2/operate/utils/__init__.py
+-rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc2/operate/utils/gnosis.py
+-rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc2/operate/wallet/__init__.py
+-rw-r--r--   0        0        0     8292 2024-04-05 14:54:43.354467 olas_operate_middleware-0.1.0rc2/operate/wallet/master.py
+-rw-r--r--   0        0        0      803 2024-04-05 15:15:29.231331 olas_operate_middleware-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc2/PKG-INFO
```

### Comparing `olas_operate_middleware-0.1.0rc1/LICENSE` & `olas_operate_middleware-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/README.md` & `olas_operate_middleware-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/__init__.py` & `olas_operate_middleware-0.1.0rc2/operate/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/constants.py` & `olas_operate_middleware-0.1.0rc2/operate/constants.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/__init__.py` & `olas_operate_middleware-0.1.0rc2/operate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/__init__.py` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/service_staking_token/__init__.py` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/service_staking_token/contract.py` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/service_staking_token/contract.yaml` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/uniswap_v2_erc20/__init__.py` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/uniswap_v2_erc20/contract.py` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/data/contracts/uniswap_v2_erc20/contract.yaml` & `olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/http/__init__.py` & `olas_operate_middleware-0.1.0rc2/operate/http/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/http/exceptions.py` & `olas_operate_middleware-0.1.0rc2/operate/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/keys.py` & `olas_operate_middleware-0.1.0rc2/operate/keys.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/ledger/__init__.py` & `olas_operate_middleware-0.1.0rc2/operate/ledger/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
 
 """Ledger helpers."""
 
+import os
 import typing as t
 
 from operate.ledger.base import LedgerHelper
 from operate.ledger.ethereum import Ethereum
 from operate.ledger.solana import Solana
 from operate.types import ChainType, LedgerType
 
 
-ETHEREUM_RPC = "https://ethereum.publicnode.com"
-GNOSIS_RPC = "https://rpc.gnosischain.com"
-GOERLI_RPC = "https://ethereum-goerli.publicnode.com"
-SOLANA_RPC = "https://api.mainnet-beta.solana.com"
+ETHEREUM_RPC = os.environ.get("DEV_RPC", "https://ethereum.publicnode.com")
+GNOSIS_RPC = os.environ.get("DEV_RPC", "https://rpc.gnosischain.com")
+GOERLI_RPC = os.environ.get("DEV_RPC", "https://ethereum-goerli.publicnode.com")
+SOLANA_RPC = os.environ.get("DEV_RPC", "https://api.mainnet-beta.solana.com")
 
 
 DEFAULT_RPCS = {
     ChainType.ETHEREUM: ETHEREUM_RPC,
     ChainType.GNOSIS: GNOSIS_RPC,
     ChainType.GOERLI: GOERLI_RPC,
     ChainType.SOLANA: SOLANA_RPC,
@@ -61,14 +62,21 @@
 
 
 def get_default_rpc(chain: ChainType) -> str:
     """Get default RPC chain type."""
     return DEFAULT_RPCS.get(chain, ETHEREUM_RPC)
 
 
+def get_ledger_type_from_chain_type(chain: ChainType) -> LedgerType:
+    """Get LedgerType from ChainType."""
+    if chain in (ChainType.ETHEREUM, ChainType.GOERLI, ChainType.GNOSIS):
+        return LedgerType.ETHEREUM
+    return LedgerType.SOLANA
+
+
 def get_ledger_helper_by_chain(rpc: str, chain: ChainType) -> LedgerHelper:
     """Get ledger helper by chain type."""
     return CHAIN_HELPERS.get(chain, Ethereum)(rpc=rpc)
 
 
 def get_ledger_helper_by_ledger(rpc: str, ledger: LedgerHelper) -> LedgerHelper:
     """Get ledger helper by ledger type."""
```

### Comparing `olas_operate_middleware-0.1.0rc1/operate/ledger/base.py` & `olas_operate_middleware-0.1.0rc2/operate/ledger/base.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/ledger/ethereum.py` & `olas_operate_middleware-0.1.0rc2/operate/ledger/ethereum.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/ledger/profiles.py` & `olas_operate_middleware-0.1.0rc2/operate/ledger/profiles.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/ledger/solana.py` & `olas_operate_middleware-0.1.0rc2/operate/ledger/solana.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/resource.py` & `olas_operate_middleware-0.1.0rc2/operate/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.path = path
 
     @property
     def json(self) -> t.Dict:
         """To dictionary object."""
         obj = {}
         for pname, _ in self.__annotations__.items():
-            if pname.startswith("_"):
+            if pname.startswith("_") or pname == "path":
                 continue
             obj[pname] = serialize(self.__dict__[pname])
         return obj
 
     @classmethod
     def from_json(cls, obj: t.Dict) -> "LocalResource":
         """Load LocalResource from json."""
```

### Comparing `olas_operate_middleware-0.1.0rc1/operate/services/__init__.py` & `olas_operate_middleware-0.1.0rc2/operate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/services/manage.py` & `olas_operate_middleware-0.1.0rc2/operate/services/manage.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from operate.services.service import (
     Deployment,
     OnChainData,
     OnChainState,
     OnChainUserParams,
     Service,
 )
+from operate.wallet.master import MasterWalletManager
 
 
 # pylint: disable=redefined-builtin
 
 OPERATE = ".operate"
 CONFIG = "config.json"
 SERVICES = "services"
@@ -56,49 +57,48 @@
 class ServiceManager:
     """Service manager."""
 
     def __init__(
         self,
         path: Path,
         keys_manager: KeysManager,
-        master_key_path: Path,
+        wallet_manager: MasterWalletManager,
         logger: t.Optional[logging.Logger] = None,
     ) -> None:
         """
         Initialze service manager
 
         :param path: Path to service storage.
         :param keys: Keys manager.
         :param master_key_path: Path to master key.
         :param logger: logging.Logger object.
         """
         self.path = path
         self.keys_manager = keys_manager
-        self.master_key_path = master_key_path
+        self.wallet_manager = wallet_manager
         self.logger = logger or setup_logger(name="operate.manager")
 
     def setup(self) -> None:
         """Setup service manager."""
         self.path.mkdir(exist_ok=True)
-        self.keys_manager.setup()
 
     @property
     def json(self) -> t.List[t.Dict]:
         """Returns the list of available services."""
         data = []
         for path in self.path.iterdir():
             service = Service.load(path=path)
             data.append(service.json)
         return data
 
     def get_on_chain_manager(self, service: Service) -> OnChainManager:
         """Get OnChainManager instance."""
         return OnChainManager(
             rpc=service.ledger_config.rpc,
-            key=self.master_key_path,
+            wallet=self.wallet_manager.load(service.ledger_config.type),
             contracts=CONTRACTS[service.ledger_config.chain],
         )
 
     def create_or_load(
         self,
         hash: str,
         rpc: t.Optional[str] = None,
@@ -351,14 +351,45 @@
         ocm.unstake(
             service_id=service.chain_data.token,
             staking_contract=STAKING[service.ledger_config.chain],
         )
         service.chain_data.staked = False
         service.store()
 
+    def fund_service(self, hash: str) -> None:
+        """Fund service if required."""
+        service = self.create_or_load(hash=hash)
+        wallet = self.wallet_manager.load(ledger_type=service.ledger_config.type)
+        ledger_api = wallet.ledger_api(chain_type=service.ledger_config.chain)
+        agent_fund_requirement = service.chain_data.user_params.fund_requirements.agent
+
+        self.logger.info("Funding agents")
+        for key in service.keys:
+            agent_balance = ledger_api.get_balance(address=key.address)
+            if agent_balance < agent_fund_requirement:
+                to_transfer = agent_fund_requirement - agent_balance
+                self.logger.info(f"Transferring {to_transfer} units to {key.address}")
+                wallet.transfer(
+                    to=key.address,
+                    amount=to_transfer,
+                    chain_type=service.ledger_config.chain,
+                )
+
+        self.logger.info("Funding safe")
+        safe_fund_requirement = service.chain_data.user_params.fund_requirements.safe
+        safe_balanace = ledger_api.get_balance(wallet.safe)
+        if safe_balanace < safe_fund_requirement:
+            to_transfer = safe_fund_requirement - safe_balanace
+            self.logger.info(f"Transferring {to_transfer} units to {wallet.safe}")
+            wallet.transfer(
+                to=t.cast(str, wallet.safe),
+                amount=to_transfer,
+                chain_type=service.ledger_config.chain,
+            )
+
     def deploy_service_locally(self, hash: str, force: bool = False) -> Deployment:
         """
         Deploy service locally
 
         :param hash: Service hash
         :param force: Remove previous deployment and start a new one.
         """
```

### Comparing `olas_operate_middleware-0.1.0rc1/operate/services/protocol.py` & `olas_operate_middleware-0.1.0rc2/operate/services/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,144 +45,42 @@
 from hexbytes import HexBytes
 
 from operate.data import DATA_DIR
 from operate.data.contracts.service_staking_token.contract import (
     ServiceStakingTokenContract,
 )
 from operate.types import ContractAddresses
-
-
-ZERO_ETH = 0
+from operate.utils.gnosis import (
+    MultiSendOperation,
+    SafeOperation,
+    hash_payload_to_hex,
+    skill_input_hex_to_payload,
+)
+from operate.wallet.master import MasterWallet
 
 
 class StakingState(Enum):
     """Staking state enumeration for the staking."""
 
     UNSTAKED = 0
     STAKED = 1
     EVICTED = 2
 
 
-NULL_ADDRESS: str = "0x" + "0" * 40
-MAX_UINT256 = 2**256 - 1
-
-
-class SafeOperation(Enum):
-    """Operation types."""
-
-    CALL = 0
-    DELEGATE_CALL = 1
-    CREATE = 2
-
-
-class MultiSendOperation(Enum):
-    """Operation types."""
-
-    CALL = 0
-    DELEGATE_CALL = 1
-
-
-def hash_payload_to_hex(  # pylint: disable=too-many-arguments,too-many-locals
-    safe_tx_hash: str,
-    ether_value: int,
-    safe_tx_gas: int,
-    to_address: str,
-    data: bytes,
-    operation: int = SafeOperation.CALL.value,
-    base_gas: int = 0,
-    safe_gas_price: int = 0,
-    gas_token: str = NULL_ADDRESS,
-    refund_receiver: str = NULL_ADDRESS,
-    use_flashbots: bool = False,
-    gas_limit: int = 0,
-    raise_on_failed_simulation: bool = False,
-) -> str:
-    """Serialise to a hex string."""
-    if len(safe_tx_hash) != 64:  # should be exactly 32 bytes!
-        raise ValueError(
-            "cannot encode safe_tx_hash of non-32 bytes"
-        )  # pragma: nocover
-
-    if len(to_address) != 42 or len(gas_token) != 42 or len(refund_receiver) != 42:
-        raise ValueError("cannot encode address of non 42 length")  # pragma: nocover
-
-    if (
-        ether_value > MAX_UINT256
-        or safe_tx_gas > MAX_UINT256
-        or base_gas > MAX_UINT256
-        or safe_gas_price > MAX_UINT256
-        or gas_limit > MAX_UINT256
-    ):
-        raise ValueError(
-            "Value is bigger than the max 256 bit value"
-        )  # pragma: nocover
-
-    if operation not in [v.value for v in SafeOperation]:
-        raise ValueError("SafeOperation value is not valid")  # pragma: nocover
-
-    if not isinstance(use_flashbots, bool):
-        raise ValueError(
-            f"`use_flashbots` value ({use_flashbots}) is not valid. A boolean value was expected instead"
-        )
-
-    ether_value_ = ether_value.to_bytes(32, "big").hex()
-    safe_tx_gas_ = safe_tx_gas.to_bytes(32, "big").hex()
-    operation_ = operation.to_bytes(1, "big").hex()
-    base_gas_ = base_gas.to_bytes(32, "big").hex()
-    safe_gas_price_ = safe_gas_price.to_bytes(32, "big").hex()
-    use_flashbots_ = use_flashbots.to_bytes(32, "big").hex()
-    gas_limit_ = gas_limit.to_bytes(32, "big").hex()
-    raise_on_failed_simulation_ = raise_on_failed_simulation.to_bytes(32, "big").hex()
-
-    concatenated = (
-        safe_tx_hash
-        + ether_value_
-        + safe_tx_gas_
-        + to_address
-        + operation_
-        + base_gas_
-        + safe_gas_price_
-        + gas_token
-        + refund_receiver
-        + use_flashbots_
-        + gas_limit_
-        + raise_on_failed_simulation_
-        + data.hex()
-    )
-    return concatenated
-
-
-def skill_input_hex_to_payload(payload: str) -> dict:
-    """Decode payload."""
-    tx_params = dict(
-        safe_tx_hash=payload[:64],
-        ether_value=int.from_bytes(bytes.fromhex(payload[64:128]), "big"),
-        safe_tx_gas=int.from_bytes(bytes.fromhex(payload[128:192]), "big"),
-        to_address=payload[192:234],
-        operation=int.from_bytes(bytes.fromhex(payload[234:236]), "big"),
-        base_gas=int.from_bytes(bytes.fromhex(payload[236:300]), "big"),
-        safe_gas_price=int.from_bytes(bytes.fromhex(payload[300:364]), "big"),
-        gas_token=payload[364:406],
-        refund_receiver=payload[406:448],
-        use_flashbots=bool.from_bytes(bytes.fromhex(payload[448:512]), "big"),
-        gas_limit=int.from_bytes(bytes.fromhex(payload[512:576]), "big"),
-        raise_on_failed_simulation=bool.from_bytes(
-            bytes.fromhex(payload[576:640]), "big"
-        ),
-        data=bytes.fromhex(payload[640:]),
-    )
-    return tx_params
-
-
 class StakingManager(OnChainHelper):
     """Helper class for staking a service."""
 
-    def __init__(self, key: Path, chain_type: ChainType = ChainType.CUSTOM) -> None:
+    def __init__(
+        self,
+        key: Path,
+        chain_type: ChainType = ChainType.CUSTOM,
+        password: Optional[str] = None,
+    ) -> None:
         """Initialize object."""
-        super().__init__(key=key, chain_type=chain_type)
+        super().__init__(key=key, chain_type=chain_type, password=password)
         self.staking_ctr = t.cast(
             ServiceStakingTokenContract,
             ServiceStakingTokenContract.from_dir(
                 directory=str(DATA_DIR / "contracts" / "service_staking_token")
             ),
         )
 
@@ -357,20 +255,26 @@
             dry_run=False,
         )
 
 
 class OnChainManager:
     """On chain service management."""
 
-    def __init__(self, rpc: str, key: Path, contracts: ContractAddresses) -> None:
+    def __init__(
+        self,
+        rpc: str,
+        wallet: MasterWallet,
+        contracts: ContractAddresses,
+        chain_type: t.Optional[ChainType] = None,
+    ) -> None:
         """On chain manager."""
         self.rpc = rpc
-        self.key = key
-        self.chain_type = ChainType.CUSTOM
+        self.wallet = wallet
         self.contracts = contracts
+        self.chain_type = chain_type or ChainType.CUSTOM
 
     def _patch(self) -> None:
         """Patch contract and chain config."""
         ChainConfigs.get(self.chain_type).rpc = self.rpc
         if self.chain_type != ChainType.CUSTOM:
             return
 
@@ -379,25 +283,27 @@
 
     @property
     def crypto(self) -> Crypto:
         """Load crypto object."""
         self._patch()
         _, crypto = OnChainHelper.get_ledger_and_crypto_objects(
             chain_type=self.chain_type,
-            key=self.key,
+            key=self.wallet.key_path,
+            password=self.wallet.password,
         )
         return crypto
 
     @property
     def ledger_api(self) -> LedgerApi:
         """Load ledger api object."""
         self._patch()
         ledger_api, _ = OnChainHelper.get_ledger_and_crypto_objects(
             chain_type=self.chain_type,
-            key=self.key,
+            key=self.wallet.key_path,
+            password=self.wallet.password,
         )
         return ledger_api
 
     def info(self, token_id: int) -> t.Dict:
         """Get service info."""
         self._patch()
         ledger_api, _ = OnChainHelper.get_ledger_and_crypto_objects(
@@ -446,15 +352,16 @@
         token: t.Optional[str] = None,
     ) -> t.Dict:
         """Mint service."""
         # TODO: Support for update
         self._patch()
         manager = MintManager(
             chain_type=self.chain_type,
-            key=self.key,
+            key=self.wallet.key_path,
+            password=self.wallet.password,
             update_token=update_token,
         )
 
         # Prepare for minting
         (
             manager.load_package_configuration(
                 package_path=package_path, package_type=PackageType.SERVICE
@@ -465,25 +372,30 @@
             .publish_metadata()
         )
 
         with tempfile.TemporaryDirectory() as temp, contextlib.redirect_stdout(
             io.StringIO()
         ):
             with cd(temp):
-                method = (
-                    manager.mint_service
-                    if update_token is None
-                    else manager.update_service
-                )
-                method(
+                kwargs = dict(
                     number_of_slots=number_of_slots,
                     cost_of_bond=cost_of_bond,
                     threshold=threshold,
                     token=token,
                 )
+                # TODO: Enable after consulting smart contracts team re a safe
+                # being a service owner
+                # if update_token is None:
+                #     kwargs["owner"] = self.wallet.safe # noqa: F401
+                method = (
+                    manager.mint_service
+                    if update_token is None
+                    else manager.update_service
+                )
+                method(**kwargs)
                 (metadata,) = Path(temp).glob("*.json")
                 published = {
                     "token": int(Path(metadata).name.replace(".json", "")),
                     "metadata": json.loads(Path(metadata).read_text(encoding="utf-8")),
                 }
         return published
 
@@ -495,15 +407,16 @@
         """Activate service."""
         logging.info(f"Activating service {service_id}...")
         self._patch()
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
-                key=self.key,
+                key=self.wallet.key_path,
+                password=self.wallet.password,
             ).check_is_service_token_secured(
                 token=token,
             ).activate_service()
 
     def register(
         self,
         service_id: int,
@@ -513,15 +426,16 @@
     ) -> None:
         """Register instance."""
         logging.info(f"Registering service {service_id}...")
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
-                key=self.key,
+                key=self.wallet.key_path,
+                password=self.wallet.password,
             ).check_is_service_token_secured(
                 token=token,
             ).register_instance(
                 instances=instances,
                 agent_ids=agents,
             )
 
@@ -534,15 +448,16 @@
         """Deploy service."""
         logging.info(f"Deploying service {service_id}...")
         self._patch()
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
-                key=self.key,
+                key=self.wallet.key_path,
+                password=self.wallet.password,
             ).check_is_service_token_secured(
                 token=token,
             ).deploy_service(
                 reuse_multisig=reuse_multisig,
             )
 
     def swap(  # pylint: disable=too-many-arguments,too-many-locals
@@ -553,15 +468,16 @@
     ) -> None:
         """Swap safe owner."""
         logging.info(f"Swapping safe for service {service_id} [{multisig}]...")
         self._patch()
         manager = ServiceManager(
             service_id=service_id,
             chain_type=self.chain_type,
-            key=self.key,
+            key=self.wallet.key_path,
+            password=self.wallet.password,
         )
         with tempfile.TemporaryDirectory() as temp_dir:
             key_file = Path(temp_dir, "key.txt")
             key_file.write_text(owner_key, encoding="utf-8")
             owner_crypto = EthereumCrypto(private_key_path=str(key_file))
         owner_cryptos: list[EthereumCrypto] = [owner_crypto]
         owners = [
@@ -641,62 +557,67 @@
         """Terminate service."""
         logging.info(f"Terminating service {service_id}...")
         self._patch()
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
-                key=self.key,
+                key=self.wallet.key_path,
+                password=self.wallet.password,
             ).check_is_service_token_secured(
                 token=token,
             ).terminate_service()
 
     def unbond(self, service_id: int, token: t.Optional[str] = None) -> None:
         """Unbond service."""
         logging.info(f"Unbonding service {service_id}...")
         self._patch()
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
-                key=self.key,
+                key=self.wallet.key_path,
+                password=self.wallet.password,
             ).check_is_service_token_secured(
                 token=token,
             ).unbond_service()
 
     def staking_slots_available(self, staking_contract: str) -> bool:
         """Stake service."""
         self._patch()
         return StakingManager(
-            key=self.key,
+            key=self.wallet.key_path,
+            password=self.wallet.password,
             chain_type=self.chain_type,
         ).slots_available(
             staking_contract=staking_contract,
         )
 
     def stake(
         self,
         service_id: int,
         service_registry: str,
         staking_contract: str,
     ) -> None:
         """Stake service."""
         self._patch()
         StakingManager(
-            key=self.key,
+            key=self.wallet.key_path,
+            password=self.wallet.password,
             chain_type=self.chain_type,
         ).stake(
             service_id=service_id,
             service_registry=service_registry,
             staking_contract=staking_contract,
         )
 
     def unstake(self, service_id: int, staking_contract: str) -> None:
         """Unstake service."""
         self._patch()
         StakingManager(
-            key=self.key,
+            key=self.wallet.key_path,
+            password=self.wallet.password,
             chain_type=self.chain_type,
         ).unstake(
             service_id=service_id,
             staking_contract=staking_contract,
         )
```

### Comparing `olas_operate_middleware-0.1.0rc1/operate/services/service.py` & `olas_operate_middleware-0.1.0rc2/operate/services/service.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc1/operate/types.py` & `olas_operate_middleware-0.1.0rc2/operate/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 _CHAIN_ID_TO_CHAIN_NAME = {
     1: "ethereum",
     5: "goerli",
     100: "gnosis",
     1399811149: "solana",
 }
 
+_CHAIN_NAME_TO_ID = {val: key for key, val in _CHAIN_ID_TO_CHAIN_NAME.items()}
+
 _LEDGER_TYPE_TO_ENUM = {
     "ethereum": 0,
     "solana": 1,
 }
 
 
 class LedgerType(enum.IntEnum):
@@ -63,23 +65,38 @@
     SOLANA = 1
 
     @classmethod
     def from_string(cls, chain: str) -> "LedgerType":
         """Load from string."""
         return cls(_LEDGER_TYPE_TO_ENUM[chain.lower()])
 
+    @property
+    def config_file(self) -> str:
+        """Config filename."""
+        return f"{self.name.lower()}.json"
+
+    @property
+    def key_file(self) -> str:
+        """Key filename."""
+        return f"{self.name.lower()}.txt"
+
 
 class ChainType(enum.IntEnum):
     """Chain type enum."""
 
     ETHEREUM = 0
     GOERLI = 1
     GNOSIS = 2
     SOLANA = 3
 
+    @property
+    def id(self) -> int:
+        """Returns chain id."""
+        return _CHAIN_NAME_TO_ID[self.name.lower()]
+
     @classmethod
     def from_string(cls, chain: str) -> "ChainType":
         """Load from string."""
         return cls(_CHAIN_NAME_TO_ENUM[chain.lower()])
 
     @classmethod
     def from_id(cls, cid: int) -> "ChainType":
@@ -164,16 +181,16 @@
 
     volumes: t.Dict[str, str]
 
 
 class FundRequirementsTemplate(TypedDict):
     """Fund requirement template."""
 
-    agent: float
-    safe: float
+    agent: int
+    safe: int
 
 
 class ConfigurationTemplate(TypedDict):
     """Configuration template."""
 
     nft: str
     rpc: str
```

### Comparing `olas_operate_middleware-0.1.0rc1/pyproject.toml` & `olas_operate_middleware-0.1.0rc2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olas-operate-middleware"
-version = "0.1.0-rc1"
+version = "0.1.0-rc2"
 description = ""
 authors = ["David Vilela <dvilelaf@gmail.com>", "Viraj Patel <vptl185@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "operate" }
 ]
 include = [
@@ -15,16 +15,16 @@
 ]
 
 [tool.poetry.scripts]
 operate = "operate.cli:main"
 
 [tool.poetry.dependencies]
 python = "<4.0,>=3.8"
-open-autonomy = ">=0.14.7"
-open-aea-ledger-ethereum = ">=1.48.0.post1"
+open-autonomy = ">=0.14.10"
+open-aea-ledger-ethereum = ">=1.50.0"
 docker = "6.1.2"
 clea = ">=0.1.0rc4"
 starlette = ">=0.36.3"
 uvicorn = ">=0.27.0"
 requests-toolbelt = "1.0.0"
 fastapi = ">=0.110.0"
```

### Comparing `olas_operate_middleware-0.1.0rc1/PKG-INFO` & `olas_operate_middleware-0.1.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: olas-operate-middleware
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: 
 Author: David Vilela
 Author-email: dvilelaf@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: clea (>=0.1.0rc4)
 Requires-Dist: docker (==6.1.2)
 Requires-Dist: fastapi (>=0.110.0)
-Requires-Dist: open-aea-ledger-ethereum (>=1.48.0.post1)
-Requires-Dist: open-autonomy (>=0.14.7)
+Requires-Dist: open-aea-ledger-ethereum (>=1.50.0)
+Requires-Dist: open-autonomy (>=0.14.10)
 Requires-Dist: requests-toolbelt (==1.0.0)
 Requires-Dist: starlette (>=0.36.3)
 Requires-Dist: uvicorn (>=0.27.0)
 Description-Content-Type: text/markdown
 
 # Olas Operate
 Electron + NextJS + Python Backend application to one-click run Agents.
```

