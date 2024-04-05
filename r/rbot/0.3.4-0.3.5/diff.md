# Comparing `tmp/rbot-0.3.4.tar.gz` & `tmp/rbot-0.3.5.tar.gz`

## Comparing `rbot-0.3.4.tar` & `rbot-0.3.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 rbot-0.3.4/local_dependencies/rbot_blockon/Cargo.toml
--rw-r--r--   0      501       20      767 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_blockon/src/lib.rs
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 rbot-0.3.4/local_dependencies/rbot_server/Cargo.toml
--rw-r--r--   0      501       20       33 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_server/src/lib.rs
--rw-r--r--   0      501       20     2825 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_server/src/server.rs
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 rbot-0.3.4/local_dependencies/bybit/Cargo.toml
--rw-r--r--   0      501       20     4764 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/bybit/src/config.rs
--rw-r--r--   0      501       20       95 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/bybit/src/lib.rs
--rw-r--r--   0      501       20    23812 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/bybit/src/market.rs
--rw-r--r--   0      501       20    76796 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/bybit/src/message.rs
--rw-r--r--   0      501       20    23741 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/bybit/src/rest.rs
--rw-r--r--   0      501       20    13993 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/bybit/src/ws.rs
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 rbot-0.3.4/local_dependencies/rbot_market/Cargo.toml
--rw-r--r--   0      501       20       33 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_market/src/lib.rs
--rw-r--r--   0      501       20    22336 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_market/src/market.rs
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 rbot-0.3.4/local_dependencies/rbot_session/Cargo.toml
--rw-r--r--   0      501       20      200 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_session/src/lib.rs
--rw-r--r--   0      501       20    32196 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_session/src/logger.rs
--rw-r--r--   0      501       20     6612 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_session/src/mod_test.rs
--rw-r--r--   0      501       20     7671 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_session/src/orderlist.rs
--rw-r--r--   0      501       20     2856 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_session/src/orderlist.test.rs
--rw-r--r--   0      501       20      337 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_session/src/python_if.rs
--rw-r--r--   0      501       20    31941 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_session/src/runner.rs
--rw-r--r--   0      501       20    42145 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_session/src/session.rs
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 rbot-0.3.4/local_dependencies/binance/Cargo.toml
--rw-r--r--   0      501       20     3410 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/binance/src/config.rs
--rw-r--r--   0      501       20      150 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/binance/src/lib.rs
--rw-r--r--   0      501       20    24921 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/binance/src/market.rs
--rw-r--r--   0      501       20    45249 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/binance/src/message.rs
--rw-r--r--   0      501       20    18660 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/binance/src/rest.rs
--rw-r--r--   0      501       20    11070 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/binance/src/ws.rs
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 rbot-0.3.4/local_dependencies/rbot_lib/Cargo.toml
--rw-r--r--   0      501       20     8046 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/ch.rs
--rw-r--r--   0      501       20     4905 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/config.rs
--rw-r--r--   0      501       20     1268 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/env.rs
--rw-r--r--   0      501       20    10601 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/hub.rs
--rw-r--r--   0      501       20     2143 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/logger.rs
--rw-r--r--   0      501       20      385 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/mod.rs
--rw-r--r--   0      501       20    45435 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/order.rs
--rw-r--r--   0      501       20    19640 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/orderbook.rs
--rw-r--r--   0      501       20     5311 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/time.rs
--rw-r--r--   0      501       20     3848 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/common/util.rs
--rw-r--r--   0      501       20    24315 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/db/df.rs
--rw-r--r--   0      501       20     1929 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/db/fs.rs
--rw-r--r--   0      501       20      132 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/db/mod.rs
--rw-r--r--   0      501       20      105 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/db/polars_test.rs
--rw-r--r--   0      501       20    58746 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/db/sqlite.rs
--rw-r--r--   0      501       20       42 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/lib.rs
--rw-r--r--   0      501       20       98 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/net/mod.rs
--rw-r--r--   0      501       20    22252 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/net/rest.rs
--rw-r--r--   0      501       20    11478 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/net/udp.rs
--rw-r--r--   0      501       20    34626 2024-04-04 14:50:54.000000 rbot-0.3.4/local_dependencies/rbot_lib/src/net/ws.rs
--rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 rbot-0.3.4/Cargo.toml
--rw-r--r--   0      501       20     7652 2024-04-04 14:50:54.000000 rbot-0.3.4/LICENSE.txt
--rw-r--r--   0      501       20     9473 2024-04-04 14:50:54.000000 rbot-0.3.4/README.md
--rw-r--r--   0      501       20      119 2024-04-04 14:50:54.000000 rbot-0.3.4/copyright.txt
--rw-r--r--   0      501       20      605 2024-04-04 14:50:54.000000 rbot-0.3.4/pyproject.toml
--rw-r--r--   0      501       20      600 2024-04-04 14:50:54.000000 rbot-0.3.4/python/rbot/__init__.py
--rw-r--r--   0      501       20       54 2024-04-04 14:50:54.000000 rbot-0.3.4/requirements.txt
--rw-r--r--   0      501       20     2373 2024-04-04 14:50:54.000000 rbot-0.3.4/src/lib.rs
--rw-r--r--   0        0        0     9979 1970-01-01 00:00:00.000000 rbot-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 rbot-0.3.5/local_dependencies/rbot_server/Cargo.toml
+-rw-r--r--   0      501       20       33 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_server/src/lib.rs
+-rw-r--r--   0      501       20     2825 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_server/src/server.rs
+-rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 rbot-0.3.5/local_dependencies/rbot_blockon/Cargo.toml
+-rw-r--r--   0      501       20      767 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_blockon/src/lib.rs
+-rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 rbot-0.3.5/local_dependencies/rbot_session/Cargo.toml
+-rw-r--r--   0      501       20      200 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_session/src/lib.rs
+-rw-r--r--   0      501       20    32196 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_session/src/logger.rs
+-rw-r--r--   0      501       20     6612 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_session/src/mod_test.rs
+-rw-r--r--   0      501       20     7671 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_session/src/orderlist.rs
+-rw-r--r--   0      501       20     2856 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_session/src/orderlist.test.rs
+-rw-r--r--   0      501       20      337 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_session/src/python_if.rs
+-rw-r--r--   0      501       20    31941 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_session/src/runner.rs
+-rw-r--r--   0      501       20    42145 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_session/src/session.rs
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 rbot-0.3.5/local_dependencies/bybit/Cargo.toml
+-rw-r--r--   0      501       20     4764 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/bybit/src/config.rs
+-rw-r--r--   0      501       20       95 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/bybit/src/lib.rs
+-rw-r--r--   0      501       20    23812 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/bybit/src/market.rs
+-rw-r--r--   0      501       20    76796 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/bybit/src/message.rs
+-rw-r--r--   0      501       20    23741 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/bybit/src/rest.rs
+-rw-r--r--   0      501       20    13993 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/bybit/src/ws.rs
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 rbot-0.3.5/local_dependencies/rbot_market/Cargo.toml
+-rw-r--r--   0      501       20       33 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_market/src/lib.rs
+-rw-r--r--   0      501       20    22336 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_market/src/market.rs
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 rbot-0.3.5/local_dependencies/binance/Cargo.toml
+-rw-r--r--   0      501       20     3410 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/binance/src/config.rs
+-rw-r--r--   0      501       20      150 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/binance/src/lib.rs
+-rw-r--r--   0      501       20    24921 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/binance/src/market.rs
+-rw-r--r--   0      501       20    45249 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/binance/src/message.rs
+-rw-r--r--   0      501       20    18660 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/binance/src/rest.rs
+-rw-r--r--   0      501       20    11070 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/binance/src/ws.rs
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 rbot-0.3.5/local_dependencies/rbot_lib/Cargo.toml
+-rw-r--r--   0      501       20     8046 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/ch.rs
+-rw-r--r--   0      501       20     4905 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/config.rs
+-rw-r--r--   0      501       20     1268 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/env.rs
+-rw-r--r--   0      501       20    10601 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/hub.rs
+-rw-r--r--   0      501       20     2143 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/logger.rs
+-rw-r--r--   0      501       20      385 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/mod.rs
+-rw-r--r--   0      501       20    45435 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/order.rs
+-rw-r--r--   0      501       20    19640 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/orderbook.rs
+-rw-r--r--   0      501       20     5311 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/time.rs
+-rw-r--r--   0      501       20     3848 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/common/util.rs
+-rw-r--r--   0      501       20    24315 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/db/df.rs
+-rw-r--r--   0      501       20     1929 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/db/fs.rs
+-rw-r--r--   0      501       20      132 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/db/mod.rs
+-rw-r--r--   0      501       20      105 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/db/polars_test.rs
+-rw-r--r--   0      501       20    58746 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/db/sqlite.rs
+-rw-r--r--   0      501       20       42 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/lib.rs
+-rw-r--r--   0      501       20       98 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/net/mod.rs
+-rw-r--r--   0      501       20    22252 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/net/rest.rs
+-rw-r--r--   0      501       20    11478 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/net/udp.rs
+-rw-r--r--   0      501       20    34626 2024-04-05 03:55:51.000000 rbot-0.3.5/local_dependencies/rbot_lib/src/net/ws.rs
+-rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 rbot-0.3.5/Cargo.toml
+-rw-r--r--   0      501       20     7652 2024-04-05 03:55:51.000000 rbot-0.3.5/LICENSE.txt
+-rw-r--r--   0      501       20     9584 2024-04-05 03:55:51.000000 rbot-0.3.5/README.md
+-rw-r--r--   0      501       20      119 2024-04-05 03:55:51.000000 rbot-0.3.5/copyright.txt
+-rw-r--r--   0      501       20      841 2024-04-05 03:55:51.000000 rbot-0.3.5/pyproject.toml
+-rw-r--r--   0      501       20      600 2024-04-05 03:55:51.000000 rbot-0.3.5/python/rbot/__init__.py
+-rw-r--r--   0      501       20       54 2024-04-05 03:55:51.000000 rbot-0.3.5/requirements.txt
+-rw-r--r--   0      501       20     2373 2024-04-05 03:55:51.000000 rbot-0.3.5/src/lib.rs
+-rw-r--r--   0        0        0    10288 1970-01-01 00:00:00.000000 rbot-0.3.5/PKG-INFO
```

### Comparing `rbot-0.3.4/local_dependencies/rbot_blockon/src/lib.rs` & `rbot-0.3.5/local_dependencies/rbot_blockon/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_server/src/server.rs` & `rbot-0.3.5/local_dependencies/rbot_server/src/server.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/bybit/Cargo.toml` & `rbot-0.3.5/local_dependencies/bybit/Cargo.toml`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/bybit/src/config.rs` & `rbot-0.3.5/local_dependencies/bybit/src/config.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/bybit/src/market.rs` & `rbot-0.3.5/local_dependencies/bybit/src/market.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/bybit/src/message.rs` & `rbot-0.3.5/local_dependencies/bybit/src/message.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/bybit/src/rest.rs` & `rbot-0.3.5/local_dependencies/bybit/src/rest.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/bybit/src/ws.rs` & `rbot-0.3.5/local_dependencies/bybit/src/ws.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_market/Cargo.toml` & `rbot-0.3.5/local_dependencies/rbot_market/Cargo.toml`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_market/src/market.rs` & `rbot-0.3.5/local_dependencies/rbot_market/src/market.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_session/Cargo.toml` & `rbot-0.3.5/local_dependencies/rbot_session/Cargo.toml`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_session/src/logger.rs` & `rbot-0.3.5/local_dependencies/rbot_session/src/logger.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_session/src/mod_test.rs` & `rbot-0.3.5/local_dependencies/rbot_session/src/mod_test.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_session/src/orderlist.rs` & `rbot-0.3.5/local_dependencies/rbot_session/src/orderlist.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_session/src/orderlist.test.rs` & `rbot-0.3.5/local_dependencies/rbot_session/src/orderlist.test.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_session/src/runner.rs` & `rbot-0.3.5/local_dependencies/rbot_session/src/runner.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_session/src/session.rs` & `rbot-0.3.5/local_dependencies/rbot_session/src/session.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/binance/Cargo.toml` & `rbot-0.3.5/local_dependencies/binance/Cargo.toml`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/binance/src/config.rs` & `rbot-0.3.5/local_dependencies/binance/src/config.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/binance/src/market.rs` & `rbot-0.3.5/local_dependencies/binance/src/market.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/binance/src/message.rs` & `rbot-0.3.5/local_dependencies/binance/src/message.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/binance/src/rest.rs` & `rbot-0.3.5/local_dependencies/binance/src/rest.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/binance/src/ws.rs` & `rbot-0.3.5/local_dependencies/binance/src/ws.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/Cargo.toml` & `rbot-0.3.5/local_dependencies/rbot_lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/ch.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/ch.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/config.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/config.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/env.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/env.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/hub.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/hub.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/logger.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/logger.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/order.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/order.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/orderbook.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/orderbook.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/time.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/time.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/common/util.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/common/util.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/db/df.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/db/df.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/db/fs.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/db/fs.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/db/sqlite.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/db/sqlite.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/net/rest.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/net/rest.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/net/udp.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/net/udp.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/local_dependencies/rbot_lib/src/net/ws.rs` & `rbot-0.3.5/local_dependencies/rbot_lib/src/net/ws.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/Cargo.toml` & `rbot-0.3.5/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rbot"
-version = "0.3.4"
+version = "0.3.5"
 edition = "2021"
 exclude = ["test/**"]
 
 [lib]
 name = "rbot"
 crate-type = ["cdylib", "rlib"]
