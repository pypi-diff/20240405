# Comparing `tmp/ain-py-1.1.0.tar.gz` & `tmp/ain-py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ain-py-1.1.0.tar", last modified: Wed Mar 13 01:46:49 2024, max compression
+gzip compressed data, was "ain-py-1.2.0.tar", last modified: Fri Apr  5 02:13:19 2024, max compression
```

## Comparing `ain-py-1.1.0.tar` & `ain-py-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-03-13 01:46:49.530880 ain-py-1.1.0/
--rw-r--r--   0 dongilseo   (501) staff       (20)     1778 2024-03-13 01:46:49.530017 ain-py-1.1.0/PKG-INFO
--rw-r--r--   0 dongilseo   (501) staff       (20)      707 2024-03-05 01:53:30.000000 ain-py-1.1.0/README.md
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-03-13 01:46:49.517951 ain-py-1.1.0/ain/
--rw-r--r--   0 dongilseo   (501) staff       (20)        0 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/__init__.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     2154 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/account.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     9740 2024-03-05 01:53:30.000000 ain-py-1.1.0/ain/ain.py
--rw-r--r--   0 dongilseo   (501) staff       (20)       38 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/constants.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-03-13 01:46:49.520250 ain-py-1.1.0/ain/db/
--rw-r--r--   0 dongilseo   (501) staff       (20)      844 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/db/__init__.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     2312 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/db/push_id.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    18994 2024-03-05 01:53:30.000000 ain-py-1.1.0/ain/db/ref.py
--rw-r--r--   0 dongilseo   (501) staff       (20)      420 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/errors.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     1605 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/net.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     2326 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/provider.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-03-13 01:46:49.521803 ain-py-1.1.0/ain/signer/
--rw-r--r--   0 dongilseo   (501) staff       (20)     2283 2024-03-05 01:53:30.000000 ain-py-1.1.0/ain/signer/__init__.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     6728 2024-03-05 01:53:30.000000 ain-py-1.1.0/ain/signer/default_signer.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    13973 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/types.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-03-13 01:46:49.523309 ain-py-1.1.0/ain/utils/
--rw-r--r--   0 dongilseo   (501) staff       (20)    20474 2024-03-05 01:53:30.000000 ain-py-1.1.0/ain/utils/__init__.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    10552 2023-08-31 04:32:09.000000 ain-py-1.1.0/ain/utils/v3keystore.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    14142 2024-03-05 01:53:30.000000 ain-py-1.1.0/ain/wallet.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-03-13 01:46:49.529223 ain-py-1.1.0/ain_py.egg-info/
--rw-r--r--   0 dongilseo   (501) staff       (20)     1778 2024-03-13 01:46:49.000000 ain-py-1.1.0/ain_py.egg-info/PKG-INFO
--rw-r--r--   0 dongilseo   (501) staff       (20)      562 2024-03-13 01:46:49.000000 ain-py-1.1.0/ain_py.egg-info/SOURCES.txt
--rw-r--r--   0 dongilseo   (501) staff       (20)        1 2024-03-13 01:46:49.000000 ain-py-1.1.0/ain_py.egg-info/dependency_links.txt
--rw-r--r--   0 dongilseo   (501) staff       (20)        1 2024-03-13 01:46:49.000000 ain-py-1.1.0/ain_py.egg-info/not-zip-safe
--rw-r--r--   0 dongilseo   (501) staff       (20)      136 2024-03-13 01:46:49.000000 ain-py-1.1.0/ain_py.egg-info/requires.txt
--rw-r--r--   0 dongilseo   (501) staff       (20)        4 2024-03-13 01:46:49.000000 ain-py-1.1.0/ain_py.egg-info/top_level.txt
--rw-r--r--   0 dongilseo   (501) staff       (20)       38 2024-03-13 01:46:49.531134 ain-py-1.1.0/setup.cfg
--rw-r--r--   0 dongilseo   (501) staff       (20)     1546 2024-03-13 01:22:56.000000 ain-py-1.1.0/setup.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-03-13 01:46:49.528133 ain-py-1.1.0/tests/
--rw-r--r--   0 dongilseo   (501) staff       (20)    33146 2024-03-05 01:53:30.000000 ain-py-1.1.0/tests/test_ain.py
--rw-r--r--   0 dongilseo   (501) staff       (20)      950 2023-08-31 04:32:09.000000 ain-py-1.1.0/tests/test_ain_account.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    11096 2023-08-31 04:32:09.000000 ain-py-1.1.0/tests/test_ain_raw.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    23247 2024-03-05 01:53:30.000000 ain-py-1.1.0/tests/test_ain_utils.py
+drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.407527 ain-py-1.2.0/
+-rw-r--r--   0 dongilseo   (501) staff       (20)     1778 2024-04-05 02:13:19.404497 ain-py-1.2.0/PKG-INFO
+-rw-r--r--   0 dongilseo   (501) staff       (20)      707 2024-03-13 06:12:07.000000 ain-py-1.2.0/README.md
+drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.388115 ain-py-1.2.0/ain/
+-rw-r--r--   0 dongilseo   (501) staff       (20)        0 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/__init__.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)     2154 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/account.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)    14690 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/ain.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)       38 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/constants.py
+drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.390369 ain-py-1.2.0/ain/db/
+-rw-r--r--   0 dongilseo   (501) staff       (20)      844 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/db/__init__.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)     2312 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/db/push_id.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)    20683 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/db/ref.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)      420 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/errors.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)     2436 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/net.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)     2601 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/provider.py
+drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.392189 ain-py-1.2.0/ain/signer/
+-rw-r--r--   0 dongilseo   (501) staff       (20)     2283 2024-03-13 06:12:07.000000 ain-py-1.2.0/ain/signer/__init__.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)     6728 2024-03-13 06:12:07.000000 ain-py-1.2.0/ain/signer/default_signer.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)    14237 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/types.py
+drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.394374 ain-py-1.2.0/ain/utils/
+-rw-r--r--   0 dongilseo   (501) staff       (20)    20474 2024-03-25 00:42:04.000000 ain-py-1.2.0/ain/utils/__init__.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)    10552 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/utils/v3keystore.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)    16311 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/wallet.py
+drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.401980 ain-py-1.2.0/ain_py.egg-info/
+-rw-r--r--   0 dongilseo   (501) staff       (20)     1778 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/PKG-INFO
+-rw-r--r--   0 dongilseo   (501) staff       (20)      562 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/SOURCES.txt
+-rw-r--r--   0 dongilseo   (501) staff       (20)        1 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/dependency_links.txt
+-rw-r--r--   0 dongilseo   (501) staff       (20)        1 2024-03-13 01:46:49.000000 ain-py-1.2.0/ain_py.egg-info/not-zip-safe
+-rw-r--r--   0 dongilseo   (501) staff       (20)      136 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/requires.txt
+-rw-r--r--   0 dongilseo   (501) staff       (20)        4 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/top_level.txt
+-rw-r--r--   0 dongilseo   (501) staff       (20)       38 2024-04-05 02:13:19.407763 ain-py-1.2.0/setup.cfg
+-rw-r--r--   0 dongilseo   (501) staff       (20)     1546 2024-04-05 02:04:58.000000 ain-py-1.2.0/setup.py
+drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.400479 ain-py-1.2.0/tests/
+-rw-r--r--   0 dongilseo   (501) staff       (20)    41295 2024-04-05 01:51:54.000000 ain-py-1.2.0/tests/test_ain.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)      950 2023-08-31 04:32:09.000000 ain-py-1.2.0/tests/test_ain_account.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)    11096 2023-08-31 04:32:09.000000 ain-py-1.2.0/tests/test_ain_raw.py
+-rw-r--r--   0 dongilseo   (501) staff       (20)    23247 2024-03-25 00:42:04.000000 ain-py-1.2.0/tests/test_ain_utils.py
```

### Comparing `ain-py-1.1.0/PKG-INFO` & `ain-py-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ain-py
-Version: 1.1.0
+Version: 1.2.0
 Summary: AI Network Client Library for Python3
 Home-page: https://github.com/ainblockchain/ain-py
 Author: AIN Dev Team
 Author-email: dev@ainetwork.ai
 License: MPL license
 Keywords: ain,ainetwork,ainblockchain,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ain-py-1.1.0/README.md` & `ain-py-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/ain/account.py` & `ain-py-1.2.0/ain/account.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/ain/ain.py` & `ain-py-1.2.0/ain/ain.py`

 * *Files 26% similar despite different names*

```diff
@@ -60,105 +60,314 @@
         Args:
             signer (Signer): The signer to set.
         """
         self.signer = signer
 
     # TODO(kriii): Return objects typing.
 
-    async def getBlock(
+    async def getLastBlock(self) -> Any:
+        """Fetches the last block.
+
+        Args:
+
+        Returns:
+            The last block.
+        """
+        return await self.provider.send(
+            "ain_getLastBlock", {}
+        )
+
+    async def getLastBlockNumber(self) -> int:
+        """Fetches the last block number.
+
+        Args:
+
+        Returns:
+            The last block number.
+        """
+        return await self.provider.send(
+            "ain_getLastBlockNumber", {}
+        )
+
+    async def getBlockByNumber(
         self,
-        blockHashOrBlockNumber: Union[str, int],
+        blockNumber: int,
         returnTransactionObjects: bool = False,
     ) -> Any:
-        """Gets a block with the given hash or block number.
+        """Gets a block with the given block number.
 
         Args:
-            blockHashOrBlockNumber (Union[str, int]): The block hash or the block number.
+            blockNumber (int): The block number.
             returnTransactionObjects (bool): If `True`, returns the full transaction objects.
                 If `False`, returns only the transaction hashes. Default to `False`.
         
         Returns:
-            The block with the given hash or block number.
+            The block with the given block number.
         """
