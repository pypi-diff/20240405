# Comparing `tmp/assemblyline-4.5.1.dev7.tar.gz` & `tmp/assemblyline-4.5.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-4.5.1.dev7.tar", last modified: Thu Feb 22 17:19:51 2024, max compression
+gzip compressed data, was "assemblyline-4.5.1.dev8.tar", last modified: Thu Feb 22 20:16:24 2024, max compression
```

## Comparing `assemblyline-4.5.1.dev7.tar` & `assemblyline-4.5.1.dev8.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.468601 assemblyline-4.5.1.dev7/
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (127)       47 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2530 2024-02-22 17:19:51.468601 assemblyline-4.5.1.dev7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.448600 assemblyline-4.5.1.dev7/assemblyline/
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-02-22 17:19:47.000000 assemblyline-4.5.1.dev7/assemblyline/VERSION
--rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.448600 assemblyline-4.5.1.dev7/assemblyline/cachestore/
--rw-r--r--   0 vsts      (1001) docker     (127)     3463 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/cachestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.456600 assemblyline-4.5.1.dev7/assemblyline/common/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4138 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/archiving.py
--rw-r--r--   0 vsts      (1001) docker     (127)  2243670 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/attack_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13368 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/backupmanager.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2369 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/banner.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16341 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/bundling.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5668 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/caching.py
--rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/chunk.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41768 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/classification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/classification.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     5811 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/cleanup_filestore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2132 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/codec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5031 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/comms.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2587 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5784 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/custom.magic
--rw-r--r--   0 vsts      (1001) docker     (127)    39136 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/custom.yara
--rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/dict_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2550 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/digests.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2713 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/entropy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1903 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      584 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8581 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/forge.py
--rw-r--r--   0 vsts      (1001) docker     (127)   288720 2024-02-22 17:19:51.000000 assemblyline-4.5.1.dev7/assemblyline/common/frequency.c
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/frequency.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)     6450 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/heuristics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1398 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/hexdump.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23161 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/identify.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19309 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/identify_defaults.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/importing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4229 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/iprange.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5281 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/isotime.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4310 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/logformat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/lucene.lark
--rw-r--r--   0 vsts      (1001) docker     (127)     1105 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/memory_zip.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5230 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/net.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21606 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/net_static.py
--rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/null.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1515 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/path.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28598 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/postprocess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/random_user.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3379 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/security.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/common/signaturing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7396 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/str_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12687 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/tag_safelist.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     3904 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1052 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/threading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/uid.py
--rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/common/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.456600 assemblyline-4.5.1.dev7/assemblyline/datasource/
--rw-r--r--   0 vsts      (1001) docker     (127)      433 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/datasource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2183 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/datasource/al.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1462 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/datasource/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/datasource/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.460600 assemblyline-4.5.1.dev7/assemblyline/datastore/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/bulk.py
--rw-r--r--   0 vsts      (1001) docker     (127)    88221 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61668 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/store.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.460600 assemblyline-4.5.1.dev7/assemblyline/datastore/support/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/support/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9424 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/support/build.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/datastore/support/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.460600 assemblyline-4.5.1.dev7/assemblyline/filestore/
--rw-r--r--   0 vsts      (1001) docker     (127)    10460 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.460600 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7891 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/azure.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2720 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9648 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/http.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5429 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/local.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6828 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/s3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6558 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/filestore/transport/sftp.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.460600 assemblyline-4.5.1.dev7/assemblyline/odm/
--rw-r--r--   0 vsts      (1001) docker     (127)     1854 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54611 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/odm/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.460600 assemblyline-4.5.1.dev7/assemblyline/odm/messages/
--rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1505 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/alerter_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1532 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/archive_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/changes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2476 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/dispatcher_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1299 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/dispatching.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1546 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/expiry_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/ingest_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/scaler_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/scaler_status_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1787 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/service_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1275 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/service_timing_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2190 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/submission.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4109 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1116 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/messages/vacuum_heartbeat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.464601 assemblyline-4.5.1.dev7/assemblyline/odm/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3071 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/actions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13978 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3932 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/badlist.py
--rw-r--r--   0 vsts      (1001) docker     (127)      281 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/cached_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)    71484 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/emptyresult.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/error.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5057 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/filescore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/heuristic.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.464601 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/
--rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.464601 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/filetypes/
--rw-r--r--   0 vsts      (1001) docker     (127)       61 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/filetypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24751 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/filetypes/pe.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5726 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/ontology.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.464601 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1843 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/antivirus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13798 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/malware_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/network.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/process.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2507 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/sandbox.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2961 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/signature.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3635 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9421 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2683 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/retrohunt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3098 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10968 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/service.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8161 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/service_delta.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/signature.py
--rw-r--r--   0 vsts      (1001) docker     (127)      695 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/statistics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8791 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/submission.py
--rw-r--r--   0 vsts      (1001) docker     (127)      843 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/submission_summary.py
--rw-r--r--   0 vsts      (1001) docker     (127)      638 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/submission_tree.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36489 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10371 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/user.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/user_favorites.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2508 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/user_settings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1895 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/models/workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.464601 assemblyline-4.5.1.dev7/assemblyline/odm/random_data/
--rw-r--r--   0 vsts      (1001) docker     (127)    17934 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/random_data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2956 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/random_data/create_test_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25241 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/odm/random_data/sample_rules.yar
--rw-r--r--   0 vsts      (1001) docker     (127)     9244 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/odm/random_data/sample_suricata.rules
--rw-r--r--   0 vsts      (1001) docker     (127)    14862 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/odm/randomizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.464601 assemblyline-4.5.1.dev7/assemblyline/remote/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/remote/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.468601 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/
--rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1661 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/counters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/events.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7000 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/exporting_counter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6018 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/hash.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1442 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/lock.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.468601 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1793 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/comms.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/multi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2871 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/named.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7394 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/priority.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2902 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/set.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/user_quota_tracker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.468601 assemblyline-4.5.1.dev7/assemblyline/run/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/run/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53139 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/assemblyline/run/cli.py
--rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/run/pubsub_reader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3760 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/run/suricata_importer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4791 2024-02-22 17:19:35.000000 assemblyline-4.5.1.dev7/assemblyline/run/yara_importer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 17:19:51.448600 assemblyline-4.5.1.dev7/assemblyline.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2530 2024-02-22 17:19:51.000000 assemblyline-4.5.1.dev7/assemblyline.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     6198 2024-02-22 17:19:51.000000 assemblyline-4.5.1.dev7/assemblyline.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-22 17:19:51.000000 assemblyline-4.5.1.dev7/assemblyline.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-02-22 17:19:51.000000 assemblyline-4.5.1.dev7/assemblyline.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-22 17:19:51.000000 assemblyline-4.5.1.dev7/assemblyline.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-02-22 17:19:51.468601 assemblyline-4.5.1.dev7/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     3812 2024-02-22 17:19:36.000000 assemblyline-4.5.1.dev7/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       47 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2530 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.732298 assemblyline-4.5.1.dev8/assemblyline/
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-02-22 20:16:21.000000 assemblyline-4.5.1.dev8/assemblyline/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.732298 assemblyline-4.5.1.dev8/assemblyline/cachestore/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3463 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/cachestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/common/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4138 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/archiving.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  2243670 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/attack_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13368 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/backupmanager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2369 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/banner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16341 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/bundling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5668 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/caching.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/chunk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41768 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/classification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/classification.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     5811 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/cleanup_filestore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2132 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/codec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5031 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2587 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5841 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/custom.magic
+-rw-r--r--   0 vsts      (1001) docker     (127)    39136 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/custom.yara
+-rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/dict_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2550 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/digests.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2713 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/entropy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1903 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      584 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8581 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/forge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   288720 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline/common/frequency.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/frequency.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)     6450 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/heuristics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1398 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/hexdump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23161 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/identify.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19383 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/identify_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/importing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4229 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/iprange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5281 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/isotime.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4310 2024-02-22 20:16:07.000000 assemblyline-4.5.1.dev8/assemblyline/common/log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/logformat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/lucene.lark
+-rw-r--r--   0 vsts      (1001) docker     (127)     1105 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/memory_zip.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5230 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/net.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21606 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/net_static.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/null.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1515 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28598 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/postprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/random_user.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3379 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/security.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/common/signaturing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7396 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/str_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12687 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/tag_safelist.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3904 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1052 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/threading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/uid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/common/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/datasource/
+-rw-r--r--   0 vsts      (1001) docker     (127)      433 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datasource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2183 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datasource/al.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1462 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datasource/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datasource/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/datastore/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/bulk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    88221 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61668 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/store.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/datastore/support/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/support/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9424 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/support/build.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/datastore/support/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/filestore/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10460 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7891 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/azure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2720 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9648 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/http.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5429 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/local.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6828 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/s3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6558 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/filestore/transport/sftp.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.748298 assemblyline-4.5.1.dev8/assemblyline/odm/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1854 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54611 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.752298 assemblyline-4.5.1.dev8/assemblyline/odm/messages/
+-rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1505 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/alerter_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1532 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/archive_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/changes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2476 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/dispatcher_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1299 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/dispatching.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1546 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/expiry_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/ingest_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/scaler_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/scaler_status_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1787 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/service_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1275 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/service_timing_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2190 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4109 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1116 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/messages/vacuum_heartbeat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3071 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13978 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3932 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/badlist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      281 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/cached_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    71484 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/emptyresult.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5057 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/filescore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/heuristic.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/
+-rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/filetypes/
+-rw-r--r--   0 vsts      (1001) docker     (127)       61 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/filetypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24751 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/filetypes/pe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5726 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/ontology.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1843 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/antivirus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13798 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/malware_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/process.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2507 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/sandbox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2961 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3635 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9421 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2683 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/retrohunt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3098 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10968 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/service.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8161 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/service_delta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      695 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/statistics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8791 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      843 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/submission_summary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      638 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/submission_tree.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36489 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10371 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/user.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/user_favorites.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2508 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/user_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1895 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/models/workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17934 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2956 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/create_test_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25241 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/sample_rules.yar
+-rw-r--r--   0 vsts      (1001) docker     (127)     9244 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/odm/random_data/sample_suricata.rules
+-rw-r--r--   0 vsts      (1001) docker     (127)    14862 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/odm/randomizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.756298 assemblyline-4.5.1.dev8/assemblyline/remote/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1661 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/counters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7000 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/exporting_counter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6018 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/hash.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1442 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/lock.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1793 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/multi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2871 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/named.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7394 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/priority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2902 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/set.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/user_quota_tracker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/assemblyline/run/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/run/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53139 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/assemblyline/run/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/run/pubsub_reader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3760 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/run/suricata_importer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4791 2024-02-22 20:16:06.000000 assemblyline-4.5.1.dev8/assemblyline/run/yara_importer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:24.732298 assemblyline-4.5.1.dev8/assemblyline.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2530 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     6198 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-22 20:16:24.000000 assemblyline-4.5.1.dev8/assemblyline.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-02-22 20:16:24.760298 assemblyline-4.5.1.dev8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     3812 2024-02-22 20:16:08.000000 assemblyline-4.5.1.dev8/setup.py
```

### Comparing `assemblyline-4.5.1.dev7/LICENCE.md` & `assemblyline-4.5.1.dev8/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/PKG-INFO` & `assemblyline-4.5.1.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.5.1.dev7
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-4.5.1.dev7/README.md` & `assemblyline-4.5.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/cachestore/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/cachestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/archiving.py` & `assemblyline-4.5.1.dev8/assemblyline/common/archiving.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/attack_map.py` & `assemblyline-4.5.1.dev8/assemblyline/common/attack_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/backupmanager.py` & `assemblyline-4.5.1.dev8/assemblyline/common/backupmanager.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/banner.py` & `assemblyline-4.5.1.dev8/assemblyline/common/banner.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/bundling.py` & `assemblyline-4.5.1.dev8/assemblyline/common/bundling.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/caching.py` & `assemblyline-4.5.1.dev8/assemblyline/common/caching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/chunk.py` & `assemblyline-4.5.1.dev8/assemblyline/common/chunk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/classification.py` & `assemblyline-4.5.1.dev8/assemblyline/common/classification.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/classification.yml` & `assemblyline-4.5.1.dev8/assemblyline/common/classification.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/cleanup_filestore.py` & `assemblyline-4.5.1.dev8/assemblyline/common/cleanup_filestore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/codec.py` & `assemblyline-4.5.1.dev8/assemblyline/common/codec.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/comms.py` & `assemblyline-4.5.1.dev8/assemblyline/common/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/constants.py` & `assemblyline-4.5.1.dev8/assemblyline/common/constants.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/custom.magic` & `assemblyline-4.5.1.dev8/assemblyline/common/custom.magic`

 * *Files 2% similar despite different names*

```diff
@@ -142,7 +142,9 @@
 >0x1000 string oat custom: executable/android/oat
 # Assemblyline Ontology files
 0 string {"odm_type\":\ "Assemblyline\ Result\ Ontology" custom: assemblyline/ontology
 # Assemblyline uri files
 0 string #\ Assemblyline\ URI\ file\n custom: uri
 # OneNote .onetoc2
 0 string \xa1\x2f\xff\x43\xd9\xef\x76\x4c\x9e\xe2\x10\xea\x57\x22\x76\x5f custom: document/office/onenote
+# Minidump Files
+0 string MDMP custom: metadata/minidump
```

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/custom.yara` & `assemblyline-4.5.1.dev8/assemblyline/common/custom.yara`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/dict_utils.py` & `assemblyline-4.5.1.dev8/assemblyline/common/dict_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/digests.py` & `assemblyline-4.5.1.dev8/assemblyline/common/digests.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/entropy.py` & `assemblyline-4.5.1.dev8/assemblyline/common/entropy.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/exceptions.py` & `assemblyline-4.5.1.dev8/assemblyline/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/file.py` & `assemblyline-4.5.1.dev8/assemblyline/common/file.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/forge.py` & `assemblyline-4.5.1.dev8/assemblyline/common/forge.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/frequency.c` & `assemblyline-4.5.1.dev8/assemblyline/common/frequency.c`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/frequency.pyx` & `assemblyline-4.5.1.dev8/assemblyline/common/frequency.pyx`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/heuristics.py` & `assemblyline-4.5.1.dev8/assemblyline/common/heuristics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/hexdump.py` & `assemblyline-4.5.1.dev8/assemblyline/common/hexdump.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/identify.py` & `assemblyline-4.5.1.dev8/assemblyline/common/identify.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/identify_defaults.py` & `assemblyline-4.5.1.dev8/assemblyline/common/identify_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
     {"al_type": "code/xml", "regex": r"xml"},
     {"al_type": "image/tim", "regex": r"TIM image"},
     {"al_type": "network/sff", "regex": r"Frame Format"},
     {"al_type": "shortcut/windows", "regex": r"^MS Windows shortcut"},
     {"al_type": "document/email", "regex": r"Mime entity text"},
     {"al_type": "document/email", "regex": r"MIME entity, ASCII text"},
     {"al_type": "metadata/sysmon/evt", "regex": r"MS Windows Vista Event Log"},
+    {"al_type": "metadata/minidump", "regex": r"Mini DuMP crash report"},
     {"al_type": "image/emf", "regex": r"Windows Enhanced Metafile"},
     {"al_type": "resource/msvc", "regex": r"MSVC \.res"},
     {"al_type": "pgp/pubkey", "regex": r"^PGP public key"},
     {"al_type": "pgp/privkey", "regex": r"^PGP private key block"},
     {"al_type": "pgp/encrypted", "regex": r"^PGP RSA encrypted session key"},
     {"al_type": "pgp/message", "regex": r"^PGP message Public-Key Encrypted Session Key"},
     {"al_type": "gpg/symmetric", "regex": r"^GPG symmetrically encrypted data"},
```

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/iprange.py` & `assemblyline-4.5.1.dev8/assemblyline/common/iprange.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/isotime.py` & `assemblyline-4.5.1.dev8/assemblyline/common/isotime.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/log.py` & `assemblyline-4.5.1.dev8/assemblyline/common/log.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/logformat.py` & `assemblyline-4.5.1.dev8/assemblyline/common/logformat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/lucene.lark` & `assemblyline-4.5.1.dev8/assemblyline/common/lucene.lark`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/memory_zip.py` & `assemblyline-4.5.1.dev8/assemblyline/common/memory_zip.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/metrics.py` & `assemblyline-4.5.1.dev8/assemblyline/common/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/net.py` & `assemblyline-4.5.1.dev8/assemblyline/common/net.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/net_static.py` & `assemblyline-4.5.1.dev8/assemblyline/common/net_static.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/path.py` & `assemblyline-4.5.1.dev8/assemblyline/common/path.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/postprocess.py` & `assemblyline-4.5.1.dev8/assemblyline/common/postprocess.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/random_user.py` & `assemblyline-4.5.1.dev8/assemblyline/common/random_user.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/security.py` & `assemblyline-4.5.1.dev8/assemblyline/common/security.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/signaturing.py` & `assemblyline-4.5.1.dev8/assemblyline/common/signaturing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/str_utils.py` & `assemblyline-4.5.1.dev8/assemblyline/common/str_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/tag_safelist.yml` & `assemblyline-4.5.1.dev8/assemblyline/common/tag_safelist.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/tagging.py` & `assemblyline-4.5.1.dev8/assemblyline/common/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/threading.py` & `assemblyline-4.5.1.dev8/assemblyline/common/threading.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/common/uid.py` & `assemblyline-4.5.1.dev8/assemblyline/common/uid.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datasource/al.py` & `assemblyline-4.5.1.dev8/assemblyline/datasource/al.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datasource/alert.py` & `assemblyline-4.5.1.dev8/assemblyline/datasource/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datasource/common.py` & `assemblyline-4.5.1.dev8/assemblyline/datasource/common.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datastore/bulk.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/bulk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datastore/collection.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datastore/exceptions.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datastore/helper.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datastore/store.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/store.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datastore/support/build.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/support/build.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/datastore/support/schemas.py` & `assemblyline-4.5.1.dev8/assemblyline/datastore/support/schemas.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/filestore/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/filestore/transport/azure.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/azure.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/filestore/transport/base.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/filestore/transport/ftp.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/ftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/filestore/transport/http.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/http.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/filestore/transport/local.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/local.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/filestore/transport/s3.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/s3.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/filestore/transport/sftp.py` & `assemblyline-4.5.1.dev8/assemblyline/filestore/transport/sftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/base.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/alert.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/alerter_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/alerter_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/archive_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/archive_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/changes.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/changes.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/dispatcher_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/dispatcher_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/dispatching.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/dispatching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/expiry_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/expiry_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/ingest_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/ingest_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/metrics.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/scaler_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/scaler_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/scaler_status_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/scaler_status_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/service_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/service_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/service_timing_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/service_timing_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/submission.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/task.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/task.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/messages/vacuum_heartbeat.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/messages/vacuum_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/actions.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/actions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/alert.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/badlist.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/badlist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/config.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/config.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/error.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/error.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/file.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/file.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/filescore.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/filescore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/heuristic.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/heuristic.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/filetypes/pe.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/filetypes/pe.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/ontology.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/antivirus.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/antivirus.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/malware_config.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/malware_config.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/network.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/network.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/process.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/process.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/sandbox.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/sandbox.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/ontology/results/signature.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/ontology/results/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/replay.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/result.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/result.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/retrohunt.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/retrohunt.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/safelist.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/service.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/service.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/service_delta.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/service_delta.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/signature.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/statistics.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/statistics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/submission.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/submission_summary.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/submission_summary.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/submission_tree.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/submission_tree.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/tagging.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/user.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/user.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/user_favorites.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/user_favorites.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/user_settings.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/user_settings.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/models/workflow.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/models/workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/random_data/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/random_data/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/random_data/create_test_data.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/random_data/create_test_data.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/random_data/sample_rules.yar` & `assemblyline-4.5.1.dev8/assemblyline/odm/random_data/sample_rules.yar`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/random_data/sample_suricata.rules` & `assemblyline-4.5.1.dev8/assemblyline/odm/random_data/sample_suricata.rules`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/odm/randomizer.py` & `assemblyline-4.5.1.dev8/assemblyline/odm/randomizer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/__init__.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/cache.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/cache.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/counters.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/counters.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/events.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/events.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/exporting_counter.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/exporting_counter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/hash.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/hash.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/lock.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/lock.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/comms.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/multi.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/multi.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/named.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/named.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/queues/priority.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/queues/priority.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/set.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/set.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/remote/datatypes/user_quota_tracker.py` & `assemblyline-4.5.1.dev8/assemblyline/remote/datatypes/user_quota_tracker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/run/cli.py` & `assemblyline-4.5.1.dev8/assemblyline/run/cli.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/run/pubsub_reader.py` & `assemblyline-4.5.1.dev8/assemblyline/run/pubsub_reader.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/run/suricata_importer.py` & `assemblyline-4.5.1.dev8/assemblyline/run/suricata_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline/run/yara_importer.py` & `assemblyline-4.5.1.dev8/assemblyline/run/yara_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/assemblyline.egg-info/PKG-INFO` & `assemblyline-4.5.1.dev8/assemblyline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.5.1.dev7
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-4.5.1.dev7/assemblyline.egg-info/SOURCES.txt` & `assemblyline-4.5.1.dev8/assemblyline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev7/setup.py` & `assemblyline-4.5.1.dev8/setup.py`

 * *Files identical despite different names*

