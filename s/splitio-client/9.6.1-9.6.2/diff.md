# Comparing `tmp/splitio_client-9.6.1.tar.gz` & `tmp/splitio_client-9.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splitio_client-9.6.1.tar", last modified: Thu Feb 15 21:51:48 2024, max compression
+gzip compressed data, was "dist/splitio_client-9.6.2.tar", last modified: Fri Apr  5 19:57:31 2024, max compression
```

## Comparing `splitio_client-9.6.1.tar` & `splitio_client-9.6.2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2024-02-15 21:51:48.000000 splitio_client-9.6.1/PKG-INFO
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5240 2024-02-15 21:50:24.000000 splitio_client-9.6.1/README.md
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2024-02-15 21:51:48.000000 splitio_client-9.6.1/setup.cfg
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1737 2024-02-15 21:50:24.000000 splitio_client-9.6.1/setup.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/api/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2430 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/auth.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5170 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4015 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/commons.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2917 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/events.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5179 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2873 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2829 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/splits.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4063 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/api/telemetry.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/client/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    24159 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5405 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/config.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    29723 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/factory.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20321 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/input_validator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/key.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/listener.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/localhost.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3497 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/client/util.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/engine/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/engine/cache/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/cache/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/cache/lru.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7143 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/evaluator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/filters.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/engine/hashfns/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/hashfns/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/hashfns/legacy.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/hashfns/murmur3py.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/engine/impressions/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2928 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/impressions/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7105 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/impressions/adapters.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/impressions/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/impressions/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/impressions/strategies.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3049 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/impressions/unique_keys_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/splitters.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    13487 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/engine/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/exceptions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/factories.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/key.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/models/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/datatypes.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/events.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/models/grammar/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4099 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/condition.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/models/grammar/matchers/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/matchers/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/matchers/base.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/matchers/keys.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/matchers/misc.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/matchers/numeric.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/matchers/sets.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/matchers/string.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/grammar/partitions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/notification.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7964 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/splits.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    36838 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2037 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/models/token.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/push/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9110 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    15365 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/parser.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3241 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/processor.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/segmentworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/splitsse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5601 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/splitworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/sse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/push/status_tracker.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/recorder/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/recorder/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/recorder/recorder.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/storage/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8718 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/storage/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/storage/adapters/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/storage/adapters/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/storage/adapters/cache_trait.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    19144 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/storage/adapters/redis.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/storage/adapters/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    26459 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/storage/inmemmory.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    33160 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/storage/pluggable.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    28191 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/storage/redis.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/sync/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/event.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/impression.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12506 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/segment.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21424 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/split.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    23444 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3254 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2961 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/unique_keys.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/sync/util.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/tasks/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/events_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/impressions_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/segment_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/split_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/telemetry_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/unique_keys_sync.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/tasks/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6142 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/util/asynctask.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/tasks/util/workerpool.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/util/backoff.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/util/decorators.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2457 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/util/storage_helper.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/util/threadutil.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/util/time.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       22 2024-02-15 21:50:24.000000 splitio_client-9.6.1/splitio/version.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio_client.egg-info/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio_client.egg-info/PKG-INFO
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3259 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio_client.egg-info/SOURCES.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio_client.egg-info/dependency_links.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      310 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio_client.egg-info/requires.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        8 2024-02-15 21:51:48.000000 splitio_client-9.6.1/splitio_client.egg-info/top_level.txt
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2024-04-05 19:57:31.000000 splitio_client-9.6.2/PKG-INFO
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5240 2024-04-05 19:55:06.000000 splitio_client-9.6.2/README.md
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2024-04-05 19:57:31.000000 splitio_client-9.6.2/setup.cfg
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1738 2024-04-05 19:55:06.000000 splitio_client-9.6.2/setup.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/api/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2430 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/auth.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5170 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/client.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4015 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/commons.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2917 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/events.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5179 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2873 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/segments.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2829 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/splits.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4063 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/telemetry.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/client/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    24159 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/client.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5405 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/config.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    29723 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/factory.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20321 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/input_validator.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/key.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/listener.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/localhost.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3497 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/util.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/engine/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/engine/cache/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/cache/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/cache/lru.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7143 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/evaluator.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/filters.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/engine/hashfns/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/hashfns/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/hashfns/legacy.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/hashfns/murmur3py.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/engine/impressions/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2928 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7354 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/adapters.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/strategies.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3049 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/unique_keys_tracker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/splitters.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    13487 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/exceptions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/factories.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/key.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/models/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/datatypes.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/events.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/models/grammar/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4099 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/condition.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/base.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/keys.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/misc.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/numeric.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/sets.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/string.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/partitions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/notification.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/segments.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7964 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/splits.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    36838 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2037 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/token.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/push/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9110 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    15365 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/parser.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3241 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/processor.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/segmentworker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/splitsse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5601 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/splitworker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/sse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/status_tracker.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/recorder/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/recorder/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/recorder/recorder.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/storage/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8718 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/storage/adapters/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/adapters/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/adapters/cache_trait.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    19144 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/adapters/redis.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/adapters/util.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    26459 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/inmemmory.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    33160 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/pluggable.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    28191 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/redis.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/sync/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/event.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/impression.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12506 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/segment.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21424 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/split.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    23444 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3254 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2961 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/unique_keys.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/util.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/tasks/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/events_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/impressions_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/segment_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/split_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/telemetry_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/unique_keys_sync.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/tasks/util/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/util/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6142 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/util/asynctask.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/util/workerpool.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/util/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/backoff.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/decorators.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2457 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/storage_helper.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/threadutil.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/time.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       22 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/version.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/PKG-INFO
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3259 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      311 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/requires.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        8 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/top_level.txt
```

### Comparing `splitio_client-9.6.1/PKG-INFO` & `splitio_client-9.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: splitio_client
-Version: 9.6.1
+Version: 9.6.2
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.6.1
+Download-URL: https://github.com/splitio/python-client/tarball/9.6.2
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `splitio_client-9.6.1/README.md` & `splitio_client-9.6.2/README.md`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/setup.py` & `splitio_client-9.6.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from os import path
 from setuptools import setup, find_packages
 
 TESTS_REQUIRES = [
     'flake8',
     'pytest==7.0.1',
-    'pytest-mock>=3.5.1',
+    'pytest-mock==3.12.0',
     'coverage==6.2',
     'pytest-cov',
     'importlib-metadata==4.2',
     'tomli==1.2.3',
     'iniconfig==1.1.1',
     'attrs==22.1.0'
 ]