-        if type(blockHashOrBlockNumber) is str:
-            return await self.provider.send(
-                "ain_getBlockByHash",
-                {
-                    "getFullTransactions": returnTransactionObjects,
-                    "hash": blockHashOrBlockNumber,
-                },
-            )
-        elif type(blockHashOrBlockNumber) is int:
-            return await self.provider.send(
-                "ain_getBlockByNumber",
-                {
-                    "getFullTransactions": returnTransactionObjects,
-                    "number": blockHashOrBlockNumber,
-                },
-            )
-        else:
-            raise TypeError("blockHashOrBlockNumber has invalid type")
+        return await self.provider.send(
+            "ain_getBlockByNumber",
+            {
+                "getFullTransactions": returnTransactionObjects,
+                "number": blockNumber,
+            },
+        )
 
-    async def getProposer(
+    async def getBlockByHash(
         self,
-        blockHashOrBlockNumber: Union[str, int],
+        blockHash: str,
+        returnTransactionObjects: bool = False,
     ) -> Any:
-        """Gets an address of the proposer of the given block.
+        """Gets a block with the given block hash.
 
         Args:
-            blockHashOrBlockNumber (Union[str, int]): The block hash or the block number.
+            blockHash (str): The block hash.
+            returnTransactionObjects (bool): If `True`, returns the full transaction objects.
+                If `False`, returns only the transaction hashes. Default to `False`.
+        
+        Returns:
+            The block with the given block hash.
+        """
+        return await self.provider.send(
+            "ain_getBlockByHash",
+            {
+                "getFullTransactions": returnTransactionObjects,
+                "hash": blockHash,
+            },
+        )
+
+    async def getBlockList(
+        self,
+        begin: int,
+        end: int,
+    ) -> List[Any]:
+        """"Fetches blocks with a block number range.
 
+        Args:
+            begin (int): The begining block number (inclusive).
+            end (int): The ending block number (exclusive).
+        
         Returns:
-            The address of the proposer of the given block.
+            The block list.
+        """
+        return await self.provider.send(
+            "ain_getBlockList",
+            {
+                "from": begin,
+                "to": end,
+            },
+        )
+
+    async def getBlockHeadersList(
+        self,
+        begin: int,
+        end: int,
+    ) -> List[Any]:
+        """Fetches block headers with a block number range.
+
+        Args:
+            begin (int): The begining block number (inclusive).
+            end (int): The ending block number (exclusive).
+        
+        Returns:
+            The block headers list.
+        """
+        return await self.provider.send(
+            "ain_getBlockHeadersList",
+            {
+                "from": begin,
+                "to": end,
+            },
+        )
+
+    async def getBlockTransactionCountByNumber(
+        self,
+        blockNumber: int,
+    ) -> int:
+        """Fetches block transaction count with a block number.
+
+        Args:
+            blockNumber (int): The block number.
+        
+        Returns:
+            The block transaction count.
+        """
+        return await self.provider.send(
+            "ain_getBlockTransactionCountByNumber",
+            {
+                "number": blockNumber,
+            },
+        )
+
+    async def getBlockTransactionCountByHash(
+        self,
+        blockHash: str,
+    ) -> int:
+        """Fetches block transaction count with a block hash.
+
+        Args:
+            blockHash (str): The block hash.
+        
+        Returns:
+            The block transaction count.
+        """
+        return await self.provider.send(
+            "ain_getBlockTransactionCountByHash",
+            {
+                "hash": blockHash,
+            },
+        )
+
+    async def getValidatorInfo(
+        self,
+        address: str,
+    ) -> Any:
+        """Fetches the information of the given validator address.
+
+        Args:
+            address (str): The block number.
+        
+        Returns:
+            The validator information.
         """
-        if type(blockHashOrBlockNumber) is str:
-            return await self.provider.send(
-                "ain_getProposerByHash", {"hash": blockHashOrBlockNumber}
-            )
-        elif type(blockHashOrBlockNumber) is int:
-            return await self.provider.send(
-                "ain_getProposerByNumber", {"number": blockHashOrBlockNumber}
-            )
-        else:
-            raise TypeError("blockHashOrBlockNumber has invalid type")
+        return await self.provider.send(
+            "ain_getValidatorInfo",
+            {
+                "address": address,
+            },
+        )
 
-    async def getValidators(
+    async def getValidatorsByNumber(
         self,
-        blockHashOrBlockNumber: Union[str, int],
+        blockNumber: int,
     ) -> Any:
-        """Gets the list of validators for a given block
+        """Fetches the validator list of a block with a block number.
 
         Args:
-            blockHashOrBlockNumber (Union[str, int]): The block hash or the block number.
+            blockNumber (int): The block number.
             
         Returns:
-            The list of validators for a given block.
+            The list of validators of the given block.
+        """
+        return await self.provider.send(
+            "ain_getValidatorsByNumber", {"number": blockNumber}
+        )
+
+    async def getValidatorsByHash(
+        self,
+        blockHash: str,
+    ) -> Any:
+        """Fetches the validator list of a block with a block hash.
+
+        Args:
+            blockHash (str): The block hash.
+            
+        Returns:
+            The list of validators of the given block.
+        """
+        return await self.provider.send(
+            "ain_getValidatorsByHash", {"hash": blockHash}
+        )
+
+    async def getProposerByNumber(
+        self,
+        blockNumber: int,
+    ) -> str:
+        """Fetches the block proproser's address of a block with a block number.
+
+        Args:
+            blockNumber (int): The block number.
+
+        Returns:
+            The address of the proposer of the given block.
+        """
+        return await self.provider.send(
+            "ain_getProposerByNumber", {"number": blockNumber}
+        )
+
+    async def getProposerByHash(
+        self,
+        blockHash: str,
+    ) -> str:
+        """Fetches the block proproser's address of a block with a block hash.
+
+        Args:
+            blockHash (str): The block hash.
+
+        Returns:
+            The address of the proposer of the given block.
+        """
+        return await self.provider.send(
+            "ain_getProposerByHash", {"hash": blockHash}
+        )
+
+    async def getPendingTransactions(self) -> Any:
+        """Fetches pending transactions.
+
+        Args:
+
+        Returns:
+            The pending transactions.
+        """
+        return await self.provider.send("ain_getPendingTransactions", {})
+
+    async def getTransactionPoolSizeUtilization(self) -> Any:
+        """Fetches transaction pool size utilization.
+
+        Args:
+
+        Returns:
+            The transaction pool size utilization.
         """
-        if type(blockHashOrBlockNumber) is str:
-            return await self.provider.send(
-                "ain_getValidatorsByHash", {"hash": blockHashOrBlockNumber}
-            )
-        elif type(blockHashOrBlockNumber) is int:
-            return await self.provider.send(
-                "ain_getValidatorsByNumber", {"number": blockHashOrBlockNumber}
-            )
-        else:
-            raise TypeError("blockHashOrBlockNumber has invalid type")
+        return await self.provider.send("ain_getTransactionPoolSizeUtilization", {})
 
-    async def getTransaction(self, transactionHash: str) -> Any:
+    async def getTransactionByHash(self, transactionHash: str) -> Any:
         """Gets a transaction with the given transaction hash.
 
         Args:
             transactionHash (str): The transaction hash.
 
         Returns:
             The transaction with the given transaction hash.
         """
         return await self.provider.send("ain_getTransactionByHash", {"hash": transactionHash})
 
+    async def getTransactionByBlockHashAndIndex(self, blockHash: str, index: int) -> Any:
+        """Fetches a transaction's information with a block hash and an index.
+
+        Args:
+            blockHash (str): The block hash.
+            index (int): The transaction index in the block
+
+        Returns:
+            The transaction with the given parameter values.
+        """
+        return await self.provider.send(
+            "ain_getTransactionByBlockHashAndIndex",
+            {
+                "block_hash": blockHash,
+                "index": index
+            })
+
+    async def getTransactionByBlockNumberAndIndex(self, blockNumber: int, index: int) -> Any:
+        """Fetches a transaction's information with a block number and an index.
+
+        Args:
+            blockHash (int): The block number.
+            index (int): The transaction index in the block
+
+        Returns:
+            The transaction with the given parameter values.
+        """
+        return await self.provider.send(
+            "ain_getTransactionByBlockNumberAndIndex",
+            {
+                "block_number": blockNumber,
+                "index": index
+            })
+
     async def getStateUsage(self, appName: str) -> Any:
         """Gets a state usage with the given app name.
 
         Args:
             appName (str): The app name;
 
         Returns:
```

### Comparing `ain-py-1.1.0/ain/db/__init__.py` & `ain-py-1.2.0/ain/db/__init__.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/ain/db/push_id.py` & `ain-py-1.2.0/ain/db/push_id.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/ain/db/ref.py` & `ain-py-1.2.0/ain/db/ref.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     SetMultiOperation,
     TransactionInput,
     ValueOnlyTransactionInput,
     SetMultiTransactionInput,
     EvalRuleInput,
     EvalOwnerInput,
     MatchInput,
+    StateInfoInput,
     GetOptions,
 )
 from ain.db.push_id import PushId
 
 if TYPE_CHECKING:
     from ain.ain import Ain
 
@@ -409,14 +410,56 @@
             The owner configs that are related to the input ref.
         """
         ref = self._path
         if params is not None and hasattr(params, "ref"):
             ref = Reference.extendPath(ref, getattr(params, "ref", None))
         return await self._ain.provider.send("ain_matchOwner", {"ref": ref})
 
+    async def getStateProof(self, params: StateInfoInput = None) -> Any:
+        """Fetches the state proof of a global blockchain state path.
+
+        Args:
+            params (StateInfoInput): The state info input object.
+            
+        Returns:
+            The return value of the blockchain API.
+        """
+        ref = self._path
+        if params is not None and hasattr(params, "ref"):
+            ref = Reference.extendPath(ref, getattr(params, "ref", None))
+        return await self._ain.provider.send("ain_getStateProof", {"ref": ref})
+
+    async def getProofHash(self, params: StateInfoInput = None) -> Any:
+        """Fetches the proof hash of a global blockchain state path.
+
+        Args:
+            params (StateInfoInput): The state info input object.
+            
+        Returns:
+            The return value of the blockchain API.
+        """
+        ref = self._path
+        if params is not None and hasattr(params, "ref"):
+            ref = Reference.extendPath(ref, getattr(params, "ref", None))
+        return await self._ain.provider.send("ain_getProofHash", {"ref": ref})
+
+    async def getStateInfo(self, params: StateInfoInput = None) -> Any:
+        """Fetches the state information of a global blockchain state path.
+
+        Args:
+            params (StateInfoInput): The state info input object.
+            
+        Returns:
+            The return value of the blockchain API.
+        """
+        ref = self._path
+        if params is not None and hasattr(params, "ref"):
+            ref = Reference.extendPath(ref, getattr(params, "ref", None))
+        return await self._ain.provider.send("ain_getStateInfo", {"ref": ref})
+
     @staticmethod
     def buildGetRequest(type: GetOperationType, ref: str, options: GetOptions = None) -> dict:
         """Builds a get request.
 
         Args:
             type (GetOperationType): The type of get operation.
             ref (str): The path that you want to make transaction.
```

### Comparing `ain-py-1.1.0/ain/net.py` & `ain-py-1.2.0/ain/net.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Any
 from ain.provider import Provider
 from ain.constants import BLOCKCHAIN_PROTOCOL_VERSION
 
 class Network:
     """Class for the AIN Blockchain network status checker."""
 
     provider: Provider
@@ -9,34 +10,50 @@
     protoVer: str
     """The protocol version of the blockchain."""
     
     def __init__(self, provider: Provider):
         self.provider = provider
         self.protoVer = BLOCKCHAIN_PROTOCOL_VERSION
 
-    async def isListening(self):
-        """Returns whether the node is listening for network connections."""
-        return await self.provider.send("net_listening")
-    
-    async def getNetworkId(self):
-        """Returns the id of the network the node is connected to."""
+    async def getNetworkId(self) -> int:
+        """Fetches the ID of the network the blokchain node is connected to."""
         return await self.provider.send("net_getNetworkId")
 
-    async def checkProtocolVersion(self):
+    async def getChainId(self) -> int:
+        """Fetches the ID of the chain the blokchain node is validating."""
+        return await self.provider.send("net_getChainId")
+
+    async def isListening(self) -> bool:
+        """Checks whether the blockchain node is listening for network connections."""
+        return await self.provider.send("net_listening")
+
+    async def isSyncing(self) -> bool:
+        """Checks whether the blockchain node is syncing with the network or not."""
+        return await self.provider.send("net_syncing")
+
+    async def getPeerCount(self) -> int:
+        """Fetches the number of the peers the blockchain node is connected to."""
+        return await self.provider.send("net_peerCount")
+
+    async def getConsensusStatus(self) -> Any:
+        """Fetches the consensus status of the network."""
+        return await self.provider.send("net_consensusStatus")
+
+    async def getRawConsensusStatus(self) -> Any:
+        """Fetches the consensus status raw data of the network."""
+        return await self.provider.send("net_rawConsensusStatus")
+
+    async def getPeerCandidateInfo(self) -> Any:
+        """Fetches the peer candidate information of the blockchain node."""
+        return await self.provider.send("p2p_getPeerCandidateInfo")
+
+    async def checkProtocolVersion(self) -> bool:
         """Checks the protocol version."""
         return await self.provider.send("ain_checkProtocolVersion")
     
-    async def getProtocolVersion(self):
+    async def getProtocolVersion(self) -> str:
         """Returns the protocol version of the node."""
         return await self.provider.send("ain_getProtocolVersion")
     
-    async def getPeerCount(self):
-        """Returns the number of peers the provider node is connected to."""
-        return await self.provider.send("net_peerCount")
-
-    async def isSyncing(self):
-        """Returns whether the node is syncing with the network or not."""
-        return await self.provider.send("net_syncing")
-
-    async def getEventHandlerNetworkInfo(self):
+    async def getEventHandlerNetworkInfo(self) -> Any:
         """Returns the event handler network information."""
         return await self.provider.send("net_getEventHandlerNetworkInfo")
```

### Comparing `ain-py-1.1.0/ain/provider.py` & `ain-py-1.2.0/ain/provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Any
 import aiohttp
 import json
 from urllib.parse import urlparse, urljoin
 from jsonrpcclient import request, parse, Ok, Error
 from typing import TYPE_CHECKING
 from ain.errors import BlockchainError
 
@@ -23,14 +24,24 @@
         self._ain = ain
         parsed = urlparse(endpoint)
         if parsed.scheme == "" or parsed.netloc == "":
             raise ValueError("Invalid endpoint received.")
         self.endPoint = parsed.geturl()
         self.apiEndPoint = urljoin(self.endPoint, JSON_RPC_ENDPOINT)
 
+    async def getAddress(self) -> str:
+        """Fetches the blockchain node's address.
+
+        Args:
+            
+        Returns:
+            The return value of the blockchain API.
+        """
+        return await self.send("ain_getAddress", {})
+
     async def send(self, rpcMethod: str, params: dict = {}):
         """Creates the JSON-RPC payload and sends it to the node.
 
         Args:
             rpcMethod (str): The JSON-RPC method name.
             params (dict): The parameters for the payload.
```

### Comparing `ain-py-1.1.0/ain/signer/__init__.py` & `ain-py-1.2.0/ain/signer/__init__.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/ain/signer/default_signer.py` & `ain-py-1.2.0/ain/signer/default_signer.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/ain/types.py` & `ain-py-1.2.0/ain/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,7 +446,20 @@
         ref: str = None,
         is_global: bool = None,
     ):
         if ref is not None:
             self.ref = ref
         if is_global is not None:
             self.is_global = is_global
