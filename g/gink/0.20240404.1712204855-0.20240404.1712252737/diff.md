# Comparing `tmp/gink-0.20240404.1712204855.tar.gz` & `tmp/gink-0.20240404.1712252737.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240404.1712204855.tar", last modified: Thu Apr  4 04:27:38 2024, max compression
+gzip compressed data, was "gink-0.20240404.1712252737.tar", last modified: Thu Apr  4 17:45:41 2024, max compression
```

## Comparing `gink-0.20240404.1712204855.tar` & `gink-0.20240404.1712252737.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.538324 gink-0.20240404.1712204855/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.538324 gink-0.20240404.1712204855/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.546325 gink-0.20240404.1712204855/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    20537 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17862 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    53281 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10202 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:41.256835 gink-0.20240404.1712252737/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-04 17:45:41.256835 gink-0.20240404.1712252737/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:41.236835 gink-0.20240404.1712252737/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:41.240835 gink-0.20240404.1712252737/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:41.248835 gink-0.20240404.1712252737/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17862 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/impl/websocket_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:41.252835 gink-0.20240404.1712252737/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10202 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-04 17:45:35.000000 gink-0.20240404.1712252737/gink/tests/test_websocket_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:45:41.252835 gink-0.20240404.1712252737/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-04 17:45:41.000000 gink-0.20240404.1712252737/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-04 17:45:41.000000 gink-0.20240404.1712252737/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:45:41.000000 gink-0.20240404.1712252737/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 17:45:41.000000 gink-0.20240404.1712252737/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 17:45:41.000000 gink-0.20240404.1712252737/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:45:41.256835 gink-0.20240404.1712252737/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-04 17:45:37.000000 gink-0.20240404.1712252737/setup.py
```

### Comparing `gink-0.20240404.1712204855/LICENSE` & `gink-0.20240404.1712252737/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/PKG-INFO` & `gink-0.20240404.1712252737/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240404.1712204855
+Version: 0.20240404.1712252737
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240404.1712204855/README.md` & `gink-0.20240404.1712252737/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/__init__.py` & `gink-0.20240404.1712252737/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/__main__.py` & `gink-0.20240404.1712252737/gink/__main__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/behavior_pb2.py` & `gink-0.20240404.1712252737/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/bundle_pb2.py` & `gink-0.20240404.1712252737/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/change_pb2.py` & `gink-0.20240404.1712252737/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/claim_pb2.py` & `gink-0.20240404.1712252737/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/clearance_pb2.py` & `gink-0.20240404.1712252737/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/container_pb2.py` & `gink-0.20240404.1712252737/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/entry_pb2.py` & `gink-0.20240404.1712252737/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/key_pb2.py` & `gink-0.20240404.1712252737/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/log_file_pb2.py` & `gink-0.20240404.1712252737/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/movement_pb2.py` & `gink-0.20240404.1712252737/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/muid_pb2.py` & `gink-0.20240404.1712252737/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/pair_pb2.py` & `gink-0.20240404.1712252737/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/sync_message_pb2.py` & `gink-0.20240404.1712252737/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/builders/value_pb2.py` & `gink-0.20240404.1712252737/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/abstract_store.py` & `gink-0.20240404.1712252737/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/addressable.py` & `gink-0.20240404.1712252737/gink/impl/addressable.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from typing import Dict
 
 class Addressable:
     def __init__(self, database: Database, muid: Muid):
         self._database: Database = database
         self._muid: Muid = muid
 
+    def get_muid(self):
+        return self._muid
+
     def __eq__(self, other):
         return isinstance(other, self.__class__) and other._muid == self._muid
 
     def __hash__(self):
         return hash(self._muid)
 
     def get_properties_values_by_name_as_dict(self, as_of: GenericTimestamp = None):
```

### Comparing `gink-0.20240404.1712204855/gink/impl/attribution.py` & `gink-0.20240404.1712252737/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/box.py` & `gink-0.20240404.1712252737/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/builders.py` & `gink-0.20240404.1712252737/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/bundle_info.py` & `gink-0.20240404.1712252737/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/bundle_wrapper.py` & `gink-0.20240404.1712252737/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/bundler.py` & `gink-0.20240404.1712252737/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/chain_tracker.py` & `gink-0.20240404.1712252737/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/coding.py` & `gink-0.20240404.1712252737/gink/impl/coding.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,35 @@
 FLOAT_INF = float("inf")
 INT_INF = 0xffffffffffffffff
 ZERO_64: bytes = b"\x00" * 8
 KEY_MAX: int = 2**53 - 1
 deletion = Deletion()
 inclusion = Inclusion()
 
