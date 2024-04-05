# Comparing `tmp/simular_evm-0.2.1.tar.gz` & `tmp/simular_evm-0.2.2.tar.gz`

## Comparing `simular_evm-0.2.1.tar` & `simular_evm-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,38 @@
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 simular_evm-0.2.1/Cargo.toml
--rw-r--r--   0     1001      127     3198 2024-03-21 00:03:59.000000 simular_evm-0.2.1/.github/workflows/build-release.yml
--rw-r--r--   0     1001      127     1576 2024-03-21 00:03:59.000000 simular_evm-0.2.1/.github/workflows/mdbook.yml
--rw-r--r--   0     1001      127     1292 2024-03-21 00:03:59.000000 simular_evm-0.2.1/.github/workflows/test_pypi.yml
--rw-r--r--   0     1001      127      601 2024-03-21 00:03:59.000000 simular_evm-0.2.1/.gitignore
--rw-r--r--   0     1001      127    11354 2024-03-21 00:03:59.000000 simular_evm-0.2.1/LICENSE
--rw-r--r--   0     1001      127      291 2024-03-21 00:03:59.000000 simular_evm-0.2.1/Makefile
--rw-r--r--   0     1001      127     1625 2024-03-21 00:03:59.000000 simular_evm-0.2.1/README.md
--rw-r--r--   0     1001      127      794 2024-03-21 00:03:59.000000 simular_evm-0.2.1/bench/simple.py
--rw-r--r--   0     1001      127      344 2024-03-21 00:03:59.000000 simular_evm-0.2.1/docs/book.toml
--rw-r--r--   0     1001      127      235 2024-03-21 00:03:59.000000 simular_evm-0.2.1/docs/src/SUMMARY.md
--rw-r--r--   0     1001      127     3453 2024-03-21 00:03:59.000000 simular_evm-0.2.1/docs/src/getstarted.md
--rw-r--r--   0     1001      127     1342 2024-03-21 00:03:59.000000 simular_evm-0.2.1/docs/src/overview.md
--rw-r--r--   0     1001      127      258 2024-03-21 00:03:59.000000 simular_evm-0.2.1/docs/src/reference/contract.md
--rw-r--r--   0     1001      127     5515 2024-03-21 00:03:59.000000 simular_evm-0.2.1/docs/src/reference/pyabi.md
--rw-r--r--   0     1001      127     5321 2024-03-21 00:03:59.000000 simular_evm-0.2.1/docs/src/reference/pyevm.md
--rw-r--r--   0     1001      127       19 2024-03-21 00:03:59.000000 simular_evm-0.2.1/docs/src/reference/utils.md
--rw-r--r--   0     1001      127      102 2024-03-21 00:03:59.000000 simular_evm-0.2.1/simular/__init__.py
--rw-r--r--   0     1001      127     4687 2024-03-21 00:03:59.000000 simular_evm-0.2.1/simular/contract.py
--rw-r--r--   0     1001      127     4290 2024-03-21 00:03:59.000000 simular_evm-0.2.1/simular/utils.py
--rw-r--r--   0     1001      127     6640 2024-03-21 00:03:59.000000 simular_evm-0.2.1/src/core/abi.rs
--rw-r--r--   0     1001      127    15424 2024-03-21 00:03:59.000000 simular_evm-0.2.1/src/core/baseevm.rs
--rw-r--r--   0     1001      127       69 2024-03-21 00:03:59.000000 simular_evm-0.2.1/src/core/mod.rs
--rw-r--r--   0     1001      127      463 2024-03-21 00:03:59.000000 simular_evm-0.2.1/src/core/snapshot.rs
--rw-r--r--   0     1001      127      256 2024-03-21 00:03:59.000000 simular_evm-0.2.1/src/lib.rs
--rw-r--r--   0     1001      127      695 2024-03-21 00:03:59.000000 simular_evm-0.2.1/src/py/mod.rs
--rw-r--r--   0     1001      127     6285 2024-03-21 00:03:59.000000 simular_evm-0.2.1/src/py/pyabi.rs
--rw-r--r--   0     1001      127     4789 2024-03-21 00:03:59.000000 simular_evm-0.2.1/src/py/pyevm.rs
--rw-r--r--   0     1001      127      911 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/conftest.py
--rw-r--r--   0     1001      127    26594 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/fixtures/KitchenSink.json
--rw-r--r--   0     1001      127      787 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/fixtures/contracts/KitchenSink.sol
--rw-r--r--   0     1001      127      653 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/fixtures/contracts/MockERC20.sol
--rw-r--r--   0     1001      127     4031 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/fixtures/erc20.abi
--rw-r--r--   0     1001      127     8722 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/fixtures/erc20.bin
--rw-r--r--   0     1001      127      288 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/fixtures/usdc_addresses.json
--rw-r--r--   0     1001      127    53190 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/fixtures/usdc_cache.json
--rw-r--r--   0     1001      127     1376 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/test_contract.py
--rw-r--r--   0     1001      127     2878 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/test_pyabi.py
--rw-r--r--   0     1001      127     1821 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/test_pyevm.py
--rw-r--r--   0     1001      127      933 2024-03-21 00:03:59.000000 simular_evm-0.2.1/tests/test_snapshot.py
--rw-r--r--   0     1001      127    90661 2024-03-21 00:04:07.000000 simular_evm-0.2.1/Cargo.lock
--rw-r--r--   0     1001      127     1285 2024-03-21 00:03:59.000000 simular_evm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 simular_evm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 simular_evm-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      127     3198 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.github/workflows/build-release.yml
+-rw-r--r--   0     1001      127     1576 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.github/workflows/mdbook.yml
+-rw-r--r--   0     1001      127     1292 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.github/workflows/test_pypi.yml
+-rw-r--r--   0     1001      127      610 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.gitignore
+-rw-r--r--   0     1001      127      817 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.readthedocs.yaml
+-rw-r--r--   0     1001      127    11354 2024-04-05 13:15:29.000000 simular_evm-0.2.2/LICENSE
+-rw-r--r--   0     1001      127      327 2024-04-05 13:15:29.000000 simular_evm-0.2.2/Makefile
+-rw-r--r--   0     1001      127     1805 2024-04-05 13:15:29.000000 simular_evm-0.2.2/README.md
+-rw-r--r--   0     1001      127      806 2024-04-05 13:15:29.000000 simular_evm-0.2.2/bench/simple.py
+-rw-r--r--   0     1001      127     1116 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/conf.py
+-rw-r--r--   0     1001      127     2645 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/contract.rst
+-rw-r--r--   0     1001      127       17 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/evm.rst
+-rw-r--r--   0     1001      127      854 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/getstarted.rst
+-rw-r--r--   0     1001      127     1398 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/index.rst
+-rw-r--r--   0     1001      127      800 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/make.bat
+-rw-r--r--   0     1001      127       37 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/requirements.txt
+-rw-r--r--   0     1001      127      145 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/toc.rst
+-rw-r--r--   0     1001      127       31 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/utils.rst
+-rw-r--r--   0     1001      127       86 2024-04-05 13:15:29.000000 simular_evm-0.2.2/simular/__init__.py
+-rw-r--r--   0     1001      127     4876 2024-04-05 13:15:29.000000 simular_evm-0.2.2/simular/contract.py
+-rw-r--r--   0     1001      127     4081 2024-04-05 13:15:29.000000 simular_evm-0.2.2/simular/utils.py
+-rw-r--r--   0     1001      127      541 2024-04-05 13:15:29.000000 simular_evm-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      127     2509 2024-04-05 13:15:29.000000 simular_evm-0.2.2/src/pyabi.rs
+-rw-r--r--   0     1001      127     6141 2024-04-05 13:15:29.000000 simular_evm-0.2.2/src/pyevm.rs
+-rw-r--r--   0     1001      127      753 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/conftest.py
+-rw-r--r--   0     1001      127    26594 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/KitchenSink.json
+-rw-r--r--   0     1001      127      787 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/contracts/KitchenSink.sol
+-rw-r--r--   0     1001      127      653 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/contracts/MockERC20.sol
+-rw-r--r--   0     1001      127     4031 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/erc20.abi
+-rw-r--r--   0     1001      127     8722 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/erc20.bin
+-rw-r--r--   0     1001      127      288 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/usdc_addresses.json
+-rw-r--r--   0     1001      127     2221 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/test_contract.py
+-rw-r--r--   0     1001      127     1633 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/test_pyabi.py
+-rw-r--r--   0     1001      127     1592 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/test_pyevm.py
+-rw-r--r--   0     1001      127    90177 2024-04-05 13:15:35.000000 simular_evm-0.2.2/Cargo.lock
+-rw-r--r--   0     1001      127     1429 2024-04-05 13:15:29.000000 simular_evm-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 simular_evm-0.2.2/PKG-INFO
```

### Comparing `simular_evm-0.2.1/.github/workflows/build-release.yml` & `simular_evm-0.2.2/.github/workflows/build-release.yml`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/.github/workflows/mdbook.yml` & `simular_evm-0.2.2/.github/workflows/mdbook.yml`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/.github/workflows/test_pypi.yml` & `simular_evm-0.2.2/.github/workflows/test_pypi.yml`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/.gitignore` & `simular_evm-0.2.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -57,7 +57,8 @@
 tests/dump_usdc.py
 
 # Mdbook
 docs/book
 
 todo.md
 
+uniswap/
```