+
+class StateInfoInput:
+    """Class for the state information input."""
+
+    ref: Optional[str]
+    """The path that you want to query with."""
+
+    def __init__(
+        self,
+        ref: str = None,
+    ):
+        if ref is not None:
+            self.ref = ref
```

### Comparing `ain-py-1.1.0/ain/utils/__init__.py` & `ain-py-1.2.0/ain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/ain/utils/v3keystore.py` & `ain-py-1.2.0/ain/utils/v3keystore.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/ain/wallet.py` & `ain-py-1.2.0/ain/wallet.py`

 * *Files 8% similar despite different names*

```diff
@@ -217,22 +217,74 @@
 
         Args:
             address (str, Optional): The address of the account.
                 If `address` is `None`, returns the balance of the default account address. Defaults to `None`.
                 If `address` is `None` and default account is not set, raises `ValueError`.
 
         Returns:
-            str: The AIN balance of the given account.
+            int: The AIN balance of the given account.
         """
         if address is None:
             addr = self.getImpliedAddress()
         else:
             addr = toChecksumAddress(address)
         return await self.ain.db.ref(f"/accounts/{addr}/balance").getValue()
 
+    async def getNonce(self, address: str = None, source: str = None) -> int:
+        """Fetches an account's nonce value, which is the current transaction count of the account.
+
+        Args:
+            address (str, Optional): The address of the account.
+                If `address` is `None`, it uses the default account address. Defaults to `None`.
+                If `address` is `None` and default account is not set, raises `ValueError`.
+            source (str, Optional): The source of the data.
+                It could be either the pending transaction pool ("pending") or
+                the committed blocks ("committed"). The default value is "committed".
+
+        Returns:
+            int: The nonce of the given account.
+        """
+        if address is None:
+            addr = self.getImpliedAddress()
+        else:
+            addr = toChecksumAddress(address)
+        return await self.ain.provider.send(
+            "ain_getNonce",
+            {
+                "address": addr,
+                "from": source,
+            },
+        )
+
+    async def getTimestamp(self, address: str = None, source: str = None) -> int:
+        """Fetches an account's timestamp value, which is the timestamp of the last transaction signed by the account with nonce = -2.
+
+        Args:
+            address (str, Optional): The address of the account.
+                If `address` is `None`, it uses the default account address. Defaults to `None`.
+                If `address` is `None` and default account is not set, raises `ValueError`.
+            source (str, Optional): The source of the data.
+                It could be either the pending transaction pool ("pending") or
+                the committed blocks ("committed"). The default value is "committed".
+
+        Returns:
+            int: The timestamp of the given account.
+        """
+        if address is None:
+            addr = self.getImpliedAddress()
+        else:
+            addr = toChecksumAddress(address)
+        return await self.ain.provider.send(
+            "ain_getTimestamp",
+            {
+                "address": addr,
+                "from": source,
+            },
+        )
+
     async def transfer(self, toAddress: str, value: float, fromAddress: str = None, nonce: int = None, gas_price: int = None, isDryrun = False):
         """Sends a transfer transaction to the network.
 
         Args:
             toAddress (str): The AIN blockchain address that wants to transfer AIN to.
             value (float): The amount of the transferring AIN.
             fromAddress (str, Optional): The AIN blockchain address that wants to transfer AIN from.
