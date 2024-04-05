# Comparing `tmp/shippo_legacy-2.1.5.tar.gz` & `tmp/shippo_legacy-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo_legacy-2.1.5.tar", max compression
+gzip compressed data, was "shippo_legacy-2.1.6.tar", max compression
```

## Comparing `shippo_legacy-2.1.5.tar` & `shippo_legacy-2.1.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0     1089 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/LICENSE
--rw-r--r--   0        0        0     4051 2024-04-04 23:02:54.480881 shippo_legacy-2.1.5/README.md
--rw-r--r--   0        0        0      638 2024-04-04 22:07:13.168830 shippo_legacy-2.1.5/pyproject.toml
--rw-r--r--   0        0        0      291 2024-04-04 23:04:04.864122 shippo_legacy-2.1.5/shippo/__init__.py
--rw-r--r--   0        0        0     7982 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/api_requestor.py
--rw-r--r--   0        0        0      928 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/certificate_blacklist.py
--rw-r--r--   0        0        0     1178 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/config.py
--rw-r--r--   0        0        0     1370 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/error.py
--rw-r--r--   0        0        0     7110 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/http_client.py
--rw-r--r--   0        0        0    22719 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/resource.py
--rw-r--r--   0        0        0      322 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/__init__.py
--rw-r--r--   0        0        0     2020 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/address/test_create
--rw-r--r--   0        0        0     1932 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/address/test_invalid_create
--rw-r--r--   0        0        0     1380 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/address/test_invalid_retrieve
--rw-r--r--   0        0        0     4019 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/address/test_invalid_validate
--rw-r--r--   0        0        0     2398 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/address/test_list_all
--rw-r--r--   0        0        0     2040 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/address/test_list_page_size
--rw-r--r--   0        0        0     3733 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/address/test_retrieve
--rw-r--r--   0        0        0     3754 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/address/test_validate
--rw-r--r--   0        0        0    56862 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_add
--rw-r--r--   0        0        0     3181 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_create
--rw-r--r--   0        0        0    48246 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_add
--rw-r--r--   0        0        0     3194 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_create
--rw-r--r--   0        0        0     1436 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_purchase
--rw-r--r--   0        0        0     6349 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_remove
--rw-r--r--   0        0        0     1379 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_retrieve
--rw-r--r--   0        0        0    12397 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_purchase
--rw-r--r--   0        0        0    58918 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_remove
--rw-r--r--   0        0        0     6919 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_retrieve
--rw-r--r--   0        0        0     4266 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_create
--rw-r--r--   0        0        0     1685 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_invalid_create
--rw-r--r--   0        0        0     1403 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_invalid_retrieve
--rw-r--r--   0        0        0     2393 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_list_all
--rw-r--r--   0        0        0     1958 2024-04-04 16:56:13.849160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_list_page_size
--rw-r--r--   0        0        0     6108 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_retrieve
--rw-r--r--   0        0        0     1921 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_create
--rw-r--r--   0        0        0     1541 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_invalid_create
--rw-r--r--   0        0        0     1388 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_invalid_retrieve
--rw-r--r--   0        0        0     2018 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_list_all
--rw-r--r--   0        0        0     1777 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_list_page_size
--rw-r--r--   0        0        0     3598 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_retrieve
--rw-r--r--   0        0        0    24862 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_create
--rw-r--r--   0        0        0     1424 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_invalid_create
--rw-r--r--   0        0        0     1381 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_invalid_retrieve
--rw-r--r--   0        0        0     3295 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_list_all
--rw-r--r--   0        0        0     1968 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_list_page_size
--rw-r--r--   0        0        0    26738 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_retrieve
--rw-r--r--   0        0        0     3327 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/order/test_create
--rw-r--r--   0        0        0     1704 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/order/test_invalid_create
--rw-r--r--   0        0        0     1696 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/order/test_invalid_retrieve
--rw-r--r--   0        0        0     2851 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/order/test_list_all
--rw-r--r--   0        0        0     2609 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/order/test_list_page_size
--rw-r--r--   0        0        0     5873 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/order/test_retrieve
--rw-r--r--   0        0        0     1833 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_create
--rw-r--r--   0        0        0     1382 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_invalid_create
--rw-r--r--   0        0        0     1378 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_invalid_retrieve
--rw-r--r--   0        0        0     1971 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_list_all
--rw-r--r--   0        0        0     1811 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_list_page_size
--rw-r--r--   0        0        0     3467 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_retrieve
--rw-r--r--   0        0        0    15830 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/pickup/test_create
--rw-r--r--   0        0        0     1372 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/rate/test_invalid_retrieve
--rw-r--r--   0        0        0    22397 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/rate/test_retrieve
--rw-r--r--   0        0        0    11504 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_create
--rw-r--r--   0        0        0    20598 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_get_rate
--rw-r--r--   0        0        0    20586 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_get_rates_blocking
--rw-r--r--   0        0        0     1809 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_invalid_create
--rw-r--r--   0        0        0     1395 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_invalid_get_rate
--rw-r--r--   0        0        0     1380 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_invalid_retrieve
--rw-r--r--   0        0        0    10883 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_list_all
--rw-r--r--   0        0        0     5231 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_list_page_size
--rw-r--r--   0        0        0    16622 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_retrieve
--rw-r--r--   0        0        0     2819 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/track/test_create
--rw-r--r--   0        0        0     2706 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/track/test_get_status
--rw-r--r--   0        0        0     3067 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/track/test_invalid_create
--rw-r--r--   0        0        0     2693 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/track/test_invalid_get_status
--rw-r--r--   0        0        0    22400 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_create
--rw-r--r--   0        0        0     1259 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_invalid_create
--rw-r--r--   0        0        0     1387 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_invalid_retrieve
--rw-r--r--   0        0        0     2852 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_list_all
--rw-r--r--   0        0        0     1833 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_list_page_size
--rw-r--r--   0        0        0    24169 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_retrieve
--rw-r--r--   0        0        0    15373 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/helper.py
--rw-r--r--   0        0        0        0 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/integration/__init__.py
--rw-r--r--   0        0        0     3022 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/integration/test_integration.py
--rw-r--r--   0        0        0     2928 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_address.py
--rw-r--r--   0        0        0     2330 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_api_requestor.py
--rw-r--r--   0        0        0     5860 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_batch.py
--rw-r--r--   0        0        0     3203 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_customs_declaration.py
--rw-r--r--   0        0        0     2430 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_customs_item.py
--rw-r--r--   0        0        0     5592 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_http_client.py
--rw-r--r--   0        0        0     2511 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_manifest.py
--rw-r--r--   0        0        0     2409 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_order.py
--rw-r--r--   0        0        0     2260 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_parcel.py
--rw-r--r--   0        0        0     1690 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_pickup.py
--rw-r--r--   0        0        0     1426 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_rate.py
--rw-r--r--   0        0        0     3211 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_shipment.py
--rw-r--r--   0        0        0     2826 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_track.py
--rw-r--r--   0        0        0     2897 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/test/test_transaction.py
--rw-r--r--   0        0        0     1164 2024-04-04 16:56:13.853160 shippo_legacy-2.1.5/shippo/util.py
--rw-r--r--   0        0        0       18 2024-04-04 22:17:53.621897 shippo_legacy-2.1.5/shippo/version.py
--rw-r--r--   0        0        0     5041 1970-01-01 00:00:00.000000 shippo_legacy-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/LICENSE
+-rw-r--r--   0        0        0     4051 2024-04-04 23:02:54.480881 shippo_legacy-2.1.6/README.md
+-rw-r--r--   0        0        0      654 2024-04-05 15:54:00.369374 shippo_legacy-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0      291 2024-04-05 15:57:41.334940 shippo_legacy-2.1.6/shippo/__init__.py
+-rw-r--r--   0        0        0     7982 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/api_requestor.py
+-rw-r--r--   0        0        0      928 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/certificate_blacklist.py
+-rw-r--r--   0        0        0     1178 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/config.py
+-rw-r--r--   0        0        0     1370 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/error.py
+-rw-r--r--   0        0        0     7110 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/http_client.py
+-rw-r--r--   0        0        0    22719 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/resource.py
+-rw-r--r--   0        0        0      322 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/__init__.py
+-rw-r--r--   0        0        0     2020 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/address/test_create
+-rw-r--r--   0        0        0     1932 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/address/test_invalid_create
+-rw-r--r--   0        0        0     1380 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/address/test_invalid_retrieve
+-rw-r--r--   0        0        0     4019 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/address/test_invalid_validate
+-rw-r--r--   0        0        0     2398 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/address/test_list_all
+-rw-r--r--   0        0        0     2040 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/address/test_list_page_size
+-rw-r--r--   0        0        0     3733 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/address/test_retrieve
+-rw-r--r--   0        0        0     3754 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/address/test_validate
+-rw-r--r--   0        0        0    56862 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_add
+-rw-r--r--   0        0        0     3181 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_create
+-rw-r--r--   0        0        0    48246 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_add
+-rw-r--r--   0        0        0     3194 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_create
+-rw-r--r--   0        0        0     1436 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_purchase
+-rw-r--r--   0        0        0     6349 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_remove
+-rw-r--r--   0        0        0     1379 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_retrieve
+-rw-r--r--   0        0        0    12397 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_purchase
+-rw-r--r--   0        0        0    58918 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_remove
+-rw-r--r--   0        0        0     6919 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_retrieve
+-rw-r--r--   0        0        0     4266 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_create
+-rw-r--r--   0        0        0     1685 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_invalid_create
+-rw-r--r--   0        0        0     1403 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_invalid_retrieve
+-rw-r--r--   0        0        0     2393 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_list_all
+-rw-r--r--   0        0        0     1958 2024-04-04 16:56:13.849160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_list_page_size
+-rw-r--r--   0        0        0     6108 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_retrieve
+-rw-r--r--   0        0        0     1921 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_create
+-rw-r--r--   0        0        0     1541 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_invalid_create
+-rw-r--r--   0        0        0     1388 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_invalid_retrieve
+-rw-r--r--   0        0        0     2018 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_list_all
+-rw-r--r--   0        0        0     1777 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_list_page_size
+-rw-r--r--   0        0        0     3598 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_retrieve
+-rw-r--r--   0        0        0    24862 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_create
+-rw-r--r--   0        0        0     1424 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_invalid_create
+-rw-r--r--   0        0        0     1381 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_invalid_retrieve
+-rw-r--r--   0        0        0     3295 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_list_all
+-rw-r--r--   0        0        0     1968 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_list_page_size
+-rw-r--r--   0        0        0    26738 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_retrieve
+-rw-r--r--   0        0        0     3327 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/order/test_create
+-rw-r--r--   0        0        0     1704 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/order/test_invalid_create
+-rw-r--r--   0        0        0     1696 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/order/test_invalid_retrieve
+-rw-r--r--   0        0        0     2851 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/order/test_list_all
+-rw-r--r--   0        0        0     2609 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/order/test_list_page_size
+-rw-r--r--   0        0        0     5873 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/order/test_retrieve
+-rw-r--r--   0        0        0     1833 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_create
+-rw-r--r--   0        0        0     1382 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_invalid_create
+-rw-r--r--   0        0        0     1378 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_invalid_retrieve
+-rw-r--r--   0        0        0     1971 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_list_all
+-rw-r--r--   0        0        0     1811 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_list_page_size
+-rw-r--r--   0        0        0     3467 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_retrieve
+-rw-r--r--   0        0        0    15830 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/pickup/test_create
+-rw-r--r--   0        0        0     1372 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/rate/test_invalid_retrieve
+-rw-r--r--   0        0        0    22397 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/rate/test_retrieve
+-rw-r--r--   0        0        0    11504 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_create
+-rw-r--r--   0        0        0    20598 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_get_rate
+-rw-r--r--   0        0        0    20586 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_get_rates_blocking
+-rw-r--r--   0        0        0     1809 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_invalid_create
+-rw-r--r--   0        0        0     1395 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_invalid_get_rate
+-rw-r--r--   0        0        0     1380 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_invalid_retrieve
+-rw-r--r--   0        0        0    10883 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_list_all
+-rw-r--r--   0        0        0     5231 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_list_page_size
+-rw-r--r--   0        0        0    16622 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_retrieve
+-rw-r--r--   0        0        0     2819 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/track/test_create
+-rw-r--r--   0        0        0     2706 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/track/test_get_status
+-rw-r--r--   0        0        0     3067 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/track/test_invalid_create
+-rw-r--r--   0        0        0     2693 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/track/test_invalid_get_status
+-rw-r--r--   0        0        0    22400 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_create
+-rw-r--r--   0        0        0     1259 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_invalid_create
+-rw-r--r--   0        0        0     1387 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_invalid_retrieve
+-rw-r--r--   0        0        0     2852 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_list_all
+-rw-r--r--   0        0        0     1833 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_list_page_size
+-rw-r--r--   0        0        0    24169 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_retrieve
+-rw-r--r--   0        0        0    15373 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/helper.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/integration/__init__.py
+-rw-r--r--   0        0        0     3022 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/integration/test_integration.py
+-rw-r--r--   0        0        0     2928 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_address.py
+-rw-r--r--   0        0        0     2330 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_api_requestor.py
+-rw-r--r--   0        0        0     5860 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_batch.py
+-rw-r--r--   0        0        0     3203 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_customs_declaration.py
+-rw-r--r--   0        0        0     2430 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_customs_item.py
+-rw-r--r--   0        0        0     5592 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_http_client.py
+-rw-r--r--   0        0        0     2511 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_manifest.py
+-rw-r--r--   0        0        0     2409 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_order.py
+-rw-r--r--   0        0        0     2260 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_parcel.py
+-rw-r--r--   0        0        0     1690 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_pickup.py
+-rw-r--r--   0        0        0     1426 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_rate.py
+-rw-r--r--   0        0        0     3211 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_shipment.py
+-rw-r--r--   0        0        0     2826 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_track.py
+-rw-r--r--   0        0        0     2897 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/test/test_transaction.py
+-rw-r--r--   0        0        0     1164 2024-04-04 16:56:13.853160 shippo_legacy-2.1.6/shippo/util.py
+-rw-r--r--   0        0        0       18 2024-04-05 15:53:52.357462 shippo_legacy-2.1.6/shippo/version.py
+-rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 shippo_legacy-2.1.6/PKG-INFO
```

### Comparing `shippo_legacy-2.1.5/LICENSE` & `shippo_legacy-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/README.md` & `shippo_legacy-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/pyproject.toml` & `shippo_legacy-2.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core~=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "shippo-legacy"
-version = "2.1.5"
+version = "2.1.6"
 authors = [
   "rapid537 <rapid537@zoho.com>",
 ]
 description = "Shipping API Python library (USPS, FedEx, UPS and more)"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -17,10 +17,11 @@
 ]
 homepage = "https://github.com/rapid537/shippo-legacy.git"
 packages = [
     { include = "shippo" }
 ]
 
 [tool.poetry.dependencies]
