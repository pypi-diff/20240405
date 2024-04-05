# Comparing `tmp/graphsense-python-1.4.2.tar.gz` & `tmp/graphsense-python-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphsense-python-1.4.2.tar", last modified: Thu Jan 25 16:06:37 2024, max compression
+gzip compressed data, was "graphsense-python-1.6.0.tar", last modified: Fri Apr  5 15:36:48 2024, max compression
```

## Comparing `graphsense-python-1.4.2.tar` & `graphsense-python-1.6.0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:06:37.102805 graphsense-python-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-01-25 16:06:37.102805 graphsense-python-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:06:37.078805 graphsense-python-1.4.2/graphsense/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:06:37.082805 graphsense-python-1.4.2/graphsense/api/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34591 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/addresses_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/blocks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14434 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/bulk_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    44568 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/entities_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/general_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/rates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23068 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26083 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api/txs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36870 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:06:37.082805 graphsense-python-1.4.2/graphsense/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17105 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:06:37.090805 graphsense-python-1.4.2/graphsense/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13663 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/actor_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/actors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16199 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/address.py
--rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/address_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/address_tag_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/address_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/address_tx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13107 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/address_tx_utxo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/address_txs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/concept.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/currency_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/entity_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/height.py
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/labeled_item_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/labeled_item_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/link.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/link_utxo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/links.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/neighbor_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/neighbor_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/neighbor_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    12505 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/neighbor_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_by_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_leaf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_level1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_level2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_level3.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_level4.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_level5.py
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/search_result_level6.py
--rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/token_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/token_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/token_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    17839 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/tx.py
--rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/tx_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/tx_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/tx_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/tx_utxo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/tx_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/tx_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/txs_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model/values.py
--rw-r--r--   0 runner    (1001) docker     (127)    80262 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:06:37.090805 graphsense-python-1.4.2/graphsense/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/graphsense/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:06:37.102805 graphsense-python-1.4.2/graphsense_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-01-25 16:06:37.000000 graphsense-python-1.4.2/graphsense_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-01-25 16:06:37.000000 graphsense-python-1.4.2/graphsense_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 16:06:37.000000 graphsense-python-1.4.2/graphsense_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-25 16:06:37.000000 graphsense-python-1.4.2/graphsense_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-25 16:06:37.000000 graphsense-python-1.4.2/graphsense_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-25 16:06:37.102805 graphsense-python-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:06:37.102805 graphsense-python-1.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_actor_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_actors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_address_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_address_tag_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_address_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_address_tx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_address_tx_utxo.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_address_txs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_addresses_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_blocks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_bulk_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_currency_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_entities_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_entity_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_general_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_height.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_labeled_item_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_labeled_item_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_link_utxo.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_neighbor_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_neighbor_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_neighbor_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_neighbor_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_rates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_by_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_leaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_level1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_level2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_level3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_level4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_level5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_search_result_level6.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_token_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_token_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_token_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tx_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tx_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tx_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tx_utxo.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tx_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_tx_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_txs_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_txs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-01-25 16:06:24.000000 graphsense-python-1.4.2/test/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:36:48.360966 graphsense-python-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-05 15:36:48.360966 graphsense-python-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:36:48.336966 graphsense-python-1.6.0/graphsense/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:36:48.336966 graphsense-python-1.6.0/graphsense/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36063 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/addresses_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/blocks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14434 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/bulk_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46040 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/entities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/general_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/rates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23068 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26083 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api/txs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36870 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:36:48.336966 graphsense-python-1.6.0/graphsense/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17105 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:36:48.348966 graphsense-python-1.6.0/graphsense/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13663 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/actor_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/actors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16199 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/address_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/address_tag_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/address_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/address_tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13107 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/address_tx_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/address_txs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/currency_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/entity_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/height.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/labeled_item_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/labeled_item_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/link_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/neighbor_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/neighbor_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/neighbor_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12505 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/neighbor_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_by_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_leaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_level2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_level3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_level4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_level5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/search_result_level6.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/token_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/token_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/token_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17839 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/tx_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/tx_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/tx_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/tx_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/tx_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/tx_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/txs_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80262 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:36:48.348966 graphsense-python-1.6.0/graphsense/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/graphsense/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:36:48.360966 graphsense-python-1.6.0/graphsense_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-05 15:36:48.000000 graphsense-python-1.6.0/graphsense_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-05 15:36:48.000000 graphsense-python-1.6.0/graphsense_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:36:48.000000 graphsense-python-1.6.0/graphsense_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 15:36:48.000000 graphsense-python-1.6.0/graphsense_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 15:36:48.000000 graphsense-python-1.6.0/graphsense_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 15:36:48.360966 graphsense-python-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:36:48.360966 graphsense-python-1.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_actor_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_actors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_address_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_address_tag_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_address_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_address_tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_address_tx_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_address_txs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_addresses_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_blocks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_bulk_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_currency_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_entities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_entity_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_general_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_labeled_item_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_labeled_item_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_link_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_neighbor_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_neighbor_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_neighbor_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_neighbor_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_rates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_by_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_leaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_level2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_level3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_level4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_level5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_search_result_level6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_token_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_token_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_token_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tx_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tx_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tx_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tx_utxo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tx_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_tx_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_txs_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_txs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-05 15:36:44.000000 graphsense-python-1.6.0/test/test_values.py
```

### Comparing `graphsense-python-1.4.2/LICENSE` & `graphsense-python-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/PKG-INFO` & `graphsense-python-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphsense-python
-Version: 1.4.2
+Version: 1.6.0
 Summary: GraphSense API
 Home-page: 
 Author: Iknaio Cryptoasset Analytics GmbH
 Author-email: contact@ikna.io
 Keywords: OpenAPI,OpenAPI-Generator,GraphSense API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -13,16 +13,16 @@
 Requires-Dist: python-dateutil
 
 # graphsense-python
 GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.4.2
