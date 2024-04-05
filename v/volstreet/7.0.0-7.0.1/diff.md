# Comparing `tmp/volstreet-7.0.0.tar.gz` & `tmp/volstreet-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.0.0.tar", last modified: Fri Apr  5 03:06:03 2024, max compression
+gzip compressed data, was "volstreet-7.0.1.tar", last modified: Fri Apr  5 04:38:41 2024, max compression
```

## Comparing `volstreet-7.0.0.tar` & `volstreet-7.0.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.474074 volstreet-7.0.0/
--rw-rw-rw-   0        0        0     1260 2024-04-05 03:06:03.474074 volstreet-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.0.0/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1085 2024-04-05 03:06:03.474074 volstreet-7.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.395563 volstreet-7.0.0/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.0.0/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.411185 volstreet-7.0.0/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.0.0/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.0.0/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.0.0/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    13897 2024-04-03 08:06:51.000000 volstreet-7.0.0/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     3534 2024-03-27 14:07:30.000000 volstreet-7.0.0/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.0.0/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.0.0/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.433311 volstreet-7.0.0/volstreet/backtests/
--rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/backtests/data_handling.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.0.0/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    47182 2024-03-26 10:23:44.000000 volstreet-7.0.0/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.0.0/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.0.0/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    18739 2024-03-14 09:00:56.000000 volstreet-7.0.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6034 2024-03-14 09:55:23.000000 volstreet-7.0.0/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.442821 volstreet-7.0.0/volstreet/datamodule/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.0.0/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.0.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.0.0/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.442821 volstreet-7.0.0/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     2090 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.442821 volstreet-7.0.0/volstreet/strategies/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0     5684 2024-04-03 08:06:51.000000 volstreet-7.0.0/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    28833 2024-04-04 11:05:16.000000 volstreet-7.0.0/volstreet/strategies/execution.py
--rw-rw-rw-   0        0        0    58696 2024-04-04 15:28:05.000000 volstreet-7.0.0/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     9310 2024-04-05 02:48:44.000000 volstreet-7.0.0/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    85340 2024-04-04 15:24:09.000000 volstreet-7.0.0/volstreet/strategies/strats.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.458451 volstreet-7.0.0/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.0.0/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26065 2024-04-04 11:05:16.000000 volstreet-7.0.0/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0     9793 2024-04-05 02:44:31.000000 volstreet-7.0.0/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    12025 2024-04-04 15:02:10.000000 volstreet-7.0.0/volstreet/trade_interface/order_placement.py
--rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.0.0/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.458451 volstreet-7.0.0/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     2963 2024-04-05 02:45:53.000000 volstreet-7.0.0/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.0.0/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.0.0/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.474074 volstreet-7.0.0/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.0.0/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.0.0/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.0.0/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.0.0/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.0.0/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:06:03.474074 volstreet-7.0.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1260 2024-04-05 03:06:03.000000 volstreet-7.0.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2374 2024-04-05 03:06:03.000000 volstreet-7.0.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:06:03.000000 volstreet-7.0.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      443 2024-04-05 03:06:03.000000 volstreet-7.0.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 03:06:03.000000 volstreet-7.0.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:41.011581 volstreet-7.0.1/
+-rw-rw-rw-   0        0        0     1260 2024-04-05 04:38:41.011581 volstreet-7.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.0.1/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1085 2024-04-05 04:38:41.012796 volstreet-7.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:40.923216 volstreet-7.0.1/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.0.1/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:40.944149 volstreet-7.0.1/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.0.1/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.0.1/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.0.1/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    13897 2024-04-03 08:06:51.000000 volstreet-7.0.1/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     3534 2024-03-27 14:07:30.000000 volstreet-7.0.1/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.0.1/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.0.1/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:40.963297 volstreet-7.0.1/volstreet/backtests/
+-rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/backtests/data_handling.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.0.1/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    47182 2024-03-26 10:23:44.000000 volstreet-7.0.1/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.0.1/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.0.1/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    18739 2024-03-14 09:00:56.000000 volstreet-7.0.1/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     6034 2024-03-14 09:55:23.000000 volstreet-7.0.1/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:40.976252 volstreet-7.0.1/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.0.1/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.0.1/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.0.1/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:40.977249 volstreet-7.0.1/volstreet/historical_info/
+-rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     2090 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:40.988394 volstreet-7.0.1/volstreet/strategies/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5684 2024-04-03 08:06:51.000000 volstreet-7.0.1/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    28833 2024-04-04 11:05:16.000000 volstreet-7.0.1/volstreet/strategies/execution.py
+-rw-rw-rw-   0        0        0    58696 2024-04-04 15:28:05.000000 volstreet-7.0.1/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     9310 2024-04-05 02:48:44.000000 volstreet-7.0.1/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    89782 2024-04-05 04:35:38.000000 volstreet-7.0.1/volstreet/strategies/strats.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:40.995466 volstreet-7.0.1/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.0.1/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26065 2024-04-04 11:05:16.000000 volstreet-7.0.1/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0     9793 2024-04-05 02:44:31.000000 volstreet-7.0.1/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    12025 2024-04-04 15:02:10.000000 volstreet-7.0.1/volstreet/trade_interface/order_placement.py
+-rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.0.1/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:41.003270 volstreet-7.0.1/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     2963 2024-04-05 02:45:53.000000 volstreet-7.0.1/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.0.1/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.0.1/volstreet/vectorized_blackscholes.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:41.009530 volstreet-7.0.1/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.0.1/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.0.1/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.0.1/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.0.1/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.0.1/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:38:41.010580 volstreet-7.0.1/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1260 2024-04-05 04:38:40.000000 volstreet-7.0.1/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2374 2024-04-05 04:38:40.000000 volstreet-7.0.1/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 04:38:40.000000 volstreet-7.0.1/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      443 2024-04-05 04:38:40.000000 volstreet-7.0.1/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 04:38:40.000000 volstreet-7.0.1/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.0.0/PKG-INFO` & `volstreet-7.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.0.0
+Version: 7.0.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.0.0/setup.cfg` & `volstreet-7.0.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 302e 300d 0a61  rsion = 7.0.0..a
+00000020: 7273 696f 6e20 3d20 372e 302e 310d 0a61  rsion = 7.0.1..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-7.0.0/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-7.0.1/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/angel_interface/async_interface.py` & `volstreet-7.0.1/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/angel_interface/base_websocket.py` & `volstreet-7.0.1/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/angel_interface/interface.py` & `volstreet-7.0.1/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/angel_interface/login.py` & `volstreet-7.0.1/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/angel_interface/order_websocket.py` & `volstreet-7.0.1/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/angel_interface/price_websocket.py` & `volstreet-7.0.1/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/angel_interface/smart_connect.py` & `volstreet-7.0.1/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/data_handling.py` & `volstreet-7.0.1/volstreet/backtests/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/database.py` & `volstreet-7.0.1/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/delta_hedging.py` & `volstreet-7.0.1/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/delta_optimizer.py` & `volstreet-7.0.1/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/framework.py` & `volstreet-7.0.1/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-7.0.1/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/tools.py` & `volstreet-7.0.1/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/trend.py` & `volstreet-7.0.1/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/backtests/underlying_info.py` & `volstreet-7.0.1/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/blackscholes.py` & `volstreet-7.0.1/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/config.py` & `volstreet-7.0.1/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/database_connection.py` & `volstreet-7.0.1/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/datamodule/analysis.py` & `volstreet-7.0.1/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/datamodule/archive.py` & `volstreet-7.0.1/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/datamodule/eod_client.py` & `volstreet-7.0.1/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/datamodule/gambling.py` & `volstreet-7.0.1/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/datamodule/intraday_data.py` & `volstreet-7.0.1/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/datamodule/stockmock.py` & `volstreet-7.0.1/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/datamodule/trading_assistance.py` & `volstreet-7.0.1/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/dealingroom.py` & `volstreet-7.0.1/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/decorators.py` & `volstreet-7.0.1/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/discord_bot.py` & `volstreet-7.0.1/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/exceptions.py` & `volstreet-7.0.1/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/historical_info/index_expiries.pkl` & `volstreet-7.0.1/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/parallelization.py` & `volstreet-7.0.1/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/performance_tracking.py` & `volstreet-7.0.1/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/strategies/error_handling.py` & `volstreet-7.0.1/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/strategies/execution.py` & `volstreet-7.0.1/volstreet/strategies/execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/strategies/helpers.py` & `volstreet-7.0.1/volstreet/strategies/helpers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/strategies/optimization.py` & `volstreet-7.0.1/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/strategies/strats.py` & `volstreet-7.0.1/volstreet/strategies/strats.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,143 +41,246 @@
 from volstreet.strategies.helpers import (
     sleep_until_next_action,
     round_shares_to_lot_size,
     most_equal_strangle,
     DeltaPosition,
     PositionMonitor,
     load_current_straddle,
-    most_even_delta_strangle,
-    is_in_final_stage,
-    check_for_universal_exit,
     approve_execution,
-    check_for_move,
-    identify_new_option,
-    check_for_overlap,
-    move_one_leg,
     notify_pnl,
     process_stop_loss_order_statuses,
 )
 from volstreet.strategies.error_handling import exit_on_error
 
 