### Comparing `simular_evm-0.2.1/LICENSE` & `simular_evm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/README.md` & `simular_evm-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 # Simular
 
+[![pypi](https://img.shields.io/pypi/v/simular-evm.svg)](https://pypi.python.org/pypi/simular-evm)
+
 A Python smart-contract API with a fast (embedded) Ethereum Virtual Machine (EVM). `Simular` creates a Python wrapper around production grade Rust based Ethereum APIs.
 
 How is it different than Brownie, Ganache, Anvil?
 - It's only an EVM, no blocks or mining
 - No HTTP/JSON-RPC. You talk directly to the EVM (and it's fast)
 - Full functionality: account transfers, contract interaction, etc...
 
@@ -13,21 +15,21 @@
 ## Features
 - `EVM`: run a local version with an in-memory database, or fork db state from a remote node.
 - `Snapshot`: dump the current state of the EVM to json for future use in pre-populating EVM storage
 - `ABI`: parse compiled Solidity json files or define a specific set of functions using `human-readable` notation
 - `Contract`: high-level, user-friendy Python API
 
 ## Build from source
-- You need `Rust`, `Python/Poetry`, and optionally `Make`.
-- Create a local Python virtual environment.  With Poetry, run `poetry install`
-- Run `make build` or run `poetry run maturin develop`
+- You need `Rust` and `Python`, and optionally `Make`. We use `hatch` for Python project management, but it's not required
+- Create a local Python virtual environment. Within that environment install Python dependencies
+- Run `make build` or `hatch run maturin develop`
 - See `simular/` for the main python api
 
 ## Getting Started
-See [Simular Documentation](https://simular-fi.github.io/simular/) for examples and API details.
+See [Simular Documentation](https://simular.readthedocs.io/en/latest/) for examples and API details.
 
 ## Standing on the shoulders of giants...
 Thanks to the following projects for making this work possible!
 - [pyO3](https://github.com/PyO3)
 - [revm](https://github.com/bluealloy/revm)
 - [alloy-rs](https://github.com/alloy-rs)
 - [eth_utils/eth_abi](https://eth-utils.readthedocs.io/en/stable/)
```

### Comparing `simular_evm-0.2.1/docs/src/overview.md` & `simular_evm-0.2.2/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,45 @@
+.. _index:
+
+simular
+=======
+
+**Simular** is a Python API you can use to deploy and interact with Ethereum 
+smart contracts and an embedded Ethereum Virtual Machine (EVM). It creates a 
+Python wrapper around production grade Rust based Ethereum APIs making it very fast.
 
-**Simular** is a Python API you can use to deploy and interact with Ethereum smart contracts and an embedded Ethereum Virtual Machine (EVM). It creates a Python wrapper around production grade Rust based Ethereum APIs making it very fast.
 
 How is it different than Brownie, Ganache, Anvil?
+
 - It's only an EVM. It doesn't include blocks and mining
 - No HTTP/JSON-RPC. You talk directly to the EVM (and it's fast)
 - Full functionality: account transfers, contract interaction, and more.
 
-The primary motivation for this work is to be able to model smart contract interaction in an Agent Based Modeling environment like [Mesa](https://mesa.readthedocs.io/en/main/).
+The primary motivation for this work is to be able to model smart contract 
+interaction in an Agent Based Modeling environment 
+like `Mesa <https://mesa.readthedocs.io/en/main/>`_.
 
-## Features
-- `EVM`: run a local version with an in-memory database, or fork db state from a remote node.
-- `Snapshot`: dump the current state of the EVM to json for future use in pre-populating EVM storage
-- `ABI`: parse compiled Solidity json files or define a specific set of functions using `human-readable` notation
-- `Contract/Utilities`: high-level, user-friendy Python API
+Features
+--------
 
+- Run a local version with an in-memory database. Or fork db state from a remote node.
+- Parse compiled Solidity json files or define a specific set of functions using `human-readable` notation
+- Dump the current state of the EVM to json for future use in pre-populating EVM storage
+- User-friendy Python API
+
+
+Standing on the shoulders of giants...
+--------------------------------------
 
-## Standing on the shoulders of giants...
 Thanks to the following projects for making this work possible!
-- [pyO3](https://github.com/PyO3)
-- [revm](https://github.com/bluealloy/revm)
-- [alloy-rs](https://github.com/alloy-rs)
-- [eth_utils/eth_abi](https://eth-utils.readthedocs.io/en/stable/) 
+
+- `pyO3 <https://github.com/PyO3>`_
+- `revm <https://github.com/bluealloy/revm>`_
+- `alloy-rs <https://github.com/alloy-rs>`_
+- `eth_utils/eth_abi <https://eth-utils.readthedocs.io/en/stable/>`_ 
+
+
+.. include:: toc.rst
+
+
+
+
```

### Comparing `simular_evm-0.2.1/simular/contract.py` & `simular_evm-0.2.2/simular/contract.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 """
 Wraps pyo3 code to provide a high-level contract API
 """
 
-from eth_abi import encode, decode
 from eth_utils import is_address
 import typing
 
-from .simular import PyEvmLocal, PyAbi, PyEvmFork
+from .simular import PyEvm, PyAbi
+
+
+def convert_for_soltypes(args: typing.Tuple):
+    if len(args) == 1:
+        i = str(args[0]).replace("'", "")
+        return f"({i})"
+    return str(args).replace("'", "")
 
 
 class Function:
     """
     Contains information needed to interact with a contract function
     """
 
-    def __init__(
-        self,
-        contract_address: str,
-        name: str,
-        client: PyEvmLocal | PyEvmLocal,
-        abi: PyAbi,
-    ):
+    def __init__(self, evm: PyEvm, abi: PyAbi, contract_address: str, name: str):
         self.name = name
-        self.client = client
+        self.evm = evm
         self.abi = abi
         self.contract_address = contract_address
 
     def call(self, *args):
         """
         Make a read-only call to the contract, returning any results. Solidity
         read-only calls are marked as `view` or `pure`. Does not commit any state
         changes to the Evm.
 
         - `args`: 0 or more expected arguments to the function
+
         Returns: the decoded result
         """
         if not self.contract_address:
             raise Exception("missing contract address. see at() method")
 
-        encoded, output_params = self.abi.encode_function_input(self.name, args)
-        (bits, _) = self.client.call(self.contract_address, encoded)
+        stargs = convert_for_soltypes(args)
+        result = self.evm.call(self.name, stargs, self.contract_address, self.abi)
+        if len(result) == 1:
+            return result[0]
+        return result
 
-        return self.__decode_output(output_params, bytes(bits))
+    def simulate(self, *args, caller: str = None, value: int = 0):
+        """
+        Simulate a write call to the contract w/o changing state.
+        """
+        if not self.contract_address:
+            raise Exception("missing contract address. see at() method")
+
+        if not is_address(caller):
+            raise Exception("caller is missing or is not a valid address")
+
+        stargs = convert_for_soltypes(args)
+        result = self.evm.simulate(
+            self.name, stargs, caller, self.contract_address, value, self.abi
+        )
+        if len(result) == 1:
+            return result[0]
+        return result
 
     def transact(self, *args, caller: str = None, value: int = 0):
         """
         Make a write call to the contract changing the state of the Evm.
         - `args`: 0 or more expected arguments to the function
         - `caller`: the address of the caller. This translates to `msg.sender` in a Solidity
         - `value` : an optional amount of Ether to send with the value ... `msg.value`
@@ -53,32 +73,25 @@
         """
         if not self.contract_address:
             raise Exception("missing contract address. see at() method")
 
         if not is_address(caller):
             raise Exception("caller is missing or is not a valid address")
 
-        encoded, output_params = self.abi.encode_function_input(self.name, args)
-        (bits, _) = self.client.transact(caller, self.contract_address, encoded, value)
-        return self.__decode_output(output_params, bytes(bits))
-
-    def __decode_output(self, params: typing.List[str], rawbits: bytes):
-        """
-        internal. Decodes the resulting bytes from the Evm into respective Python value(s)
-        based on the output type parameters of the Solidity function.
-        """
-        decoded = decode(params, rawbits)
-        if len(decoded) == 1:
-            return decoded[0]
-        else:
-            return decoded
+        stargs = convert_for_soltypes(args)
+        result = self.evm.transact(
+            self.name, stargs, caller, self.contract_address, value, self.abi
+        )
+        if len(result) == 1:
+            return result[0]
+        return result
 
 
 class Contract:
-    def __init__(self, evm: PyEvmLocal | PyEvmFork, abi: PyAbi):
+    def __init__(self, evm: PyEvm, abi: PyAbi):
         """
         Instantiate a contract from an ABI.
 
         Maps contract functions to this class.  Making function available
         as attributes on the Contract.
 
         See `utils.py` for helper functions to create a Contract
@@ -92,42 +105,48 @@
         Make solidity contract methods available as method calls. For a given function name,
         return `Function`.
 
         For example, if the ABI has the contract function 'function hello(uint256)',
         you can invoke it by name: contract.hello.transact(10)
         """
         if self.abi.has_function(name):
-            return Function(self.address, name, self.evm, self.abi)
+            return Function(self.evm, self.abi, self.address, name)
         else:
             raise Exception(f"contract function: '{name}' not found!")
 
     def at(self, address: str) -> "Contract":
         """
-        Set the contract address. Note: this is automatically set when using deploy
-        - `address`: the address of a deployed contract
-        Return self
+        Set the contract address.
+
+        .. note::
+            this is automatically set when using deploy``
+
+        Parameters
+        ----------
+        address: str
+            the address of a deployed contract
+
+        Returns
+        -------
+            self
         """
         self.address = address
         return self
 
-    def deploy(self, caller: str, args=[], value: int = 0) -> str:
+    def deploy(self, *args, caller: str = None, value: int = 0) -> str:
         """
         Deploy the contract, returning it's deployed address
         - `caller`: the address of the requester...`msg.sender`
         - `args`: a list of args (if any)
         - `value`: optional amount of Ether for the contract
         Returns the address of the deployed contract
         """
-        constructor_params = self.abi.constructor_input_types()
-        bytecode = self.abi.bytecode()
+        if not caller:
+            raise Exception("Missing required 'caller' address")
 
-        if not constructor_params and len(args) > 0:
-            raise Exception("constructor doesn't take any args")
-
-        if constructor_params:
-            if len(constructor_params) != len(args):
-                raise Exception("wrong number of args for the constructor")
-            bytecode += encode(constructor_params, args)
+        if not is_address(caller):
+            raise Exception("'caller' is not a valid ethereum address")
 
-        addr = self.evm.deploy(caller, bytecode, value)
+        stargs = convert_for_soltypes(args)
+        addr = self.evm.deploy(stargs, caller, value, self.abi)
         self.address = addr
         return addr
```

### Comparing `simular_evm-0.2.1/simular/utils.py` & `simular_evm-0.2.2/simular/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,114 +2,112 @@
 Helper functions
 """
 
 from secrets import token_hex
 from eth_utils import to_wei, is_address
 import typing
 
-from . import PyEvmLocal, PyAbi, PyEvmFork, Contract
+from . import PyEvm, PyAbi, Contract
+
+
+def ether_to_wei(value: int) -> int:
+    """Convert ether to wei"""
+    return to_wei(value, "ether")
 
 
 def generate_random_address() -> str:
-    """
-    Generate a random hex encoded account/wallet address
+    """Generate a random hex encoded account/wallet address
 
     Returns: the address
     """
     return "0x" + token_hex(20)
 
 
-def create_account(
-    evm: PyEvmLocal | PyEvmFork, address: str = None, value: int = 0
-) -> str:
+def create_account(evm: PyEvm, address: str = None, value: int = 0) -> str:
     """
-    Create an account in the EVM.
-    - evm    : PyEvmLocal | PyEvmForm.  the EVM client
+    Create an account
+
+    - evm    : PyEvm.  the EVM client
     - address: str  optional. if set it will be used for the account address.
                               Otherwise a random address will be generated.
-    - value  : int  optional. create an initial balance for the account in ether
+    - value  : int  optional. create an initial balance for the account in wei
 
     Returns: the address
     """
-    if not isinstance(evm, (PyEvmLocal, PyEvmFork)):
+    if not isinstance(evm, PyEvm):
         raise Exception("'evm' should be an instance of either PyEvmLocal or PyEvmFork")
 
-    wei = to_wei(value, "ether")
     if not address:
         address = generate_random_address()
-        evm.create_account(address, wei)
+        evm.create_account(address, value)
         return address
 
     if not is_address(address):
         raise Exception("'address' does not appear to be a valid Ethereum address")
 
-    evm.create_account(address, wei)
+    evm.create_account(address, value)
     return address
 
 
-def create_many_accounts(
-    evm: PyEvmLocal | PyEvmFork, num: int, value: int = 0
-) -> typing.List[str]:
+def create_many_accounts(evm: PyEvm, num: int, value: int = 0) -> typing.List[str]:
     """
     Create many accounts in the EVM
-    - evm    : PyEvmLocal | PyEvmForm.  the EVM client
+    - evm    : PyEvm.  the EVM client
     - num    : int  the number of accounts to create
-    - value  : int  optional. create an initial balance for each account in ether
+    - value  : int  optional. create an initial balance for each account in wei
 
     Returns a list of addresses
     """
     return [create_account(evm, value=value) for _ in range(num)]
 
 
-def contract_from_raw_abi(evm: PyEvmLocal | PyEvmFork, raw_abi: str) -> Contract:
+def contract_from_raw_abi(evm: PyEvm, raw_abi: str) -> Contract:
     """
     Create the contract given the full ABI. Full ABI should include
     `abi` and `bytecode`. This is usually a single json file from a compiled Solidity contract.
 
-    - `evm`     : PyEvmLocal | PyEvmForm.  the EVM client
+    - `evm`     : PyEvm.  the EVM client
     - `raw_abi` : abi file as un-parsed json
     Returns an instance of Contract
     """
-    if not isinstance(evm, (PyEvmLocal, PyEvmFork)):
+    if not isinstance(evm, PyEvm):
         raise Exception("'evm' should be an instance of either PyEvmLocal or PyEvmFork")
 
     if not isinstance(raw_abi, str):
         raise Exception("expected a an un-parsed json file")
 
-    abi = PyAbi.load_from_json(raw_abi)
+    abi = PyAbi.from_full_json(raw_abi)
     return Contract(evm, abi)
 
 
 def contract_from_abi_bytecode(
-    evm: PyEvmLocal | PyEvmFork, raw_abi: str, bytecode: bytes
+    evm: PyEvm, raw_abi: str, bytecode: bytes = None
 ) -> Contract:
     """
     Create a contract given the abi and bytecode.
 
-    - `evm`     : PyEvmLocal | PyEvmForm.  the EVM client
+    - `evm`     : PyEvm  the EVM client
     - `raw_abi` : abi file as un-parsed json
-    - `bytecode`: bytes
+    - `bytecode`: Optional bytes
     Returns an instance of Contract
     """
-    if not isinstance(evm, (PyEvmLocal, PyEvmFork)):
+    if not isinstance(evm, PyEvm):
         raise Exception("'evm' should be an instance of either PyEvmLocal or PyEvmFork")
 
     if not isinstance(raw_abi, str):
         raise Exception("expected a an un-parsed json file")
 
-    abi = PyAbi.load_from_parts(raw_abi, bytecode)
+    abi = PyAbi.from_abi_bytecode(raw_abi, bytecode)
     return Contract(evm, abi)
 
 
-def contract_from_inline_abi(
-    evm: PyEvmLocal | PyEvmFork, abi: typing.List[str]
-) -> Contract:
+def contract_from_inline_abi(evm: PyEvm, abi: typing.List[str]) -> Contract:
     """
     Create the contract using inline ABI.
-    - `evm` : PyEvmLocal | PyEvmForm.  the EVM client
+    - `evm` : PyEvm.  the EVM client
     - `abi` : a list of strings that describe the solidity functions of interest.
     Returns an instance of Contract
 
     Function are described in the format: 'function NAME(PARAMETER TYPES) (RETURN TYPES)'
     where:
     `NAME` if the function name
     `PARAMETER TYPES are 0 or more solidity types of any arguments to the function
@@ -119,12 +117,12 @@
     Examples:
     - "function hello(uint256,uint256)`: hello function the expects 2 int arguments and returns nothing
     - "function hello()(uint256)"`: hello function with no arguments and return an int
 
     abi = ['function hello()(uint256)', 'function world(string) (string)']
 
     """
-    if not isinstance(evm, (PyEvmLocal, PyEvmFork)):
+    if not isinstance(evm, PyEvm):
         raise Exception("'evm' should be an instance of either PyEvmLocal or PyEvmFork")
 
-    abi = PyAbi.load_from_human_readable(abi)
+    abi = PyAbi.from_human_readable(abi)
     return Contract(evm, abi)
```

### Comparing `simular_evm-0.2.1/tests/conftest.py` & `simular_evm-0.2.2/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 from pathlib import Path
-import json
 
-from simular import PyEvmLocal
+from simular import PyEvm
 
 PATH = Path(__file__).parent
 
 
 @pytest.fixture
 def bob():
     return "0xed6ff00ae6a64df0bf28e159c4a48311b931f458"
@@ -15,15 +14,15 @@
 @pytest.fixture
 def alice():
     return "0x0091410228bf6062ab28c949ba4172ee9144bfde"
 
 
 @pytest.fixture
 def evm():
-    return PyEvmLocal()
+    return PyEvm()
 
 
 @pytest.fixture
 def erc20abi():
     with open(f"{PATH}/./fixtures/erc20.abi") as f:
         ercabi = f.read()
     return ercabi
@@ -38,14 +37,7 @@
 
 
 @pytest.fixture
 def kitchen_sink_json():
     with open(f"{PATH}/./fixtures/KitchenSink.json") as f:
         rawabi = f.read()
     return rawabi
-
-
-@pytest.fixture
-def usdc_cache():
-    with open(f"{PATH}/./fixtures/usdc_cache.json") as f:
-        cache = f.read()
-    return cache
```

### Comparing `simular_evm-0.2.1/tests/fixtures/KitchenSink.json` & `simular_evm-0.2.2/tests/fixtures/KitchenSink.json`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/tests/fixtures/contracts/KitchenSink.sol` & `simular_evm-0.2.2/tests/fixtures/contracts/KitchenSink.sol`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/tests/fixtures/contracts/MockERC20.sol` & `simular_evm-0.2.2/tests/fixtures/contracts/MockERC20.sol`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/tests/fixtures/erc20.abi` & `simular_evm-0.2.2/tests/fixtures/erc20.abi`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/tests/fixtures/erc20.bin` & `simular_evm-0.2.2/tests/fixtures/erc20.bin`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.1/tests/test_contract.py` & `simular_evm-0.2.2/tests/test_contract.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pytest
 
 from simular import (
     contract_from_abi_bytecode,
     contract_from_raw_abi,
     create_account,
-    PyEvmLocal,
+    PyEvm,
     contract_from_inline_abi,
+    ether_to_wei,
 )
 
 
 def test_loading_contracts(evm):
     with pytest.raises(BaseException):
         contract_from_raw_abi(evm, "")
 
@@ -22,15 +23,15 @@
 
 def test_contract_interface(evm, bob, alice, erc20abi, erc20bin):
     create_account(evm, alice, 0)
     create_account(evm, bob, 0)
 
     erc20 = contract_from_abi_bytecode(evm, erc20abi, erc20bin)
 
-    erc20.deploy(bob, ("USD Coin", "USDC", 6))
+    erc20.deploy("USD Coin", "USDC", 6, caller=bob)
     contract_address = erc20.address
 
     assert erc20.name.call() == "USD Coin"
     assert erc20.decimals.call() == 6
     assert erc20.owner.call() == bob
 
     erc20.mint.transact(alice, 10, caller=bob)
@@ -39,13 +40,36 @@
     assert 10 == erc20.totalSupply.call()
 
     with pytest.raises(BaseException):
         # alice can't mint, she's not the owner!
         erc20.mint.transact(alice, 10, caller=alice)
 
     # Test state
-    evm2 = PyEvmLocal()
-    evm2.load_state(evm.dump_state())
+    evm2 = PyEvm.from_snapshot(evm.create_snapshot())
 
     erc20again = contract_from_inline_abi(evm2, ["function totalSupply() (uint256)"])
     erc20again.at(contract_address)
     assert 10 == erc20again.totalSupply.call()
+
+
+def test_deploy_and_test_kitchensink(evm, alice, kitchen_sink_json):
+    create_account(evm, alice, ether_to_wei(2))
+    a = contract_from_raw_abi(evm, kitchen_sink_json)
+
+    # fail on value with a non-payable constructor
+    with pytest.raises(BaseException):
+        a.deploy(caller=alice, value=1)
+
+    assert a.deploy(caller=alice)
+
+    assert 1 == a.increment.transact(caller=alice)
+    assert [2, 3] == a.increment.transact(2, caller=alice)
+    assert 4 == a.increment.simulate(caller=alice)
+    assert 3 == a.value.call()
+    assert alice == a.setInput.transact((1, 2, alice), caller=alice)
+
+    # receive
+    one_ether = ether_to_wei(1)
+    assert 0 == evm.get_balance(a.address)
+    evm.transfer(alice, a.address, one_ether)
+    assert one_ether == evm.get_balance(alice)
+    assert one_ether == evm.get_balance(a.address)
```

### Comparing `simular_evm-0.2.1/tests/test_pyabi.py` & `simular_evm-0.2.2/tests/test_pyabi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,41 @@
 from simular import PyAbi
 
 
 def test_load_from_parts(erc20abi, erc20bin):
-    abi = PyAbi.load_from_parts(erc20abi, erc20bin)
+    abi = PyAbi.from_abi_bytecode(erc20abi, erc20bin)
     assert abi.has_function("mint")
     assert abi.has_function("burn")
     assert not abi.has_fallback()
     assert not abi.has_receive()
 
-    assert ["string", "string", "uint8"] == abi.constructor_input_types()
-
     addy = "0xa32f31673577f7a717716d8b88d85a9e7bbb76d3"
-    (sig1, output) = abi.encode_function_input("mint", (addy, 2))
+    (sig1, _, _) = abi.encode_function("mint", f"({addy}, 2)")
     hexed = bytes.hex(bytes(sig1))
     og = "40c10f19000000000000000000000000a32f31673577f7a717716d8b88d85a9e7bbb76d30000000000000000000000000000000000000000000000000000000000000002"
     assert og == hexed
-    assert output == []
 
-    (sig2, output2) = abi.encode_function_input("name", ())
+    (sig2, _, _) = abi.encode_function("name", "()")
     hexed2 = bytes.hex(bytes(sig2))
     assert "06fdde03" == hexed2
-    assert output2 == ["string"]
-
-    assert len(abi.bytecode()) > 100
 
 
 def test_load_from_human_readable():
     funcs = ["function mint(address, uint256)", "function name()(string)"]
-    abi = PyAbi.load_from_human_readable(funcs)
+    abi = PyAbi.from_human_readable(funcs)
     assert abi.has_function("mint")
     assert abi.has_function("name")
 
-    addy = "0xa32f31673577f7a717716d8b88d85a9e7bbb76d3"
-    (sig1, output) = abi.encode_function_input("mint", (addy, 2))
-    hexed = bytes.hex(bytes(sig1))
-    og = "40c10f19000000000000000000000000a32f31673577f7a717716d8b88d85a9e7bbb76d30000000000000000000000000000000000000000000000000000000000000002"
-    assert og == hexed
-    assert output == []
-
-    (sig2, output2) = abi.encode_function_input("name", ())
-    hexed2 = bytes.hex(bytes(sig2))
-    assert "06fdde03" == hexed2
-    assert output2 == ["string"]
-
-    assert None == abi.bytecode()
-
 
 def test_load_full_json_abi(kitchen_sink_json):
-    abi = PyAbi.load_from_json(kitchen_sink_json)
+    abi = PyAbi.from_full_json(kitchen_sink_json)
     assert abi.has_function("increment")
     assert abi.has_function("setInput")
     assert abi.has_receive()
-    assert not abi.constructor_input_types()
-
-    inc_no_args = "d09de08a"
-    (sig1, output1) = abi.encode_function_input("increment", ())
-    hexed1 = bytes.hex(bytes(sig1))
-    assert hexed1 == inc_no_args
-    assert ["uint256"] == output1
-
-    inc_with_args = (
-        "7cf5dab00000000000000000000000000000000000000000000000000000000000000002"
-    )
-    (sig2, output2) = abi.encode_function_input("increment", (2,))
-    hexed2 = bytes.hex(bytes(sig2))
-    assert hexed2 == inc_with_args
-    assert ["uint256", "uint256"] == output2
+    assert (abi.bytecode(), False) == abi.encode_constructor("()")
 
     with_struct = "fa6a38d200000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000003000000000000000000000000a32f31673577f7a717716d8b88d85a9e7bbb76d3"
-    (sig3, output3) = abi.encode_function_input(
-        "setInput", (2, 3, "0xa32f31673577f7a717716d8b88d85a9e7bbb76d3")
+    (sig3, _, _) = abi.encode_function(
+        "setInput", "((2, 3, 0xa32f31673577f7a717716d8b88d85a9e7bbb76d3))"
     )
     hexed3 = bytes.hex(bytes(sig3))
     assert with_struct == hexed3
-    assert ["address"] == output3
```

### Comparing `simular_evm-0.2.1/tests/test_pyevm.py` & `simular_evm-0.2.2/tests/test_pyevm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from eth_utils import to_wei
 from eth_abi import decode
 
-from simular import PyEvmLocal, PyAbi
+from simular import PyEvm, PyAbi
 
 
 def test_create_account_and_balance(evm, bob):
     two_ether = to_wei(2, "ether")
 
     assert evm.get_balance(bob) == 0
     evm.create_account(bob, two_ether)
@@ -29,37 +29,28 @@
         # bob doesn't have enough...
         evm.transfer(bob, alice, two_ether)
 
     assert evm.get_balance(bob) == one_ether
     assert evm.get_balance(alice) == one_ether
 
     # dump and reload state...
-    state = evm.dump_state()
-
-    evm2 = PyEvmLocal()
-    evm2.load_state(state)
+    state = evm.create_snapshot()
+    evm2 = PyEvm.from_snapshot(state)
 
     assert evm2.get_balance(bob) == one_ether
     assert evm2.get_balance(alice) == one_ether
 
 
 def test_contract_raw_interaction(evm, bob, kitchen_sink_json):
-    abi = PyAbi.load_from_json(kitchen_sink_json)
+    abi = PyAbi.from_full_json(kitchen_sink_json)
     bytecode = abi.bytecode()
 
-    contract_address = evm.deploy(bob, bytecode, 0)
-    (enc, _) = abi.encode_function_input("increment", ())
+    contract_address = evm.deploy("()", bob, 0, abi)
+    (enc, _, _) = abi.encode_function("increment", "()")
 
     with pytest.raises(BaseException):
         evm.transact(bob, "Ox01", enc, 0)
 
-    evm.transact(bob, contract_address, enc, 0)
+    evm.transact("increment", "()", bob, contract_address, 0, abi)
 
-    (enc1, output_params) = abi.encode_function_input("value", ())
-    (result, _) = evm.call(contract_address, enc1)
-    decoded = decode(output_params, bytes(result))
-    assert decoded[0] == 1
-
-    r = evm.view_storage_slot(contract_address, 0)
-    # NOTE: little endian bytes!
-    slot_value = int.from_bytes(r, "little")
-    assert slot_value == 1
+    (enc1, _, _) = abi.encode_function("value", "()")
+    assert [1] == evm.call("value", "()", contract_address, abi)
```

### Comparing `simular_evm-0.2.1/Cargo.lock` & `simular_evm-0.2.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -42,46 +42,46 @@
 name = "allocator-api2"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
 name = "alloy-dyn-abi"
-version = "0.6.4"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2919acdad13336bc5dc26b636cdd6892c2f27fb0d4a58320a00c2713cf6a4e9a"
+checksum = "872f239c15befa27cc4f0d3d82a70b3365c2d0202562bf906eb93b299fa31882"
 dependencies = [
  "alloy-json-abi",
  "alloy-primitives",
  "alloy-sol-type-parser",
  "alloy-sol-types",
  "const-hex",
  "itoa",
  "serde",
  "serde_json",
  "winnow 0.6.5",
 ]
 
 [[package]]
 name = "alloy-json-abi"
-version = "0.6.4"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24ed0f2a6c3a1c947b4508522a53a190dba8f94dcd4e3e1a5af945a498e78f2f"
+checksum = "83a35ddfd27576474322a5869e4c123e5f3e7b2177297c18e4e82ea501cb125b"
 dependencies = [
  "alloy-primitives",
  "alloy-sol-type-parser",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "alloy-primitives"
-version = "0.6.4"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "600d34d8de81e23b6d909c094e23b3d357e01ca36b78a8c5424c501eedbe86f0"
+checksum = "99bbad0a6b588ef4aec1b5ddbbfdacd9ef04e00b979617765b03174318ee1f3a"
 dependencies = [
  "alloy-rlp",
  "arbitrary",
  "bytes",
  "cfg-if",
  "const-hex",
  "derive_arbitrary",
@@ -107,45 +107,64 @@
 dependencies = [
  "arrayvec",
  "bytes",
 ]
 
 [[package]]
 name = "alloy-sol-macro"
-version = "0.6.4"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86ec0a47740b20bc5613b8712d0d321d031c4efc58e9645af96085d5cccfc27"
+checksum = "452d929748ac948a10481fff4123affead32c553cf362841c5103dd508bdfc16"
 dependencies = [
+ "alloy-json-abi",
+ "alloy-sol-macro-input",
  "const-hex",
- "dunce",
- "heck",
+ "heck 0.4.1",
  "indexmap",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
  "syn-solidity",
  "tiny-keccak",
 ]
 
 [[package]]
+name = "alloy-sol-macro-input"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df64e094f6d2099339f9e82b5b38440b159757b6920878f28316243f8166c8d1"
+dependencies = [
+ "alloy-json-abi",
+ "const-hex",
+ "dunce",
+ "heck 0.5.0",
+ "proc-macro2",
+ "quote",
+ "serde_json",
+ "syn 2.0.58",
+ "syn-solidity",
+]
+
+[[package]]
 name = "alloy-sol-type-parser"
-version = "0.6.4"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0045cc89524e1451ccf33e8581355b6027ac7c6e494bb02959d4213ad0d8e91d"
+checksum = "715f4d09a330cc181fc7c361b5c5c2766408fa59a0bac60349dcb7baabd404cc"
 dependencies = [
  "winnow 0.6.5",
 ]
 
 [[package]]
 name = "alloy-sol-types"
-version = "0.6.4"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad09ec5853fa700d12d778ad224dcdec636af424d29fad84fb9a2f16a5b0ef09"
+checksum = "43bc2d6dfc2a19fd56644494479510f98b1ee929e04cf0d4aa45e98baa3e545b"
 dependencies = [
+ "alloy-json-abi",
  "alloy-primitives",
  "alloy-sol-macro",
  "const-hex",
  "serde",
 ]
 
 [[package]]
@@ -288,21 +307,21 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "async-trait"
-version = "0.1.78"
+version = "0.1.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "461abc97219de0eaaf81fe3ef974a540158f3d079c2ab200f891f1a2ef201e85"
+checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "async_io_stream"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6d7b9decdf35d8908a7e3ef02f64c5e9b1695e230154c0e8de3969142d9b94c"
@@ -326,28 +345,28 @@
 name = "auto_impl"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c87f3f15e7794432337fc718554eaa4dc8f04c9677a950ffe366f20a162ae42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -426,26 +445,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
-name = "blst"
-version = "0.3.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c94087b935a822949d3291a9989ad2b2051ea141eda0fd4e478a75f6aa3e604b"
-dependencies = [
- "cc",
- "glob",
- "threadpool",
- "zeroize",
-]
-
-[[package]]
 name = "bumpalo"
 version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "byte-slice-cast"
@@ -457,32 +464,18 @@
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
-dependencies = [
- "serde",
-]
-
-[[package]]
-name = "c-kzg"
-version = "1.0.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3130f3d8717cc02e668a896af24984d5d5d4e8bf12e278e982e0f1bd88a0f9af"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 dependencies = [
- "blst",
- "cc",
- "glob",
- "hex",
- "libc",
  "serde",
 ]
 
 [[package]]
 name = "cc"
 version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -492,17 +485,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "const-hex"
 version = "1.11.3"
@@ -585,17 +578,17 @@
 name = "data-encoding"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
 
 [[package]]
 name = "der"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fffa369a668c8af7dbf8b5e56c9f744fbd399949ed171606040001947de40b1c"
+checksum = "f55bf8e7b65898637379c1b74eb1551107c8294ed26d855ceb9fd1a09cfc9bc0"
 dependencies = [
  "const-oid",
  "zeroize",
 ]
 
 [[package]]
 name = "deranged"
@@ -621,15 +614,15 @@
 name = "derive_arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
@@ -744,15 +737,15 @@
 name = "enumn"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fd000fd6988e73bbe993ea3db9b1aa64906ab88766d654973924340c8cddb42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -889,17 +882,17 @@
  "wasm-bindgen-futures",
  "web-sys",
  "ws_stream_wasm",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "fastrlp"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "139834ddba373bbdd213dffe02c8d110508dcf1726c2be27e8d1f7d7e1856418"
 dependencies = [
@@ -1019,15 +1012,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1100,20 +1093,14 @@
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
-name = "glob"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
-
-[[package]]
 name = "gloo-timers"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b995a66bb87bebce9a0f4a95aed01daca4872c050bfcb21653361c03bc35e5c"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -1130,17 +1117,17 @@
  "ff",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.25"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fbd2820c5e49886948654ab546d0688ff24530286bdcf8fca3cefb16d4618eb"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -1173,14 +1160,20 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "heck"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
+
+[[package]]
 name = "hermit-abi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
@@ -1337,27 +1330,27 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
@@ -1383,17 +1376,17 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
@@ -1488,23 +1481,23 @@
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -1655,15 +1648,15 @@
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
 dependencies = [
  "proc-macro-crate 3.1.0",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
@@ -1721,15 +1714,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1741,17 +1734,17 @@
 checksum = "5cff92b6f71555b61bb9315f7c64da3ca43d87531622120fea0195fc761b4843"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.101"
+version = "0.9.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dda2b0f344e78efc2facf7d195d098df0dd72151b26ab98da807afc26c198dff"
+checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
@@ -1824,17 +1817,17 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pest"
-version = "2.7.8"
+version = "2.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56f8023d0fb78c8e03784ea1c7f3fa36e68a723138990b8d5a47d916b651e7a8"
+checksum = "311fb059dee1a7b802f036316d790138c613a4e8b180c822e3925a662e9f0c95"
 dependencies = [
  "memchr",
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
@@ -1860,22 +1853,22 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -2021,14 +2014,15 @@
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
+ "anyhow",
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -2063,28 +2057,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
@@ -2150,17 +2144,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -2173,17 +2167,17 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
@@ -2223,62 +2217,56 @@
  "web-sys",
  "webpki-roots",
  "winreg",
 ]
 
 [[package]]
 name = "revm"
-version = "7.2.0"
+version = "8.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24fd3ed4b62dc61c647552d8b781811ae25ec74d23309055077e4dfb392444d2"
+checksum = "72a454c1c650b2b2e23f0c461af09e6c31e1d15e1cbebe905a701c46b8a50afc"
 dependencies = [
  "auto_impl",
  "cfg-if",
  "dyn-clone",
- "ethers-core",
- "ethers-providers",
  "revm-interpreter",
  "revm-precompile",
- "serde",
- "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "revm-interpreter"
-version = "3.4.0"
+version = "4.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f0a1818f8c876b0d71a0714217c34da7df8a42c0462750768779d55680e4554"
+checksum = "d322f2730cd300e99d271a1704a2dfb8973d832428f5aa282aaa40e2473b5eec"
 dependencies = [
  "revm-primitives",
  "serde",
 ]
 
 [[package]]
 name = "revm-precompile"
-version = "5.1.0"
+version = "6.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a9645a70f1df1e5bd7fa8718b9ba486fac9c3f0467aa6b58e7f590d5f6fd0f7"
+checksum = "931f692f3f4fc72ec39d5d270f8e9d208c4a6008de7590ee96cf948e3b6d3f8d"
 dependencies = [
  "aurora-engine-modexp",
- "c-kzg",
  "k256",
  "once_cell",
  "revm-primitives",
  "ripemd",
- "secp256k1",
  "sha2",
  "substrate-bn",
 ]
 
 [[package]]
 name = "revm-primitives"
-version = "3.1.0"
+version = "3.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "323ad597cf75ac9cb1d161be29fcc3562426f0278a1d04741697fca556e1ceea"
+checksum = "cbbc9640790cebcb731289afb7a7d96d16ad94afeb64b5d0b66443bd151e79d6"
 dependencies = [
  "alloy-primitives",
  "auto_impl",
  "bitflags 2.5.0",
  "bitvec",
  "cfg-if",
  "dyn-clone",
@@ -2486,29 +2474,29 @@
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "scale-info"
-version = "2.11.0"
+version = "2.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ef2175c2907e7c8bc0a9c3f86aeb5ec1f3b275300ad58a44d0c3ae379a5e52e"
+checksum = "788745a868b0e751750388f4e6546eb921ef714a4317fa6954f7cde114eb2eb7"
 dependencies = [
  "cfg-if",
  "derive_more",
  "parity-scale-codec",
  "scale-info-derive",
 ]
 
 [[package]]
 name = "scale-info-derive"
-version = "2.11.0"
+version = "2.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "634d9b8eb8fd61c5cdd3390d9b2132300a7e7618955b98b8416f118c1b4e144f"
+checksum = "7dc2f4e8bc344b9fc3d5f74f72c2e55bfc38d28dc2ebc69c194a3df424e4d9ac"
 dependencies = [
  "proc-macro-crate 1.3.1",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
@@ -2548,50 +2536,31 @@
  "generic-array",
  "pkcs8",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
-name = "secp256k1"
-version = "0.28.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d24b59d129cdadea20aea4fb2352fa053712e5d713eee47d700cd4b2bc002f10"
-dependencies = [
- "rand",
- "secp256k1-sys",
-]
-
-[[package]]
-name = "secp256k1-sys"
-version = "0.9.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d1746aae42c19d583c3c1a8c646bfad910498e2051c551a7f2e3c0c9fbb7eb"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "security-framework"
-version = "2.9.2"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
+checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.1"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
+checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
@@ -2642,24 +2611,23 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
- "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
@@ -2735,28 +2703,47 @@
  "num-traits",
  "thiserror",
  "time",
 ]
 
 [[package]]
 name = "simular"
-version = "0.2.1"
+version = "0.2.2"
+dependencies = [
+ "alloy-dyn-abi",
+ "alloy-primitives",
+ "anyhow",
+ "hex",
+ "pyo3",
+ "serde",
+ "serde_json",
+ "simular-core",
+]
+
+[[package]]
+name = "simular-core"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0bd839cfebd76e663b021d026a55cf201bf61579f4cc3ce79b6aa87b1a853f5"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-json-abi",
  "alloy-primitives",
+ "alloy-sol-types",
  "anyhow",
+ "ethers-core",
  "ethers-providers",
  "hex",
  "openssl",
- "pyo3",
  "reqwest",
  "revm",
  "serde",
  "serde_json",
+ "thiserror",
+ "tokio",
 ]
 
 [[package]]
 name = "slab"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
@@ -2819,19 +2806,19 @@
 
 [[package]]
 name = "strum_macros"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "substrate-bn"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b5bbfa79abbae15dd642ea8176a21a635ff3c00059961d1ea27ad04e5b441c"
@@ -2858,33 +2845,33 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.53"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn-solidity"
-version = "0.6.4"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb3d0961cd53c23ea94eeec56ba940f636f6394788976e9f16ca5ee0aca7464a"
+checksum = "4497156948bd342b52038035a6fa514a89626e37af9d2c52a5e8d8ebcc7ee479"
 dependencies = [
  "paste",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
@@ -2947,24 +2934,15 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
-]
-
-[[package]]
-name = "threadpool"
-version = "1.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
-dependencies = [
- "num_cpus",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
@@ -3016,17 +2994,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
@@ -3039,15 +3017,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3155,15 +3133,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -3359,15 +3337,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3393,15 +3371,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -3647,15 +3625,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
@@ -3667,9 +3645,9 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
```

### Comparing `simular_evm-0.2.1/pyproject.toml` & `simular_evm-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.maturin]
 features = ["pyo3/extension-module"]
 sdist-include = ["LICENSE", "README.md"]
 
 
 [project]
 name = "simular-evm"
-version = "0.2.1"
+version = "0.2.2"
 requires-python = ">=3.11"
 authors = [
     { name = "Dave Bryson", email = "davebryson@users.noreply.github.com" },
 ]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/simular-fi/simular"
@@ -28,13 +28,22 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = ["eth-abi>=4.1.0", "eth-utils>=2.2.0"]
 
 [tool.hatch.envs.dev]
-dependencies = ["pytest>=7.4.0", "black>=23.7.0", "maturin>=1.1.0"]
+dependencies = [
+    "pytest>=7.4.0",
+    "black>=23.7.0",
+    "maturin>=1.1.0",
+    "sphinx>=7.2.6",
+    "sphinx_rtd_theme>=2.0.0",
+]
+
+[tool.hatch.envs.dev.scripts]
+docs = "sphinx-build -M html docs docs/build"
 
 [project.urls]
 Source = "https://github.com/simular-fi/simular"
 Documentation = "https://simular-fi.github.io/simular"
 Issues = "https://github.com/simular-fi/simular/issues"
```

### Comparing `simular_evm-0.2.1/PKG-INFO` & `simular_evm-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: simular-evm
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: eth-abi >=4.1.0
 Requires-Dist: eth-utils >=2.2.0
@@ -20,14 +20,16 @@
 Project-URL: Source, https://github.com/simular-fi/simular
 Project-URL: Documentation, https://simular-fi.github.io/simular
 Project-URL: Issues, https://github.com/simular-fi/simular/issues
 
 
 # Simular
 
+[![pypi](https://img.shields.io/pypi/v/simular-evm.svg)](https://pypi.python.org/pypi/simular-evm)
+
 A Python smart-contract API with a fast (embedded) Ethereum Virtual Machine (EVM). `Simular` creates a Python wrapper around production grade Rust based Ethereum APIs.
 
 How is it different than Brownie, Ganache, Anvil?
 - It's only an EVM, no blocks or mining
 - No HTTP/JSON-RPC. You talk directly to the EVM (and it's fast)
 - Full functionality: account transfers, contract interaction, etc...
 
@@ -36,21 +38,21 @@
 ## Features
 - `EVM`: run a local version with an in-memory database, or fork db state from a remote node.
 - `Snapshot`: dump the current state of the EVM to json for future use in pre-populating EVM storage
 - `ABI`: parse compiled Solidity json files or define a specific set of functions using `human-readable` notation
 - `Contract`: high-level, user-friendy Python API
 
 ## Build from source
-- You need `Rust`, `Python/Poetry`, and optionally `Make`.
-- Create a local Python virtual environment.  With Poetry, run `poetry install`
-- Run `make build` or run `poetry run maturin develop`
+- You need `Rust` and `Python`, and optionally `Make`. We use `hatch` for Python project management, but it's not required
+- Create a local Python virtual environment. Within that environment install Python dependencies
+- Run `make build` or `hatch run maturin develop`
 - See `simular/` for the main python api
 
 ## Getting Started
-See [Simular Documentation](https://simular-fi.github.io/simular/) for examples and API details.
+See [Simular Documentation](https://simular.readthedocs.io/en/latest/) for examples and API details.
 
 ## Standing on the shoulders of giants...
 Thanks to the following projects for making this work possible!
 - [pyO3](https://github.com/PyO3)
 - [revm](https://github.com/bluealloy/revm)
 - [alloy-rs](https://github.com/alloy-rs)
 - [eth_utils/eth_abi](https://eth-utils.readthedocs.io/en/stable/)
```