```

### Comparing `ain-py-1.1.0/ain_py.egg-info/PKG-INFO` & `ain-py-1.2.0/ain_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ain-py
-Version: 1.1.0
+Version: 1.2.0
 Summary: AI Network Client Library for Python3
 Home-page: https://github.com/ainblockchain/ain-py
 Author: AIN Dev Team
 Author-email: dev@ainetwork.ai
 License: MPL license
 Keywords: ain,ainetwork,ainblockchain,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ain-py-1.1.0/ain_py.egg-info/SOURCES.txt` & `ain-py-1.2.0/ain_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/setup.py` & `ain-py-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords=["ain", "ainetwork", "ainblockchain", "API"],
     name="ain-py",
     packages=find_packages(include=["ain", "ain.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/ainblockchain/ain-py",
-    version="1.1.0",
+    version="1.2.0",
     zip_safe=False,
 )
```

### Comparing `ain-py-1.1.0/tests/test_ain.py` & `ain-py-1.2.0/tests/test_ain.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     transferAddress,
 )
 from .util import (
     asyncTest,
     getRequest,
     postRequest,
     waitUntilTxFinalized,
+    eraseProtoVer,
+    eraseStateVersion,
 )
 
 TX_PATTERN = re.compile("0x[0-9a-fA-F]{64}")
 PY_VERSION = platform.python_version().replace(".", "")
 APP_NAME = "bfan"
 
 class TestNetwork(TestCase):