+def normalize_entry_builder(entry_builder: EntryBuilder, entry_muid: Muid):
+    """ Make all relative muid references absolute muid refereces within an entry.
+    """
+    container_muid = Muid.create(context=entry_muid, builder=entry_builder.container)
+    container_muid.put_into(entry_builder.container)
+
+    if entry_builder.HasField("describing"):
+        describes_muid = Muid.create(context=entry_muid, builder=entry_builder.describing)
+        describes_muid.put_into(entry_builder.describing)
+
+    if entry_builder.HasField("pointee"):
+        pointee_muid = Muid.create(context=entry_muid, builder=entry_builder.pointee)
+        pointee_muid.put_into(entry_builder.pointee)
+
+    if entry_builder.HasField("pair"):
+        left_muid = Muid.create(context=entry_muid, builder=entry_builder.pair.left)
+        left_muid.put_into(entry_builder.pair.left)
+        rite_muid = Muid.create(context=entry_muid, builder=entry_builder.pair.rite)
+        rite_muid.put_into(entry_builder.pair.rite)
+
+
 
 def ensure_entry_is_valid(builder: EntryBuilder, context: Any = object(), offset: Optional[int]=None):
     if getattr(builder, "behavior") == UNSPECIFIED:
         raise ValueError("entry lacks a behavior")
     if not builder.HasField("container"):
         raise ValueError("no container specified in entry")
     entry_muid = Muid.create(context, offset=offset)
@@ -137,18 +158,18 @@
         if behavior in [DIRECTORY, KEY_SET]:
             middle_key = decode_key(builder)
         elif behavior in (BOX, VERTEX):
             middle_key = None
         elif behavior in (SEQUENCE, VERB):
             middle_key = QueueMiddleKey(position or entry_muid.timestamp)
         elif behavior in (PROPERTY, ROLE):
-            middle_key = Muid.create(context=new_info, builder=builder.describing)  # type: ignore
+            middle_key = Muid.create(context=entry_muid, builder=builder.describing)  # type: ignore
         elif behavior in (PAIR_SET, PAIR_MAP):
-            left = Muid.create(context=new_info, builder=builder.pair.left)
-            rite = Muid.create(context=new_info, builder=builder.pair.rite)
+            left = Muid.create(context=entry_muid, builder=builder.pair.left)
+            rite = Muid.create(context=entry_muid, builder=builder.pair.rite)
             middle_key = (left, rite)
         else:
             raise AssertionError(f"unexpected behavior: {behavior}")
         expiry = getattr(builder, "expiry") or None
         return Placement(container, middle_key, entry_muid, expiry)
 
     @staticmethod
```

### Comparing `gink-0.20240404.1712204855/gink/impl/connection.py` & `gink-0.20240404.1712252737/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/container.py` & `gink-0.20240404.1712252737/gink/impl/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,14 @@
         if builder.HasField("pointee"):  # type: ignore
             pointee = getattr(builder, "pointee")
             assert address is not None
             pointee_muid = Muid.create(builder=pointee, context=address)
             return self._database.get_container(pointee_muid)
         raise Exception("unexpected")
 
-    def get_muid(self) -> Muid:
-        """ returns the global address of this container """
-        return self._muid
-
     @classmethod
     def get_behavior(cls):
         """ Gets the behavior tag/enum for the particular class. """
         assert hasattr(cls, "BEHAVIOR")
         return getattr(cls, "BEHAVIOR")
 
     @classmethod