-@exit_on_error
-def delta_hedged_strangle_lite(
+def quick_strangle_loop(
     underlying: Index | Stock,
-    exposure: int | float,
-    target_delta: float = 0.25,
-    sl_pct: float = 0.25,
-    end_time: tuple = (15, 00),
-    itm_steps_allowed: int = 2,
-    final_sl_pct: float = 0.4,
-    strategy_tag: str = "Equal delta strangle",
-    notification_url: str = None,
+    action: str,
+    iv_threshold: float,
+    take_profit: float,
+    scan_exit_time: tuple[int, int],
+    exposure: int | float = 0,
+    investment: int | float = 0,
+    stop_loss: Optional[float] = None,
+    trade_exit_time: tuple[int, int] | None = None,
+    max_counter: int = 1,
+    notification_url: Optional[str] = None,
+    strategy_tag: Optional[str] = "Quick Strangle",
 ):
-    """Strangle with stoploss based delta hedging"""
 
-    quantity_in_lots = convert_exposure_to_lots(
-        exposure, underlying.fetch_ltp(), underlying.lot_size
-    )
+    if not exposure and not investment:
+        raise ValueError("Exposure or investment must be provided")
 
-    logger.info(
-        f"{underlying.name} Starting delta hedged strangle with params: {locals()}"
-    )
-    target_strangle = None
-    while target_strangle is None and current_time().time() < time(15, 25):
-        target_strangle, _ = most_even_delta_strangle(
-            underlying, delta_range=(target_delta - 0.05, target_delta + 0.05)
+    if trade_exit_time is None:
+        trade_exit_time: datetime = datetime.combine(
+            current_time().date(), time(*scan_exit_time)
+        ) + timedelta(
+            minutes=15
+        )  # Hard coded 15 minutes past scan exit
+    else:
+        trade_exit_time: datetime = datetime.combine(
+            current_time().date(), time(*trade_exit_time)
         )
-        sleep(1)
-    if target_strangle is None:
+
+    # Entering the main function
+    if time(*scan_exit_time) < current_time().time():
         notifier(
-            f"{underlying.name} Could not find strangle with delta {target_delta}. Exiting.",
+            f"{underlying.name} {strategy_tag} not being deployed after exit time",
             notification_url,
+            "INFO",
         )
         return
 
-    notifier(
-        f"{underlying.name} Target strangle: {target_strangle}",
-        notification_url,
-    )
-    current_call_avg, current_put_avg = place_option_order_and_notify(
-        target_strangle,
-        "SELL",
-        quantity_in_lots,
-        "LIMIT",
-        order_tag=strategy_tag,
-        webhook_url=notification_url,
-        return_avg_price=True,
-    )
-    while current_time().time() < time(*end_time):
-        final_stage = is_in_final_stage(underlying, target_strangle, itm_steps_allowed)
-        universal_exit = check_for_universal_exit(
-            target_strangle,
-            current_call_avg,
-            current_put_avg,
-            final_sl_pct,
-            final_stage,
+    def entry_condition_triggered() -> bool | tuple[Strangle, float, float]:
+        nonlocal ivs, action, iv_threshold, strategy_tag, position
+
+        if action == Action.BUY:
+            strangle = min(ivs, key=ivs.get)
+        else:
+            strangle = max(ivs, key=ivs.get)
+        iv = ivs[strangle]
+        # noinspection PyTypeChecker
+        total_price = np.sum(strangle.fetch_ltp(for_type=action.value))
+        logger.info(
+            f"{underlying.name} {strategy_tag} IV is {iv} for {strangle} "
+            f"with total price {total_price}"
         )
-        if universal_exit:
-            notifier(
-                f"{underlying.name} Universal exit triggered. Exiting.",
-                notification_url,
-            )
-            break
-        sl_pct = final_sl_pct if final_stage else sl_pct
-        option_to_move = check_for_move(
-            target_strangle, current_call_avg, current_put_avg, sl_pct
+        condition = iv <= iv_threshold if action == Action.BUY else iv >= iv_threshold
+
+        if condition:
+            position.position_active = True
+            position.instrument = strangle
+            position.initiating_price = total_price
+            return True
+        else:
+            return False
+
+    def profit_condition() -> bool:
+        nonlocal action, total_current_price, position
+
+        if action == Action.BUY:
+            return total_current_price >= position.profit_threshold
+        else:
+            return total_current_price <= position.profit_threshold
+
+    def stop_loss_condition() -> bool:
+        nonlocal action, total_current_price, position
+
+        if action == Action.BUY:
+            return total_current_price <= position.stop_loss_threshold
+        else:
+            return total_current_price >= position.stop_loss_threshold
+
+    def exit_position():
+        nonlocal action, position, strategy_tag, notification_url, quantity_in_lots
+
+        exec_deets = execute_instructions(
+            {
+                position.instrument: {
+                    "action": ~action,
+                    "quantity_in_lots": quantity_in_lots,
+                    "order_tag": strategy_tag,
+                }
+            }
         )
-        if option_to_move:
-            notifier(
-                f"{underlying.name} move detected. Need to move {option_to_move.option_type}. ",
-                notification_url,
-            )
-            new_option = identify_new_option(
-                underlying, target_strangle, option_to_move
-            )
-            overlap = check_for_overlap(
-                underlying, new_option, target_strangle, itm_steps_allowed
-            )
-            if overlap:
+        call_exit_price, put_exit_price = exec_deets[position.instrument]
+        exit_price = call_exit_price + put_exit_price
+        profit_points = (exit_price - position.initiating_price) * action.num_value
+        notifier(
+            f"Exited {underlying.name} {strategy_tag} "
+            f"with profit points {profit_points}",
+            notification_url,
+            "CRUCIAL",
+        )
+        position.position_active = False
+
+    strategy_tag = f"{strategy_tag} {action.upper()}"
+    action = Action(action)
+    expiry = underlying.current_expiry
+
+    if stop_loss is None:
+        stop_loss = np.nan
+
+    position = PositionMonitor(underlying)
+
+    while (
+        current_time().time() < time(*scan_exit_time) and position.counter < max_counter
+    ) or position.position_active:
+        if not position.position_active:
+            spot = underlying.fetch_ltp()
+            basis = underlying.get_basis_for_expiry(
+                expiry=expiry, underlying_price=spot
+            )
+            above_strike = find_strike(spot + underlying.base, underlying.base)
+            below_strike = find_strike(spot - underlying.base, underlying.base)
+            above_strangle = Strangle(
+                above_strike, above_strike, underlying.name, expiry
+            )
+            below_strangle = Strangle(
+                below_strike, below_strike, underlying.name, expiry
+            )
+            above_strangle_prices = above_strangle.fetch_ltp(for_type=action.value)
+            below_strangle_price = below_strangle.fetch_ltp(for_type=action.value)
+
+            ivs = {
+                above_strangle: np.mean(
+                    above_strangle.fetch_ivs(
+                        spot=spot, r=basis, prices=above_strangle_prices
+                    )
+                ),
+                below_strangle: np.mean(
+                    below_strangle.fetch_ivs(
+                        spot=spot, r=basis, prices=below_strangle_price
+                    )
+                ),
+            }
+
+            if entry_condition_triggered():  # Enter position
+
+                if exposure != 0:
+                    quantity_in_lots = convert_exposure_to_lots(
+                        exposure, underlying.fetch_ltp(), underlying.lot_size
+                    )
+                elif investment != 0:
+                    # Calculation of quantity
+                    shares_to_buy = investment / position.initiating_price
+                    shares_to_buy = round_shares_to_lot_size(
+                        shares_to_buy, underlying.lot_size
+                    )
+                    quantity_in_lots = shares_to_buy / underlying.lot_size
+                else:
+                    raise ValueError("Exposure or investment must be provided")
+
+                # Increase the counter and add it to the strategy tag
+                position.counter += 1
+                strategy_tag = f"{strategy_tag} {position.counter}"
+
+                # Execute the trade
+                execution_details = execute_instructions(
+                    {
+                        position.instrument: {
+                            "action": action,
+                            "quantity_in_lots": quantity_in_lots,
+                            "order_tag": strategy_tag,
+                        }
+                    }
+                )
+                call_avg_price, put_avg_price = execution_details[position.instrument]
+
+                # Set the profit and stop loss thresholds
+                position.profit_threshold = position.initiating_price * (
+                    1 + (take_profit * action.num_value)
+                )
+                position.stop_loss_threshold = position.initiating_price * (
+                    1 - (stop_loss * action.num_value)
+                )
+
+                position.initiating_price = call_avg_price + put_avg_price
+
+                # CRUCIAL FOR CONTROL FLOW: Set the position as active
+                position.position_active = True
+
                 notifier(
-                    f"{underlying.name} max modifications reached. Exiting.",
+                    f"Entered {underlying.name} {strategy_tag} on {position.instrument}. "
+                    f"Avg price {call_avg_price + put_avg_price} "
+                    f"and IV {ivs[position.instrument]}. Profit trigger: "
+                    f"{position.profit_threshold} and stop trigger: "
+                    f"{position.stop_loss_threshold}",
                     notification_url,
+                    "CRUCIAL",
                 )
-                break
-            notifier(
-                f"{underlying.name} {strategy_tag} Moving {option_to_move} to {new_option}",
-                notification_url,
-            )
-            target_strangle, avg_price = move_one_leg(
-                underlying,
-                target_strangle,
-                option_to_move,
-                new_option,
-                quantity_in_lots,
-                strategy_tag,
-                notification_url,
+
+        if position.position_active:  # Check for exit conditions
+            current_call_price, current_put_price = position.instrument.fetch_ltp(
+                for_type=(~action).value
             )
-            if option_to_move.option_type == OptionType.CALL:
-                current_call_avg = avg_price
-                current_put_avg = target_strangle.put_option.fetch_ltp()
-            else:
-                current_put_avg = avg_price
-                current_call_avg = target_strangle.call_option.fetch_ltp()
+            total_current_price = current_call_price + current_put_price
             logger.info(
-                f"Updated strangle to {target_strangle} with call avg {current_call_avg} and put avg {current_put_avg}"
+                f"{underlying.name} {strategy_tag} Current price: {total_current_price} "
+                f"Target price: {position.profit_threshold} Stop loss price: {position.stop_loss_threshold}"
             )
-        sleep(1)
 
-    place_option_order_and_notify(
-        target_strangle,
-        "BUY",
-        quantity_in_lots,
-        "LIMIT",
-        order_tag=strategy_tag,
-        webhook_url=notification_url,
-    )
+            if current_time() > trade_exit_time:
+                logger.info(f"{underlying.name} {strategy_tag} exiting due to time")
+                exit_position()
+
+            if profit_condition():
+                logger.info(
+                    f"{underlying.name} {strategy_tag} profit triggered. Exiting."
+                )
+                exit_position()
+            if stop_loss_condition():
+                logger.info(
+                    f"{underlying.name} {strategy_tag} stop loss triggered. Exiting."
+                )
+                exit_position()
+
+        sleep(0.1)
+
+    notifier(f"{underlying.name} QS completed for the day", notification_url, "INFO")
 
 
 @exit_on_error
 @increase_robustness
 def delta_hedged_strangle(
     underlying: Index | Stock,
     exposure: int | float,
@@ -233,29 +336,28 @@
 
     delta_position: DeltaPosition = DeltaPosition(
         underlying=underlying,
         base_exposure_qty=base_qty_shares,
         order_tag=strategy_tag,
         notifier_url=notification_url,
     )
-    entry_priority = None
     while current_time().time() < time(*exit_time):
         if delta_position.cached_strikes is None or strike_range_different(
             underlying.get_active_strikes(tracking_strikes),
             delta_position.cached_strikes,
         ):
             delta_position.update_prospective_options(tracking_strikes, use_cache)
             logger.info(
                 f"{current_time()} {underlying.name} set active options and set "
                 f"{len(delta_position.all_options)} prospective options"
             )
         delta_position.update_underlying()
         delta_position.set_recommended_qty(target_delta, optimized)
         delta_position.adjust_recommended_qty()
-        delta_position.enter_positions(priority=entry_priority)
+        delta_position.enter_positions()
         delta_position.reset_trigger_flags()
 
         def interruption_condition():
             return abs(delta_position.aggregate_greeks().delta) > 0.07 * base_qty_shares
             # Hard coded 7% of base qty shares as the threshold for interruption
 
         # Delta hedging begins here
@@ -321,17 +423,14 @@
                             logger.info(message)
                             continue
                         else:
                             delta_position.exit_triggers["qty_breach_exit"] = True
 
                 # We will end up here if we are not hedging with atm options or if there is a breach
                 delta_position.exit_triggers["qty_breach_exit"] = True
-                entry_priority = (
-                    OptionType.PUT if aggregate_delta > 0 else OptionType.CALL
-                )
                 message = f"{underlying.name}. Shuffling position."
                 logger.info(message)
 
     # Exiting the position
     message = f"{underlying.name} {strategy_tag} exit time reached."
     notifier(message, notification_url, "INFO")
     delta_position.exit_positions()
@@ -1064,15 +1163,15 @@
                 trend_option: {
                     "action": Action.SELL,
                     "quantity_in_lots": qty_in_lots,
                     "order_tag": f"Intraday Strangle Trend Catcher",
                 }
             }
         )
-        sell_avg_price = execution_details[trend_option]
+        sell_avg_price = exec_details[trend_option]
 
         # Setting up the stop losses on underlying and trend option
 
         # Underlying stop loss
         sl_multiplier = 1 - sl if sl_type == "call" else 1 + sl
         underlying_sl_price = spot_price * sl_multiplier
 
@@ -1853,15 +1952,15 @@
 
             logger.info(
                 f"Entered {underlying.name} {position.instrument} with avg price {call_avg_price + put_avg_price}"
             )
             position.initiating_price = call_avg_price + put_avg_price
             break
 
-    sleep(0.1)
+        sleep(0.1)
 
     if not position.position_active:
         logger.info(
             f"{underlying.name} {strategy_tag} not triggered. Exiting.",
         )
         return
```

### Comparing `volstreet-7.0.0/volstreet/trade_interface/instruments.py` & `volstreet-7.0.1/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/trade_interface/order_execution.py` & `volstreet-7.0.1/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/trade_interface/order_placement.py` & `volstreet-7.0.1/volstreet/trade_interface/order_placement.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/trade_interface/underlyings.py` & `volstreet-7.0.1/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/utils/change_config.py` & `volstreet-7.0.1/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/utils/communication.py` & `volstreet-7.0.1/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/utils/core.py` & `volstreet-7.0.1/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/utils/data_io.py` & `volstreet-7.0.1/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/utils/scrip_processing.py` & `volstreet-7.0.1/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/vectorized_blackscholes.py` & `volstreet-7.0.1/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/vslogging/formatters.py` & `volstreet-7.0.1/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/vslogging/logging_config.json` & `volstreet-7.0.1/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/vslogging/logging_setup.py` & `volstreet-7.0.1/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet/vslogging/parsing.py` & `volstreet-7.0.1/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.0/volstreet.egg-info/PKG-INFO` & `volstreet-7.0.1/volstreet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.0.0
+Version: 7.0.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.0.0/volstreet.egg-info/SOURCES.txt` & `volstreet-7.0.1/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