```

### Comparing `splitio_client-9.6.1/splitio/api/auth.py` & `splitio_client-9.6.2/splitio/api/auth.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/api/client.py` & `splitio_client-9.6.2/splitio/api/client.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/api/commons.py` & `splitio_client-9.6.2/splitio/api/commons.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/api/events.py` & `splitio_client-9.6.2/splitio/api/events.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/api/impressions.py` & `splitio_client-9.6.2/splitio/api/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/api/segments.py` & `splitio_client-9.6.2/splitio/api/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/api/splits.py` & `splitio_client-9.6.2/splitio/api/splits.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/api/telemetry.py` & `splitio_client-9.6.2/splitio/api/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/client.py` & `splitio_client-9.6.2/splitio/client/client.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/config.py` & `splitio_client-9.6.2/splitio/client/config.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/factory.py` & `splitio_client-9.6.2/splitio/client/factory.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/input_validator.py` & `splitio_client-9.6.2/splitio/client/input_validator.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/key.py` & `splitio_client-9.6.2/splitio/client/key.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/listener.py` & `splitio_client-9.6.2/splitio/client/listener.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/localhost.py` & `splitio_client-9.6.2/splitio/client/localhost.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/manager.py` & `splitio_client-9.6.2/splitio/client/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/client/util.py` & `splitio_client-9.6.2/splitio/client/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/cache/lru.py` & `splitio_client-9.6.2/splitio/engine/cache/lru.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/evaluator.py` & `splitio_client-9.6.2/splitio/engine/evaluator.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/filters.py` & `splitio_client-9.6.2/splitio/engine/filters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/hashfns/__init__.py` & `splitio_client-9.6.2/splitio/engine/hashfns/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/hashfns/legacy.py` & `splitio_client-9.6.2/splitio/engine/hashfns/legacy.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/hashfns/murmur3py.py` & `splitio_client-9.6.2/splitio/engine/hashfns/murmur3py.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/impressions/__init__.py` & `splitio_client-9.6.2/splitio/engine/impressions/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/impressions/adapters.py` & `splitio_client-9.6.2/splitio/engine/impressions/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     def record_unique_keys(self, uniques):
         """
         post the unique keys to split back end.
 
         :param uniques: unique keys disctionary
         :type uniques: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
+        if len(uniques) == 0:
+            return
+
         self._telemtry_http_client.record_unique_keys({'keys': self._uniques_formatter(uniques)})
 
     def _uniques_formatter(self, uniques):
         """
         Format the unique keys dictionary array to a JSON body
 
         :param uniques: unique keys disctionary