@@ -50,25 +52,81 @@
         noTrailingSlash = "http://localhost:3000"
         ain.setProvider(noTrailingSlash)
         self.assertEqual(ain.provider.apiEndPoint, noTrailingSlash + "/" + JSON_RPC_ENDPOINT)
         ain.setProvider(noTrailingSlash + "/")
         self.assertEqual(ain.provider.apiEndPoint, noTrailingSlash + "/" + JSON_RPC_ENDPOINT)
 
     @asyncTest
+    async def testGetNetworkId(self):
+        ain = Ain(testNode)
+        self.assertEqual(await ain.net.getNetworkId(), 0)
+    
+    @asyncTest
+    async def testGetChainId(self):
+        ain = Ain(testNode)
+        self.assertEqual(await ain.net.getChainId(), 0)
+    
+    @asyncTest
+    async def testIsListening(self):
+        ain = Ain(testNode)
+        self.assertEqual(await ain.net.isListening(), True)
+    
+    @asyncTest
+    async def testIsSyncing(self):
+        ain = Ain(testNode)
+        self.assertEqual(await ain.net.isSyncing(), False)
+    
+    @asyncTest
+    async def testGetPeerCount(self):
+        ain = Ain(testNode)
+        self.assertGreater(await ain.net.getPeerCount(), 0)
+    
+    @asyncTest
+    async def testGetConsensusStatus(self):
+        ain = Ain(testNode)
+        status = await ain.net.getConsensusStatus()
+        self.assertIsNotNone(status)
+        self.assertEqual(status["state"], "RUNNING")
+    
+    @asyncTest
+    async def testGetRawConsensusStatus(self):
+        ain = Ain(testNode)
+        status = await ain.net.getRawConsensusStatus()
+        self.assertIsNotNone(status)
+        self.assertIsNotNone(status["consensus"])
+        self.assertEqual(status["consensus"]["state"], "RUNNING")
+    
+    @asyncTest
+    async def testGetPeerCandidateInfo(self):
+        ain = Ain(testNode)
+        info = await ain.net.getPeerCandidateInfo()
+        self.assertIsNotNone(info)
+        self.assertIsNotNone(info["address"])
+        self.assertEqual(info["isAvailableForConnection"], True)
+        self.assertIsNotNone(info["peerCandidateJsonRpcUrlList"])
+    
+    @asyncTest
     async def testGetProtocolVersion(self):
         ain = Ain(testNode)
         self.assertNotEqual(await ain.net.getProtocolVersion(), None)
     
     @asyncTest
     async def testCheckProtocolVersion(self):
         ain = Ain(testNode)
         res = await ain.net.checkProtocolVersion()
         self.assertEqual(res["code"], 0)
         self.assertEqual(res["result"], True)
 
