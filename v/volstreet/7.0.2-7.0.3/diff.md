# Comparing `tmp/volstreet-7.0.2.tar.gz` & `tmp/volstreet-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.0.2.tar", last modified: Fri Apr  5 04:46:07 2024, max compression
+gzip compressed data, was "volstreet-7.0.3.tar", last modified: Fri Apr  5 06:28:50 2024, max compression
```

## Comparing `volstreet-7.0.2.tar` & `volstreet-7.0.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.973679 volstreet-7.0.2/
--rw-rw-rw-   0        0        0     1260 2024-04-05 04:46:07.972659 volstreet-7.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.0.2/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1085 2024-04-05 04:46:07.974676 volstreet-7.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.904200 volstreet-7.0.2/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.0.2/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.921124 volstreet-7.0.2/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.0.2/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.0.2/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.0.2/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    13897 2024-04-03 08:06:51.000000 volstreet-7.0.2/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     3534 2024-03-27 14:07:30.000000 volstreet-7.0.2/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.0.2/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.0.2/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.933662 volstreet-7.0.2/volstreet/backtests/
--rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/backtests/data_handling.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.0.2/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    47182 2024-03-26 10:23:44.000000 volstreet-7.0.2/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.0.2/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.0.2/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    18739 2024-03-14 09:00:56.000000 volstreet-7.0.2/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6034 2024-03-14 09:55:23.000000 volstreet-7.0.2/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.942184 volstreet-7.0.2/volstreet/datamodule/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.0.2/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.0.2/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.0.2/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.943210 volstreet-7.0.2/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     2090 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.950840 volstreet-7.0.2/volstreet/strategies/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0     5684 2024-04-03 08:06:51.000000 volstreet-7.0.2/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    27771 2024-04-05 04:45:24.000000 volstreet-7.0.2/volstreet/strategies/execution.py
--rw-rw-rw-   0        0        0    58696 2024-04-04 15:28:05.000000 volstreet-7.0.2/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     9310 2024-04-05 02:48:44.000000 volstreet-7.0.2/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    89782 2024-04-05 04:35:38.000000 volstreet-7.0.2/volstreet/strategies/strats.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.958166 volstreet-7.0.2/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.0.2/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26065 2024-04-04 11:05:16.000000 volstreet-7.0.2/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0     9793 2024-04-05 02:44:31.000000 volstreet-7.0.2/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    12025 2024-04-04 15:02:10.000000 volstreet-7.0.2/volstreet/trade_interface/order_placement.py
--rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.0.2/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.965136 volstreet-7.0.2/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     2963 2024-04-05 02:45:53.000000 volstreet-7.0.2/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.0.2/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.0.2/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.970039 volstreet-7.0.2/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.0.2/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.0.2/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.0.2/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.0.2/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.0.2/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:46:07.972224 volstreet-7.0.2/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1260 2024-04-05 04:46:07.000000 volstreet-7.0.2/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2374 2024-04-05 04:46:07.000000 volstreet-7.0.2/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 04:46:07.000000 volstreet-7.0.2/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      443 2024-04-05 04:46:07.000000 volstreet-7.0.2/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 04:46:07.000000 volstreet-7.0.2/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.193170 volstreet-7.0.3/
+-rw-rw-rw-   0        0        0     1260 2024-04-05 06:28:50.193170 volstreet-7.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.0.3/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1085 2024-04-05 06:28:50.193170 volstreet-7.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.096009 volstreet-7.0.3/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.0.3/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.123869 volstreet-7.0.3/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.0.3/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.0.3/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.0.3/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    13980 2024-04-05 05:29:52.000000 volstreet-7.0.3/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     3534 2024-03-27 14:07:30.000000 volstreet-7.0.3/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.0.3/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.0.3/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.140538 volstreet-7.0.3/volstreet/backtests/
+-rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/backtests/data_handling.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.0.3/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    47182 2024-03-26 10:23:44.000000 volstreet-7.0.3/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.0.3/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.0.3/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    18739 2024-03-14 09:00:56.000000 volstreet-7.0.3/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     6034 2024-03-14 09:55:23.000000 volstreet-7.0.3/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.151563 volstreet-7.0.3/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.0.3/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.0.3/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.0.3/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.154294 volstreet-7.0.3/volstreet/historical_info/
+-rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-05 05:24:39.000000 volstreet-7.0.3/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.162622 volstreet-7.0.3/volstreet/strategies/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5684 2024-04-03 08:06:51.000000 volstreet-7.0.3/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    27771 2024-04-05 04:45:24.000000 volstreet-7.0.3/volstreet/strategies/execution.py
+-rw-rw-rw-   0        0        0    58696 2024-04-04 15:28:05.000000 volstreet-7.0.3/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     9310 2024-04-05 02:48:44.000000 volstreet-7.0.3/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    89782 2024-04-05 04:35:38.000000 volstreet-7.0.3/volstreet/strategies/strats.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.170949 volstreet-7.0.3/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.0.3/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26065 2024-04-04 11:05:16.000000 volstreet-7.0.3/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0     9793 2024-04-05 02:44:31.000000 volstreet-7.0.3/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    11706 2024-04-05 06:27:44.000000 volstreet-7.0.3/volstreet/trade_interface/order_placement.py
+-rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.0.3/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.179281 volstreet-7.0.3/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     2963 2024-04-05 02:45:53.000000 volstreet-7.0.3/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.0.3/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.0.3/volstreet/vectorized_blackscholes.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.190412 volstreet-7.0.3/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.0.3/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.0.3/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.0.3/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.0.3/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.0.3/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:28:50.190412 volstreet-7.0.3/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1260 2024-04-05 06:28:50.000000 volstreet-7.0.3/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2374 2024-04-05 06:28:50.000000 volstreet-7.0.3/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 06:28:50.000000 volstreet-7.0.3/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      443 2024-04-05 06:28:50.000000 volstreet-7.0.3/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 06:28:50.000000 volstreet-7.0.3/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.0.2/PKG-INFO` & `volstreet-7.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.0.2
+Version: 7.0.3
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.0.2/setup.cfg` & `volstreet-7.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 302e 320d 0a61  rsion = 7.0.2..a
+00000020: 7273 696f 6e20 3d20 372e 302e 330d 0a61  rsion = 7.0.3..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-7.0.2/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-7.0.3/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/angel_interface/async_interface.py` & `volstreet-7.0.3/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/angel_interface/base_websocket.py` & `volstreet-7.0.3/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/angel_interface/interface.py` & `volstreet-7.0.3/volstreet/angel_interface/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
     return ActiveSession.obj.modifyOrder(params)
 
 
 @retry_angel_api(data_type=lambda x: x["data"]["fetched"])
 @access_rate_handler(max_requests=10, per_seconds=1.2)
 @timeit()
 def _fetch_quotes(tokens: list, mode: str = "FULL"):