@@ -69,14 +72,17 @@
     def record_unique_keys(self, uniques):
         """
         post the unique keys to redis.
 
         :param uniques: unique keys disctionary
         :type uniques: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
+        if len(uniques) == 0:
+            return
+
         bulk_mtks = _uniques_formatter(uniques)
         try:
             inserted = self._redis_client.rpush(_MTK_QUEUE_KEY, *bulk_mtks)
             self._expire_keys(_MTK_QUEUE_KEY, _MTK_KEY_DEFAULT_TTL, inserted, len(bulk_mtks))
             return True
         except RedisAdapterException:
             _LOGGER.error('Something went wrong when trying to add mtks to redis')
@@ -86,14 +92,17 @@
     def flush_counters(self, to_send):
         """
         post the impression counters to redis.
 
         :param to_send: unique keys disctionary
         :type to_send: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
+        if len(to_send) == 0:
+            return
+
         try:
             resulted = 0
             counted = 0
             pipe = self._redis_client.pipeline()
             for pf_count in to_send:
                 pipe.hincrby(_IMP_COUNT_QUEUE_KEY, pf_count.feature + "::" + str(pf_count.timeframe), pf_count.count)
                 counted += pf_count.count
@@ -136,14 +145,17 @@
     def record_unique_keys(self, uniques):
         """
         post the unique keys to storage.
 
         :param uniques: unique keys disctionary
         :type uniques: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
+        if len(uniques) == 0:
+            return
+
         bulk_mtks = _uniques_formatter(uniques)
         try:
             _LOGGER.debug("record_unique_keys")
             _LOGGER.debug(uniques)
             inserted = self._adapter_client.push_items(self._prefix + _MTK_QUEUE_KEY, *bulk_mtks)
             self._expire_keys(self._prefix + _MTK_QUEUE_KEY, _MTK_KEY_DEFAULT_TTL, inserted, len(bulk_mtks))
             return True
@@ -155,14 +167,16 @@
     def flush_counters(self, to_send):
         """
         post the impression counters to storage.
 
         :param to_send: unique keys disctionary
         :type to_send: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
+        if len(to_send) == 0:
+            return
         try:
             resulted = 0
             for pf_count in to_send:
                 key = self._prefix + _IMP_COUNT_QUEUE_KEY + "." + pf_count.feature + "::" + str(pf_count.timeframe)
                 resulted = self._adapter_client.increment(key, pf_count.count)
                 self._expire_keys(key, _IMP_COUNT_KEY_DEFAULT_TTL, resulted, pf_count.count)
             return True