```

### Comparing `gink-0.20240404.1712204855/gink/impl/database.py` & `gink-0.20240404.1712252737/gink/impl/database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/deferred.py` & `gink-0.20240404.1712252737/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/directory.py` & `gink-0.20240404.1712252737/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/graph.py` & `gink-0.20240404.1712252737/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/key_set.py` & `gink-0.20240404.1712252737/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/listener.py` & `gink-0.20240404.1712252737/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/lmdb_store.py` & `gink-0.20240404.1712252737/gink/impl/lmdb_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 from .abstract_store import AbstractStore, BundleWrapper, BundleCallback
 from .chain_tracker import ChainTracker
 from .lmdb_utilities import to_last_with_prefix
 from .utilities import generate_timestamp, create_claim
 from .coding import (encode_key, create_deleting_entry, PlacementBuilderPair, decode_muts, wrap_change,
                      Placement, encode_muts, QueueMiddleKey, DIRECTORY, SEQUENCE, serialize,
                      ensure_entry_is_valid, deletion, Deletion, decode_entry_occupant, RemovalKey,
-                     LocationKey, PROPERTY, BOX, ROLE, decode_value, VERB, PAIR_MAP, PAIR_SET, KEY_SET)
+                     LocationKey, PROPERTY, BOX, ROLE, decode_value, VERB, PAIR_MAP, PAIR_SET, KEY_SET,
+                     normalize_entry_builder, VERTEX)
 
 
 class LmdbStore(AbstractStore):
     """
     """
 
     def __init__(
@@ -275,15 +276,15 @@
             self,
             to_time: MuTimestamp,
             container: Muid,
             seen: Optional[Set],
             trxn: Trxn) -> Iterable[ChangeBuilder]:
         """ Figures out which specific reset method to call to reset a container. """
         behavior = self._get_behavior(container, trxn)
-        if behavior in (DIRECTORY, BOX, ROLE, PROPERTY, KEY_SET):
+        if behavior in (DIRECTORY, BOX, ROLE, KEY_SET, VERTEX, PROPERTY):
             for change in self._get_keyed_reset(container, to_time, trxn, seen, None, behavior):
                 yield change
             return
         if behavior in (SEQUENCE, VERB):
             for change in self._get_sequence_reset(container, to_time, trxn, seen):
                 yield change
             return
@@ -372,24 +373,57 @@
                     change_builder.movement.dest = previous.get_queue_position()  # type: ignore
                 yield change_builder
             if previous == parsed_key and clear_before_to < placed_time:
                 # this entry existed there at to_time
                 entry_builder = EntryBuilder()
                 entry_muid_bytes = placements_cursor.value()
                 entry_builder.ParseFromString(trxn.get(entry_muid_bytes, db=self._entries))
-                occupant = decode_entry_occupant(Muid.from_bytes(entry_muid_bytes), entry_builder)
+                entry_muid = Muid.from_bytes(entry_muid_bytes)
+                occupant = decode_entry_occupant(entry_muid, entry_builder)
                 if isinstance(occupant, Muid) and seen is not None:
                     for change in self._container_reset_changes(to_time, occupant, seen, trxn):
                         yield change
                 if location != previous or last_clear_time > placed_time:
                     # but isn't there any longer
+                    normalize_entry_builder(entry_builder=entry_builder, entry_muid=entry_muid)
                     entry_builder.effective = parsed_key.get_queue_position()  # type: ignore
                     yield wrap_change(entry_builder)
+                    if entry_builder.behavior == VERB:
+                        for change in self._reissue_properties(
+                            trxn=trxn,
+                            describing_muid_bytes=entry_muid_bytes,
+                            to_time=to_time):
+                                yield change
             positioned = placements_cursor.next()
 
+    def _reissue_properties(
+            self,
+            trxn: Trxn,
+            describing_muid_bytes: bytes,
+            to_time: MuTimestamp,
+    ) -> Iterable[ChangeBuilder]:
+        describing_cursor = trxn.cursor(self._by_describing)
+        found = to_last_with_prefix(
+            describing_cursor, describing_muid_bytes, suffix=bytes(Muid(to_time,0,0)))
+        issued = set()
+        offset = 0
+        while found and describing_cursor.key().startswith(describing_muid_bytes):
+            describor_entry_bytes = describing_cursor.key()[16:]
+            describor_property = describing_cursor.value()
+            if describor_property not in issued:
+                issued.add(describor_property)
+                entry_builder = EntryBuilder()
+                entry_builder.ParseFromString(trxn.get(describor_entry_bytes, db=self._entries))
+                normalize_entry_builder(
+                    entry_builder=entry_builder, entry_muid=Muid.from_bytes(describor_entry_bytes))
+                offset -= 1
+                Muid(0, 0, offset).put_into(entry_builder.describing)
+                yield wrap_change(entry_builder)
+            found = describing_cursor.prev()
+
     def _get_keyed_reset(
             self,
             container: Muid,
             to_time: MuTimestamp,
             trxn: Trxn,
             seen: Optional[Set],
             single_user_key: Optional[UserKey],
@@ -831,50 +865,50 @@
             new_info: BundleInfo,
             txn: Trxn,
             offset: int,
             builder: EntryBuilder):
         retaining = bool(decode_muts(bytes(txn.get(b"entries", db=self._retentions))))
         ensure_entry_is_valid(builder=builder, context=new_info, offset=offset)
         placement_key = Placement.from_builder(builder, new_info, offset)