-- Package version: 1.4.2
+- API version: 1.6.0
+- Package version: 1.6.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `graphsense-python-1.4.2/README.md` & `graphsense-python-1.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # graphsense-python
 GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.4.2
-- Package version: 1.4.2
+- API version: 1.6.0
+- Package version: 1.6.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `graphsense-python-1.4.2/graphsense/__init__.py` & `graphsense-python-1.6.0/graphsense/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.4.2"
+__version__ = "1.6.0"
 
 # import ApiClient
 from graphsense.api_client import ApiClient
 
 # import Configuration
 from graphsense.configuration import Configuration
```

### Comparing `graphsense-python-1.4.2/graphsense/api/addresses_api.py` & `graphsense-python-1.6.0/graphsense/api/addresses_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -316,14 +316,17 @@
 
             Args:
                 currency (str): The cryptocurrency code (e.g., btc)
                 address (str): The cryptocurrency address
                 neighbor (str): Neighbor address
 
             Keyword Args:
+                min_height (Height): Return transactions starting from given height. [optional]
+                max_height (Height): Return transactions up to (including) given height. [optional]
+                order (str): Sorting order. [optional] if omitted the server will use the default value of "desc"
                 page (str): Resumption token for retrieving the next page. [optional]
                 pagesize (int): Number of items returned in a single page. [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -386,62 +389,83 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'currency',
                     'address',
                     'neighbor',
+                    'min_height',
+                    'max_height',
+                    'order',
                     'page',
                     'pagesize',
                 ],
                 'required': [
                     'currency',
                     'address',
                     'neighbor',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'order',
                 ],
                 'validation': [
                     'pagesize',
                 ]
             },
             root_map={
                 'validations': {
                     ('pagesize',): {
 
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
+                    ('order',): {
+
+                        "ASC": "asc",
+                        "DESC": "desc"
+                    },
                 },
                 'openapi_types': {
                     'currency':
                         (str,),
                     'address':
                         (str,),
                     'neighbor':
                         (str,),
+                    'min_height':
+                        (Height,),
+                    'max_height':
+                        (Height,),
+                    'order':
+                        (str,),
                     'page':
                         (str,),
                     'pagesize':
                         (int,),
                 },
                 'attribute_map': {
                     'currency': 'currency',
                     'address': 'address',
                     'neighbor': 'neighbor',
+                    'min_height': 'min_height',
+                    'max_height': 'max_height',
+                    'order': 'order',
                     'page': 'page',
                     'pagesize': 'pagesize',
                 },
                 'location_map': {
                     'currency': 'path',
                     'address': 'path',
                     'neighbor': 'query',
+                    'min_height': 'query',
+                    'max_height': 'query',
+                    'order': 'query',
                     'page': 'query',
                     'pagesize': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -646,14 +670,15 @@
                 currency (str): The cryptocurrency code (e.g., btc)
                 address (str): The cryptocurrency address
 
             Keyword Args:
                 direction (str): Incoming or outgoing transactions. [optional]
                 min_height (Height): Return transactions starting from given height. [optional]
                 max_height (Height): Return transactions up to (including) given height. [optional]
+                order (str): Sorting order. [optional] if omitted the server will use the default value of "desc"
                 token_currency (str): Return transactions of given token currency. [optional]
                 page (str): Resumption token for retrieving the next page. [optional]
                 pagesize (int): Number of items returned in a single page. [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
@@ -717,26 +742,28 @@
             params_map={
                 'all': [
                     'currency',
                     'address',
                     'direction',
                     'min_height',
                     'max_height',
+                    'order',
                     'token_currency',
                     'page',
                     'pagesize',
                 ],
                 'required': [
                     'currency',
                     'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'direction',
+                    'order',
                 ],
                 'validation': [
                     'pagesize',
                 ]
             },
             root_map={
                 'validations': {
@@ -747,49 +774,58 @@
                 },
                 'allowed_values': {
                     ('direction',): {
 
                         "IN": "in",
                         "OUT": "out"
                     },
+                    ('order',): {
+
+                        "ASC": "asc",
+                        "DESC": "desc"
+                    },
                 },
                 'openapi_types': {
                     'currency':
                         (str,),
                     'address':
                         (str,),
                     'direction':
                         (str,),
                     'min_height':
                         (Height,),
                     'max_height':
                         (Height,),
+                    'order':
+                        (str,),
                     'token_currency':
                         (str,),
                     'page':
                         (str,),
                     'pagesize':
                         (int,),
                 },
                 'attribute_map': {
                     'currency': 'currency',
                     'address': 'address',
                     'direction': 'direction',
                     'min_height': 'min_height',
                     'max_height': 'max_height',
+                    'order': 'order',
                     'token_currency': 'token_currency',
                     'page': 'page',
                     'pagesize': 'pagesize',
                 },
                 'location_map': {
                     'currency': 'path',
                     'address': 'path',
                     'direction': 'query',
                     'min_height': 'query',
                     'max_height': 'query',
+                    'order': 'query',
                     'token_currency': 'query',
                     'page': 'query',
                     'pagesize': 'query',
                 },
                 'collection_format_map': {
                 }
             },
```

### Comparing `graphsense-python-1.4.2/graphsense/api/blocks_api.py` & `graphsense-python-1.6.0/graphsense/api/blocks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/api/bulk_api.py` & `graphsense-python-1.6.0/graphsense/api/bulk_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/api/entities_api.py` & `graphsense-python-1.6.0/graphsense/api/entities_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -491,14 +491,17 @@
 
             Args:
                 currency (str): The cryptocurrency code (e.g., btc)
                 entity (int): The entity ID
                 neighbor (int): Neighbor entity
 
             Keyword Args:
+                min_height (Height): Return transactions starting from given height. [optional]
+                max_height (Height): Return transactions up to (including) given height. [optional]
+                order (str): Sorting order. [optional] if omitted the server will use the default value of "desc"
                 page (str): Resumption token for retrieving the next page. [optional]
                 pagesize (int): Number of items returned in a single page. [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -561,62 +564,83 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'currency',
                     'entity',
                     'neighbor',
+                    'min_height',
+                    'max_height',
+                    'order',
                     'page',
                     'pagesize',
                 ],
                 'required': [
                     'currency',
                     'entity',
                     'neighbor',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'order',
                 ],
                 'validation': [
                     'pagesize',
                 ]
             },
             root_map={
                 'validations': {
                     ('pagesize',): {
 
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
+                    ('order',): {
+
+                        "ASC": "asc",
+                        "DESC": "desc"
+                    },
                 },
                 'openapi_types': {
                     'currency':
                         (str,),
                     'entity':
                         (int,),
                     'neighbor':
                         (int,),
+                    'min_height':
+                        (Height,),
+                    'max_height':
+                        (Height,),
+                    'order':
+                        (str,),
                     'page':
                         (str,),
                     'pagesize':
                         (int,),
                 },
                 'attribute_map': {
                     'currency': 'currency',
                     'entity': 'entity',
                     'neighbor': 'neighbor',
+                    'min_height': 'min_height',
+                    'max_height': 'max_height',
+                    'order': 'order',
                     'page': 'page',
                     'pagesize': 'pagesize',
                 },
                 'location_map': {
                     'currency': 'path',
                     'entity': 'path',
                     'neighbor': 'query',
+                    'min_height': 'query',
+                    'max_height': 'query',
+                    'order': 'query',
                     'page': 'query',
                     'pagesize': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -833,14 +857,15 @@
                 currency (str): The cryptocurrency code (e.g., btc)
                 entity (int): The entity ID
 
             Keyword Args:
                 direction (str): Incoming or outgoing transactions. [optional]
                 min_height (Height): Return transactions starting from given height. [optional]
                 max_height (Height): Return transactions up to (including) given height. [optional]
+                order (str): Sorting order. [optional] if omitted the server will use the default value of "desc"
                 token_currency (str): Return transactions of given token currency. [optional]
                 page (str): Resumption token for retrieving the next page. [optional]
                 pagesize (int): Number of items returned in a single page. [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
@@ -904,26 +929,28 @@
             params_map={
                 'all': [
                     'currency',
                     'entity',
                     'direction',
                     'min_height',
                     'max_height',
+                    'order',
                     'token_currency',
                     'page',
                     'pagesize',
                 ],
                 'required': [
                     'currency',
                     'entity',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'direction',
+                    'order',
                 ],
                 'validation': [
                     'pagesize',
                 ]
             },
             root_map={
                 'validations': {
@@ -934,49 +961,58 @@
                 },
                 'allowed_values': {
                     ('direction',): {
 
                         "IN": "in",
                         "OUT": "out"
                     },
+                    ('order',): {
+
+                        "ASC": "asc",
+                        "DESC": "desc"
+                    },
                 },
                 'openapi_types': {
                     'currency':
                         (str,),
                     'entity':
                         (int,),
                     'direction':
                         (str,),
                     'min_height':
                         (Height,),
                     'max_height':
                         (Height,),
+                    'order':
+                        (str,),
                     'token_currency':
                         (str,),
                     'page':
                         (str,),
                     'pagesize':
                         (int,),
                 },
                 'attribute_map': {
                     'currency': 'currency',
                     'entity': 'entity',
                     'direction': 'direction',
                     'min_height': 'min_height',
                     'max_height': 'max_height',
+                    'order': 'order',
                     'token_currency': 'token_currency',
                     'page': 'page',
                     'pagesize': 'pagesize',
                 },
                 'location_map': {
                     'currency': 'path',
                     'entity': 'path',
                     'direction': 'query',
                     'min_height': 'query',
                     'max_height': 'query',
+                    'order': 'query',
                     'token_currency': 'query',
                     'page': 'query',
                     'pagesize': 'query',
                 },
                 'collection_format_map': {
                 }
             },
```

### Comparing `graphsense-python-1.4.2/graphsense/api/general_api.py` & `graphsense-python-1.6.0/graphsense/api/general_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/api/rates_api.py` & `graphsense-python-1.6.0/graphsense/api/rates_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/api/tags_api.py` & `graphsense-python-1.6.0/graphsense/api/tags_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/api/tokens_api.py` & `graphsense-python-1.6.0/graphsense/api/tokens_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/api/txs_api.py` & `graphsense-python-1.6.0/graphsense/api/txs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/api_client.py` & `graphsense-python-1.6.0/graphsense/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.4.2/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `graphsense-python-1.4.2/graphsense/apis/__init__.py` & `graphsense-python-1.6.0/graphsense/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/graphsense/configuration.py` & `graphsense-python-1.6.0/graphsense/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -402,16 +402,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.4.2\n"\
-               "SDK Package Version: 1.4.2".\
+               "Version of the API: 1.6.0\n"\
+               "SDK Package Version: 1.6.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `graphsense-python-1.4.2/graphsense/exceptions.py` & `graphsense-python-1.6.0/graphsense/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
```

### Comparing `graphsense-python-1.4.2/graphsense/model/actor.py` & `graphsense-python-1.6.0/graphsense/model/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/actor_context.py` & `graphsense-python-1.6.0/graphsense/model/actor_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/actors.py` & `graphsense-python-1.6.0/graphsense/model/actors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/address.py` & `graphsense-python-1.6.0/graphsense/model/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/address_tag.py` & `graphsense-python-1.6.0/graphsense/model/address_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/address_tag_all_of.py` & `graphsense-python-1.6.0/graphsense/model/address_tag_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/address_tags.py` & `graphsense-python-1.6.0/graphsense/model/address_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/address_tx.py` & `graphsense-python-1.6.0/graphsense/model/address_tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/address_tx_utxo.py` & `graphsense-python-1.6.0/graphsense/model/address_tx_utxo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/address_txs.py` & `graphsense-python-1.6.0/graphsense/model/address_txs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/block.py` & `graphsense-python-1.6.0/graphsense/model/block.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/concept.py` & `graphsense-python-1.6.0/graphsense/model/concept.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/currency_stats.py` & `graphsense-python-1.6.0/graphsense/model/currency_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/entity.py` & `graphsense-python-1.6.0/graphsense/model/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/entity_addresses.py` & `graphsense-python-1.6.0/graphsense/model/entity_addresses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/height.py` & `graphsense-python-1.6.0/graphsense/model/height.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/labeled_item_ref.py` & `graphsense-python-1.6.0/graphsense/model/labeled_item_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/labeled_item_refs.py` & `graphsense-python-1.6.0/graphsense/model/labeled_item_refs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/link.py` & `graphsense-python-1.6.0/graphsense/model/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/link_utxo.py` & `graphsense-python-1.6.0/graphsense/model/link_utxo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/links.py` & `graphsense-python-1.6.0/graphsense/model/links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/neighbor_address.py` & `graphsense-python-1.6.0/graphsense/model/neighbor_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/neighbor_addresses.py` & `graphsense-python-1.6.0/graphsense/model/neighbor_addresses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/neighbor_entities.py` & `graphsense-python-1.6.0/graphsense/model/neighbor_entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/neighbor_entity.py` & `graphsense-python-1.6.0/graphsense/model/neighbor_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/rate.py` & `graphsense-python-1.6.0/graphsense/model/rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/rates.py` & `graphsense-python-1.6.0/graphsense/model/rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result.py` & `graphsense-python-1.6.0/graphsense/model/search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_by_currency.py` & `graphsense-python-1.6.0/graphsense/model/search_result_by_currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_labels.py` & `graphsense-python-1.6.0/graphsense/model/search_result_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_leaf.py` & `graphsense-python-1.6.0/graphsense/model/search_result_leaf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_level1.py` & `graphsense-python-1.6.0/graphsense/model/search_result_level1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_level2.py` & `graphsense-python-1.6.0/graphsense/model/search_result_level2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_level3.py` & `graphsense-python-1.6.0/graphsense/model/search_result_level3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_level4.py` & `graphsense-python-1.6.0/graphsense/model/search_result_level4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_level5.py` & `graphsense-python-1.6.0/graphsense/model/search_result_level5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/search_result_level6.py` & `graphsense-python-1.6.0/graphsense/model/search_result_level6.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/stats.py` & `graphsense-python-1.6.0/graphsense/model/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/tag.py` & `graphsense-python-1.6.0/graphsense/model/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/taxonomy.py` & `graphsense-python-1.6.0/graphsense/model/taxonomy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/token_config.py` & `graphsense-python-1.6.0/graphsense/model/token_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/token_configs.py` & `graphsense-python-1.6.0/graphsense/model/token_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/token_values.py` & `graphsense-python-1.6.0/graphsense/model/token_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/tx.py` & `graphsense-python-1.6.0/graphsense/model/tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/tx_account.py` & `graphsense-python-1.6.0/graphsense/model/tx_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/tx_ref.py` & `graphsense-python-1.6.0/graphsense/model/tx_ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/tx_summary.py` & `graphsense-python-1.6.0/graphsense/model/tx_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/tx_utxo.py` & `graphsense-python-1.6.0/graphsense/model/tx_utxo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/tx_value.py` & `graphsense-python-1.6.0/graphsense/model/tx_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/tx_values.py` & `graphsense-python-1.6.0/graphsense/model/tx_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/txs_account.py` & `graphsense-python-1.6.0/graphsense/model/txs_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model/values.py` & `graphsense-python-1.6.0/graphsense/model/values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `graphsense-python-1.4.2/graphsense/model_utils.py` & `graphsense-python-1.6.0/graphsense/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 import inspect
```

### Comparing `graphsense-python-1.4.2/graphsense/models/__init__.py` & `graphsense-python-1.6.0/graphsense/models/__init__.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/graphsense/rest.py` & `graphsense-python-1.6.0/graphsense/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `graphsense-python-1.4.2/graphsense_python.egg-info/PKG-INFO` & `graphsense-python-1.6.0/graphsense_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphsense-python
-Version: 1.4.2
+Version: 1.6.0
 Summary: GraphSense API
 Home-page: 
 Author: Iknaio Cryptoasset Analytics GmbH
 Author-email: contact@ikna.io
 Keywords: OpenAPI,OpenAPI-Generator,GraphSense API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -13,16 +13,16 @@
 Requires-Dist: python-dateutil
 
 # graphsense-python
 GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.4.2
-- Package version: 1.4.2
+- API version: 1.6.0
+- Package version: 1.6.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `graphsense-python-1.4.2/graphsense_python.egg-info/SOURCES.txt` & `graphsense-python-1.6.0/graphsense_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/setup.py` & `graphsense-python-1.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     GraphSense API
 
     GraphSense API provides programmatic access to various ledgers' addresses, entities, blocks, transactions and tags for automated and highly efficient forensics tasks.  # noqa: E501
 
-    The version of the OpenAPI document: 1.4.2
+    The version of the OpenAPI document: 1.6.0
     Contact: contact@ikna.io
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "graphsense-python"
-VERSION = "1.4.2"
+VERSION = "1.6.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `graphsense-python-1.4.2/test/test_actor.py` & `graphsense-python-1.6.0/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_actor_context.py` & `graphsense-python-1.6.0/test/test_actor_context.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_actors.py` & `graphsense-python-1.6.0/test/test_actors.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_address.py` & `graphsense-python-1.6.0/test/test_address.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_address_tag.py` & `graphsense-python-1.6.0/test/test_address_tag.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_address_tag_all_of.py` & `graphsense-python-1.6.0/test/test_address_tag_all_of.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_address_tags.py` & `graphsense-python-1.6.0/test/test_address_tags.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_address_tx.py` & `graphsense-python-1.6.0/test/test_address_tx.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_address_tx_utxo.py` & `graphsense-python-1.6.0/test/test_address_tx_utxo.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_address_txs.py` & `graphsense-python-1.6.0/test/test_address_txs.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_addresses_api.py` & `graphsense-python-1.6.0/test/test_addresses_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_block.py` & `graphsense-python-1.6.0/test/test_block.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_blocks_api.py` & `graphsense-python-1.6.0/test/test_blocks_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_bulk_api.py` & `graphsense-python-1.6.0/test/test_bulk_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_concept.py` & `graphsense-python-1.6.0/test/test_concept.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_currency_stats.py` & `graphsense-python-1.6.0/test/test_currency_stats.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_entities_api.py` & `graphsense-python-1.6.0/test/test_entities_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_entity.py` & `graphsense-python-1.6.0/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_entity_addresses.py` & `graphsense-python-1.6.0/test/test_entity_addresses.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_general_api.py` & `graphsense-python-1.6.0/test/test_general_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_height.py` & `graphsense-python-1.6.0/test/test_height.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_labeled_item_ref.py` & `graphsense-python-1.6.0/test/test_labeled_item_ref.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_labeled_item_refs.py` & `graphsense-python-1.6.0/test/test_labeled_item_refs.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_link.py` & `graphsense-python-1.6.0/test/test_link.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_link_utxo.py` & `graphsense-python-1.6.0/test/test_link_utxo.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_links.py` & `graphsense-python-1.6.0/test/test_links.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_neighbor_address.py` & `graphsense-python-1.6.0/test/test_neighbor_address.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_neighbor_addresses.py` & `graphsense-python-1.6.0/test/test_neighbor_addresses.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_neighbor_entities.py` & `graphsense-python-1.6.0/test/test_neighbor_entities.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_neighbor_entity.py` & `graphsense-python-1.6.0/test/test_neighbor_entity.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_rate.py` & `graphsense-python-1.6.0/test/test_rate.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_rates.py` & `graphsense-python-1.6.0/test/test_rates.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_rates_api.py` & `graphsense-python-1.6.0/test/test_rates_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result.py` & `graphsense-python-1.6.0/test/test_search_result.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_by_currency.py` & `graphsense-python-1.6.0/test/test_search_result_by_currency.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_labels.py` & `graphsense-python-1.6.0/test/test_search_result_labels.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_leaf.py` & `graphsense-python-1.6.0/test/test_search_result_leaf.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_level1.py` & `graphsense-python-1.6.0/test/test_search_result_level1.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_level2.py` & `graphsense-python-1.6.0/test/test_search_result_level2.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_level3.py` & `graphsense-python-1.6.0/test/test_search_result_level3.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_level4.py` & `graphsense-python-1.6.0/test/test_search_result_level4.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_level5.py` & `graphsense-python-1.6.0/test/test_search_result_level5.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_search_result_level6.py` & `graphsense-python-1.6.0/test/test_search_result_level6.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_stats.py` & `graphsense-python-1.6.0/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tag.py` & `graphsense-python-1.6.0/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tags_api.py` & `graphsense-python-1.6.0/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_taxonomy.py` & `graphsense-python-1.6.0/test/test_taxonomy.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_token_config.py` & `graphsense-python-1.6.0/test/test_token_config.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_token_configs.py` & `graphsense-python-1.6.0/test/test_token_configs.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_token_values.py` & `graphsense-python-1.6.0/test/test_token_values.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tokens_api.py` & `graphsense-python-1.6.0/test/test_tokens_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tx.py` & `graphsense-python-1.6.0/test/test_tx.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tx_account.py` & `graphsense-python-1.6.0/test/test_tx_account.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tx_ref.py` & `graphsense-python-1.6.0/test/test_tx_ref.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tx_summary.py` & `graphsense-python-1.6.0/test/test_tx_summary.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tx_utxo.py` & `graphsense-python-1.6.0/test/test_tx_utxo.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tx_value.py` & `graphsense-python-1.6.0/test/test_tx_value.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_tx_values.py` & `graphsense-python-1.6.0/test/test_tx_values.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_txs_account.py` & `graphsense-python-1.6.0/test/test_txs_account.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_txs_api.py` & `graphsense-python-1.6.0/test/test_txs_api.py`

 * *Files identical despite different names*

### Comparing `graphsense-python-1.4.2/test/test_values.py` & `graphsense-python-1.6.0/test/test_values.py`

 * *Files identical despite different names*