```

### Comparing `splitio_client-9.6.1/splitio/engine/impressions/impressions.py` & `splitio_client-9.6.2/splitio/engine/impressions/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/impressions/manager.py` & `splitio_client-9.6.2/splitio/engine/impressions/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/impressions/strategies.py` & `splitio_client-9.6.2/splitio/engine/impressions/strategies.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/impressions/unique_keys_tracker.py` & `splitio_client-9.6.2/splitio/engine/impressions/unique_keys_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/splitters.py` & `splitio_client-9.6.2/splitio/engine/splitters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/engine/telemetry.py` & `splitio_client-9.6.2/splitio/engine/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/datatypes.py` & `splitio_client-9.6.2/splitio/models/datatypes.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/condition.py` & `splitio_client-9.6.2/splitio/models/grammar/condition.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/matchers/__init__.py` & `splitio_client-9.6.2/splitio/models/grammar/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/matchers/base.py` & `splitio_client-9.6.2/splitio/models/grammar/matchers/base.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/matchers/keys.py` & `splitio_client-9.6.2/splitio/models/grammar/matchers/keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/matchers/misc.py` & `splitio_client-9.6.2/splitio/models/grammar/matchers/misc.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/matchers/numeric.py` & `splitio_client-9.6.2/splitio/models/grammar/matchers/numeric.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/matchers/sets.py` & `splitio_client-9.6.2/splitio/models/grammar/matchers/sets.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/matchers/string.py` & `splitio_client-9.6.2/splitio/models/grammar/matchers/string.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/grammar/partitions.py` & `splitio_client-9.6.2/splitio/models/grammar/partitions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/impressions.py` & `splitio_client-9.6.2/splitio/models/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/notification.py` & `splitio_client-9.6.2/splitio/models/notification.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/segments.py` & `splitio_client-9.6.2/splitio/models/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/splits.py` & `splitio_client-9.6.2/splitio/models/splits.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/telemetry.py` & `splitio_client-9.6.2/splitio/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/models/token.py` & `splitio_client-9.6.2/splitio/models/token.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/push/manager.py` & `splitio_client-9.6.2/splitio/push/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/push/parser.py` & `splitio_client-9.6.2/splitio/push/parser.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/push/processor.py` & `splitio_client-9.6.2/splitio/push/processor.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/push/segmentworker.py` & `splitio_client-9.6.2/splitio/push/segmentworker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/push/splitsse.py` & `splitio_client-9.6.2/splitio/push/splitsse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/push/splitworker.py` & `splitio_client-9.6.2/splitio/push/splitworker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/push/sse.py` & `splitio_client-9.6.2/splitio/push/sse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/push/status_tracker.py` & `splitio_client-9.6.2/splitio/push/status_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/recorder/recorder.py` & `splitio_client-9.6.2/splitio/recorder/recorder.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/storage/__init__.py` & `splitio_client-9.6.2/splitio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/storage/adapters/cache_trait.py` & `splitio_client-9.6.2/splitio/storage/adapters/cache_trait.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/storage/adapters/redis.py` & `splitio_client-9.6.2/splitio/storage/adapters/redis.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/storage/adapters/util.py` & `splitio_client-9.6.2/splitio/storage/adapters/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/storage/inmemmory.py` & `splitio_client-9.6.2/splitio/storage/inmemmory.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/storage/pluggable.py` & `splitio_client-9.6.2/splitio/storage/pluggable.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/storage/redis.py` & `splitio_client-9.6.2/splitio/storage/redis.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/event.py` & `splitio_client-9.6.2/splitio/sync/event.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/impression.py` & `splitio_client-9.6.2/splitio/sync/impression.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/manager.py` & `splitio_client-9.6.2/splitio/sync/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/segment.py` & `splitio_client-9.6.2/splitio/sync/segment.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/split.py` & `splitio_client-9.6.2/splitio/sync/split.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/synchronizer.py` & `splitio_client-9.6.2/splitio/sync/synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/telemetry.py` & `splitio_client-9.6.2/splitio/sync/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/unique_keys.py` & `splitio_client-9.6.2/splitio/sync/unique_keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/sync/util.py` & `splitio_client-9.6.2/splitio/sync/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/__init__.py` & `splitio_client-9.6.2/splitio/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/events_sync.py` & `splitio_client-9.6.2/splitio/tasks/events_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/impressions_sync.py` & `splitio_client-9.6.2/splitio/tasks/impressions_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/segment_sync.py` & `splitio_client-9.6.2/splitio/tasks/segment_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/split_sync.py` & `splitio_client-9.6.2/splitio/tasks/split_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/telemetry_sync.py` & `splitio_client-9.6.2/splitio/tasks/telemetry_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/unique_keys_sync.py` & `splitio_client-9.6.2/splitio/tasks/unique_keys_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/util/asynctask.py` & `splitio_client-9.6.2/splitio/tasks/util/asynctask.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/tasks/util/workerpool.py` & `splitio_client-9.6.2/splitio/tasks/util/workerpool.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/util/backoff.py` & `splitio_client-9.6.2/splitio/util/backoff.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/util/storage_helper.py` & `splitio_client-9.6.2/splitio/util/storage_helper.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/util/threadutil.py` & `splitio_client-9.6.2/splitio/util/threadutil.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio/util/time.py` & `splitio_client-9.6.2/splitio/util/time.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.1/splitio_client.egg-info/PKG-INFO` & `splitio_client-9.6.2/splitio_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: splitio-client
-Version: 9.6.1
+Version: 9.6.2
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.6.1
+Download-URL: https://github.com/splitio/python-client/tarball/9.6.2
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `splitio_client-9.6.1/splitio_client.egg-info/SOURCES.txt` & `splitio_client-9.6.2/splitio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