-        placer_muid = placement_key.placer
+        entry_muid = placement_key.placer
         container_muid = placement_key.container
         serialized_placement_key = bytes(placement_key)
         if builder.behavior in (Behavior.DIRECTORY, Behavior.BOX, Behavior.PROPERTY, Behavior.ROLE):
             found_entry = self.get_entry_by_key(container_muid, placement_key.middle)
             if found_entry:
                 if retaining:
-                    removal_key = bytes(container_muid) + bytes(found_entry.address) + bytes(placer_muid)
+                    removal_key = bytes(container_muid) + bytes(found_entry.address) + bytes(entry_muid)
                     txn.put(removal_key, b"", db=self._removals)
                 else:
                     self._remove_entry(found_entry.address, txn)
-        entry_muid = placer_muid
         entry_bytes = bytes(entry_muid)
         txn.put(entry_bytes, serialize(builder), db=self._entries)
         txn.put(serialized_placement_key, entry_bytes, db=self._placements)
-        entries_loc_key = bytes(LocationKey(entry_muid, placer_muid))
-        txn.put(entries_loc_key, serialized_placement_key, db=self._locations)
+        entries_loc_key = bytes(LocationKey(entry_muid, entry_muid))
+        if builder.behavior in (VERB, SEQUENCE):
+            txn.put(entries_loc_key, serialized_placement_key, db=self._locations)
         if builder.HasField("describing"):
-            describing_muid = Muid.create(new_info, builder.describing)
-            descriptor_key = bytes(describing_muid) + bytes(placer_muid)
+            describing_muid = Muid.create(entry_muid, builder.describing)
+            descriptor_key = bytes(describing_muid) + bytes(entry_muid)
             txn.put(descriptor_key, bytes(container_muid), db=self._by_describing)
         if builder.HasField("pointee"):
-            pointee_muid = Muid.create(new_info, builder.pointee)
-            pointee_key = bytes(pointee_muid) + bytes(placer_muid)
+            pointee_muid = Muid.create(entry_muid, builder.pointee)
+            pointee_key = bytes(pointee_muid) + bytes(entry_muid)
             txn.put(pointee_key, bytes(container_muid), db=self._by_pointee)
         if builder.HasField("pair"):
-            left = Muid.create(context=placer_muid, builder=builder.pair.left)
-            rite = Muid.create(context=placer_muid, builder=builder.pair.rite)
-            txn.put(bytes(left) + bytes(placer_muid), entry_bytes, db=self._by_side)
-            txn.put(bytes(rite) + bytes(placer_muid), entry_bytes, db=self._by_side)
+            left = Muid.create(context=entry_muid, builder=builder.pair.left)
+            rite = Muid.create(context=entry_muid, builder=builder.pair.rite)
+            txn.put(bytes(left) + bytes(entry_muid), entry_bytes, db=self._by_side)
+            txn.put(bytes(rite) + bytes(entry_muid), entry_bytes, db=self._by_side)
         if container_muid == Muid(-1, -1, Behavior.PROPERTY):
             if builder.HasField("value") and builder.HasField("describing"):
                 describing_muid = Muid.create(new_info, builder.describing)
                 name = decode_value(builder.value)
                 if isinstance(name, str):
-                    by_name_key = name.encode() + b"\x00" + bytes(placer_muid)
+                    by_name_key = name.encode() + b"\x00" + bytes(entry_muid)
                     txn.put(by_name_key, bytes(describing_muid), db=self._by_name)
 
     def _remove_entry(self, entry_muid: Muid, trxn: Trxn):
         entry_muid_bytes = bytes(entry_muid)
         entry_payload = trxn.pop(entry_muid_bytes, db=self._entries)
         if entry_payload is None:
             self._logger.warning(f"entry already gone? {entry_muid}")