+python = "^3.6"
 chardet = "^5.2.0"
 requests = "^2.31.0"
 simplejson = ">=3.16.0, <=3.17.2"
```

### Comparing `shippo_legacy-2.1.5/shippo/api_requestor.py` & `shippo_legacy-2.1.6/shippo/api_requestor.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/certificate_blacklist.py` & `shippo_legacy-2.1.6/shippo/certificate_blacklist.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/config.py` & `shippo_legacy-2.1.6/shippo/config.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/error.py` & `shippo_legacy-2.1.6/shippo/error.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/http_client.py` & `shippo_legacy-2.1.6/shippo/http_client.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/resource.py` & `shippo_legacy-2.1.6/shippo/resource.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/address/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/address/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/address/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/address/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/address/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/address/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/address/test_invalid_validate` & `shippo_legacy-2.1.6/shippo/test/fixtures/address/test_invalid_validate`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/address/test_list_all` & `shippo_legacy-2.1.6/shippo/test/fixtures/address/test_list_all`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/address/test_list_page_size` & `shippo_legacy-2.1.6/shippo/test/fixtures/address/test_list_page_size`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/address/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/address/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/address/test_validate` & `shippo_legacy-2.1.6/shippo/test/fixtures/address/test_validate`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_add` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_add`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_add` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_add`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_purchase` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_purchase`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_remove` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_remove`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_purchase` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_purchase`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_remove` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_remove`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/batch/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/batch/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_list_all` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_list_all`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_list_page_size` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_list_page_size`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-declaration/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-declaration/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_list_all` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_list_all`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_list_page_size` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_list_page_size`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/customs-item/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/customs-item/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_list_all` & `shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_list_all`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_list_page_size` & `shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_list_page_size`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/manifest/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/manifest/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/order/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/order/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/order/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/order/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/order/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/order/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/order/test_list_all` & `shippo_legacy-2.1.6/shippo/test/fixtures/order/test_list_all`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/order/test_list_page_size` & `shippo_legacy-2.1.6/shippo/test/fixtures/order/test_list_page_size`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/order/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/order/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_list_all` & `shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_list_all`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_list_page_size` & `shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_list_page_size`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/parcel/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/parcel/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/pickup/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/pickup/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/rate/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/rate/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/rate/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/rate/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_get_rate` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_get_rate`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_get_rates_blocking` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_get_rates_blocking`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_invalid_get_rate` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_invalid_get_rate`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_list_all` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_list_all`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_list_page_size` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_list_page_size`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/shipment/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/shipment/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/track/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/track/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/track/test_get_status` & `shippo_legacy-2.1.6/shippo/test/fixtures/track/test_get_status`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/track/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/track/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/track/test_invalid_get_status` & `shippo_legacy-2.1.6/shippo/test/fixtures/track/test_invalid_get_status`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_invalid_create` & `shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_invalid_create`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_invalid_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_invalid_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_list_all` & `shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_list_all`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_list_page_size` & `shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_list_page_size`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/fixtures/transaction/test_retrieve` & `shippo_legacy-2.1.6/shippo/test/fixtures/transaction/test_retrieve`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/helper.py` & `shippo_legacy-2.1.6/shippo/test/helper.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/integration/test_integration.py` & `shippo_legacy-2.1.6/shippo/test/integration/test_integration.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_address.py` & `shippo_legacy-2.1.6/shippo/test/test_address.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_api_requestor.py` & `shippo_legacy-2.1.6/shippo/test/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_batch.py` & `shippo_legacy-2.1.6/shippo/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_customs_declaration.py` & `shippo_legacy-2.1.6/shippo/test/test_customs_declaration.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_customs_item.py` & `shippo_legacy-2.1.6/shippo/test/test_customs_item.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_http_client.py` & `shippo_legacy-2.1.6/shippo/test/test_http_client.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_manifest.py` & `shippo_legacy-2.1.6/shippo/test/test_manifest.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_order.py` & `shippo_legacy-2.1.6/shippo/test/test_order.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_parcel.py` & `shippo_legacy-2.1.6/shippo/test/test_parcel.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_pickup.py` & `shippo_legacy-2.1.6/shippo/test/test_pickup.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_rate.py` & `shippo_legacy-2.1.6/shippo/test/test_rate.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_shipment.py` & `shippo_legacy-2.1.6/shippo/test/test_shipment.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_track.py` & `shippo_legacy-2.1.6/shippo/test/test_track.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/test/test_transaction.py` & `shippo_legacy-2.1.6/shippo/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/shippo/util.py` & `shippo_legacy-2.1.6/shippo/util.py`

 * *Files identical despite different names*

### Comparing `shippo_legacy-2.1.5/PKG-INFO` & `shippo_legacy-2.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: shippo-legacy
-Version: 2.1.5
+Version: 2.1.6
 Summary: Shipping API Python library (USPS, FedEx, UPS and more)
 Home-page: https://github.com/rapid537/shippo-legacy.git
 Author: rapid537
 Author-email: rapid537@zoho.com
+Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