+class TestProvider(TestCase):
+    @asyncTest
+    async def testGetAddress(self):
+        ain = Ain(testNode)
+        res = await ain.provider.getAddress()
+        self.assertIsNotNone(res)
+
 class TestWallet(TestCase):
     def testCreateAccount(self):
         ain = Ain(testNode)
         ain.wallet.create(2)
         self.assertEqual(ain.wallet.length, 2)
 
     def testAddFromV3Keystore(self):
@@ -147,14 +205,26 @@
     @asyncTest
     async def testGetBalance(self):
         ain = Ain(testNode)
         ain.wallet.addAndSetDefaultAccount(accountSk)
         self.assertGreaterEqual(await ain.wallet.getBalance(), 0)
 
     @asyncTest
+    async def testGetNonce(self):
+        ain = Ain(testNode)
+        ain.wallet.addAndSetDefaultAccount(accountSk)
+        self.assertEqual(await ain.wallet.getNonce(), 0)
+
+    @asyncTest
+    async def testGetTimestamp(self):
+        ain = Ain(testNode)
+        ain.wallet.addAndSetDefaultAccount(accountSk)
+        self.assertEqual(await ain.wallet.getTimestamp(), 0)
+
+    @asyncTest
     async def testTransferIsDryrunTrue(self):
         ain = Ain(testNode)
         ain.wallet.addAndSetDefaultAccount(accountSk)
         balanceBefore = await ain.wallet.getBalance()
         await ain.wallet.transfer(transferAddress, 100, nonce=-1, isDryrun=True)  # isDryrun = True
         balanceAfter = await ain.wallet.getBalance()
         self.assertEqual(balanceBefore, balanceAfter)  # NOT changed!
@@ -279,32 +349,132 @@
                 }
             ],
             "nonce": -1
         })
         await waitUntilTxFinalized(testNode, createApps["result"]["tx_hash"])
 
     @asyncTest