```

### Comparing `rbot-0.3.4/LICENSE.txt` & `rbot-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/README.md` & `rbot-0.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 ohlcv = market.ohlcv(
     start_time=0,           # start time in unix timestamp(microseconds)
     end_time=0,             # end time in unix timestamp(microseconds)
     window_sec=60           # ohlc bar window size in seconds
 )
 ```
 The OHLCV data is a polars data frames with the following columns:
-* timestamp
+* timestamp (in asc order)
 * open
 * high
 * low
 * close
 * volume (sum of volume in order size)
 * count (number of ticks)
 
@@ -149,28 +149,39 @@
 
 ### Session API
 In your `on_init`, `on_tick`, `on_clock`, and `on_update`, you can use `session` object to get market information, place order, cancel order, etc.
 
 #### OHLCV data
 ```python
 ohlcv = session.ohlcv(
-    start_time=0,           # start time in unix timestamp(microseconds)
-    end_time=0,             # end time in unix timestamp(microseconds)
-    window_sec=60           # ohlc bar window size in seconds
+    interval=60,        # ohlc bar window size in seconds
+    count=10,           # number of bars to generate
 )
 ```
+
+The OHLCV data is a polars data frames with the following columns:
+* timestamp (in asc order)
+* open
+* high
+* low
+* close
+* volume (sum of volume in order size)
+* count (number of ticks)
+
+
 ### order book
 ```python
 bid, ask = session.board
 ```
 `bid`, `ask` are polars dataframes with the following columns:
 * price: price of the order
 * size: size of the order
 * sum: cumulative size of the order
 
+
 ### place order
 #### market order
 ```python
 size = 0.001
 market_order = session.market_order("BUY", size)
 ```
```