+    assert len(tokens) <= 50, "Maximum 50 tokens can be fetched at once for now."
     payload = defaultdict(list)
     for token in tokens:
         exchange = token_exchange_dict.get(token)
         if exchange:
             payload[exchange].append(token)
     payload = dict(payload)
     return ActiveSession.obj.getMarketData(mode, payload)
```

### Comparing `volstreet-7.0.2/volstreet/angel_interface/login.py` & `volstreet-7.0.3/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/angel_interface/order_websocket.py` & `volstreet-7.0.3/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/angel_interface/price_websocket.py` & `volstreet-7.0.3/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/angel_interface/smart_connect.py` & `volstreet-7.0.3/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/data_handling.py` & `volstreet-7.0.3/volstreet/backtests/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/database.py` & `volstreet-7.0.3/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/delta_hedging.py` & `volstreet-7.0.3/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/delta_optimizer.py` & `volstreet-7.0.3/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/framework.py` & `volstreet-7.0.3/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-7.0.3/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/tools.py` & `volstreet-7.0.3/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/trend.py` & `volstreet-7.0.3/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/backtests/underlying_info.py` & `volstreet-7.0.3/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/blackscholes.py` & `volstreet-7.0.3/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/config.py` & `volstreet-7.0.3/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/database_connection.py` & `volstreet-7.0.3/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/datamodule/analysis.py` & `volstreet-7.0.3/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/datamodule/archive.py` & `volstreet-7.0.3/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/datamodule/eod_client.py` & `volstreet-7.0.3/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/datamodule/gambling.py` & `volstreet-7.0.3/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/datamodule/intraday_data.py` & `volstreet-7.0.3/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/datamodule/stockmock.py` & `volstreet-7.0.3/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/datamodule/trading_assistance.py` & `volstreet-7.0.3/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/dealingroom.py` & `volstreet-7.0.3/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/decorators.py` & `volstreet-7.0.3/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/discord_bot.py` & `volstreet-7.0.3/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/exceptions.py` & `volstreet-7.0.3/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/historical_info/index_expiries.pkl` & `volstreet-7.0.3/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/parallelization.py` & `volstreet-7.0.3/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/strategies/error_handling.py` & `volstreet-7.0.3/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/strategies/execution.py` & `volstreet-7.0.3/volstreet/strategies/execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/strategies/helpers.py` & `volstreet-7.0.3/volstreet/strategies/helpers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/strategies/optimization.py` & `volstreet-7.0.3/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/strategies/strats.py` & `volstreet-7.0.3/volstreet/strategies/strats.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/trade_interface/instruments.py` & `volstreet-7.0.3/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/trade_interface/order_execution.py` & `volstreet-7.0.3/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/trade_interface/order_placement.py` & `volstreet-7.0.3/volstreet/trade_interface/order_placement.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,25 +206,15 @@
             for token in (instrument.call_token, instrument.put_token)
         }
         tokens = option_tokens | strangle_tokens
         return fetch_quotes(tokens, structure="dict")
 
     order_params = []
 
-    # if all params contain "price" key, then we don't need to fetch ltp_cache
-    if not all("price" in params for params in instructions.values()):
-        ltp_cache = fetch_market_depth(
-            [
-                instr
-                for instr in instructions.keys()
-                if "price" not in instructions[instr]
-            ]
-        )
-    else:
-        ltp_cache = {}
+    ltp_cache = fetch_market_depth([instr for instr in instructions.keys()])
 
     for instr, params in instructions.items():
         action = params["action"]
 
         if isinstance(instr, Option):
             target_depth = (~action).value.lower()
             price = params.pop(
```

### Comparing `volstreet-7.0.2/volstreet/trade_interface/underlyings.py` & `volstreet-7.0.3/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/utils/change_config.py` & `volstreet-7.0.3/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/utils/communication.py` & `volstreet-7.0.3/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/utils/core.py` & `volstreet-7.0.3/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/utils/data_io.py` & `volstreet-7.0.3/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/utils/scrip_processing.py` & `volstreet-7.0.3/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/vectorized_blackscholes.py` & `volstreet-7.0.3/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/vslogging/formatters.py` & `volstreet-7.0.3/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/vslogging/logging_config.json` & `volstreet-7.0.3/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/vslogging/logging_setup.py` & `volstreet-7.0.3/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet/vslogging/parsing.py` & `volstreet-7.0.3/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.2/volstreet.egg-info/PKG-INFO` & `volstreet-7.0.3/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.0.2
+Version: 7.0.3
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.0.2/volstreet.egg-info/SOURCES.txt` & `volstreet-7.0.3/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