-    async def test00GetBlock(self):
-        block = await self.ain.getBlock(3)
+    async def test00GetLastBlock(self):
+        block = await self.ain.getLastBlock()
+        self.assertIsNotNone(block)
         hash = block.get("hash", "")
-        self.assertDictEqual(await self.ain.getBlock(hash), block)
-
+        self.assertIsNotNone(hash)
+        number = block.get("number", 0)
+        self.assertGreater(number, 0)
+
+    @asyncTest
+    async def test00GetLastBlockNumber(self):
+        number = await self.ain.getLastBlockNumber()
+        self.assertGreater(number, 0)
+
+    @asyncTest
+    async def test00GetBlockByNumber(self):
+        lastBlock = await self.ain.getLastBlock()
+        self.assertIsNotNone(lastBlock)
+        self.assertIsNotNone(lastBlock["number"])
+        block = await self.ain.getBlockByNumber(lastBlock["number"])
+        self.assertIsNotNone(block)
+        self.assertEqual(block["number"], lastBlock["number"])
+        self.assertEqual(block["hash"], lastBlock["hash"])
+
+    @asyncTest
+    async def test00GetBlockByHash(self):
+        lastBlock = await self.ain.getLastBlock()
+        self.assertIsNotNone(lastBlock)
+        self.assertIsNotNone(lastBlock["hash"])
+        block = await self.ain.getBlockByHash(lastBlock["hash"])
+        self.assertIsNotNone(block)
+        self.assertEqual(block["number"], lastBlock["number"])
+        self.assertEqual(block["hash"], lastBlock["hash"])
+
+    @asyncTest
+    async def test00GetBlockList(self):
+        lastBlockNumber = await self.ain.getLastBlockNumber()
+        self.assertIsNotNone(lastBlockNumber)
+        self.assertGreaterEqual(lastBlockNumber, 0)
+        blockList = await self.ain.getBlockList(lastBlockNumber - 1, lastBlockNumber + 1)
+        self.assertIsNotNone(blockList)
+        self.assertEqual(len(blockList), 2)
+        self.assertEqual(blockList[0]["number"], lastBlockNumber - 1)
+        self.assertEqual(blockList[1]["number"], lastBlockNumber)
+
+    @asyncTest
+    async def test00GetBlockHeadersList(self):
+        lastBlockNumber = await self.ain.getLastBlockNumber()
+        self.assertIsNotNone(lastBlockNumber)
+        self.assertGreaterEqual(lastBlockNumber, 0)
+        blockList = await self.ain.getBlockHeadersList(lastBlockNumber - 1, lastBlockNumber + 1)
+        self.assertIsNotNone(blockList)
+        self.assertEqual(len(blockList), 2)
+        self.assertEqual(blockList[0]["number"], lastBlockNumber - 1)
+        self.assertEqual(blockList[1]["number"], lastBlockNumber)
+
+    @asyncTest
+    async def test00GetBlockTransactionCountByNumber(self):
+        lastBlockNumber = await self.ain.getLastBlockNumber()
+        self.assertIsNotNone(lastBlockNumber)
+        self.assertGreaterEqual(lastBlockNumber, 0)
+        txCount = await self.ain.getBlockTransactionCountByNumber(lastBlockNumber)
+        self.assertIsNotNone(txCount)
+
+    @asyncTest
+    async def test00GetBlockTransactionCountByHash(self):
+        lastBlock= await self.ain.getLastBlock()
+        self.assertIsNotNone(lastBlock)
+        self.assertIsNotNone(lastBlock["hash"])
+        txCount = await self.ain.getBlockTransactionCountByHash(lastBlock["hash"])
+        self.assertIsNotNone(txCount)
+
+    @asyncTest
+    async def test00GetValidatorInfo(self):
+        lastBlock= await self.ain.getLastBlock()
+        self.assertIsNotNone(lastBlock)
+        self.assertIsNotNone(lastBlock["proposer"])
+        validatorInfo = await self.ain.getValidatorInfo(lastBlock["proposer"])
+        self.assertIsNotNone(validatorInfo)
+
+    @asyncTest
+    async def test00GetValidatorsByNumber(self):
+        lastBlock= await self.ain.getLastBlock()
+        self.assertIsNotNone(lastBlock)
+        self.assertIsNotNone(lastBlock["number"])
+        validators = await self.ain.getValidatorsByNumber(lastBlock["number"])
+        self.assertDictEqual(validators, lastBlock["validators"])
+    
     @asyncTest
-    async def test00GetProposer(self):
-        proposer = await self.ain.getProposer(1)
-        block = await self.ain.getBlock(1)
-        hash = block.get("hash", "")
-        self.assertEqual(await self.ain.getProposer(hash), proposer)
+    async def test00GetValidatorsByHash(self):
+        lastBlock= await self.ain.getLastBlock()
+        self.assertIsNotNone(lastBlock)
+        self.assertIsNotNone(lastBlock["hash"])
+        validators = await self.ain.getValidatorsByHash(lastBlock["hash"])
+        self.assertDictEqual(validators, lastBlock["validators"])
+    
+    @asyncTest
+    async def test00GetProposerByNumber(self):
+        lastBlock= await self.ain.getLastBlock()
+        self.assertIsNotNone(lastBlock)
+        self.assertIsNotNone(lastBlock["number"])
+        proposer = await self.ain.getProposerByNumber(lastBlock["number"])
+        self.assertEqual(proposer, lastBlock["proposer"])
+    
+    @asyncTest
+    async def test00GetProposerByHash(self):
+        lastBlock= await self.ain.getLastBlock()
+        self.assertIsNotNone(lastBlock)
+        self.assertIsNotNone(lastBlock["hash"])
+        proposer = await self.ain.getProposerByHash(lastBlock["hash"])
+        self.assertEqual(proposer, lastBlock["proposer"])
 
     @asyncTest