```

### Comparing `gink-0.20240404.1712204855/gink/impl/lmdb_utilities.py` & `gink-0.20240404.1712252737/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/log_backed_store.py` & `gink-0.20240404.1712252737/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/memory_store.py` & `gink-0.20240404.1712252737/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/muid.py` & `gink-0.20240404.1712252737/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/pair_map.py` & `gink-0.20240404.1712252737/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/pair_set.py` & `gink-0.20240404.1712252737/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/property.py` & `gink-0.20240404.1712252737/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/role.py` & `gink-0.20240404.1712252737/gink/impl/role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/selectable_console.py` & `gink-0.20240404.1712252737/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/sequence.py` & `gink-0.20240404.1712252737/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/tuples.py` & `gink-0.20240404.1712252737/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/typedefs.py` & `gink-0.20240404.1712252737/gink/impl/typedefs.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/utilities.py` & `gink-0.20240404.1712252737/gink/impl/utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/watcher.py` & `gink-0.20240404.1712252737/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/impl/websocket_connection.py` & `gink-0.20240404.1712252737/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_box.py` & `gink-0.20240404.1712252737/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_chain_tracker.py` & `gink-0.20240404.1712252737/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_change_set_info.py` & `gink-0.20240404.1712252737/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_code_values.py` & `gink-0.20240404.1712252737/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_container.py` & `gink-0.20240404.1712252737/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_database.py` & `gink-0.20240404.1712252737/gink/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_demo.py` & `gink-0.20240404.1712252737/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_directory.py` & `gink-0.20240404.1712252737/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_graph.py` & `gink-0.20240404.1712252737/gink/tests/test_graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,7 +55,35 @@
             verb.create_edge(noun1, noun2, "beautiful")
             verb.create_edge(noun1, noun2, "world", timestamp)
             messages = [edge.get_value() for edge in verb.get_edges()]
             assert messages == ["hello", "world", "beautiful"], messages
             edge1.move(dest=generate_timestamp())
             messages = [edge.get_value() for edge in verb.get_edges()]
             assert messages == ["world", "beautiful", "hello"], messages
+
+def test_reissue_properties():
+    for store in [LmdbStore()]:
+        with closing(store):
+            db = Database(store)
+            noun1 = Vertex(database=db)
+            noun2 = Vertex(database=db)
+            verb = Verb(database=db)
+            edge1 = verb.create_edge(noun1, noun2, "hello")
+            edge1.set_property_value_by_name("foo", "bar")
+            edge1.set_property_value_by_name("foo", "baz")
+            timestamp = generate_timestamp()
+            edge1.set_property_value_by_name("foo", "bat")
+            assert edge1.get_property_value_by_name("foo") == "bat"
+            before_removed = list(noun1.get_edges_from())
+            assert len(before_removed) == 1, before_removed
+            edge1.remove()
+            after_removed = list(noun1.get_edges_from())
+            assert len(after_removed) == 0, after_removed
+            bundler = Bundler()
+            db.reset(to_time=timestamp, bundler=bundler)
+            db.commit(bundler)
+            after_reset = list(noun1.get_edges_from())
+            assert len(after_reset) == 1, after_reset
+            edge2 = after_reset[0]
+            assert edge2.get_muid() != edge1.get_muid()
+            val_after_reset = edge2.get_property_value_by_name("foo")
+            assert val_after_reset == "baz", val_after_reset
```

### Comparing `gink-0.20240404.1712204855/gink/tests/test_key_set.py` & `gink-0.20240404.1712252737/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_lmdb_store.py` & `gink-0.20240404.1712252737/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_logbackedstore.py` & `gink-0.20240404.1712252737/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_muid.py` & `gink-0.20240404.1712252737/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_names.py` & `gink-0.20240404.1712252737/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_pair_map.py` & `gink-0.20240404.1712252737/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_pair_set.py` & `gink-0.20240404.1712252737/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_property.py` & `gink-0.20240404.1712252737/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_role.py` & `gink-0.20240404.1712252737/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_sequence.py` & `gink-0.20240404.1712252737/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_store.py` & `gink-0.20240404.1712252737/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink/tests/test_websocket_connection.py` & `gink-0.20240404.1712252737/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/gink.egg-info/PKG-INFO` & `gink-0.20240404.1712252737/gink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240404.1712204855
+Version: 0.20240404.1712252737
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240404.1712204855/gink.egg-info/SOURCES.txt` & `gink-0.20240404.1712252737/gink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712204855/setup.py` & `gink-0.20240404.1712252737/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240404.1712204855',
+    version='0.20240404.1712252737',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

