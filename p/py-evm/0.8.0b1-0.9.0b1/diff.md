# Comparing `tmp/py-evm-0.8.0b1.tar.gz` & `tmp/py-evm-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-evm-0.8.0b1.tar", last modified: Mon Oct  9 19:47:48 2023, max compression
+gzip compressed data, was "py-evm-0.9.0b1.tar", last modified: Mon Feb  5 20:14:56 2024, max compression
```

## Comparing `py-evm-0.8.0b1.tar` & `py-evm-0.9.0b1.tar`

### file list

```diff
@@ -1,337 +1,478 @@
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.533648 py-evm-0.8.0b1/
--rw-r--r--   0 fselmo     (501) staff       (20)     1095 2023-07-25 20:21:23.000000 py-evm-0.8.0b1/LICENSE
--rw-r--r--   0 fselmo     (501) staff       (20)      141 2023-07-25 20:21:23.000000 py-evm-0.8.0b1/MANIFEST.in
--rw-r--r--   0 fselmo     (501) staff       (20)     3079 2023-10-09 19:47:48.533439 py-evm-0.8.0b1/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)     2157 2023-07-25 20:21:23.000000 py-evm-0.8.0b1/README.md
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.428050 py-evm-0.8.0b1/eth/
--rw-r--r--   0 fselmo     (501) staff       (20)      368 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.436463 py-evm-0.8.0b1/eth/_utils/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      687 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/address.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.437584 py-evm-0.8.0b1/eth/_utils/blake2/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/blake2/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1841 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/blake2/coders.py
--rwxr-xr-x   0 fselmo     (501) staff       (20)     5991 2023-10-09 19:13:49.000000 py-evm-0.8.0b1/eth/_utils/blake2/compression.py
--rw-r--r--   0 fselmo     (501) staff       (20)      980 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/bn128.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3924 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/datatypes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1013 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/db.py
--rw-r--r--   0 fselmo     (501) staff       (20)       40 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/empty.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8124 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/env.py
--rw-r--r--   0 fselmo     (501) staff       (20)      612 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/generator.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5042 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/logging.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1540 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/module_loading.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2671 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/numeric.py
--rw-r--r--   0 fselmo     (501) staff       (20)      337 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/padding.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3284 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/rlp.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1749 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/spoof.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1343 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3379 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)      385 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_utils/version.py
--rw-r--r--   0 fselmo     (501) staff       (20)      364 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/_warnings.py
--rw-r--r--   0 fselmo     (501) staff       (20)   117213 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/abc.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.439791 py-evm-0.8.0b1/eth/chains/
--rw-r--r--   0 fselmo     (501) staff       (20)      223 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    25965 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/base.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.440741 py-evm-0.8.0b1/eth/chains/goerli/
--rw-r--r--   0 fselmo     (501) staff       (20)     1305 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/goerli/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      270 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/goerli/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2554 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/header.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.441601 py-evm-0.8.0b1/eth/chains/mainnet/
--rw-r--r--   0 fselmo     (501) staff       (20)     4409 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/mainnet/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1199 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/mainnet/constants.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.442499 py-evm-0.8.0b1/eth/chains/ropsten/
--rw-r--r--   0 fselmo     (501) staff       (20)     2131 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/ropsten/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      847 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/ropsten/constants.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.443047 py-evm-0.8.0b1/eth/chains/tester/
--rw-r--r--   0 fselmo     (501) staff       (20)     5919 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/chains/tester/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.446778 py-evm-0.8.0b1/eth/consensus/
--rw-r--r--   0 fselmo     (501) staff       (20)      313 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      968 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/applier.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.450284 py-evm-0.8.0b1/eth/consensus/clique/
--rw-r--r--   0 fselmo     (501) staff       (20)      271 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/clique/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5208 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/clique/_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5383 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/clique/clique.py
--rw-r--r--   0 fselmo     (501) staff       (20)      486 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/clique/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3368 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/clique/datatypes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2949 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/clique/encoding.py
--rw-r--r--   0 fselmo     (501) staff       (20)      158 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/clique/exceptions.py
--rw-r--r--   0 fselmo     (501) staff       (20)    11157 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/clique/snapshot_manager.py
--rw-r--r--   0 fselmo     (501) staff       (20)      187 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/context.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6858 2023-10-09 19:13:49.000000 py-evm-0.8.0b1/eth/consensus/ethash.py
--rw-r--r--   0 fselmo     (501) staff       (20)      683 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/noproof.py
--rw-r--r--   0 fselmo     (501) staff       (20)      819 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/consensus/pos.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4234 2023-10-09 19:13:48.000000 py-evm-0.8.0b1/eth/consensus/pow.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3962 2023-10-09 19:13:48.000000 py-evm-0.8.0b1/eth/constants.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.460064 py-evm-0.8.0b1/eth/db/
--rw-r--r--   0 fselmo     (501) staff       (20)      714 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3460 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/accesslog.py
--rw-r--r--   0 fselmo     (501) staff       (20)    24411 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/account.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4277 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/atomic.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.461171 py-evm-0.8.0b1/eth/db/backends/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/backends/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2497 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/backends/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)      890 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/backends/memory.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2874 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/batch.py
--rw-r--r--   0 fselmo     (501) staff       (20)      971 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/cache.py
--rw-r--r--   0 fselmo     (501) staff       (20)    19206 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/chain.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5873 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/chain_gaps.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7394 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/diff.py
--rw-r--r--   0 fselmo     (501) staff       (20)      506 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/hash_trie.py
--rw-r--r--   0 fselmo     (501) staff       (20)    24129 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/header.py
--rw-r--r--   0 fselmo     (501) staff       (20)    17008 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/journal.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1306 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/keymap.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1354 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/schema.py
--rw-r--r--   0 fselmo     (501) staff       (20)    16562 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/slow_journal.py
--rw-r--r--   0 fselmo     (501) staff       (20)    16442 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1393 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/trie.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1660 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/db/witness.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.462046 py-evm-0.8.0b1/eth/estimators/
--rw-r--r--   0 fselmo     (501) staff       (20)      514 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/estimators/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3427 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/estimators/gas.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4115 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/exceptions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.466251 py-evm-0.8.0b1/eth/precompiles/
--rw-r--r--   0 fselmo     (501) staff       (20)      398 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      962 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/blake2.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1502 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/ecadd.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1390 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/ecmul.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3257 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/ecpairing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1512 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/ecrecover.py
--rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/identity.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3934 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/modexp.py
--rw-r--r--   0 fselmo     (501) staff       (20)      670 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/ripemd160.py
--rw-r--r--   0 fselmo     (501) staff       (20)      541 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/precompiles/sha256.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/py.typed
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.469442 py-evm-0.8.0b1/eth/rlp/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/rlp/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1022 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/rlp/accounts.py
--rw-r--r--   0 fselmo     (501) staff       (20)      904 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/rlp/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5417 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/rlp/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      603 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/rlp/logs.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1285 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/rlp/receipts.py
--rw-r--r--   0 fselmo     (501) staff       (20)      387 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/rlp/sedes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3611 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/rlp/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.470821 py-evm-0.8.0b1/eth/tools/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.473861 py-evm-0.8.0b1/eth/tools/_utils/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/_utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      662 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/_utils/deprecation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      190 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/_utils/git.py
--rw-r--r--   0 fselmo     (501) staff       (20)      556 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/_utils/hashing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1564 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/_utils/mappings.py
--rw-r--r--   0 fselmo     (501) staff       (20)    18084 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/_utils/normalization.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4410 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/_utils/slow_code_stream.py
--rw-r--r--   0 fselmo     (501) staff       (20)      903 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/_utils/vyper.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.474294 py-evm-0.8.0b1/eth/tools/builder/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/builder/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.474938 py-evm-0.8.0b1/eth/tools/builder/chain/
--rw-r--r--   0 fselmo     (501) staff       (20)     2936 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/builder/chain/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    15254 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/builder/chain/builders.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.476022 py-evm-0.8.0b1/eth/tools/db/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/db/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5191 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/db/atomic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2269 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/db/base.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.477676 py-evm-0.8.0b1/eth/tools/fixtures/
--rw-r--r--   0 fselmo     (501) staff       (20)      615 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      887 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/_utils.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.479965 py-evm-0.8.0b1/eth/tools/fixtures/fillers/
--rw-r--r--   0 fselmo     (501) staff       (20)      282 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/fillers/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2456 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/fillers/_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)    12716 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/fillers/common.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3461 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/fillers/formatters.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1307 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/fillers/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2758 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/fillers/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1737 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/fillers/vm.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2079 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/generation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9361 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/helpers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3068 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/fixtures/loading.py
--rw-r--r--   0 fselmo     (501) staff       (20)      791 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/mining.py
--rw-r--r--   0 fselmo     (501) staff       (20)      476 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/tools/rlp.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2693 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/typing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8548 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/validation.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.486829 py-evm-0.8.0b1/eth/vm/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    26238 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)      632 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/chain_context.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4438 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/code_stream.py
--rw-r--r--   0 fselmo     (501) staff       (20)    19222 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2124 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/execution_context.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.487259 py-evm-0.8.0b1/eth/vm/forks/
--rw-r--r--   0 fselmo     (501) staff       (20)      899 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.489109 py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/
--rw-r--r--   0 fselmo     (501) staff       (20)      856 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      993 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      287 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1084 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      523 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1134 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.492153 py-evm-0.8.0b1/eth/vm/forks/berlin/
--rw-r--r--   0 fselmo     (501) staff       (20)      772 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      784 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2441 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      327 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      374 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6417 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/logic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2922 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4606 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/receipts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1187 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)    15395 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/berlin/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.494634 py-evm-0.8.0b1/eth/vm/forks/byzantium/
--rw-r--r--   0 fselmo     (501) staff       (20)     3584 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/byzantium/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      485 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/byzantium/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1016 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/byzantium/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      235 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/byzantium/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3368 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/byzantium/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3526 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/byzantium/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      222 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/byzantium/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1231 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/byzantium/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.497326 py-evm-0.8.0b1/eth/vm/forks/constantinople/
--rw-r--r--   0 fselmo     (501) staff       (20)     1106 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      484 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      757 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      329 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      406 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1574 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      221 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      334 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1235 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/constantinople/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.500199 py-evm-0.8.0b1/eth/vm/forks/frontier/
--rw-r--r--   0 fselmo     (501) staff       (20)     3732 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3412 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3715 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)       96 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3529 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)    20228 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7686 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      140 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/transaction_context.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5952 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1603 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/frontier/validation.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.503378 py-evm-0.8.0b1/eth/vm/forks/gray_glacier/
--rw-r--r--   0 fselmo     (501) staff       (20)      855 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/gray_glacier/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1068 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/gray_glacier/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      317 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/gray_glacier/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1119 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/gray_glacier/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      556 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/gray_glacier/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1170 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/gray_glacier/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.507086 py-evm-0.8.0b1/eth/vm/forks/homestead/
--rw-r--r--   0 fselmo     (501) staff       (20)     1250 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      466 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2289 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)       61 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9656 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      637 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      640 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2281 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)      518 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/homestead/validation.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.509970 py-evm-0.8.0b1/eth/vm/forks/istanbul/
--rw-r--r--   0 fselmo     (501) staff       (20)      817 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      469 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1421 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      316 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      384 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1664 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      206 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      909 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1798 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/istanbul/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.514211 py-evm-0.8.0b1/eth/vm/forks/london/
--rw-r--r--   0 fselmo     (501) staff       (20)     2260 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5828 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      810 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      470 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5618 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      895 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      629 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/receipts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4881 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      544 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9486 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)      855 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/london/validation.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.516403 py-evm-0.8.0b1/eth/vm/forks/muir_glacier/
--rw-r--r--   0 fselmo     (501) staff       (20)      842 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/muir_glacier/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/muir_glacier/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      537 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/muir_glacier/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      443 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/muir_glacier/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      137 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/muir_glacier/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/muir_glacier/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1212 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/muir_glacier/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.518333 py-evm-0.8.0b1/eth/vm/forks/paris/
--rw-r--r--   0 fselmo     (501) staff       (20)     2117 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/paris/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1039 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/paris/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      379 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/paris/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2284 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/paris/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      686 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/paris/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      666 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/paris/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1121 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/paris/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.520595 py-evm-0.8.0b1/eth/vm/forks/petersburg/
--rw-r--r--   0 fselmo     (501) staff       (20)     1036 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/petersburg/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/petersburg/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      531 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/petersburg/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      110 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/petersburg/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      386 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/petersburg/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1399 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/petersburg/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/petersburg/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1211 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/petersburg/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.523583 py-evm-0.8.0b1/eth/vm/forks/shanghai/
--rw-r--r--   0 fselmo     (501) staff       (20)      667 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9048 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1655 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      196 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      824 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      821 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/logic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1531 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      751 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1099 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1515 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/shanghai/withdrawals.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.525737 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/
--rw-r--r--   0 fselmo     (501) staff       (20)      429 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2145 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)      484 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3322 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      169 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1221 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1465 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2866 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.527202 py-evm-0.8.0b1/eth/vm/forks/tangerine_whistle/
--rw-r--r--   0 fselmo     (501) staff       (20)      469 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/tangerine_whistle/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      428 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/tangerine_whistle/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      225 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/tangerine_whistle/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2106 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/tangerine_whistle/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      227 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/forks/tangerine_whistle/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2626 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/gas_meter.py
--rw-r--r--   0 fselmo     (501) staff       (20)      540 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/header.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3425 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/interrupt.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.531501 py-evm-0.8.0b1/eth/vm/logic/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4805 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/arithmetic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1113 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/block.py
--rw-r--r--   0 fselmo     (501) staff       (20)    13394 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/call.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2824 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/comparison.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6418 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/context.py
--rw-r--r--   0 fselmo     (501) staff       (20)      944 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/duplication.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1508 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/flow.py
--rw-r--r--   0 fselmo     (501) staff       (20)      507 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/invalid.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1355 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/logging.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1102 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/memory.py
--rw-r--r--   0 fselmo     (501) staff       (20)      640 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/sha3.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2176 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/stack.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3939 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)      974 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/swap.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9727 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/logic/system.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2134 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/memory.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3214 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/message.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2785 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/mnemonics.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1864 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/opcode.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2432 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/opcode_values.py
--rw-r--r--   0 fselmo     (501) staff       (20)      416 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/spoof.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7713 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/stack.py
--rw-r--r--   0 fselmo     (501) staff       (20)    10406 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      875 2023-09-13 20:03:28.000000 py-evm-0.8.0b1/eth/vm/transaction_context.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-10-09 19:47:48.533101 py-evm-0.8.0b1/py_evm.egg-info/
--rw-r--r--   0 fselmo     (501) staff       (20)     3079 2023-10-09 19:47:44.000000 py-evm-0.8.0b1/py_evm.egg-info/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)     8484 2023-10-09 19:47:48.000000 py-evm-0.8.0b1/py_evm.egg-info/SOURCES.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-10-09 19:47:44.000000 py-evm-0.8.0b1/py_evm.egg-info/dependency_links.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2021-11-19 17:48:51.000000 py-evm-0.8.0b1/py_evm.egg-info/not-zip-safe
--rw-r--r--   0 fselmo     (501) staff       (20)     1853 2023-10-09 19:47:44.000000 py-evm-0.8.0b1/py_evm.egg-info/requires.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        4 2023-10-09 19:47:44.000000 py-evm-0.8.0b1/py_evm.egg-info/top_level.txt
--rw-r--r--   0 fselmo     (501) staff       (20)     1117 2023-09-05 17:44:23.000000 py-evm-0.8.0b1/pyproject.toml
--rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-10-09 19:47:48.533719 py-evm-0.8.0b1/setup.cfg
--rw-r--r--   0 fselmo     (501) staff       (20)     3911 2023-10-09 19:47:15.000000 py-evm-0.8.0b1/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.876028 py-evm-0.9.0b1/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     7198 2024-02-05 20:14:56.876028 py-evm-0.9.0b1/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3412 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.840029 py-evm-0.9.0b1/eth/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      366 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/_utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      687 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/address.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/_utils/blake2/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/blake2/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1841 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/blake2/coders.py
+-rwxrwxr-x   0 pacrob    (1000) pacrob    (1000)     5988 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/_utils/blake2/compression.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      980 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/bn128.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3924 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/datatypes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1013 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/db.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       40 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/empty.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8144 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/_utils/env.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      612 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/generator.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5102 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/_utils/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/logging.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1540 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/module_loading.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2512 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/numeric.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      337 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/padding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3284 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/rlp.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1749 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/spoof.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1343 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3379 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_utils/transactions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      384 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/_utils/version.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      364 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/_warnings.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)   116943 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/abc.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/chains/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      223 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/chains/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    25999 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/chains/base.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/chains/goerli/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1305 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/chains/goerli/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      270 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/chains/goerli/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2554 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/chains/header.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/chains/mainnet/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4409 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/chains/mainnet/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1199 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/chains/mainnet/constants.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/chains/ropsten/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2131 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/chains/ropsten/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      847 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/chains/ropsten/constants.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/chains/tester/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5958 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/chains/tester/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/consensus/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      243 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/consensus/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      968 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/applier.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.844029 py-evm-0.9.0b1/eth/consensus/clique/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      229 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/consensus/clique/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5205 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/consensus/clique/_utils.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5382 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/consensus/clique/clique.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      486 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/clique/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3368 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/clique/datatypes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2949 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/clique/encoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      158 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/clique/exceptions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11157 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/consensus/clique/snapshot_manager.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      187 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/context.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6858 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/ethash.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      683 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/noproof.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      819 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/pos.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4234 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/consensus/pow.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3962 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/constants.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/db/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      714 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3460 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/accesslog.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    24290 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/db/account.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4284 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/db/atomic.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/db/backends/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/backends/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2487 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/db/backends/base.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      890 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/backends/memory.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2874 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/batch.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      971 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/db/cache.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    19190 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/db/chain.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5872 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/db/chain_gaps.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7394 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/diff.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      506 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/hash_trie.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    24128 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/db/header.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    17008 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/journal.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1306 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/keymap.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1378 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/db/schema.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    16560 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/db/slow_journal.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    16433 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/db/storage.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1393 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/trie.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1660 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/db/witness.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/estimators/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      514 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/estimators/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3427 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/estimators/gas.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3895 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/exceptions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/precompiles/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      272 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/precompiles/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      962 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/blake2.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1502 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/ecadd.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1390 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/ecmul.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3257 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/ecpairing.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1512 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/ecrecover.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      472 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/identity.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3934 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/modexp.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      670 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/ripemd160.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      541 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/precompiles/sha256.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/py.typed
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/rlp/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/rlp/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1022 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/rlp/accounts.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      904 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/rlp/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5417 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/rlp/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      603 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/rlp/logs.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1285 2023-12-19 18:40:11.000000 py-evm-0.9.0b1/eth/rlp/receipts.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      387 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/rlp/sedes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3611 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/rlp/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/tools/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/tools/_utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/_utils/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      662 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/_utils/deprecation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      190 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/_utils/git.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      556 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/_utils/hashing.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1576 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/tools/_utils/mappings.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    17997 2024-01-25 18:38:53.000000 py-evm-0.9.0b1/eth/tools/_utils/normalization.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4410 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/_utils/slow_code_stream.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      903 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/_utils/vyper.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/tools/builder/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/builder/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/tools/builder/chain/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2908 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/tools/builder/chain/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    15296 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/tools/builder/chain/builders.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.848029 py-evm-0.9.0b1/eth/tools/db/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/db/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5190 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/tools/db/atomic.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2269 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/db/base.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.852029 py-evm-0.9.0b1/eth/tools/fixtures/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      559 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/tools/fixtures/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      887 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/fixtures/_utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.852029 py-evm-0.9.0b1/eth/tools/fixtures/fillers/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      226 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/tools/fixtures/fillers/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2456 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/fixtures/fillers/_utils.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12780 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/tools/fixtures/fillers/common.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3461 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/fixtures/fillers/formatters.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1264 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/tools/fixtures/fillers/main.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2758 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/fixtures/fillers/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1781 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/tools/fixtures/fillers/vm.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2079 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/fixtures/generation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     9359 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/tools/fixtures/helpers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3068 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/fixtures/loading.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      791 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/mining.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      476 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/tools/rlp.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2501 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/typing.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8548 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/validation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.852029 py-evm-0.9.0b1/eth/vm/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    26128 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/vm/base.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      632 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/chain_context.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4432 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/code_stream.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    19109 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2124 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/execution_context.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.852029 py-evm-0.9.0b1/eth/vm/forks/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      689 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/vm/forks/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.852029 py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      856 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      993 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      277 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1084 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      523 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1134 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.852029 py-evm-0.9.0b1/eth/vm/forks/berlin/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      772 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      784 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2441 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      327 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      374 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6416 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/logic.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2952 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4606 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/receipts.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1187 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    15395 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/berlin/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.852029 py-evm-0.9.0b1/eth/vm/forks/byzantium/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3584 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/byzantium/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      485 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/byzantium/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1016 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/byzantium/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      235 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/byzantium/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3392 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/byzantium/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3526 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/byzantium/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      222 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/byzantium/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1231 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/byzantium/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.856029 py-evm-0.9.0b1/eth/vm/forks/constantinople/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1106 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      484 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      757 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      329 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      406 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1574 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      221 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      334 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/storage.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1235 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/constantinople/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.856029 py-evm-0.9.0b1/eth/vm/forks/frontier/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3732 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3412 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3659 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       96 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3529 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    20228 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7609 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      140 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/transaction_context.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5952 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/transactions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1603 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/frontier/validation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.856029 py-evm-0.9.0b1/eth/vm/forks/gray_glacier/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      855 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/gray_glacier/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1068 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/gray_glacier/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      307 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/gray_glacier/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1119 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/gray_glacier/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      556 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/gray_glacier/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1170 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/gray_glacier/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.856029 py-evm-0.9.0b1/eth/vm/forks/homestead/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1250 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      466 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2263 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       61 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     9656 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      637 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      640 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2281 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/transactions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      518 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/homestead/validation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.856029 py-evm-0.9.0b1/eth/vm/forks/istanbul/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      817 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      469 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1421 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      316 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      384 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1664 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      206 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      909 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/storage.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1798 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/istanbul/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.856029 py-evm-0.9.0b1/eth/vm/forks/london/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2260 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/london/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5828 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/vm/forks/london/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      810 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/london/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      470 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/london/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5618 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/london/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      925 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/london/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      742 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/london/receipts.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4877 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/london/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      544 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/london/storage.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     9486 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/london/transactions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      855 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/london/validation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.860029 py-evm-0.9.0b1/eth/vm/forks/muir_glacier/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      842 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/muir_glacier/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      472 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/muir_glacier/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      537 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/muir_glacier/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      443 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/muir_glacier/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      137 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/muir_glacier/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      209 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/muir_glacier/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1212 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/muir_glacier/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.860029 py-evm-0.9.0b1/eth/vm/forks/paris/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2117 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/paris/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1104 2024-01-25 18:38:53.000000 py-evm-0.9.0b1/eth/vm/forks/paris/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      379 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/paris/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2284 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/paris/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      686 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/paris/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      666 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/paris/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1121 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/paris/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.860029 py-evm-0.9.0b1/eth/vm/forks/petersburg/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1036 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/petersburg/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      472 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/petersburg/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      531 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/petersburg/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      110 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/petersburg/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      386 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/petersburg/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1399 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/petersburg/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      209 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/petersburg/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1211 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/petersburg/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.860029 py-evm-0.9.0b1/eth/vm/forks/shanghai/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      667 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8580 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1655 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      196 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      824 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/headers.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      821 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/logic.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1531 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      751 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1099 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/transactions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1515 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/shanghai/withdrawals.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.860029 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      429 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2145 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/_utils.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      484 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3283 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      169 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1221 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1443 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2866 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/transactions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.860029 py-evm-0.9.0b1/eth/vm/forks/tangerine_whistle/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      469 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/tangerine_whistle/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      428 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/tangerine_whistle/computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      225 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/tangerine_whistle/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2106 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/tangerine_whistle/opcodes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      227 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/forks/tangerine_whistle/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2506 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/gas_meter.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      540 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/vm/header.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3425 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/interrupt.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/eth/vm/logic/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4805 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/arithmetic.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1113 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/block.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    13286 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/logic/call.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2824 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/comparison.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6418 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/context.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1306 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/duplication.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1508 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/flow.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      507 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/invalid.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1355 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/logging.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1102 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/memory.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      640 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/sha3.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3542 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/stack.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3939 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/storage.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1338 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/logic/swap.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     9792 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/logic/system.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2087 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/memory.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3214 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/message.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2785 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/vm/mnemonics.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1682 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/opcode.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2432 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/eth/vm/opcode_values.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      416 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/spoof.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4871 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/eth/vm/stack.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10406 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      875 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/eth/vm/transaction_context.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/py_evm.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     7198 2024-02-05 20:14:55.000000 py-evm-0.9.0b1/py_evm.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12752 2024-02-05 20:14:56.000000 py-evm-0.9.0b1/py_evm.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-02-05 20:14:55.000000 py-evm-0.9.0b1/py_evm.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/py_evm.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1098 2024-02-05 20:14:55.000000 py-evm-0.9.0b1/py_evm.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       12 2024-02-05 20:14:55.000000 py-evm-0.9.0b1/py_evm.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3619 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/pyproject.toml
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/scripts/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/scripts/benchmark/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/scripts/benchmark/_utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/_utils/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      724 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/_utils/address.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1487 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/_utils/chain_plumbing.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1066 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/_utils/compile.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      394 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/_utils/format.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      540 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/_utils/meters.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3556 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/_utils/reporting.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      373 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/_utils/shellart.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/scripts/benchmark/checks/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      192 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/checks/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1389 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/checks/base_benchmark.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8711 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/checks/deploy_dos.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10608 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/checks/erc20_interact.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1479 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/checks/import_empty_blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1314 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/checks/mine_empty_blocks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4133 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/checks/simple_value_transfers.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/scripts/benchmark/contract_data/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      282 2023-12-18 19:39:48.000000 py-evm-0.9.0b1/scripts/benchmark/contract_data/__init__.py
+-rwxrwxr-x   0 pacrob    (1000) pacrob    (1000)     3531 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/scripts/benchmark/run.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-02-05 20:14:56.876028 py-evm-0.9.0b1/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2842 2024-02-05 20:14:16.000000 py-evm-0.9.0b1/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/tests/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8483 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/conftest.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/tests/core/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/tests/core/address-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2301 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/address-utils/test_address_generation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.864029 py-evm-0.9.0b1/tests/core/builder-tools/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6429 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/builder-tools/test_chain_builder.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4477 2024-01-31 19:15:56.000000 py-evm-0.9.0b1/tests/core/builder-tools/test_chain_construction.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3301 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/builder-tools/test_chain_initializer.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/chain-object/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2230 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/chain-object/test_build_block_incrementally.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10048 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/chain-object/test_chain.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5715 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/chain-object/test_chain_get_ancestors.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3743 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/chain-object/test_chain_reorganization.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2241 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/chain-object/test_chain_retrieval_of_vm_class.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7329 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/chain-object/test_contract_call.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1801 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/chain-object/test_create_transaction.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    26309 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/chain-object/test_gas_estimation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/code-stream/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8971 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/code-stream/test_code_stream.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/consensus/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    19983 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/consensus/test_clique_consensus.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1879 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/consensus/test_clique_encoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7438 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/consensus/test_clique_utils.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2595 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/consensus/test_consensus_engine.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2510 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/consensus/test_pow_mining.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/datatype-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2913 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/datatype-utils/test_configurable_class.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/env-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2085 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/env-utils/test_env_bool.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1191 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/env-utils/test_env_float.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1880 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/env-utils/test_env_int.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2057 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/env-utils/test_env_list.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1237 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/env-utils/test_env_string.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      751 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/env-utils/test_get.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/fixture-tools/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2730 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/fixture-tools/test_normalize_state.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1666 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/fixtures.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/gas_meter/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2480 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/gas_meter/test_gas_meter.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/generator-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      785 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/generator-utils/test_cached_iterable.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1141 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/helpers.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/hexadecimal-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1305 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/hexadecimal-utils/test_encode_and_decode.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/memory/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2406 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/memory/test_memory.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/message-object/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2454 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/message-object/test_message_object.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/numeric-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      347 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/numeric-utils/test_get_highest_bit_length.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      598 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/numeric-utils/test_int_to_bytes32.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      909 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/numeric-utils/test_integer_squareroot.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/opcodes/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    49046 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/opcodes/test_opcodes.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/padding-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      493 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/padding-utils/test_padding.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/precompiles/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6065 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/precompiles/test_blake2.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/stack/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4033 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/stack/test_stack.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       48 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/test_import.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/tester/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5571 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/tester/test_generate_vm_configuration.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/transaction-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3547 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/transaction-utils/conftest.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7642 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/transaction-utils/test_receipt_encoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4686 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/transaction-utils/test_transaction_encoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4647 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/transaction-utils/test_transaction_signature_validation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.868028 py-evm-0.9.0b1/tests/core/validation/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11685 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/validation/test_eth1_validation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5297 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/validation/test_transaction_validation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2740 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/validation/test_withdrawal_validation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/tests/core/vm/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      770 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/conftest.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/tests/core/vm/fixtures/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    42672 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/vm/fixtures/modexp_precompile_test_vectors.json
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    13088 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_base_computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3612 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_clique_validation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3305 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2554 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_contract_code_size_limit.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1561 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/vm/test_frontier_computation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4254 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_interrupt.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11599 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_london.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    20561 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_mainnet_dao_fork.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1341 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_modexp_precompile.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11519 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_rewards.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2098 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/core/vm/test_shanghai.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3042 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_validate_transaction.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7340 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_vm.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1176 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_vm_class_configurations.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5792 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/core/vm/test_vm_state.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/tests/database/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2299 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/database/test_accesslog.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10639 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/database/test_account_db.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5747 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/database/test_batch_db.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1349 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/database/test_database_api.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4667 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/database/test_db_diff.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    19577 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/database/test_eth1_chaindb.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1361 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/database/test_hash_trie.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    41897 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/database/test_header_db.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    22823 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/database/test_journal_db.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1486 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/database/test_leveldb_db_backend.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/tests/fillers/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/fillers/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1932 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/fillers/build_json.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/tests/fillers/vm_fillers/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/fillers/vm_fillers/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/tests/json-fixtures/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/tests/json-fixtures/blockchain/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    45753 2024-01-25 18:38:53.000000 py-evm-0.9.0b1/tests/json-fixtures/blockchain/test_blockchain.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3060 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/json-fixtures/test_difficulty.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5682 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/json-fixtures/test_transactions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8582 2024-01-12 22:24:40.000000 py-evm-0.9.0b1/tests/json-fixtures/test_virtual_machine.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-05 20:14:56.872028 py-evm-0.9.0b1/tests/rlp-fixtures/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    42848 2023-12-18 19:39:49.000000 py-evm-0.9.0b1/tests/rlp-fixtures/ropston_epoch_headers.rlp
```

### Comparing `py-evm-0.8.0b1/LICENSE` & `py-evm-0.9.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/PKG-INFO` & `py-evm-0.9.0b1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,88 @@
-Metadata-Version: 2.1
-Name: py-evm
-Version: 0.8.0b1
-Summary: Python implementation of the Ethereum Virtual Machine
-Home-page: https://github.com/ethereum/py-evm
-Author: Ethereum Foundation
-Author-email: piper@pipermerriam.com
-License: MIT
-Keywords: ethereum blockchain evm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: eth
-Provides-Extra: eth-extra
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: benchmark
-Provides-Extra: docs
-Provides-Extra: dev
-License-File: LICENSE
-
 # Python Implementation of the Ethereum protocol
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/py-evm.svg?style=shield)](https://circleci.com/gh/ethereum/py-evm)
 [![PyPI version](https://badge.fury.io/py/py-evm.svg)](https://badge.fury.io/py/py-evm)
 [![Python versions](https://img.shields.io/pypi/pyversions/py-evm.svg)](https://pypi.python.org/pypi/py-evm)
-[![Docs build](https://readthedocs.org/projects/py-evm/badge/?version=latest)](http://py-evm.readthedocs.io/en/latest/?badge=latest)
-
+[![Docs build](https://readthedocs.org/projects/py-evm/badge/?version=latest)](https://py-evm.readthedocs.io/en/latest/?badge=latest)
 
 ## Py-EVM
 
 Py-EVM is an implementation of the Ethereum protocol in Python. It contains the low level
-primitives for the existing Ethereum 1.0 chain as well as emerging support for the upcoming
-Ethereum 2.0 / Serenity spec.
+primitives for the original proof-of-work (POW), (formerly known as Ethereum 1.0) chain
+as well as emerging support for the proof-of-stake (POS) (formerly known as Ethereum 2.0) spec.
 
 ### Goals
 
 Py-EVM aims to eventually become the defacto Python implementation of the Ethereum protocol,
-enabling a wide array of use cases for both public and private chains. 
+enabling a wide array of use cases for both public and private chains.
 
 In particular Py-EVM aims to:
 
-- be a reference implementation of the Ethereum 1.0 and 2.0 implementation in one of the most widely used and understood languages, Python.
+- be a reference implementation of the Ethereum POW and POS implementations in one of the most widely used and understood languages, Python.
 
 - be easy to understand and modifiable
 
 - have clear and simple APIs
 
 - come with solid, friendly documentation
 
 - deliver the low level primitives to build various clients on top (including *full* and *light* clients)
 
 - be highly flexible to support both research as well as alternate use cases like private chains.
 
-
 ## Quickstart
 
+```sh
+python -m pip install py-evm
+```
+
 [Get started in 5 minutes](https://py-evm.readthedocs.io/en/latest/guides/quickstart.html)
 
 ## Documentation
 
 Check out the [documentation on our official website](https://py-evm.readthedocs.io/en/latest/)
 
+## Developer Setup
+
+If you would like to hack on py-evm, please check out the [Snake Charmers
+Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
+for information on how we do:
+
+- Testing
+- Pull Requests
+- Documentation
+
+We use [pre-commit](https://pre-commit.com/) to maintain consistent code style. Once
+installed, it will run automatically with every commit. You can also run it manually
+with `make lint`. If you need to make a commit that skips the `pre-commit` checks, you
+can do so with `git commit --no-verify`.
+
+### Development Environment Setup
+
+```sh
+git clone git@github.com:ethereum/py-evm.git
+cd py-evm
+virtualenv -p python3 venv
+. venv/bin/activate
+python -m pip install -e ".[dev]"
+pre-commit install
+```
+
+### Release setup
+
+To release a new version:
+
+```sh
+make release bump=$$VERSION_PART_TO_BUMP$$
+```
+
+To issue the next version in line, specify which part to bump,
+like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
+main branch, except when releasing a beta (in which case the beta is released from main,
+and the previous stable branch is released from said branch).
+
 ## Want to help?
 
 Want to file a bug, contribute some code, or improve documentation? Excellent! Read up on our
 guidelines for [contributing](https://py-evm.readthedocs.io/en/latest/contributing.html) and then check out one of our issues that are labeled [Good First Issue](https://github.com/ethereum/py-evm/issues?q=is%3Aissue+is%3Aopen+label%3A%22Good+First+Issue%22).
```

### Comparing `py-evm-0.8.0b1/eth/_utils/address.py` & `py-evm-0.9.0b1/eth/_utils/address.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/blake2/coders.py` & `py-evm-0.9.0b1/eth/_utils/blake2/coders.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/blake2/compression.py` & `py-evm-0.9.0b1/eth/_utils/blake2/compression.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,14 @@
     t_offset_counters: Tuple[int, int],
     final_block_flag: bool,
 ) -> bytes:
     """
     'F Compression' from section 3.2 of RFC 7693:
     https://tools.ietf.org/html/rfc7693#section-3.2
     """
-
     # Dereference these for [very small] speed improvement.
     # Perhaps more than anything, this makes the code
     # easier to read.
     MASKBITS = Blake2b.MASKBITS
     WORDBITS = Blake2b.WORDBITS
     IV = Blake2b.IV
     ROT1 = Blake2b.ROT1
@@ -103,15 +102,15 @@
     sigma_schedule_len = len(sigma_schedule)
 
     # convert block (if bytes) into tuple of 16 LE words
     # *later versions of blake2b use the tuple form, but older versions use bytes
     m = (
         block
         if isinstance(block, tuple)
-        else struct.unpack_from("<16%s" % Blake2b.WORDFMT, bytes(block))
+        else struct.unpack_from(f"<16{Blake2b.WORDFMT}", bytes(block))
     )
 
     v = [0] * 16
     v[0:8] = h_starting_state
     v[8:12] = IV[:4]
     v[12] = t_offset_counters[0] ^ IV[4]
     v[13] = t_offset_counters[1] ^ IV[5]
```

### Comparing `py-evm-0.8.0b1/eth/_utils/bn128.py` & `py-evm-0.9.0b1/eth/_utils/bn128.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/datatypes.py` & `py-evm-0.9.0b1/eth/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/db.py` & `py-evm-0.9.0b1/eth/_utils/db.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/env.py` & `py-evm-0.9.0b1/eth/_utils/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,14 @@
 
 class empty:
     """
     We use this sentinel object, instead of None, as None is a plausible value
     for a default in real Python code.
     """
 
-    pass
-
 
 def get_env_value(name: str, required: bool = False, default: Any = empty) -> str:
     """
     Core function for extracting the environment variable.
 
     Enforces mutual exclusivity between `required` and `default` keywords.
 
@@ -52,15 +50,16 @@
         value = os.environ.get(name, default)
     return value
 
 
 def env_int(
     name: str, required: bool = False, default: Union[Type[empty], int] = empty
 ) -> int:
-    """Pulls an environment variable out of the environment and casts it to an
+    """
+    Pulls an environment variable out of the environment and casts it to an
     integer. If the name is not present in the environment and no default is
     specified then a ``ValueError`` will be raised. Similarly, if the
     environment value is not castable to an integer, a ``ValueError`` will be
     raised.
 
     :param name: The name of the environment variable be pulled
     :type name: str
@@ -82,15 +81,16 @@
         )
     return int(value)
 
 
 def env_float(
     name: str, required: bool = False, default: Union[Type[empty], float] = empty
 ) -> float:
-    """Pulls an environment variable out of the environment and casts it to an
+    """
+    Pulls an environment variable out of the environment and casts it to an
     float. If the name is not present in the environment and no default is
     specified then a ``ValueError`` will be raised. Similarly, if the
     environment value is not castable to an float, a ``ValueError`` will be
     raised.
 
     :param name: The name of the environment variable be pulled
     :type name: str
@@ -115,15 +115,16 @@
 
 def env_bool(
     name: str,
     truthy_values: Iterable[Any] = TRUE_VALUES,
     required: bool = False,
     default: Union[Type[empty], bool] = empty,
 ) -> bool:
-    """Pulls an environment variable out of the environment returning it as a
+    """
+    Pulls an environment variable out of the environment returning it as a
     boolean. The strings ``'True'`` and ``'true'`` are the default *truthy*
     values. If not present in the environment and no default is specified,
     ``None`` is returned.
 
     :param name: The name of the environment variable be pulled
     :type name: str
 
@@ -145,15 +146,16 @@
         return None
     return value in TRUE_VALUES
 
 
 def env_string(
     name: str, required: bool = False, default: Union[Type[empty], str] = empty
 ) -> str:
-    """Pulls an environment variable out of the environment returning it as a
+    """
+    Pulls an environment variable out of the environment returning it as a
     string. If not present in the environment and no default is specified, an
     empty string is returned.
 
     :param name: The name of the environment variable be pulled
     :type name: str
 
     :param required: Whether the environment variable is required. If ``True``
@@ -173,15 +175,16 @@
 
 def env_list(
     name: str,
     separator: str = ",",
     required: bool = False,
     default: Union[Type[empty], List[Any]] = empty,
 ) -> List[Any]:
-    """Pulls an environment variable out of the environment, splitting it on a
+    """
+    Pulls an environment variable out of the environment, splitting it on a
     separator, and returning it as a list. Extra whitespace on the list values
     is stripped. List values that evaluate as falsy are removed. If not present
     and no default specified, an empty list is returned.
 
     :param name: The name of the environment variable be pulled
     :type name: str
 
@@ -209,15 +212,16 @@
 
 def get(
     name: str,
     required: bool = False,
     default: Union[Type[empty], T] = empty,
     type: Type[T] = None,
 ) -> T:
-    """Generic getter for environment variables. Handles defaults,
+    """
+    Generic getter for environment variables. Handles defaults,
     required-ness, and what type to expect.
 
     :param name: The name of the environment variable be pulled
     :type name: str
 
     :param required: Whether the environment variable is required. If ``True``
     and the variable is not present, a ``KeyError`` is raised.
```

### Comparing `py-evm-0.8.0b1/eth/_utils/generator.py` & `py-evm-0.9.0b1/eth/_utils/generator.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/headers.py` & `py-evm-0.9.0b1/eth/_utils/headers.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,20 +57,20 @@
 
 def fill_header_params_from_parent(
     parent: BlockHeaderAPI,
     gas_limit: int,
     difficulty: int,
     timestamp: int,
     coinbase: Address = ZERO_ADDRESS,
-    nonce: bytes = None,
-    extra_data: bytes = None,
-    transaction_root: bytes = None,
-    state_root: bytes = None,
-    mix_hash: bytes = None,
-    receipt_root: bytes = None,
+    nonce: Optional[bytes] = None,
+    extra_data: Optional[bytes] = None,
+    transaction_root: Optional[bytes] = None,
+    state_root: Optional[bytes] = None,
+    mix_hash: Optional[bytes] = None,
+    receipt_root: Optional[bytes] = None,
 ) -> Dict[str, HeaderParams]:
     if parent is None:
         parent_hash = GENESIS_PARENT_HASH
         block_number = GENESIS_BLOCK_NUMBER
         if state_root is None:
             state_root = BLANK_ROOT_HASH
     else:
```

### Comparing `py-evm-0.8.0b1/eth/_utils/module_loading.py` & `py-evm-0.9.0b1/eth/_utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/numeric.py` & `py-evm-0.9.0b1/eth/_utils/numeric.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import decimal
-import functools
 import itertools
 from typing import (
     Union,
 )
 
 from eth_typing import (
     Hash32,
@@ -26,24 +25,21 @@
         raise ValueError(f"Value cannot be negative: Got: {value}")
     if value > UINT_256_MAX:
         raise ValueError(f"Value exeeds maximum UINT256 size.  Got: {value}")
     value_bytes = value.to_bytes(32, "big")
     return Hash32(value_bytes)
 
 
-def ceilXX(value: int, ceiling: int) -> int:
-    remainder = value % ceiling
-    if remainder == 0:
-        return value
-    else:
-        return value + ceiling - remainder
+# hotspot, optimized
+def ceil32(x: int) -> int:
+    return (x + 31) & ~31
 
 
-ceil32 = functools.partial(ceilXX, ceiling=32)
-ceil8 = functools.partial(ceilXX, ceiling=8)
+def ceil8(x: int) -> int:
+    return (x + 7) & ~7
 
 
 def unsigned_to_signed(value: int) -> int:
     if value <= UINT_255_MAX:
         return value
     else:
         return value - UINT_256_CEILING
```

### Comparing `py-evm-0.8.0b1/eth/_utils/rlp.py` & `py-evm-0.9.0b1/eth/_utils/rlp.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/spoof.py` & `py-evm-0.9.0b1/eth/_utils/spoof.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/state.py` & `py-evm-0.9.0b1/eth/_utils/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/_utils/transactions.py` & `py-evm-0.9.0b1/eth/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/abc.py` & `py-evm-0.9.0b1/eth/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,15 +467,14 @@
         But if you must access the original v, then you can cast to this API
         first (after checking that type_id is None).
         """
         ...
 
 
 class UnsignedTransactionAPI(BaseTransactionAPI):
-
     """
     A class representing a transaction before it is signed.
     """
 
     nonce: int
     gas_price: int
     gas: int
@@ -650,15 +649,14 @@
     #
     @abstractmethod
     def validate(self) -> None:
         """
         Hook called during instantiation to ensure that all transaction
         parameters pass validation rules.
         """
-
         ...
 
     #
     # Signature and Sender
     #
     @property
     @abstractmethod
@@ -811,15 +809,17 @@
 
     @abstractmethod
     def __init__(
         self,
         header: BlockHeaderAPI,
         transactions: Sequence[SignedTransactionAPI],
         uncles: Sequence[BlockHeaderAPI],
-        withdrawals: Sequence[WithdrawalAPI] = None,  # only present post-Shanghai
+        withdrawals: Optional[
+            Sequence[WithdrawalAPI]
+        ] = None,  # only present post-Shanghai
     ) -> None:
         ...
 
     @classmethod
     @abstractmethod
     def get_transaction_builder(cls) -> Type[TransactionBuilderAPI]:
         """
@@ -1036,16 +1036,14 @@
     The readable/writeable object returned by an atomic database when we start building
     a batch of writes to commit.
 
     Reads to this database will observe writes written during batching,
     but the writes will not actually persist until this object is committed.
     """
 
-    pass
-
 
 class AtomicDatabaseAPI(DatabaseAPI):
     """
     Like ``BatchDB``, but immediately write out changes if they are
     not in an ``atomic_batch()`` context.
     """
 
@@ -1503,34 +1501,20 @@
     @classmethod
     @abstractmethod
     def as_opcode(
         cls: Type[T],
         logic_fn: Callable[["ComputationAPI"], None],
         mnemonic: str,
         gas_cost: int,
-    ) -> T:
+    ) -> "OpcodeAPI":
         """
         Class factory method for turning vanilla functions into Opcodes.
         """
         ...
 
-    @abstractmethod
-    def __copy__(self) -> "OpcodeAPI":
-        """
-        Return a copy of the opcode.
-        """
-        ...
-
-    @abstractmethod
-    def __deepcopy__(self, memo: Any) -> "OpcodeAPI":
-        """
-        Return a deep copy of the opcode.
-        """
-        ...
-
 
 class ChainContextAPI(ABC):
     """
     Immutable chain context information that remains constant over the VM execution.
     """
 
     @abstractmethod
@@ -2768,15 +2752,14 @@
     def build_computation(
         self, message: MessageAPI, transaction: SignedTransactionAPI
     ) -> "ComputationAPI":
         """
         Apply the ``message`` to the VM and use the given ``transaction`` to
         retrieve the context from.
         """
-
         ...
 
     @abstractmethod
     def finalize_computation(
         self, transaction: SignedTransactionAPI, computation: "ComputationAPI"
     ) -> "ComputationAPI":
         """
@@ -3408,15 +3391,14 @@
         receipt: ReceiptAPI,
     ) -> None:
         """
         A hook for a subclass to use as a way to note that a transaction was applied.
         This only gets triggered as part of `apply_all_transactions`, which is called
         by `block_import`.
         """
-        pass
 
     #
     # Execution
     #
     @abstractmethod
     def apply_transaction(
         self, header: BlockHeaderAPI, transaction: SignedTransactionAPI
```

### Comparing `py-evm-0.8.0b1/eth/chains/base.py` & `py-evm-0.9.0b1/eth/chains/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import operator
 import random
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
+    Optional,
     Sequence,
     Tuple,
     Type,
 )
 
 from eth_typing import (
     Address,
@@ -710,16 +711,16 @@
         header_params = {k: v for k, v in kwargs.items() if k in header_fields}
         return base_header.copy(**header_params)
 
     def mine_all(
         self,
         transactions: Sequence[SignedTransactionAPI],
         *args: Any,
-        parent_header: BlockHeaderAPI = None,
-        withdrawals: Sequence[WithdrawalAPI] = None,
+        parent_header: Optional[BlockHeaderAPI] = None,
+        withdrawals: Optional[Sequence[WithdrawalAPI]] = None,
         **kwargs: Any,
     ) -> Tuple[BlockImportResult, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
         if parent_header is None:
             base_header = self.header
         else:
             base_header = self.create_header_from_parent(parent_header)
```

### Comparing `py-evm-0.8.0b1/eth/chains/goerli/__init__.py` & `py-evm-0.9.0b1/eth/chains/goerli/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/chains/header.py` & `py-evm-0.9.0b1/eth/chains/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/chains/mainnet/__init__.py` & `py-evm-0.9.0b1/eth/chains/mainnet/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/chains/mainnet/constants.py` & `py-evm-0.9.0b1/eth/chains/mainnet/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/chains/ropsten/__init__.py` & `py-evm-0.9.0b1/eth/chains/ropsten/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/chains/ropsten/constants.py` & `py-evm-0.9.0b1/eth/chains/ropsten/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/chains/tester/__init__.py` & `py-evm-0.9.0b1/eth/chains/tester/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import collections
 import operator
 from typing import (
     Any,
     Generator,
+    Optional,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
 from eth_typing import BlockNumber
@@ -54,15 +55,16 @@
 
 ForkStartBlocks = Sequence[Tuple[BlockNumber, Union[str, Type[VirtualMachineAPI]]]]
 VMStartBlock = Tuple[BlockNumber, Type[VirtualMachineAPI]]
 
 
 @to_tuple
 def _generate_vm_configuration(
-    *fork_start_blocks: ForkStartBlocks, dao_start_block: Union[int, bool] = None
+    *fork_start_blocks: ForkStartBlocks,
+    dao_start_block: Optional[Union[int, bool]] = None,
 ) -> Generator[VMStartBlock, None, None]:
     """
     fork_start_blocks should be 2-tuples of (start_block, fork_name_or_vm_class)
 
     dao_start_block determines whether the Homestead fork will support the DAO
     fork and if so, at what block.
 
@@ -153,15 +155,15 @@
         We don't validate the proof of work seal on the tester chain.
         """
         pass
 
     def configure_forks(
         self,
         *fork_start_blocks: ForkStartBlocks,
-        dao_start_block: Union[int, bool] = None,
+        dao_start_block: Optional[Union[int, bool]] = None,
     ) -> None:
         """
         On demand configuration of fork rules.  This is a foot gun that if used
         incorrectly could cause weird VM errors.
 
         It should generally only be used on a genesis chain (head block == 0).
         Modifying the fork rules, especially if the modification effects
```

### Comparing `py-evm-0.8.0b1/eth/consensus/applier.py` & `py-evm-0.9.0b1/eth/consensus/applier.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/consensus/clique/_utils.py` & `py-evm-0.9.0b1/eth/consensus/clique/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 
 @to_tuple
 def get_signers_at_checkpoint(header: BlockHeaderAPI) -> Iterable[Address]:
     """
     Read the list of signers from a checkpoint header.
     """
-
     signers_length = len(header.extra_data) - VANITY_LENGTH - SIGNATURE_LENGTH
 
     if signers_length % COMMON_ADDRESS_LENGTH != 0:
         raise ValidationError("Checkpoint header must contain list of signers")
 
     signer_count = int(
         (len(header.extra_data) - VANITY_LENGTH - SIGNATURE_LENGTH)
@@ -69,29 +68,27 @@
 
 def get_signature_hash(header: BlockHeaderAPI) -> Hash32:
     """
     Return the hash that is signed by the block producer. It is defined as the hash of
     the ``header`` except that the last 65 bytes of the ``extra_data`` (the signature)
     are removed before calculating the hash.
     """
-
     if len(header.extra_data) < SIGNATURE_LENGTH:
         raise ValueError("header.extra_data too short to contain signature")
 
     signature_header: BlockHeaderAPI = header.copy(
         extra_data=header.extra_data[: len(header.extra_data) - SIGNATURE_LENGTH]
     )
     return signature_header.hash
 
 
 def get_block_signer(header: BlockHeaderAPI) -> Address:
     """
     Return the address of the signer of the ``header``.
     """
-
     signature_hash = get_signature_hash(header)
 
     signature_bytes = header.extra_data[-SIGNATURE_LENGTH:]
 
     signature = keys.Signature(signature_bytes=signature_bytes)
 
     return signature.recover_public_key_from_msg_hash(
```

### Comparing `py-evm-0.8.0b1/eth/consensus/clique/clique.py` & `py-evm-0.9.0b1/eth/consensus/clique/clique.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,14 @@
     def validate_seal_extension(
         self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
     ) -> None:
         """
         Validate the seal of the given ``header`` according
         to the Clique consensus rules.
         """
-
         if header.block_number == 0:
             return
 
         validate_header_integrity(header, self._epoch_length)
 
         signer = get_block_signer(header)
         snapshot = self._snapshot_manager.get_or_create_snapshot(
```

### Comparing `py-evm-0.8.0b1/eth/consensus/clique/datatypes.py` & `py-evm-0.9.0b1/eth/consensus/clique/datatypes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/consensus/clique/encoding.py` & `py-evm-0.9.0b1/eth/consensus/clique/encoding.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/consensus/clique/snapshot_manager.py` & `py-evm-0.9.0b1/eth/consensus/clique/snapshot_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 )
 from .exceptions import (
     SnapshotNotFound,
 )
 
 
 def make_snapshot_lookup_key(block_hash: Hash32) -> bytes:
-    return b"block-hash-to-snapshot:%s" % block_hash
+    return f"block-hash-to-snapshot:{block_hash}".encode()
 
 
 class SnapshotManager:
     """
     The ``SnapshotManager`` is responsible for managing the snapshots that hold the
     current state of the consensus engine. It creates new snapshots by applying headers
     on top of existing snapshots. It comes with APIs to create,
@@ -73,32 +73,31 @@
     ) -> BlockHeaderAPI:
         for parent in parents:
             if parent.hash == block_hash:
                 return parent
         try:
             return self._chain_db.get_block_header_by_hash(block_hash)
         except HeaderNotFound:
-            raise ValidationError("Unknown ancestor %s", encode_hex(block_hash))
+            raise ValidationError(f"Unknown ancestor {encode_hex(block_hash)}")
 
     def _create_snapshot_from_checkpoint_header(
         self, header: BlockHeaderAPI
     ) -> Snapshot:
         signers = get_signers_at_checkpoint(header)
-        self.logger.debug2("Created snapshot from checkpoint at %s", header)
+        self.logger.debug2(f"Created snapshot from checkpoint at {header}")
 
         snapshot = MutableSnapshot(
             signers=list(signers), block_hash=header.hash, votes=[], tallies={}
         )
         return self.add_snapshot(snapshot)
 
     def apply(self, current_snapshot: Snapshot, header: BlockHeaderAPI) -> Snapshot:
         """
         Apply the given header on top of the current snapshot to create a new snapshot.
         """
-
         if is_checkpoint(header.block_number, self._epoch_length):
             return self._create_snapshot_from_checkpoint_header(header)
 
         snapshot = current_snapshot.get_mutable_clone(header.hash)
 
         if header.nonce in {NONCE_AUTH, NONCE_DROP}:
             signer = get_block_signer(header)
@@ -120,19 +119,19 @@
                 )
                 snapshot.votes.append(vote)
 
                 tally = snapshot.tallies[header.coinbase]
                 if tally.votes > len(snapshot.signers) / 2:
                     if tally.action is VoteAction.NOMINATE:
                         snapshot.signers.append(header.coinbase)
-                        self.logger.debug("New signer added: %s", header.coinbase)
+                        self.logger.debug(f"New signer added: {header.coinbase}")
                     else:
                         if header.coinbase in snapshot.signers:
                             snapshot.signers.remove(header.coinbase)
-                            self.logger.debug("Signer removed: %s", header.coinbase)
+                            self.logger.debug(f"Signer removed: {header.coinbase}")
 
                     for vote in snapshot.votes.copy():
                         # Discard any pending votes *from* the added or removed member
                         if vote.signer == header.coinbase:
                             if self.retract_vote(snapshot, vote.subject, vote.action):
                                 snapshot.votes.remove(vote)
 
@@ -205,27 +204,26 @@
         for parent in reversed(parents):
             new_snapshot = self.apply(new_snapshot, parent)
 
         new_snapshot = self.apply(new_snapshot, header)
 
         if is_checkpoint(header.block_number, self._epoch_length):
             self.logger.debug2(
-                "Persisting checkpoint snapshot at %s", header.block_number
+                f"Persisting checkpoint snapshot at {header.block_number}",
             )
             self.persist_snapshot(new_snapshot)
 
         return new_snapshot
 
     def get_snapshot(self, block_number: int, block_hash: Hash32) -> Snapshot:
         """
         Return a ``Snapshot`` if it exists in memory, on-disk or can be computed
         directly from a header that serves as a checkpoint.
         Otherwise raise a ``SnapshotNotFound`` error.
         """
-
         # We first try to find the snapshot in memory
         if block_hash in self._snapshots:
             return self._snapshots[block_hash]
 
         if is_checkpoint(block_number, self._epoch_length):
             try:
                 # We might have it saved on disk
```

### Comparing `py-evm-0.8.0b1/eth/consensus/ethash.py` & `py-evm-0.9.0b1/eth/consensus/ethash.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/consensus/noproof.py` & `py-evm-0.9.0b1/eth/consensus/noproof.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/consensus/pos.py` & `py-evm-0.9.0b1/eth/consensus/pos.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/consensus/pow.py` & `py-evm-0.9.0b1/eth/consensus/pow.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/constants.py` & `py-evm-0.9.0b1/eth/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/__init__.py` & `py-evm-0.9.0b1/eth/db/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/accesslog.py` & `py-evm-0.9.0b1/eth/db/accesslog.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/account.py` & `py-evm-0.9.0b1/eth/db/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,17 +458,16 @@
     def make_state_root(self) -> Hash32:
         for _address, store in self._dirty_account_stores():
             store.make_storage_root()
 
         for address, storage_root in self._get_changed_roots():
             if self.account_exists(address) or storage_root != BLANK_ROOT_HASH:
                 self.logger.debug2(
-                    "Updating account 0x%s to storage root 0x%s",
-                    address.hex(),
-                    storage_root.hex(),
+                    f"Updating account 0x{address.hex()} to storage root "
+                    f"0x{storage_root.hex()}",
                 )
                 self._set_storage_root(address, storage_root)
 
         self._journaldb.persist()
 
         diff = self._journaltrie.diff()
         if diff.deleted_keys() or diff.pending_items():
@@ -516,15 +515,15 @@
         #   will get added to _accessed_accounts correctly. Account accesses that
         #   are cached do not add the address to the list of accessed accounts.
         self._account_cache.clear()
 
         # persist accounts
         self._validate_generated_root()
         new_root_hash = self.state_root
-        self.logger.debug2("Persisting new state root: 0x%s", new_root_hash.hex())
+        self.logger.debug2(f"Persisting new state root: 0x{new_root_hash.hex()}")
         with self._raw_store_db.atomic_batch() as write_batch:
             self._batchtrie.commit_to(write_batch, apply_deletes=False)
             self._batchdb.commit_to(write_batch, apply_deletes=False)
         self._root_hash_at_last_persist = new_root_hash
 
         return meta_witness
 
@@ -575,31 +574,29 @@
         if not self.logger.show_debug2:
             return
 
         diff = self._journaltrie.diff()
         for address in sorted(diff.pending_keys()):
             account = self._get_account(Address(address))
             self.logger.debug2(
-                "Pending Account %s: balance %d, nonce %d, storage root %s, code hash %s",  # noqa: E501
-                to_checksum_address(address),
-                account.balance,
-                account.nonce,
-                encode_hex(account.storage_root),
-                encode_hex(account.code_hash),
+                f"Pending Account {to_checksum_address(address)}: "
+                f"balance {account.balance}, "
+                f"nonce {account.nonce}, "
+                f"storage root {encode_hex(account.storage_root)}, "
+                f"code hash {encode_hex(account.code_hash)}"
             )
         for deleted_address in sorted(diff.deleted_keys()):
             # Check if the account was accessed before accessing/logging
             # info about the address
             was_account_accessed = deleted_address in self._accessed_accounts
             cast_deleted_address = Address(deleted_address)
             self.logger.debug2(
-                "Deleted Account %s, empty? %s, exists? %s",
-                to_checksum_address(deleted_address),
-                self.account_is_empty(cast_deleted_address),
-                self.account_exists(cast_deleted_address),
+                f"Deleted Account {to_checksum_address(deleted_address)}, "
+                f"empty? {self.account_is_empty(cast_deleted_address)}, "
+                f"exists? {self.account_exists(cast_deleted_address)}"
             )
             # If the account was not accessed previous to the log,
             # (re)mark it as not accessed
             if not was_account_accessed:
                 self._accessed_accounts.remove(cast_deleted_address)
 
     def _apply_account_diff_without_proof(
@@ -615,17 +612,16 @@
         # for accounts that were not needed during normal execution. We only need these
         # nodes to refactor the trie.
         for delete_key in diff.deleted_keys():
             try:
                 del trie[delete_key]
             except trie_exceptions.MissingTrieNode as exc:
                 self.logger.debug(
-                    "Missing node while deleting account with key %s: %s",
-                    encode_hex(delete_key),
-                    exc,
+                    "Missing node while deleting account with key "
+                    f"{encode_hex(delete_key)}: {exc}"
                 )
                 raise MissingAccountTrieNode(
                     exc.missing_node_hash,
                     self._root_hash_at_last_persist,
                     exc.requested_key,
                 ) from exc
 
@@ -645,17 +641,15 @@
         #   - We need the full body of the old (1, 2) leaf node, to rebuild
 
         for key, val in diff.pending_items():
             try:
                 trie[key] = val
             except trie_exceptions.MissingTrieNode as exc:
                 self.logger.debug(
-                    "Missing node on account update key %s to %s: %s",
-                    encode_hex(key),
-                    encode_hex(val),
-                    exc,
+                    f"Missing node on account update key {encode_hex(key)} to "
+                    f"{encode_hex(val)}: {exc}"
                 )
                 raise MissingAccountTrieNode(
                     exc.missing_node_hash,
                     self._root_hash_at_last_persist,
                     exc.requested_key,
                 ) from exc
```

### Comparing `py-evm-0.8.0b1/eth/db/atomic.py` & `py-evm-0.9.0b1/eth/db/atomic.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,16 @@
         intended to be used by AtomicDB.
         """
         readable_write_batch: AtomicDBWriteBatch = cls(write_target_db)
         try:
             yield readable_write_batch
         except Exception:
             cls.logger.exception(
-                "Unexpected error in atomic db write, dropped partial writes: %r",
-                readable_write_batch._diff(),
+                "Unexpected error in atomic db write, dropped partial writes: "
+                f"{repr(readable_write_batch._diff())}"
             )
             raise
         else:
             readable_write_batch._commit()
         finally:
             # force a shutdown of this batch, to prevent out-of-context usage
             readable_write_batch._track_diff = None
```

### Comparing `py-evm-0.8.0b1/eth/db/backends/base.py` & `py-evm-0.9.0b1/eth/db/backends/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,9 +73,7 @@
             if some_bad_condition:
                 raise Exception("something went wrong, erase all the pending changes")
 
             db[key2] = val2
             # when exiting the context, the values are saved either key and key2 will
             # both be saved, or neither will
     """
-
-    pass
```

### Comparing `py-evm-0.8.0b1/eth/db/backends/memory.py` & `py-evm-0.9.0b1/eth/db/backends/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/batch.py` & `py-evm-0.9.0b1/eth/db/batch.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/cache.py` & `py-evm-0.9.0b1/eth/db/cache.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/chain.py` & `py-evm-0.9.0b1/eth/db/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,17 +293,16 @@
 
         if block.uncles:
             uncles_hash = cls._persist_uncles(db, block.uncles)
         else:
             uncles_hash = EMPTY_UNCLE_HASH
         if uncles_hash != block.header.uncles_hash:
             raise ValidationError(
-                "Block's uncles_hash (%s) does not match actual uncles' hash (%s)",
-                block.header.uncles_hash,
-                uncles_hash,
+                f"Block's uncles_hash ({block.header.uncles_hash}) does not match "
+                f"actual uncles' hash ({uncles_hash})"
             )
         new_canonical_hashes = tuple(header.hash for header in new_canonical_headers)
         old_canonical_hashes = tuple(header.hash for header in old_canonical_headers)
 
         cls._update_chain_gaps(db, block)
         return new_canonical_hashes, old_canonical_hashes
```

### Comparing `py-evm-0.8.0b1/eth/db/chain_gaps.py` & `py-evm-0.9.0b1/eth/db/chain_gaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     return block_number >= tip_child
 
 
 def fill_gap(newly_persisted: BlockNumber, base_gaps: ChainGaps) -> GapInfo:
     """
     Remove a gap, for a new header that was canonicalized.
     """
-
     current_gaps, tip_child = base_gaps
 
     if newly_persisted == tip_child:
         # This is adding a consecutive header at the very tail
         new_gaps = (current_gaps, BlockNumber(newly_persisted + 1))
         gap_change = GapChange.TailWrite
     elif newly_persisted > tip_child:
```

### Comparing `py-evm-0.8.0b1/eth/db/diff.py` & `py-evm-0.9.0b1/eth/db/diff.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/header.py` & `py-evm-0.9.0b1/eth/db/header.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,14 @@
     ) -> ChainGaps:
         """
         A single block number was found to no longer be canonical. At doc-time,
         this only happens because it does not link up with a checkpoint header.
         So de-canonicalize this block number and insert a gap in the tracked
         chain gaps.
         """
-
         db.delete(SchemaV1.make_block_number_to_hash_lookup_key(block_num))
 
         new_gaps = reopen_gap(block_num, base_gaps)
         if new_gaps != base_gaps:
             db.set(
                 SchemaV1.make_header_chain_gaps_lookup_key(),
                 rlp.encode(new_gaps, sedes=chain_gaps),
```

### Comparing `py-evm-0.8.0b1/eth/db/journal.py` & `py-evm-0.9.0b1/eth/db/journal.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/keymap.py` & `py-evm-0.9.0b1/eth/db/keymap.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/schema.py` & `py-evm-0.9.0b1/eth/db/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 class SchemaV1(SchemaAPI):
     @staticmethod
     def make_canonical_head_hash_lookup_key() -> bytes:
         return b"v1:canonical_head_hash"
 
     @staticmethod
     def make_block_number_to_hash_lookup_key(block_number: BlockNumber) -> bytes:
-        number_to_hash_key = b"block-number-to-hash:%d" % block_number
+        number_to_hash_key = f"block-number-to-hash:{block_number}".encode()
         return number_to_hash_key
 
     @staticmethod
     def make_block_hash_to_score_lookup_key(block_hash: Hash32) -> bytes:
-        return b"block-hash-to-score:%s" % block_hash
+        return f"block-hash-to-score:{block_hash}".encode()
 
     @staticmethod
     def make_header_chain_gaps_lookup_key() -> bytes:
         return b"v1:header_chain_gaps"
 
     @staticmethod
     def make_chain_gaps_lookup_key() -> bytes:
@@ -35,12 +35,12 @@
         """
         Checkpoint header hashes stored as concatenated 32 byte values
         """
         return b"v1:checkpoint-header-hashes-list"
 
     @staticmethod
     def make_transaction_hash_to_block_lookup_key(transaction_hash: Hash32) -> bytes:
-        return b"transaction-hash-to-block:%s" % transaction_hash
+        return f"transaction-hash-to-block:{transaction_hash}".encode()
 
     @staticmethod
     def make_withdrawal_hash_to_block_lookup_key(withdrawal_hash: Hash32) -> bytes:
-        return b"withdrawal-hash-to-block:%s" % withdrawal_hash
+        return f"withdrawal-hash-to-block:{withdrawal_hash}".encode()
```

### Comparing `py-evm-0.8.0b1/eth/db/slow_journal.py` & `py-evm-0.9.0b1/eth/db/slow_journal.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     def has_clear(self, check_changeset_id: uuid.UUID) -> bool:
         for changeset_id in reversed(self.journal_data.keys()):
             if changeset_id in self._clears_at:
                 return True
             elif check_changeset_id == changeset_id:
                 return False
         raise ValidationError(
-            "Changeset ID %s is not in the journal" % check_changeset_id
+            f"Changeset ID {check_changeset_id} is not in the journal"
         )
 
     def commit_changeset(
         self, changeset_id: uuid.UUID
     ) -> Dict[bytes, Union[bytes, DeletedEntry]]:
         """
         Collapses all changes for the given changeset into the previous
```

### Comparing `py-evm-0.8.0b1/eth/db/storage.py` & `py-evm-0.9.0b1/eth/db/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,14 @@
         """
         Revert back to the previous trie, using the index returned by a
         :meth:`~new_trie` call. The index returned by that call returns you
         to the trie in place *before* the call.
 
         :param trie_index: index for reviving the previous trie
         """
-
         if trie_index >= len(self._historical_write_tries):
             raise ValidationError(
                 f"Trying to roll back a delete to index {trie_index}, but there are "
                 f"only {len(self._historical_write_tries)} indices available."
             )
 
         (
@@ -341,16 +340,15 @@
             else:
                 if current_val != b"":
                     # only try to delete the value if it's present
                     del self._journal_storage[key]
 
     def delete(self) -> None:
         self.logger.debug2(
-            "Deleting all storage in account 0x%s",
-            self._address.hex(),
+            f"Deleting all storage in account 0x{self._address.hex()}",
         )
         self._journal_storage.clear()
         self._storage_cache.reset_cache()
 
         # Empty out the storage lookup trie (keeping history, in case of a revert)
         new_clear_count = self._storage_lookup.new_trie()
 
@@ -370,15 +368,15 @@
         self._clear_count[CLEAR_COUNT_KEY_NAME] = to_bytes(new_clear_count)
 
     def record(self, checkpoint: JournalDBCheckpoint) -> None:
         self._journal_storage.record(checkpoint)
         self._clear_count.record(checkpoint)
 
     def discard(self, checkpoint: JournalDBCheckpoint) -> None:
-        self.logger.debug2("discard checkpoint %r", checkpoint)
+        self.logger.debug2(f"discard checkpoint {repr(checkpoint)}")
         latest_clear_count = to_int(self._clear_count[CLEAR_COUNT_KEY_NAME])
 
         if self._journal_storage.has_checkpoint(checkpoint):
             self._journal_storage.discard(checkpoint)
             self._clear_count.discard(checkpoint)
         else:
             # if the checkpoint comes before this account started tracking,
```

### Comparing `py-evm-0.8.0b1/eth/db/trie.py` & `py-evm-0.9.0b1/eth/db/trie.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/db/witness.py` & `py-evm-0.9.0b1/eth/db/witness.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/estimators/__init__.py` & `py-evm-0.9.0b1/eth/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/estimators/gas.py` & `py-evm-0.9.0b1/eth/estimators/gas.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/exceptions.py` & `py-evm-0.9.0b1/eth/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,20 @@
 
 
 class PyEVMError(Exception):
     """
     Base class for all py-evm errors.
     """
 
-    pass
-
 
 class VMNotFound(PyEVMError):
     """
     Raised when no VM is available for the provided block number.
     """
 
-    pass
-
 
 class StateRootNotFound(PyEVMError):
     """
     Raised when the requested state root is not present in our DB.
     """
 
     @property
@@ -38,24 +34,20 @@
 class BlockNotFound(PyEVMError):
     """
     Raised when the block with the given number/hash does not exist.
     This will happen, for example, if the transactions or uncles are not
     saved in the database.
     """
 
-    pass
-
 
 class TransactionNotFound(PyEVMError):
     """
     Raised when the transaction with the given hash or block index does not exist.
     """
 
-    pass
-
 
 class UnrecognizedTransactionType(PyEVMError):
     """
     Raised when an encoded transaction is using a first byte that is valid, but
     unrecognized. According to EIP 2718, the byte may be in the range [0, 0x7f].
     As of the Berlin hard fork, all of those versions are undefined, except for
     0x01 in EIP 2930.
@@ -67,57 +59,45 @@
 
 
 class ReceiptNotFound(PyEVMError):
     """
     Raised when the Receipt with the given receipt index does not exist.
     """
 
-    pass
-
 
 class ParentNotFound(HeaderNotFound):
     """
     Raised when the parent of a given block does not exist.
     """
 
-    pass
-
 
 class CanonicalHeadNotFound(PyEVMError):
     """
     Raised when the chain has no canonical head.
     """
 
-    pass
-
 
 class GapTrackingCorrupted(PyEVMError):
     """
     Raised when the tracking of chain gaps appears to be corrupted
     (e.g. overlapping gaps)
     """
 
-    pass
-
 
 class CheckpointsMustBeCanonical(PyEVMError):
     """
     Raised when a persisted header attempts to de-canonicalize a checkpoint
     """
 
-    pass
-
 
 class Halt(PyEVMError):
     """
     Raised when an opcode function halts vm execution.
     """
 
-    pass
-
 
 class VMError(PyEVMError):
     """
     Base class for errors raised during VM execution.
     """
 
     burns_gas = True
@@ -125,82 +105,64 @@
 
 
 class OutOfGas(VMError):
     """
     Raised when a VM execution has run out of gas.
     """
 
-    pass
-
 
 class InsufficientStack(VMError):
     """
     Raised when the stack is empty.
     """
 
-    pass
-
 
 class FullStack(VMError):
     """
     Raised when the stack is full.
     """
 
-    pass
-
 
 class InvalidJumpDestination(VMError):
     """
     Raised when the jump destination for a JUMPDEST operation is invalid.
     """
 
-    pass
-
 
 class InvalidInstruction(VMError):
     """
     Raised when an opcode is invalid.
     """
 
-    pass
-
 
 class InsufficientFunds(VMError):
     """
     Raised when an account has insufficient funds to transfer the
     requested value.
     """
 
-    pass
-
 
 class StackDepthLimit(VMError):
     """
     Raised when the call stack has exceeded it's maximum allowed depth.
     """
 
-    pass
-
 
 class ContractCreationCollision(VMError):
     """
     Raised when there was an address collision during contract creation.
     """
 
-    pass
-
 
 class IncorrectContractCreationAddress(VMError):
     """
     Raised when the address provided by transaction does not
     match the calculated contract creation address.
     """
 
-    pass
-
 
 class Revert(VMError):
     """
     Raised when the REVERT opcode occured
     """
 
     burns_gas = False
@@ -209,26 +171,20 @@
 
 class WriteProtection(VMError):
     """
     Raised when an attempt to modify the state database is made while
     operating inside of a STATICCALL context.
     """
 
-    pass
-
 
 class OutOfBoundsRead(VMError):
     """
     Raised when an attempt was made to read data beyond the
     boundaries of the buffer (such as with RETURNDATACOPY)
     """
 
-    pass
-
 
 class ReservedBytesInCode(VMError):
     """
     Raised when bytes for the code to be deployed are reserved
     for a particular reason.
     """
-
-    pass
```

### Comparing `py-evm-0.8.0b1/eth/precompiles/blake2.py` & `py-evm-0.9.0b1/eth/precompiles/blake2.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/precompiles/ecadd.py` & `py-evm-0.9.0b1/eth/precompiles/ecadd.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/precompiles/ecmul.py` & `py-evm-0.9.0b1/eth/precompiles/ecmul.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/precompiles/ecpairing.py` & `py-evm-0.9.0b1/eth/precompiles/ecpairing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/precompiles/ecrecover.py` & `py-evm-0.9.0b1/eth/precompiles/ecrecover.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/precompiles/modexp.py` & `py-evm-0.9.0b1/eth/precompiles/modexp.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/precompiles/ripemd160.py` & `py-evm-0.9.0b1/eth/precompiles/ripemd160.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/precompiles/sha256.py` & `py-evm-0.9.0b1/eth/precompiles/sha256.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/rlp/accounts.py` & `py-evm-0.9.0b1/eth/rlp/accounts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/rlp/blocks.py` & `py-evm-0.9.0b1/eth/rlp/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/rlp/headers.py` & `py-evm-0.9.0b1/eth/rlp/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/rlp/logs.py` & `py-evm-0.9.0b1/eth/rlp/logs.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/rlp/receipts.py` & `py-evm-0.9.0b1/eth/rlp/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/rlp/transactions.py` & `py-evm-0.9.0b1/eth/rlp/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/_utils/deprecation.py` & `py-evm-0.9.0b1/eth/tools/_utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/_utils/hashing.py` & `py-evm-0.9.0b1/eth/tools/_utils/hashing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/_utils/mappings.py` & `py-evm-0.9.0b1/eth/tools/_utils/mappings.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 
 def is_cleanly_mergable(*dicts: Dict[Any, Any]) -> bool:
     """
     Check that nothing will be overwritten when
     dictionaries are merged using `deep_merge`.
 
-    Examples:
+    Examples
+    --------
 
         >>> is_cleanly_mergable({"a": 1}, {"b": 2}, {"c": 3})
         True
         >>> is_cleanly_mergable({"a": 1}, {"b": 2}, {"a": 0, c": 3})
         False
         >>> is_cleanly_mergable({"a": 1, "b": {"ba": 2}}, {"c": 3, {"b": {"bb": 4}})
         True
```

### Comparing `py-evm-0.8.0b1/eth/tools/_utils/normalization.py` & `py-evm-0.9.0b1/eth/tools/_utils/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Callable,
     Dict,
     Iterable,
     List,
     Mapping,
     Sequence,
     Tuple,
+    TypedDict,
     Union,
     cast,
 )
 
 from eth_typing import (
     Address,
     HexStr,
@@ -41,17 +42,14 @@
     compose,
     concat,
     curried,
     curry,
     identity,
     merge,
 )
-from mypy_extensions import (
-    TypedDict,
-)
 
 from eth.constants import (
     CREATE_CONTRACT_ADDRESS,
 )
 from eth.tools._utils.mappings import (
     deep_merge,
     is_cleanly_mergable,
@@ -179,15 +177,16 @@
     return normalize
 
 
 #
 # Composition
 #
 def state_definition_to_dict(state_definition: GeneralState) -> AccountState:
-    """Convert a state definition to the canonical dict form.
+    """
+    Convert a state definition to the canonical dict form.
 
     State can either be defined in the canonical form, or as a list of sub states that
     are then merged to one. Sub states can either be given as dictionaries themselves,
     or as tuples where the last element is the value and all others the keys for this
     value in the nested state dictionary. Example:
 
     ```
@@ -378,23 +377,21 @@
                 ("data", "data"),
             ]
             if index_key in indexes
         },
     )
 
 
-FixtureAccountDetails = TypedDict(
-    "FixtureAccountDetails",
-    {
-        "balance": HexStr,
-        "nonce": HexStr,
-        "code": HexStr,
-        "storage": Dict[HexStr, HexStr],
-    },
-)
+class FixtureAccountDetails(TypedDict):
+    balance: HexStr
+    nonce: HexStr
+    code: HexStr
+    storage: Dict[HexStr, HexStr]
+
+
 FixtureAccountState = Dict[Address, FixtureAccountDetails]
 
 
 def normalize_account_state(account_state: FixtureAccountState) -> AccountState:
     return {
         to_canonical_address(address): {
             "balance": to_int(state["balance"]),
@@ -507,15 +504,15 @@
         "s": to_int(transaction["s"]),
         "v": to_int(transaction["v"]),
         "to": decode_hex(transaction["to"]),
         "value": to_int(transaction["value"]),
     }
     if "type" in transaction:
         type_id = to_int(transaction["type"])
-        if type_id == 1:
+        if type_id in (0, 1):
             custom_fields = {
                 "type": type_id,
                 "gasPrice": to_int(transaction["gasPrice"]),
                 "chainId": to_int(transaction["chainId"]),
             }
         elif type_id == 2:
             custom_fields = {
```

### Comparing `py-evm-0.8.0b1/eth/tools/_utils/slow_code_stream.py` & `py-evm-0.9.0b1/eth/tools/_utils/slow_code_stream.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/_utils/vyper.py` & `py-evm-0.9.0b1/eth/tools/_utils/vyper.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/builder/chain/__init__.py` & `py-evm-0.9.0b1/eth/tools/builder/chain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .builders import (  # noqa: F401
+from .builders import (
     at_block_number,
     build,
     chain_id,
     chain_split,
     copy,
     dao_fork_at,
     disable_dao_fork,
@@ -12,15 +12,15 @@
     genesis,
     import_block,
     import_blocks,
     mine_block,
     mine_blocks,
     name,
 )
-from .builders import (  # noqa: F401
+from .builders import (
     byzantium_at,
     frontier_at,
     homestead_at,
     spurious_dragon_at,
     tangerine_whistle_at,
     constantinople_at,
     petersburg_at,
```

### Comparing `py-evm-0.8.0b1/eth/tools/builder/chain/builders.py` & `py-evm-0.9.0b1/eth/tools/builder/chain/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 import time
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
+    Optional,
     Tuple,
     Type,
     Union,
     cast,
 )
 
 from eth_typing import (
@@ -357,17 +358,17 @@
     state = deep_merge(defaults, base_state)
     return state
 
 
 @curry
 def genesis(
     chain_class: ChainAPI,
-    db: AtomicDatabaseAPI = None,
-    params: Dict[str, HeaderParams] = None,
-    state: GeneralState = None,
+    db: Optional[AtomicDatabaseAPI] = None,
+    params: Optional[Dict[str, HeaderParams]] = None,
+    state: Optional[GeneralState] = None,
 ) -> ChainAPI:
     """
     Initialize the given chain class with the given genesis header parameters
     and chain state.
     """
     if state is None:
         genesis_state: AccountState = {}
@@ -393,17 +394,15 @@
 # Builders (build actual blockchain)
 #
 @curry
 def mine_block(chain: MiningChainAPI, **kwargs: Any) -> MiningChainAPI:
     """
     Mine a new block on the chain.  Header parameters for the new block can be
     overridden using keyword arguments.
-
     """
-
     if not isinstance(chain, MiningChainAPI):
         raise ValidationError("`mine_block` may only be used on MiningChain instances")
 
     transactions = kwargs.pop("transactions", ())
 
     chain.mine_all(transactions, **kwargs)
     return chain
```

### Comparing `py-evm-0.8.0b1/eth/tools/db/atomic.py` & `py-evm-0.9.0b1/eth/tools/db/atomic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import pytest
-
 from eth_utils import (
     ValidationError,
 )
+import pytest
 
 from eth.abc import (
     AtomicDatabaseAPI,
 )
 
 
 class AtomicDatabaseBatchAPITestSuite:
```

### Comparing `py-evm-0.8.0b1/eth/tools/db/base.py` & `py-evm-0.9.0b1/eth/tools/db/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/_utils.py` & `py-evm-0.9.0b1/eth/tools/fixtures/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/fillers/_utils.py` & `py-evm-0.9.0b1/eth/tools/fixtures/fillers/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/fillers/common.py` & `py-evm-0.9.0b1/eth/tools/fixtures/fillers/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     partial,
     wraps,
 )
 from typing import (
     Any,
     Callable,
     Dict,
+    Optional,
 )
 
 from eth_utils import (
     apply_formatters_to_dict,
     decode_hex,
     to_canonical_address,
 )
@@ -102,27 +103,27 @@
 
 #
 # Filler Generation
 #
 
 
 def setup_filler(
-    name: str, environment: Dict[Any, Any] = None
+    name: str, environment: Optional[Dict[Any, Any]] = None
 ) -> Dict[str, Dict[str, Any]]:
     environment = normalize_environment(environment or {})
     return {
         name: {
             "env": environment,
             "pre": {},
         }
     }
 
 
 def setup_main_filler(
-    name: str, environment: Dict[Any, Any] = None
+    name: str, environment: Optional[Dict[Any, Any]] = None
 ) -> Dict[str, Dict[str, Any]]:
     """
     Kick off the filler generation process by creating the general filler scaffold with
     a test name and general information about the testing environment.
 
     For tests for the main chain, the `environment` parameter is expected to be a
     dictionary with some or all of the following keys:
@@ -261,17 +262,17 @@
     expect = existing_expects + [new_expect]
     test_update = assoc_in(test_update, [test_name, "expect"], expect)
 
     return deep_merge(filler, test_update)
 
 
 def expect(
-    post_state: Dict[str, Any] = None,
-    networks: Any = None,
-    transaction: TransactionDict = None,
+    post_state: Optional[Dict[str, Any]] = None,
+    networks: Optional[Any] = None,
+    transaction: Optional[TransactionDict] = None,
 ) -> Callable[..., Dict[str, Any]]:
     """
     Specify the expected result for the test.
 
     For state tests, multiple expectations can be given, differing in the transaction
     data, gas limit, and value, in the applicable networks, and as a result also in the
     post state. VM tests support only a single expectation with no specified network and
```

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/fillers/formatters.py` & `py-evm-0.9.0b1/eth/tools/fixtures/fillers/formatters.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/fillers/main.py` & `py-evm-0.9.0b1/eth/tools/fixtures/fillers/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     Any,
     Dict,
+    Optional,
 )
 
 from eth_utils.toolz import (
     assoc_in,
     merge,
 )
 
@@ -22,40 +23,38 @@
 from .state import (
     fill_state_test,
 )
 from .vm import (
     fill_vm_test,
 )
 
-FILLED_WITH_TEMPLATE = "py-evm-{version}"
-
 
 #
 # Primary test filler
 #
 def fill_test(
     filler: Dict[str, Any],
-    info: Dict[str, Any] = None,
+    info: Optional[Dict[str, Any]] = None,
     apply_formatter: bool = True,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> Dict[str, Any]:
     test_name = get_test_name(filler)
     test = filler[test_name]
 
     if "transaction" in test:
         filled = fill_state_test(filler)
         formatter = filled_state_test_formatter
     elif "exec" in test:
         filled = fill_vm_test(filler, **kwargs)
         formatter = filled_vm_test_formatter
     else:
         raise ValueError("Given filler does not appear to be for VM or state test")
 
     info = merge(
-        {"filledwith": FILLED_WITH_TEMPLATE.format(version=get_version_from_git())},
+        {"filledwith": f"py-evm-{get_version_from_git()}"},
         info if info else {},
     )
     filled = assoc_in(filled, [test_name, "_info"], info)
 
     if apply_formatter:
         return formatter(filled)
     else:
```

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/fillers/state.py` & `py-evm-0.9.0b1/eth/tools/fixtures/fillers/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/fillers/vm.py` & `py-evm-0.9.0b1/eth/tools/fixtures/fillers/vm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import (
     Any,
     Dict,
     Iterable,
+    Optional,
     Tuple,
     Union,
 )
 
 from eth.tools._utils.hashing import (
     hash_log_entries,
 )
@@ -25,18 +26,18 @@
     get_test_name,
 )
 
 
 def fill_vm_test(
     filler: Dict[str, Any],
     *,
-    call_creates: Any = None,
-    gas_price: Union[int, str] = None,
+    call_creates: Optional[Any] = None,
+    gas_price: Optional[Union[int, str]] = None,
     gas_remaining: Union[int, str] = 0,
-    logs: Iterable[Tuple[bytes, Tuple[int, ...], bytes]] = None,
+    logs: Optional[Iterable[Tuple[bytes, Tuple[int, ...], bytes]]] = None,
     output: bytes = b""
 ) -> Dict[str, Dict[str, Any]]:
     test_name = get_test_name(filler)
     test = filler[test_name]
 
     environment = normalize_environment(test["env"])
     pre_state = normalize_state(test["pre"])
```

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/generation.py` & `py-evm-0.9.0b1/eth/tools/fixtures/generation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/helpers.py` & `py-evm-0.9.0b1/eth/tools/fixtures/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
         raise ValueError(f"Network {network} does not match any known VM rules")
 
 
 def genesis_fields_from_fixture(fixture: Dict[str, Any]) -> Dict[str, Any]:
     """
     Convert all genesis fields in a fixture to a dictionary of header fields and values.
     """
-
     header_fields = fixture["genesisBlockHeader"]
     base_fields = {
         "parent_hash": header_fields["parentHash"],
         "uncles_hash": header_fields["uncleHash"],
         "coinbase": header_fields["coinbase"],
         "state_root": header_fields["stateRoot"],
         "transaction_root": header_fields["transactionsTrie"],
@@ -215,15 +214,14 @@
 def genesis_params_from_fixture(fixture: Dict[str, Any]) -> Dict[str, Any]:
     """
     Convert a genesis fixture into a dict of the configurable header fields and values.
 
     Some fields cannot be explicitly set when creating a new header, like
     parent_hash, which is automatically set to the empty hash.
     """
-
     params = genesis_fields_from_fixture(fixture)
 
     # Confirm that (currently) non-configurable defaults are set correctly,
     #   then remove them because they cannot be configured on the header.
     defaults = (
         ("parent_hash", constants.GENESIS_PARENT_HASH),
         ("uncles_hash", constants.EMPTY_UNCLE_HASH),
```

### Comparing `py-evm-0.8.0b1/eth/tools/fixtures/loading.py` & `py-evm-0.9.0b1/eth/tools/fixtures/loading.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/tools/mining.py` & `py-evm-0.9.0b1/eth/tools/mining.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/typing.py` & `py-evm-0.9.0b1/eth/typing.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,43 +7,45 @@
     Iterable,
     List,
     NewType,
     Optional,
     Sequence,
     Tuple,
     Type,
+    TypedDict,
     TypeVar,
     Union,
 )
 
 from eth_typing import (
     Address,
     BlockNumber,
     Hash32,
     HexStr,
 )
-from mypy_extensions import (
-    TypedDict,
-)
 
 if TYPE_CHECKING:
     from eth.abc import (  # noqa: F401
         BlockHeaderAPI,
         SignedTransactionAPI,
         VirtualMachineAPI,
         WithdrawalAPI,
     )
 
 
 JournalDBCheckpoint = NewType("JournalDBCheckpoint", int)
 
-AccountDetails = TypedDict(
-    "AccountDetails",
-    {"balance": int, "nonce": int, "code": bytes, "storage": Dict[int, int]},
-)
+
+class AccountDetails(TypedDict):
+    balance: int
+    nonce: int
+    code: bytes
+    storage: Dict[int, int]
+
+
 AccountState = Dict[Address, AccountDetails]
 AccountDiff = Iterable[Tuple[Address, str, Union[int, bytes], Union[int, bytes]]]
 
 
 class Block(TypedDict, total=False):
     header: "BlockHeaderAPI"
     transactions: Sequence["SignedTransactionAPI"]
@@ -66,36 +68,31 @@
 
 GenesisDict = Dict[str, Union[int, BlockNumber, bytes, Hash32]]
 
 BytesOrView = Union[bytes, memoryview]
 
 Normalizer = Callable[[Dict[Any, Any]], Dict[str, Any]]
 
-RawAccountDetails = TypedDict(
-    "RawAccountDetails",
-    {
-        "balance": HexStr,
-        "nonce": HexStr,
-        "code": HexStr,
-        "storage": Dict[HexStr, HexStr],
-    },
-)
 
-TransactionDict = TypedDict(
-    "TransactionDict",
-    {
-        "nonce": int,
-        "gasLimit": int,
-        "gasPrice": int,
-        "to": Address,
-        "value": int,
-        "data": bytes,
-        "secretKey": bytes,
-    },
-)
+class RawAccountDetails(TypedDict):
+    balance: HexStr
+    nonce: HexStr
+    code: HexStr
+    storage: Dict[HexStr, HexStr]
+
+
+class TransactionDict(TypedDict):
+    nonce: int
+    gasLimit: int
+    gasPrice: int
+    to: Address
+    value: int
+    data: bytes
+    secretKey: bytes
+
 
 TransactionNormalizer = Callable[[TransactionDict], TransactionDict]
 
 VMFork = Tuple[BlockNumber, Type["VirtualMachineAPI"]]
 
 VMConfiguration = Sequence[VMFork]
```

### Comparing `py-evm-0.8.0b1/eth/validation.py` & `py-evm-0.9.0b1/eth/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/base.py` & `py-evm-0.9.0b1/eth/vm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,25 +456,21 @@
         # EIP-161:
         # Even if block reward is zero, the coinbase is still touched here. This was
         # not likely to ever happen in PoW, except maybe in some very niche cases, but
         # happens now in PoS. In these cases, the coinbase may end up zeroed after the
         # computation and thus should be marked for deletion since it was touched.
         self.state.delta_balance(block.header.coinbase, block_reward)
         self.logger.debug(
-            "BLOCK REWARD: %s -> %s",
-            block_reward,
-            encode_hex(block.header.coinbase),
+            f"BLOCK REWARD: {block_reward} -> {encode_hex(block.header.coinbase)}"
         )
 
         for uncle in block.uncles:
             uncle_reward = self.get_uncle_reward(block.number, uncle)
             self.logger.debug(
-                "UNCLE REWARD REWARD: %s -> %s",
-                uncle_reward,
-                encode_hex(uncle.coinbase),
+                f"UNCLE REWARD REWARD: {uncle_reward} -> {encode_hex(uncle.coinbase)}"
             )
             self.state.delta_balance(uncle.coinbase, uncle_reward)
 
     def finalize_block(self, block: BlockAPI) -> BlockAndMetaWitness:
         if block.number > 0:
             snapshot = self.state.snapshot()
             try:
@@ -490,20 +486,18 @@
         meta_witness = self.state.persist()
 
         final_block = block.copy(
             header=block.header.copy(state_root=self.state.state_root)
         )
 
         self.logger.debug(
-            "%s reads %d unique node hashes, %d addresses, %d bytecodes, and %d storage slots",  # noqa: E501
-            final_block,
-            len(meta_witness.hashes),
-            len(meta_witness.accounts_queried),
-            len(meta_witness.account_bytecodes_queried),
-            meta_witness.total_slots_queried,
+            f"{final_block} reads {len(meta_witness.hashes)} unique node hashes, "
+            f"{len(meta_witness.accounts_queried)} addresses, "
+            f"{len(meta_witness.account_bytecodes_queried)} bytecodes, and "
+            f"{meta_witness.total_slots_queried} storage slots"
         )
 
         return BlockAndMetaWitness(final_block, meta_witness)
 
     def pack_block(self, block: BlockAPI, *args: Any, **kwargs: Any) -> BlockAPI:
         if "uncles" in kwargs:
             uncles = kwargs.pop("uncles")
@@ -720,17 +714,16 @@
         validate_gas_limit(header.gas_limit, parent_header.gas_limit)
 
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         try:
             self._consensus.validate_seal(header)
         except ValidationError as exc:
             self.cls_logger.debug(
-                "Failed to validate seal on header: %r. Error: %s",
-                header.as_dict(),
-                exc,
+                f"Failed to validate seal on header: {repr(header.as_dict())}. "
+                f"Error: {exc}"
             )
             raise
 
     def validate_seal_extension(
         self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
     ) -> None:
         self._consensus.validate_seal_extension(header, parents)
```

### Comparing `py-evm-0.8.0b1/eth/vm/chain_context.py` & `py-evm-0.9.0b1/eth/vm/chain_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/code_stream.py` & `py-evm-0.9.0b1/eth/vm/code_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,22 +50,24 @@
     def __len__(self) -> int:
         return self._length_cache
 
     def __getitem__(self, i: int) -> int:
         return self._raw_code_bytes[i]
 
     def __iter__(self) -> Iterator[int]:
-        # a very performance-sensitive method
-        pc = self.program_counter
-        while pc < self._length_cache:
-            opcode = self._raw_code_bytes[pc]
-            self.program_counter = pc + 1
+        # a performance-sensitive method
+        while True:
+            try:
+                opcode = self._raw_code_bytes[self.program_counter]
+            except IndexError:
+                break
+
+            self.program_counter += 1
             yield opcode
-            # a read might have adjusted the pc during the last yield
-            pc = self.program_counter
+            # note: a read might have adjusted the pc during the yield
 
         yield STOP
 
     def peek(self) -> int:
         pc = self.program_counter
         if pc < self._length_cache:
             return self._raw_code_bytes[pc]
```

### Comparing `py-evm-0.8.0b1/eth/vm/computation.py` & `py-evm-0.9.0b1/eth/vm/computation.py`

 * *Files 4% similar despite different names*

```diff
@@ -347,19 +347,17 @@
                 except KeyError:
                     opcode_fn = InvalidOpcode(opcode)
 
                 if show_debug2:
                     # We dig into some internals for debug logs
                     base_comp = cast(BaseComputation, computation)
                     computation.logger.debug2(
-                        "OPCODE: 0x%x (%s) | pc: %s | stack: %s",
-                        opcode,
-                        opcode_fn.mnemonic,
-                        max(0, computation.code.program_counter - 1),
-                        base_comp._stack,
+                        f"OPCODE: 0x{opcode:x} ({opcode_fn.mnemonic}) | "
+                        f"pc: {max(0, computation.code.program_counter - 1)} | "
+                        f"stack: {base_comp._stack}"
                     )
 
                 try:
                     opcode_fn(computation=computation)
                 except Halt:
                     break
 
@@ -411,19 +409,16 @@
         after_size = ceil32(start_position + size)
 
         before_cost = memory_gas_cost(before_size)
         after_cost = memory_gas_cost(after_size)
 
         if self.logger.show_debug2:
             self.logger.debug2(
-                "MEMORY: size (%s -> %s) | cost (%s -> %s)",
-                before_size,
-                after_size,
-                before_cost,
-                after_cost,
+                f"MEMORY: size ({before_size} -> {after_size}) | "
+                f"cost ({before_cost} -> {after_cost})"
             )
 
         if size:
             if before_cost < after_cost:
                 gas_fee = after_cost - before_cost
                 self._gas_meter.consume_gas(
                     gas_fee,
@@ -478,15 +473,14 @@
 
     @classmethod
     def consume_initcode_gas_cost(cls, computation: ComputationAPI) -> None:
         # this method does not become relevant until the Shanghai hard fork
         """
         Before starting the computation, consume initcode gas cost.
         """
-        pass
 
     # -- stack management -- #
     def stack_swap(self, position: int) -> None:
         return self._stack.swap(position)
 
     def stack_dup(self, position: int) -> None:
         return self._stack.dup(position)
@@ -562,46 +556,43 @@
 
     # -- context manager API -- #
     def __enter__(self) -> ComputationAPI:
         if self.logger.show_debug2:
             self.logger.debug2(
                 (
                     "MESSAGE COMPUTATION STARTING: "
-                    "from: %s | to: %s | value: %s | depth %s | static: %s | gas: %s"
+                    f"from: {encode_hex(self.msg.sender)} | "
+                    f"to: {encode_hex(self.msg.to)} | "
+                    f"value: {self.msg.value} | "
+                    f"depth: {self.msg.depth} | "
+                    f"static: {'y' if self.msg.is_static else 'n'} | "
+                    f"gas: {self.msg.gas}"
                 ),
-                encode_hex(self.msg.sender),
-                encode_hex(self.msg.to),
-                self.msg.value,
-                self.msg.depth,
-                "y" if self.msg.is_static else "n",
-                self.msg.gas,
             )
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Union[None, bool]:
         if exc_value and isinstance(exc_value, VMError):
             if self.logger.show_debug2:
                 self.logger.debug2(
                     (
                         "COMPUTATION ERROR: "
-                        "gas: %s | from: %s | to: %s | value: %s | "
-                        "depth: %s | static: %s | error: %s"
+                        f"gas: {self.msg.gas} | "
+                        f"from: {encode_hex(self.msg.sender)} | "
+                        f"to: {encode_hex(self.msg.to)} | "
+                        f"value: {self.msg.value} | "
+                        f"depth: {self.msg.depth} | "
+                        f"static: {'y' if self.msg.is_static else 'n'} | "
+                        f"error: {exc_value}"
                     ),
-                    self.msg.gas,
-                    encode_hex(self.msg.sender),
-                    encode_hex(self.msg.to),
-                    self.msg.value,
-                    self.msg.depth,
-                    "y" if self.msg.is_static else "n",
-                    exc_value,
                 )
 
             self._error = exc_value
             if self.should_burn_gas:
                 self.consume_gas(
                     self._gas_meter.gas_remaining,
                     reason=" ".join(
@@ -619,20 +610,18 @@
             # suppress VM exceptions
             return True
 
         elif exc_type is None and self.logger.show_debug2:
             self.logger.debug2(
                 (
                     "COMPUTATION SUCCESS: "
-                    "from: %s | to: %s | value: %s | depth: %s | static: %s "
-                    "| gas-used: %s | gas-remaining: %s"
+                    f"from: {encode_hex(self.msg.sender)} | "
+                    f"to: {encode_hex(self.msg.to)} | "
+                    f"value: {self.msg.value} | "
+                    f"depth: {self.msg.depth} | "
+                    f"static: {'y' if self.msg.is_static else 'n'} | "
+                    f"gas-used: {self.get_gas_used()} | "
+                    f"gas-remaining: {self._gas_meter.gas_remaining}"
                 ),
-                encode_hex(self.msg.sender),
-                encode_hex(self.msg.to),
-                self.msg.value,
-                self.msg.depth,
-                "y" if self.msg.is_static else "n",
-                self.get_gas_used(),
-                self._gas_meter.gas_remaining,
             )
 
         return None
```

### Comparing `py-evm-0.8.0b1/eth/vm/execution_context.py` & `py-evm-0.9.0b1/eth/vm/execution_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/blocks.py` & `py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/headers.py` & `py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/state.py` & `py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/arrow_glacier/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/arrow_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/berlin/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/berlin/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/berlin/blocks.py` & `py-evm-0.9.0b1/eth/vm/forks/berlin/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/berlin/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/berlin/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/berlin/logic.py` & `py-evm-0.9.0b1/eth/vm/forks/berlin/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 def _mark_address_warm(computation: ComputationAPI, address: Address) -> bool:
     """
     Mark the given address as warm if it was not previously.
 
     :return was_cold: True if the account was not previously accessed
         during this transaction
     """
-
     if computation.state.is_address_warm(address):
         return False
     else:
         computation.state.mark_address_warm(address)
         return True
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/berlin/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/berlin/opcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 from eth_utils.toolz import (
     merge,
 )
 
 from eth import (
     constants,
 )
+from eth.abc import (
+    OpcodeAPI,
+)
 from eth.vm import (
     mnemonics,
     opcode_values,
 )
 from eth.vm.forks.byzantium.opcodes import (
     ensure_no_static,
 )
 from eth.vm.forks.muir_glacier.opcodes import (
     MUIR_GLACIER_OPCODES,
 )
 from eth.vm.forks.tangerine_whistle.constants import (
     GAS_SELFDESTRUCT_EIP150,
 )
 from eth.vm.opcode import (
-    Opcode,
     as_opcode,
 )
 
 from . import (
     logic,
 )
 
-UPDATED_OPCODES: Dict[int, Opcode] = {
+UPDATED_OPCODES: Dict[int, OpcodeAPI] = {
     opcode_values.BALANCE: as_opcode(
         gas_cost=constants.GAS_NULL,
         logic_fn=logic.balance_eip2929,
         mnemonic=mnemonics.BALANCE,
     ),
     opcode_values.EXTCODESIZE: as_opcode(
         gas_cost=constants.GAS_NULL,
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/berlin/receipts.py` & `py-evm-0.9.0b1/eth/vm/forks/berlin/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/berlin/state.py` & `py-evm-0.9.0b1/eth/vm/forks/berlin/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/berlin/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/berlin/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/byzantium/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/byzantium/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/byzantium/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/byzantium/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/byzantium/headers.py` & `py-evm-0.9.0b1/eth/vm/forks/byzantium/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     Any,
     Callable,
+    Optional,
 )
 
 from eth_utils.toolz import (
     curry,
 )
 
 from eth._utils.db import (
@@ -89,15 +90,15 @@
         )
     return create_frontier_header_from_parent(parent_header, **header_params)
 
 
 @curry
 def configure_header(
     vm: VirtualMachineAPI,
-    difficulty_fn: Callable[[BlockHeaderAPI, int], int] = None,
+    difficulty_fn: Optional[Callable[[BlockHeaderAPI, int], int]] = None,
     **header_params: Any,
 ) -> BlockHeaderAPI:
     validate_header_params_for_configuration(header_params)
 
     with vm.get_header().build_changeset(**header_params) as changeset:
         if (
             "timestamp" in header_params
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/byzantium/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/byzantium/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/byzantium/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/byzantium/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/constantinople/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/constantinople/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/constantinople/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/constantinople/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/constantinople/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/constantinople/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/constantinople/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/constantinople/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/frontier/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/frontier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/frontier/blocks.py` & `py-evm-0.9.0b1/eth/vm/forks/frontier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/frontier/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/frontier/computation.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,18 +72,16 @@
                     f"Insufficient funds: {sender_balance} < {message.value}"
                 )
 
             state.delta_balance(message.sender, -1 * message.value)
             state.delta_balance(message.storage_address, message.value)
 
             cls.logger.debug2(
-                "TRANSFERRED: %s from %s -> %s",
-                message.value,
-                encode_hex(message.sender),
-                encode_hex(message.storage_address),
+                f"TRANSFERRED: {message.value} from {encode_hex(message.sender)} -> "
+                f"{encode_hex(message.storage_address)}"
             )
 
         state.touch_account(message.storage_address)
 
         computation = cls.apply_computation(
             state,
             message,
@@ -118,14 +116,13 @@
                         contract_code_gas_fee,
                         reason="Write contract code for CREATE",
                     )
                 except OutOfGas:
                     computation.output = b""
                 else:
                     cls.logger.debug2(
-                        "SETTING CODE: %s -> length: %s | hash: %s",
-                        encode_hex(message.storage_address),
-                        len(contract_code),
-                        encode_hex(keccak(contract_code)),
+                        f"SETTING CODE: {encode_hex(message.storage_address)} -> "
+                        f"length: {len(contract_code)} | "
+                        f"hash: {encode_hex(keccak(contract_code))}"
                     )
                     state.set_code(message.storage_address, contract_code)
             return computation
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/frontier/headers.py` & `py-evm-0.9.0b1/eth/vm/forks/frontier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/frontier/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/frontier/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/frontier/state.py` & `py-evm-0.9.0b1/eth/vm/forks/frontier/state.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,27 +86,23 @@
             code = transaction.data
         else:
             contract_address = None
             data = transaction.data
             code = self.vm_state.get_code(transaction.to)
 
         self.vm_state.logger.debug2(
-            (
-                "TRANSACTION: sender: %s | to: %s | value: %s | gas: %s | "
-                "gas-price: %s | s: %s | r: %s | y_parity: %s | data-hash: %s"
-            ),
-            encode_hex(transaction.sender),
-            encode_hex(transaction.to),
-            transaction.value,
-            transaction.gas,
-            transaction.gas_price,
-            transaction.s,
-            transaction.r,
-            transaction.y_parity,
-            encode_hex(keccak(transaction.data)),
+            f"TRANSACTION: sender: {encode_hex(transaction.sender)} | "
+            f"to: {encode_hex(transaction.to)} | "
+            f"value: {transaction.value} | "
+            f"gas: {transaction.gas} | "
+            f"gas-price: {transaction.gas_price} | "
+            f"s: {transaction.s} | "
+            f"r: {transaction.r} | "
+            f"y_parity: {transaction.y_parity} | "
+            f"data-hash: {encode_hex(keccak(transaction.data))}"
         )
 
         message = Message(
             gas=message_gas,
             to=transaction.to,
             sender=transaction.sender,
             value=transaction.value,
@@ -130,16 +126,16 @@
                     message, transaction_context
                 )
                 computation.error = ContractCreationCollision(
                     f"Address collision while creating contract: "
                     f"{encode_hex(message.storage_address)}"
                 )
                 self.vm_state.logger.debug2(
-                    "Address collision while creating contract: %s",
-                    encode_hex(message.storage_address),
+                    "Address collision while creating contract: "
+                    f"{encode_hex(message.storage_address)}"
                 )
             else:
                 computation = self.vm_state.computation_class.apply_create_message(
                     self.vm_state,
                     message,
                     transaction_context,
                 )
@@ -172,39 +168,37 @@
         gas_remaining = computation.get_gas_remaining()
         gas_used = transaction.gas - gas_remaining
         gas_refund = self.calculate_gas_refund(computation, gas_used)
         gas_refund_amount = (gas_refund + gas_remaining) * transaction_context.gas_price
 
         if gas_refund_amount:
             self.vm_state.logger.debug2(
-                "TRANSACTION REFUND: %s -> %s",
-                gas_refund_amount,
-                encode_hex(computation.msg.sender),
+                f"TRANSACTION REFUND: {gas_refund_amount} -> "
+                f"{encode_hex(computation.msg.sender)}"
             )
             self.vm_state.delta_balance(computation.msg.sender, gas_refund_amount)
 
         # Beneficiary Fees
         gas_used = transaction.gas - gas_remaining - gas_refund
         transaction_fee = gas_used * self.vm_state.get_tip(transaction)
 
         # EIP-161:
         # Even if the txn fee is zero, the coinbase is still touched here. Post-merge,
         # with no block reward, in the cases where the txn fee is also zero, the
         # coinbase may end up zeroed after the computation and thus should be marked
         # for deletion since it was touched.
         self.vm_state.logger.debug2(
-            "TRANSACTION FEE: %s -> %s",
-            transaction_fee,
-            encode_hex(self.vm_state.coinbase),
+            f"TRANSACTION FEE: {transaction_fee} -> "
+            f"{encode_hex(self.vm_state.coinbase)}"
         )
         self.vm_state.delta_balance(self.vm_state.coinbase, transaction_fee)
 
         # Process Self Destructs
         for account, _ in computation.get_accounts_for_deletion():
-            self.vm_state.logger.debug2("DELETING ACCOUNT: %s", encode_hex(account))
+            self.vm_state.logger.debug2(f"DELETING ACCOUNT: {encode_hex(account)}")
             self.vm_state.delete_account(account)
 
         return computation
 
 
 class FrontierState(BaseState):
     computation_class: Type[ComputationAPI] = FrontierComputation
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/frontier/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/frontier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/frontier/validation.py` & `py-evm-0.9.0b1/eth/vm/forks/frontier/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/gray_glacier/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/gray_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/gray_glacier/blocks.py` & `py-evm-0.9.0b1/eth/vm/forks/gray_glacier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/gray_glacier/headers.py` & `py-evm-0.9.0b1/eth/vm/forks/gray_glacier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/gray_glacier/state.py` & `py-evm-0.9.0b1/eth/vm/forks/gray_glacier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/gray_glacier/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/gray_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/homestead/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/homestead/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/homestead/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/homestead/computation.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,18 +63,17 @@
                     # Different from Frontier: reverts state on gas failure while
                     # writing contract code.
                     computation.error = err
                     state.revert(snapshot)
                 else:
                     if cls.logger:
                         cls.logger.debug2(
-                            "SETTING CODE: %s -> length: %s | hash: %s",
-                            encode_hex(message.storage_address),
-                            len(contract_code),
-                            encode_hex(keccak(contract_code)),
+                            f"SETTING CODE: {encode_hex(message.storage_address)} -> "
+                            f"length: {len(contract_code)} | "
+                            f"hash: {encode_hex(keccak(contract_code))}"
                         )
 
                     state.set_code(message.storage_address, contract_code)
                     state.commit(snapshot)
             else:
                 state.commit(snapshot)
             return computation
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/homestead/headers.py` & `py-evm-0.9.0b1/eth/vm/forks/homestead/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/homestead/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/homestead/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/homestead/state.py` & `py-evm-0.9.0b1/eth/vm/forks/homestead/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/homestead/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/homestead/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/homestead/validation.py` & `py-evm-0.9.0b1/eth/vm/forks/homestead/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/istanbul/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/istanbul/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/istanbul/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/istanbul/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/istanbul/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/istanbul/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/istanbul/storage.py` & `py-evm-0.9.0b1/eth/vm/forks/istanbul/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/istanbul/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/istanbul/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/london/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/blocks.py` & `py-evm-0.9.0b1/eth/vm/forks/london/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/london/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/headers.py` & `py-evm-0.9.0b1/eth/vm/forks/london/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/london/opcodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 from eth_utils.toolz import (
     merge,
 )
 
 from eth import (
     constants,
 )
+from eth.abc import (
+    OpcodeAPI,
+)
 from eth.vm import (
     mnemonics,
     opcode_values,
 )
 from eth.vm.forks.berlin.opcodes import (
     BERLIN_OPCODES,
 )
 from eth.vm.forks.byzantium.opcodes import (
     ensure_no_static,
 )
 from eth.vm.logic import (
     block,
 )
 from eth.vm.opcode import (
-    Opcode,
     as_opcode,
 )
 
 from . import (
     storage,
 )
 
-UPDATED_OPCODES: Dict[int, Opcode] = {
+UPDATED_OPCODES: Dict[int, OpcodeAPI] = {
     opcode_values.BASEFEE: as_opcode(
         gas_cost=constants.GAS_BASE,
         logic_fn=block.basefee,
         mnemonic=mnemonics.BASEFEE,
     ),
     opcode_values.SSTORE: as_opcode(
         gas_cost=constants.GAS_NULL,
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/receipts.py` & `py-evm-0.9.0b1/eth/vm/forks/london/receipts.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .constants import (
     DYNAMIC_FEE_TRANSACTION_TYPE,
 )
 
 
 class LondonTypedReceipt(BerlinTypedReceipt):
     codecs: Dict[int, Type[Receipt]] = {
-        ACCESS_LIST_TRANSACTION_TYPE: Receipt,
-        DYNAMIC_FEE_TRANSACTION_TYPE: Receipt,
+        # mypy errors due to Receipt inheriting but not defining abstractmethods
+        ACCESS_LIST_TRANSACTION_TYPE: Receipt,  # type: ignore
+        DYNAMIC_FEE_TRANSACTION_TYPE: Receipt,  # type: ignore
     }
 
 
 class LondonReceiptBuilder(BerlinReceiptBuilder):
     typed_receipt_class = LondonTypedReceipt
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/state.py` & `py-evm-0.9.0b1/eth/vm/forks/london/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,19 +71,18 @@
             code = transaction.data
         else:
             contract_address = None
             data = transaction.data
             code = self.vm_state.get_code(transaction.to)
 
         self.vm_state.logger.debug2(
-            ("TRANSACTION: %r; sender: %s | to: %s | data-hash: %s"),
-            transaction,
-            encode_hex(transaction.sender),
-            encode_hex(transaction.to),
-            encode_hex(keccak(transaction.data)),
+            f"TRANSACTION: {repr(transaction)}; "
+            f"sender: {encode_hex(transaction.sender)} | "
+            f"to: {encode_hex(transaction.to)} | "
+            f"data-hash: {encode_hex(keccak(transaction.data))}"
         )
 
         message = Message(
             gas=message_gas,
             to=transaction.to,
             sender=transaction.sender,
             value=transaction.value,
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/storage.py` & `py-evm-0.9.0b1/eth/vm/forks/london/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/london/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/london/validation.py` & `py-evm-0.9.0b1/eth/vm/forks/london/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/muir_glacier/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/muir_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/muir_glacier/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/muir_glacier/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/muir_glacier/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/muir_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/paris/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/paris/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/paris/blocks.py` & `py-evm-0.9.0b1/eth/vm/forks/paris/blocks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from abc import (
     ABC,
 )
 from typing import (
     Type,
 )
 
+from eth_typing import (
+    Hash32,
+)
 from eth_utils import (
     encode_hex,
 )
 from rlp.sedes import (
     CountableList,
 )
 
 from eth.abc import (
     TransactionBuilderAPI,
 )
 from eth.vm.forks.gray_glacier.blocks import (
     GrayGlacierBlock,
     GrayGlacierBlockHeader,
-    GrayGlacierMiningHeader,
 )
 
 from ..london.blocks import (
     LondonBackwardsHeader,
 )
 from .transactions import (
     ParisTransactionBuilder,
 )
 
 
-class ParisMiningHeader(GrayGlacierMiningHeader, ABC):
-    pass
-
-
 class ParisBlockHeader(GrayGlacierBlockHeader, ABC):
     def __str__(self) -> str:
         return f"<ParisBlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>"
 
+    @property
+    def mining_hash(self) -> Hash32:
+        raise ValueError("Mining hash is not available post merge.")
+
 
 class ParisBlock(GrayGlacierBlock):
     transaction_builder: Type[TransactionBuilderAPI] = ParisTransactionBuilder
     fields = [
         ("header", ParisBlockHeader),
         ("transactions", CountableList(transaction_builder)),
         # no uncles in pos, max_length=0
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/paris/headers.py` & `py-evm-0.9.0b1/eth/vm/forks/paris/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/paris/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/paris/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/paris/state.py` & `py-evm-0.9.0b1/eth/vm/forks/paris/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/paris/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/paris/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/petersburg/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/petersburg/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/petersburg/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/petersburg/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/petersburg/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/petersburg/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/petersburg/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/petersburg/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/__init__.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/blocks.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 from eth._utils.headers import (
     new_timestamp_from_parent,
 )
 from eth.abc import (
     BlockHeaderAPI,
     BlockHeaderSedesAPI,
     ChainDatabaseAPI,
-    MiningHeaderAPI,
     ReceiptAPI,
     ReceiptBuilderAPI,
     SignedTransactionAPI,
     TransactionBuilderAPI,
     WithdrawalAPI,
 )
 from eth.constants import (
@@ -80,48 +79,35 @@
 from .transactions import (
     ShanghaiTransactionBuilder,
 )
 from .withdrawals import (
     Withdrawal,
 )
 
-UNMINED_SHANGHAI_HEADER_FIELDS = [
-    ("parent_hash", hash32),
-    ("uncles_hash", hash32),
-    ("coinbase", address),
-    ("state_root", trie_root),
-    ("transaction_root", trie_root),
-    ("receipt_root", trie_root),
-    ("bloom", uint256),
-    ("difficulty", big_endian_int),
-    ("block_number", big_endian_int),
-    ("gas_limit", big_endian_int),
-    ("gas_used", big_endian_int),
-    ("timestamp", big_endian_int),
-    ("extra_data", binary),
-    ("base_fee_per_gas", big_endian_int),
-    ("withdrawals_root", trie_root),
-]
-
-
-class ShanghaiMiningHeader(rlp.Serializable, MiningHeaderAPI, ABC):
-    fields = UNMINED_SHANGHAI_HEADER_FIELDS
-
 
 class ShanghaiBlockHeader(rlp.Serializable, BlockHeaderAPI, ABC):
-    # `mix_hash` and `nonce` were fields before `base_fee_per_gas` and
-    # `withdrawals_root` and, thus, appear in the block header before them.
-    fields = (
-        UNMINED_SHANGHAI_HEADER_FIELDS[:13]
-        + [
-            ("mix_hash", binary),
-            ("nonce", Binary(8, allow_empty=True)),
-        ]
-        + UNMINED_SHANGHAI_HEADER_FIELDS[13:]
-    )
+    fields = [
+        ("parent_hash", hash32),
+        ("uncles_hash", hash32),
+        ("coinbase", address),
+        ("state_root", trie_root),
+        ("transaction_root", trie_root),
+        ("receipt_root", trie_root),
+        ("bloom", uint256),
+        ("difficulty", big_endian_int),
+        ("block_number", big_endian_int),
+        ("gas_limit", big_endian_int),
+        ("gas_used", big_endian_int),
+        ("timestamp", big_endian_int),
+        ("extra_data", binary),
+        ("mix_hash", binary),
+        ("nonce", Binary(8, allow_empty=True)),
+        ("base_fee_per_gas", big_endian_int),
+        ("withdrawals_root", trie_root),
+    ]
 
     def __init__(
         self,
         difficulty: int,
         block_number: BlockNumber,
         gas_limit: int,
         timestamp: int = None,
@@ -181,17 +167,15 @@
     def hash(self) -> Hash32:
         if self._hash is None:
             self._hash = keccak(rlp.encode(self))
         return cast(Hash32, self._hash)
 
     @property
     def mining_hash(self) -> Hash32:
-        non_pow_fields = self[:-3] + self[-1:]
-        result = keccak(rlp.encode(non_pow_fields, ShanghaiMiningHeader))
-        return cast(Hash32, result)
+        raise ValueError("Mining hash is not available post merge.")
 
     @property
     def hex_hash(self) -> str:
         return encode_hex(self.hash)
 
     @property
     def is_genesis(self) -> bool:
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/headers.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/logic.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/logic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/state.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/shanghai/withdrawals.py` & `py-evm-0.9.0b1/eth/vm/forks/shanghai/withdrawals.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/_utils.py` & `py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/computation.py` & `py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/computation.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,33 +78,31 @@
                     # writing contract code.
                     computation.error = err
                     state.revert(snapshot)
                     cls.logger.debug2(f"VMError setting contract code: {err}")
                 else:
                     if cls.logger:
                         cls.logger.debug2(
-                            "SETTING CODE: %s -> length: %s | hash: %s",
-                            encode_hex(message.storage_address),
-                            len(contract_code),
-                            encode_hex(keccak(contract_code)),
+                            f"SETTING CODE: {encode_hex(message.storage_address)} -> "
+                            f"length: {len(contract_code)} | "
+                            f"hash: {encode_hex(keccak(contract_code))}"
                         )
 
                     state.set_code(message.storage_address, contract_code)
                     state.commit(snapshot)
             else:
                 state.commit(snapshot)
             return computation
 
     @classmethod
     def validate_create_message(cls, message: MessageAPI) -> None:
         # this method does not become relevant until the Shanghai hard fork
         """
         Class method for validating a create message.
         """
-        pass
 
     @classmethod
     def validate_contract_code(cls, contract_code: bytes) -> None:
         if len(contract_code) > EIP170_CODE_SIZE_LIMIT:
             raise OutOfGas(
                 f"Contract code size exceeds EIP170 limit of {EIP170_CODE_SIZE_LIMIT}."
                 f"  Got code of size: {len(contract_code)}"
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/state.py` & `py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/state.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
         for account in touched_accounts:
             should_delete = self.vm_state.account_exists(
                 account
             ) and self.vm_state.account_is_empty(account)
             if should_delete:
                 self.vm_state.logger.debug2(
-                    "CLEARING EMPTY ACCOUNT: %s",
-                    encode_hex(account),
+                    f"CLEARING EMPTY ACCOUNT: {encode_hex(account)}"
                 )
                 self.vm_state.delete_account(account)
 
         return computation
 
 
 class SpuriousDragonState(HomesteadState):
```

### Comparing `py-evm-0.8.0b1/eth/vm/forks/spurious_dragon/transactions.py` & `py-evm-0.9.0b1/eth/vm/forks/spurious_dragon/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/forks/tangerine_whistle/opcodes.py` & `py-evm-0.9.0b1/eth/vm/forks/tangerine_whistle/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/gas_meter.py` & `py-evm-0.9.0b1/eth/vm/gas_meter.py`

 * *Files 21% similar despite different names*

```diff
@@ -65,38 +65,31 @@
                 f"- Reason: {reason}"
             )
 
         self.gas_remaining -= amount
 
         if self.logger.show_debug2:
             self.logger.debug2(
-                "GAS CONSUMPTION: %s - %s -> %s (%s)",
-                self.gas_remaining + amount,
-                amount,
-                self.gas_remaining,
-                reason,
+                f"GAS CONSUMPTION: {self.gas_remaining + amount} - {amount} -> "
+                f"{self.gas_remaining} ({reason})"
             )
 
     def return_gas(self, amount: int) -> None:
         if amount < 0:
             raise ValidationError("Gas return amount must be positive")
 
         self.gas_remaining += amount
 
         if self.logger.show_debug2:
             self.logger.debug2(
-                "GAS RETURNED: %s + %s -> %s",
-                self.gas_remaining - amount,
-                amount,
-                self.gas_remaining,
+                f"GAS RETURNED: {self.gas_remaining - amount} + {amount} -> "
+                f"{self.gas_remaining}"
             )
 
     def refund_gas(self, amount: int) -> None:
         self.gas_refunded = self.refund_strategy(self.gas_refunded, amount)
 
         if self.logger.show_debug2:
             self.logger.debug2(
-                "GAS REFUND: %s + %s -> %s",
-                self.gas_refunded - amount,
-                amount,
-                self.gas_refunded,
+                f"GAS REFUND: {self.gas_refunded - amount} + {amount} -> "
+                f"{self.gas_refunded}"
             )
```

### Comparing `py-evm-0.8.0b1/eth/vm/header.py` & `py-evm-0.9.0b1/eth/vm/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/interrupt.py` & `py-evm-0.9.0b1/eth/vm/interrupt.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/arithmetic.py` & `py-evm-0.9.0b1/eth/vm/logic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/block.py` & `py-evm-0.9.0b1/eth/vm/logic/block.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/call.py` & `py-evm-0.9.0b1/eth/vm/logic/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,16 @@
         if load_account_fee > 0:
             computation.consume_gas(
                 load_account_fee,
                 reason=f"{self.mnemonic} charges implicit account load for reading code",  # noqa: E501
             )
             if self.logger.show_debug2:
                 self.logger.debug2(
-                    "%s is charged %d for invoking code at account 0x%s",
-                    self.mnemonic,
-                    load_account_fee,
-                    code_source.hex(),
+                    f"{self.mnemonic} is charged {load_account_fee} for invoking "
+                    f"code at account 0x{code_source.hex()}"
                 )
 
         # This must be computed *after* the load account fee is charged, so
         # that the 63/64ths rule is applied against the reduced remaining gas.
         child_msg_gas, child_msg_gas_fee = self.compute_msg_gas(
             computation, gas, to, value
         )
@@ -128,19 +126,15 @@
                     f"Insufficient Funds: have: {sender_balance} | need: {value}"
                 )
             elif stack_too_deep:
                 err_message = "Stack Limit Reached"
             else:
                 raise Exception("Invariant: Unreachable code path")
 
-            self.logger.debug2(
-                "%s failure: %s",
-                self.mnemonic,
-                err_message,
-            )
+            self.logger.debug2(f"{self.mnemonic} failure: {err_message}")
             computation.return_gas(child_msg_gas)
             computation.stack_push_int(0)
         else:
             if code_address:
                 code = computation.state.get_code(code_address)
             else:
                 code = computation.state.get_code(to)
```

### Comparing `py-evm-0.8.0b1/eth/vm/logic/comparison.py` & `py-evm-0.9.0b1/eth/vm/logic/comparison.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/context.py` & `py-evm-0.9.0b1/eth/vm/logic/context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/flow.py` & `py-evm-0.9.0b1/eth/vm/logic/flow.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/logging.py` & `py-evm-0.9.0b1/eth/vm/logic/logging.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/memory.py` & `py-evm-0.9.0b1/eth/vm/logic/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/sha3.py` & `py-evm-0.9.0b1/eth/vm/logic/sha3.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/storage.py` & `py-evm-0.9.0b1/eth/vm/logic/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/logic/system.py` & `py-evm-0.9.0b1/eth/vm/logic/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from typing import (
+    Optional,
+)
+
 from eth_typing import (
     Address,
 )
 from eth_utils import (
     encode_hex,
 )
 
@@ -98,28 +102,30 @@
     computation.state.set_balance(beneficiary, local_balance + beneficiary_balance)
     # 2nd: Zero the balance of the address being deleted (must come after
     # sending to beneficiary in case the contract named itself as the
     # beneficiary.
     computation.state.set_balance(computation.msg.storage_address, 0)
 
     computation.logger.debug2(
-        "SELFDESTRUCT: %s (%s) -> %s",
-        encode_hex(computation.msg.storage_address),
-        local_balance,
-        encode_hex(beneficiary),
+        f"SELFDESTRUCT: {encode_hex(computation.msg.storage_address)} "
+        f"({local_balance}) -> {encode_hex(beneficiary)}"
     )
 
     # 3rd: Register the account to be deleted
     computation.register_account_for_deletion(beneficiary)
     raise Halt("SELFDESTRUCT")
 
 
 class CreateOpcodeStackData:
     def __init__(
-        self, endowment: int, memory_start: int, memory_length: int, salt: int = None
+        self,
+        endowment: int,
+        memory_start: int,
+        memory_length: int,
+        salt: Optional[int] = None,
     ) -> None:
         self.endowment = endowment
         self.memory_start = memory_start
         self.memory_length = memory_length
         self.salt = salt
 
 
@@ -198,16 +204,16 @@
 
         is_collision = computation.state.has_code_or_nonce(contract_address)
 
         if is_collision:
             computation.stack_push_int(0)
             computation.return_data = b""
             self.logger.debug2(
-                "Address collision while creating contract: %s",
-                encode_hex(contract_address),
+                f"Address collision while creating contract: "
+                f"{encode_hex(contract_address)}"
             )
             return
 
         child_msg = computation.prepare_child_message(
             gas=create_msg_gas,
             to=constants.CREATE_CONTRACT_ADDRESS,
             value=stack_data.endowment,
```

### Comparing `py-evm-0.8.0b1/eth/vm/memory.py` & `py-evm-0.9.0b1/eth/vm/memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import itertools
 import logging
 
 from eth._utils.numeric import (
     ceil32,
 )
 from eth.abc import (
     MemoryAPI,
@@ -28,15 +27,15 @@
 
         new_size = ceil32(start_position + size)
         if new_size <= len(self):
             return
 
         size_to_extend = new_size - len(self)
         try:
-            self._bytes.extend(itertools.repeat(0, size_to_extend))
+            self._bytes.extend(bytearray(size_to_extend))
         except BufferError:
             # we can't extend the buffer (which might involve relocating it) if a
             # memoryview (which stores a pointer into the buffer) has been created by
             # read() and not released. Callers of read() will never try to write to the
             # buffer so we're not missing anything by making a new buffer and forgetting
             # about the old one. We're keeping too much memory around but this is still
             # a net savings over having read() return a new bytes() object every time.
@@ -49,15 +48,14 @@
         if size:
             validate_uint256(start_position)
             validate_uint256(size)
             validate_is_bytes(value)
             validate_length(value, length=size)
             validate_lte(start_position + size, maximum=len(self))
 
-            for idx, v in enumerate(value):
-                self._bytes[start_position + idx] = v
+            self._bytes[start_position : start_position + len(value)] = value
 
     def read(self, start_position: int, size: int) -> memoryview:
         return memoryview(self._bytes)[start_position : start_position + size]
 
     def read_bytes(self, start_position: int, size: int) -> bytes:
         return bytes(self._bytes[start_position : start_position + size])
```

### Comparing `py-evm-0.8.0b1/eth/vm/message.py` & `py-evm-0.9.0b1/eth/vm/message.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/mnemonics.py` & `py-evm-0.9.0b1/eth/vm/mnemonics.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/opcode_values.py` & `py-evm-0.9.0b1/eth/vm/opcode_values.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/state.py` & `py-evm-0.9.0b1/eth/vm/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.8.0b1/eth/vm/transaction_context.py` & `py-evm-0.9.0b1/eth/vm/transaction_context.py`

 * *Files identical despite different names*