-    async def test00GetValidators(self):
-        validators = await self.ain.getValidators(4)
-        block = await self.ain.getBlock(4)
-        hash = block.get("hash", "")
-        self.assertDictEqual(await self.ain.getValidators(hash), validators)
+    async def test00GetStateUsage(self):
+        # with an app that does not exist yet
+        erased = eraseProtoVer(await self.ain.getStateUsage("test_new"))
+        self.assertIsNotNone(erased["available"])
+        self.assertIsNotNone(erased["usage"])
+        self.assertIsNotNone(erased["staking"])
 
     @asyncTest
     async def test00ValidateAppNameTrue(self):
         res = await self.ain.validateAppName("test_new")
         self.assertEqual(res["is_valid"], True)
         self.assertEqual(res["result"], True)
         self.assertEqual(res["code"], 0)
@@ -340,15 +510,15 @@
             }
         )
         res = await self.ain.sendTransaction(TransactionInput(operation=op), True)  # isDryrun = True
         self.assertEqual(res["result"]["code"], 0)
         targetTxHash = res["tx_hash"]
         self.assertTrue(TX_PATTERN.fullmatch(targetTxHash) is not None)
 
-        tx = await self.ain.getTransaction(targetTxHash)
+        tx = await self.ain.getTransactionByHash(targetTxHash)
         self.assertIsNone(tx)  # should be None
 
     @asyncTest
     async def test00SendTransaction(self):
         op = SetOperation(
             type="SET_OWNER",
             ref=f"/apps/test{PY_VERSION}",
@@ -366,15 +536,15 @@
             }
         )
         res = await self.ain.sendTransaction(TransactionInput(operation=op))
         self.assertEqual(res["result"]["code"], 0)
         targetTxHash = res["tx_hash"]
         self.assertTrue(TX_PATTERN.fullmatch(targetTxHash) is not None)
 
-        tx = await self.ain.getTransaction(targetTxHash)
+        tx = await self.ain.getTransactionByHash(targetTxHash)
         self.assertDictEqual(tx["transaction"]["tx_body"]["operation"], op.__dict__)
 
     @asyncTest
     async def test00SendSignedTransactionIsDryrunTrue(self):
         tx = TransactionBody(
             nonce=-1,
             gas_price=500,
@@ -400,15 +570,15 @@
         sig = self.ain.wallet.signTransaction(tx)
         res = await self.ain.sendSignedTransaction(sig, tx, True)  # isDryrun = True
         targetTxHash = res["tx_hash"]
         self.assertFalse("code" in res)
         self.assertTrue(TX_PATTERN.fullmatch(targetTxHash) is not None)
         self.assertEqual(res["result"]["code"], 0)
 
-        tx = await self.ain.getTransaction(targetTxHash)
+        tx = await self.ain.getTransactionByHash(targetTxHash)
         self.assertIsNone(tx)  # should be None
 
     @asyncTest
     async def test00SendSignedTransaction(self):
         tx = TransactionBody(
             nonce=-1,
             gas_price=500,
@@ -576,14 +746,37 @@
             await self.ain.sendTransactionBatch([])
         except BlockchainError as e:
             self.assertEqual(e.code, 30401)
             self.assertEqual(e.message, "Invalid batch transaction format.")
             raised = True
         self.assertTrue(raised)
 
+    @asyncTest
+    async def test01GetPendingTransactions(self):
+        res = await self.ain.getPendingTransactions()
+        self.assertIsNotNone(res)
+
+    @asyncTest
+    async def test01GetTransactionPoolSizeUtilization(self):
+        res = await self.ain.getTransactionPoolSizeUtilization()
+        self.assertIsNotNone(res)
+
+    @asyncTest
+    async def test01GetTransactionByBlockHashAndIndex(self):
+        genesisBlockNumber = 0
+        genesisBlock = await self.ain.getBlockByNumber(genesisBlockNumber)
+        res = await self.ain.getTransactionByBlockHashAndIndex(genesisBlock["hash"], 0)
+        self.assertIsNotNone(res)
+
+    @asyncTest
+    async def test01GetTransactionByBlockNumberAndIndex(self):
+        genesisBlockNumber = 0
+        res = await self.ain.getTransactionByBlockNumberAndIndex(genesisBlockNumber, 0)
+        self.assertIsNotNone(res)
+
 class TestDatabase(SnapshotTestCase):
     ain: Ain
     defaultAddr: str
     allowedPath: str
 
     @classmethod
     def setUpClass(cls):
@@ -906,7 +1099,25 @@
     async def test03MatchRule(self):
         self.matchSnapshot(await self.ain.db.ref(self.allowedPath).matchRule())
     
     @asyncTest
     async def test03MatchOwner(self):
         self.matchSnapshot(await self.ain.db.ref(self.allowedPath).matchOwner())
     
+    @asyncTest
+    async def test03GetStateProof(self):
+        self.assertIsNotNone(await self.ain.db.ref('/values/blockchain_params').getStateProof())
+    
+    @asyncTest
+    async def test03GetStateProofWithInput(self):
+        self.assertIsNotNone(await self.ain.db.ref('/values/blockchain_params').getStateProof(StateInfoInput(
+            ref="resource"
+        )))
+
+    @asyncTest
+    async def test03GetProofHash(self):
+        self.matchSnapshot(await self.ain.db.ref('/values/blockchain_params').getProofHash())
+
+    @asyncTest
+    async def test03GetStateInfo(self):
+        self.matchSnapshot(eraseStateVersion(await self.ain.db.ref('/rules/transfer/$from/$to/$key/value').getStateInfo()))
+
```

### Comparing `ain-py-1.1.0/tests/test_ain_account.py` & `ain-py-1.2.0/tests/test_ain_account.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/tests/test_ain_raw.py` & `ain-py-1.2.0/tests/test_ain_raw.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.1.0/tests/test_ain_utils.py` & `ain-py-1.2.0/tests/test_ain_utils.py`

 * *Files identical despite different names*