### Comparing `rbot-0.3.4/python/rbot/__init__.py` & `rbot-0.3.5/python/rbot/__init__.py`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/src/lib.rs` & `rbot-0.3.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rbot-0.3.4/PKG-INFO` & `rbot-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: rbot
-Version: 0.3.4
+Version: 0.3.5
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 License-File: LICENSE.txt
+Summary: crypt trading framework, support back_test, dry_run and real_run
 Author: @yasstake
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Documentation, https://github.com/yasstake/rusty-bot
+Project-URL: Repository, https://github.com/yasstake/rbot
 
 # rbot (Rusty bot framwrok for crypto trading)
 
 `rbot` is a python crypt trading bot framework written in Rust.
 
 The feature is;
 * Store historical transaction data(tick) in sqlite database.
@@ -91,15 +94,15 @@
 ohlcv = market.ohlcv(
     start_time=0,           # start time in unix timestamp(microseconds)
     end_time=0,             # end time in unix timestamp(microseconds)
     window_sec=60           # ohlc bar window size in seconds
 )
 ```
 The OHLCV data is a polars data frames with the following columns:
-* timestamp
+* timestamp (in asc order)
 * open
 * high
 * low
 * close
 * volume (sum of volume in order size)
 * count (number of ticks)
 
@@ -162,28 +165,39 @@
 
 ### Session API
 In your `on_init`, `on_tick`, `on_clock`, and `on_update`, you can use `session` object to get market information, place order, cancel order, etc.
 
 #### OHLCV data
 ```python
 ohlcv = session.ohlcv(
-    start_time=0,           # start time in unix timestamp(microseconds)
-    end_time=0,             # end time in unix timestamp(microseconds)
-    window_sec=60           # ohlc bar window size in seconds
+    interval=60,        # ohlc bar window size in seconds
+    count=10,           # number of bars to generate
 )
 ```
+
+The OHLCV data is a polars data frames with the following columns:
+* timestamp (in asc order)
+* open
+* high
+* low
+* close
+* volume (sum of volume in order size)
+* count (number of ticks)
+
+
 ### order book
 ```python
 bid, ask = session.board
 ```
 `bid`, `ask` are polars dataframes with the following columns:
 * price: price of the order
 * size: size of the order
 * sum: cumulative size of the order
 
+
 ### place order
 #### market order
 ```python
 size = 0.001
 market_order = session.market_order("BUY", size)
 ```
```

