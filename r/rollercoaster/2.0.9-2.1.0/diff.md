# Comparing `tmp/rollercoaster-2.0.9.tar.gz` & `tmp/rollercoaster-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rollercoaster-2.0.9.tar", last modified: Thu Apr  4 20:15:26 2024, max compression
+gzip compressed data, was "rollercoaster-2.1.0.tar", last modified: Thu Apr  4 20:16:54 2024, max compression
```

## Comparing `rollercoaster-2.0.9.tar` & `rollercoaster-2.1.0.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-04 20:15:08.000000 rollercoaster-2.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      561 2024-03-31 20:41:36.000000 rollercoaster-2.0.9/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.523309 rollercoaster-2.0.9/structures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.523309 rollercoaster-2.0.9/structures/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.547309 rollercoaster-2.0.9/structures/modules/rollercoaster/
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-04 18:35:08.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.523309 rollercoaster-2.0.9/structures/modules/rollercoaster/_interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.547309 rollercoaster-2.0.9/structures/modules/rollercoaster/_interfaces/clique/
--rw-r--r--   0 root         (0) root         (0)     1765 2024-03-31 19:50:23.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/_interfaces/clique/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.547309 rollercoaster-2.0.9/structures/modules/rollercoaster/_interfaces/clique/group/
--rw-r--r--   0 root         (0) root         (0)      294 2023-12-01 19:53:30.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/_interfaces/clique/group/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.547309 rollercoaster-2.0.9/structures/modules/rollercoaster/_status/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-03-31 20:38:10.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/_status/insurance.proc.py
--rw-r--r--   0 root         (0) root         (0)     1319 2024-03-31 20:38:20.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/_status/insurance_clouds.proc.py
--rw-rw-r--   0 root         (0) root         (0)      114 2024-03-17 06:14:54.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.523309 rollercoaster-2.0.9/structures/modules/rollercoaster/autopilot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.523309 rollercoaster-2.0.9/structures/modules/rollercoaster/autopilot/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/autopilot/bt/strategies/
--rw-r--r--   0 root         (0) root         (0)     2589 2023-11-14 05:42:13.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/autopilot/bt/strategies/example_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/climate/
--rw-r--r--   0 root         (0) root         (0)      661 2024-03-31 20:40:53.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/climate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.535309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.523309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/crypto/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/crypto/_status/
--rw-r--r--   0 root         (0) root         (0)      764 2024-04-04 18:30:31.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py
--rw-r--r--   0 root         (0) root         (0)      980 2024-03-17 20:48:31.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/crypto/retrieve.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-04-04 18:31:47.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/crypto/structure_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/shares/
--rw-rw-r--   0 root         (0) root         (0)      390 2024-03-22 18:49:35.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/shares/retrieve_one.py
--rw-rw-r--   0 root         (0) root         (0)      982 2024-03-22 18:48:12.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/
--rw-r--r--   0 root         (0) root         (0)     1039 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles/
--rw-r--r--   0 root         (0) root         (0)     1594 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles_v1/
--rw-r--r--   0 root         (0) root         (0)     2513 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        3 2023-12-28 22:53:18.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/symbols/
--rw-r--r--   0 root         (0) root         (0)      362 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/symbols/array.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.551309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/
--rw-r--r--   0 root         (0) root         (0)     2726 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/accounts/
--rw-r--r--   0 root         (0) root         (0)      717 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/accounts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2042 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/build_JWT.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/orders/
--rw-r--r--   0 root         (0) root         (0)     1260 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/products/
--rw-r--r--   0 root         (0) root         (0)     3281 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/products/candles.py
--rw-r--r--   0 root         (0) root         (0)      978 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/products/catalogue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/orders/
--rw-r--r--   0 root         (0) root         (0)     1543 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/orders/place.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/_status/
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-04 18:44:17.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/procedures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/procedures/exchanges/
--rw-rw-r--   0 root         (0) root         (0)       36 2024-04-04 19:14:12.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/procedures/exchanges/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/procedures/options/
--rw-r--r--   0 root         (0) root         (0)     1351 2024-04-04 19:00:55.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/procedures/options/combine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/lookup/
--rw-rw-r--   0 root         (0) root         (0)     1134 2024-04-04 19:45:42.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/
--rw-r--r--   0 root         (0) root         (0)     1234 2024-04-04 19:24:22.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-04-04 20:05:04.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/expirations/
--rw-r--r--   0 root         (0) root         (0)      634 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/sensors/
--rw-r--r--   0 root         (0) root         (0)      300 2023-12-12 05:03:24.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/sensors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.555309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals/
--rw-rw-r--   0 root         (0) root         (0)     3836 2024-03-24 04:00:45.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.559309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/
--rw-rw-r--   0 root         (0) root         (0)     1514 2024-03-31 20:03:17.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.559309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/
--rw-rw-r--   0 root         (0) root         (0)      813 2024-03-22 19:47:25.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py
--rw-rw-r--   0 root         (0) root         (0)     1829 2024-03-22 19:46:48.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.535309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/IRS/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.531309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/IRS/taxes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.559309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/IRS/taxes/income/
--rw-rw-r--   0 root         (0) root         (0)      410 2024-03-27 18:27:21.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/IRS/taxes/income/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.535309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.559309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/6K/
--rw-r--r--   0 root         (0) root         (0)       60 2023-11-10 17:23:06.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/6K/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.559309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/balance_sheets/
--rw-r--r--   0 root         (0) root         (0)      496 2023-11-10 17:40:32.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/balance_sheets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.559309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/balance_sheets/equity/
--rw-r--r--   0 root         (0) root         (0)      198 2023-11-10 17:28:03.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/balance_sheets/equity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.559309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/income/
--rw-r--r--   0 root         (0) root         (0)      420 2023-11-10 17:53:32.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/USA/SEC/income/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.559309 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Yahoo/
--rw-r--r--   0 root         (0) root         (0)     1824 2024-03-18 19:45:43.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Yahoo/retrieve.py
--rw-rw-r--   0 root         (0) root         (0)      934 2024-03-22 19:39:27.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Yahoo/retrieve_change.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.563309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.535309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/clock/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.563309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/clock/UTC/
--rw-r--r--   0 root         (0) root         (0)      446 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/clock/UTC/ISO.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/clock/UTC/greatness_1.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-11-09 20:46:40.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/format_percentage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.535309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/math/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.563309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/math/slope/
--rw-r--r--   0 root         (0) root         (0)      151 2023-11-23 05:19:27.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/math/slope/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.535309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/pandas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.563309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/pandas/DF/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.563309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/pandas/DF/_status/
--rw-r--r--   0 root         (0) root         (0)      519 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/pandas/DF/from_list.py
--rw-r--r--   0 root         (0) root         (0)      326 2024-03-17 21:21:47.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/pandas/DF/to_list.py
--rw-r--r--   0 root         (0) root         (0)      402 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/ratio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.563309 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/summation/
--rw-r--r--   0 root         (0) root         (0)      457 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/summation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      377 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/summation/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.543309 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.539309 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.563309 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/
--rw-r--r--   0 root         (0) root         (0)     2944 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1591 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/_status/
--rw-r--r--   0 root         (0) root         (0)     1242 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/EMA/
--rw-r--r--   0 root         (0) root         (0)       82 2023-11-14 05:05:08.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/EMA/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/RSI/
--rw-r--r--   0 root         (0) root         (0)      782 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/RSI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/SMA/
--rw-r--r--   0 root         (0) root         (0)      250 2024-01-02 06:36:59.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/SMA/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/TR/
--rw-r--r--   0 root         (0) root         (0)     1628 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/TR/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/TR/_status/
--rw-r--r--   0 root         (0) root         (0)      523 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/TR/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      792 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/TR/_status/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/VWAP/
--rw-r--r--   0 root         (0) root         (0)      593 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/VWAP/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/bolinger_bands/
--rw-r--r--   0 root         (0) root         (0)       24 2023-11-14 04:28:20.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/bolinger_bands/bolinger_bands.r.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.567308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/
--rw-r--r--   0 root         (0) root         (0)     2832 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1098 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/_status/
--rw-r--r--   0 root         (0) root         (0)     1243 2024-03-18 04:08:14.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/pandas_ta/
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-06 00:03:10.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/pandas_ta/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend2/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-02 03:30:08.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.539309 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AAS/
--rw-r--r--   0 root         (0) root         (0)     1215 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AAS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AAS/_status/
--rw-r--r--   0 root         (0) root         (0)     1230 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AAS/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AS/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AS/_status/
--rw-r--r--   0 root         (0) root         (0)      511 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AS/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      783 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AS/_status/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/pecdency/
--rw-r--r--   0 root         (0) root         (0)     1093 2024-01-06 07:15:37.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/pecdency/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1350 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/pecdency/__init__v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.543309 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.571308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/ST/
--rw-r--r--   0 root         (0) root         (0)     4116 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/ST/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/VDA/
--rw-r--r--   0 root         (0) root         (0)      433 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/VDA/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/VSA/
--rw-r--r--   0 root         (0) root         (0)      567 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/VSA/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span/
--rw-r--r--   0 root         (0) root         (0)     1557 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span/_status/
--rw-r--r--   0 root         (0) root         (0)      522 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span/_status/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_average/
--rw-r--r--   0 root         (0) root         (0)     1183 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_average/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_average/_status/
--rw-r--r--   0 root         (0) root         (0)     1248 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_reversals/
--rw-r--r--   0 root         (0) root         (0)     3688 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_reversals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_roads_v1/
--rw-r--r--   0 root         (0) root         (0)     3586 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/super_hero_trend/
--rw-r--r--   0 root         (0) root         (0)     3862 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/super_hero_trend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.575308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/super_hero_trend/win_rates/
--rw-r--r--   0 root         (0) root         (0)     1759 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/supertrend/
--rw-r--r--   0 root         (0) root         (0)      961 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/supertrend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.543309 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/AO/
--rw-r--r--   0 root         (0) root         (0)     1825 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/AO/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/superb/
--rw-r--r--   0 root         (0) root         (0)     3926 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/superb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/superb/win_rates/
--rw-r--r--   0 root         (0) root         (0)     1786 2024-03-18 04:08:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/
--rw-rw-r--   0 root         (0) root         (0)     4000 2024-04-04 17:03:41.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/ETF.py
--rw-rw-r--   0 root         (0) root         (0)        2 2024-04-04 18:06:03.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/REIT.py
--rw-rw-r--   0 root         (0) root         (0)     2162 2024-04-04 18:22:34.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/TV.py
--rw-rw-r--   0 root         (0) root         (0)     1411 2024-04-04 17:36:52.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/currency.py
--rw-rw-r--   0 root         (0) root         (0)       42 2024-04-04 18:06:43.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/penny_stocks.py
--rw-rw-r--   0 root         (0) root         (0)      415 2024-04-04 18:22:24.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/clique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/symbol/
--rw-rw-r--   0 root         (0) root         (0)      119 2024-03-31 19:49:32.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/scans/symbol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_PC_ratio/
--rw-r--r--   0 root         (0) root         (0)     5120 2024-04-04 18:12:45.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_PC_ratio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.579308 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/
--rw-r--r--   0 root         (0) root         (0)      593 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py
--rw-r--r--   0 root         (0) root         (0)     1860 2024-02-28 18:15:52.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/
--rw-r--r--   0 root         (0) root         (0)     2905 2024-03-31 18:52:09.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/_status/
--rw-r--r--   0 root         (0) root         (0)     1508 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      794 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/_status/status_2.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 19:07:37.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/clique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/show/
--rw-r--r--   0 root         (0) root         (0)      892 2024-02-28 18:15:51.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/show/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      297 2024-03-31 19:16:52.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/stats/clique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.547309 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.547309 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/options/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/options/movement_calculator/
--rw-r--r--   0 root         (0) root         (0)     1565 2024-02-28 18:15:52.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/options/movement_calculator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.547309 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/options/shapes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/options/shapes/shape_1/
--rw-r--r--   0 root         (0) root         (0)     1498 2024-02-28 18:15:52.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/options/shapes/shape_1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/shares/
--rw-rw-r--   0 root         (0) root         (0)        7 2024-03-24 04:01:12.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/shares/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.547309 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/shares/shapes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/shares/shapes/shape_1/
--rw-r--r--   0 root         (0) root         (0)       11 2023-11-21 16:53:15.000000 rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/shares/shapes/shape_1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:15:26.583308 rollercoaster-2.0.9/structures/modules/rollercoaster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-04 20:15:26.000000 rollercoaster-2.0.9/structures/modules/rollercoaster.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8342 2024-04-04 20:15:26.000000 rollercoaster-2.0.9/structures/modules/rollercoaster.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-04 20:15:26.000000 rollercoaster-2.0.9/structures/modules/rollercoaster.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       55 2024-04-04 20:15:26.000000 rollercoaster-2.0.9/structures/modules/rollercoaster.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-04-04 20:15:26.000000 rollercoaster-2.0.9/structures/modules/rollercoaster.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       14 2024-04-04 20:15:26.000000 rollercoaster-2.0.9/structures/modules/rollercoaster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3157 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-04-04 20:16:45.000000 rollercoaster-2.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1950 2024-04-04 20:16:40.000000 rollercoaster-2.1.0/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.465856 rollercoaster-2.1.0/structures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.465856 rollercoaster-2.1.0/structures/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-04 18:35:08.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.465856 rollercoaster-2.1.0/structures/modules/rollercoaster/_interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/_interfaces/clique/
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-03-31 19:50:23.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/_interfaces/clique/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/_interfaces/clique/group/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-12-01 19:53:30.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/_interfaces/clique/group/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/_status/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-03-31 20:38:10.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/_status/insurance.proc.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2024-03-31 20:38:20.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/_status/insurance_clouds.proc.py
+-rw-rw-r--   0 root         (0) root         (0)      114 2024-03-17 06:14:54.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.465856 rollercoaster-2.1.0/structures/modules/rollercoaster/autopilot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.465856 rollercoaster-2.1.0/structures/modules/rollercoaster/autopilot/bt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/autopilot/bt/strategies/
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-11-14 05:42:13.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/autopilot/bt/strategies/example_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/climate/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-03-31 20:40:53.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/climate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.465856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/crypto/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/crypto/_status/
+-rw-r--r--   0 root         (0) root         (0)      764 2024-04-04 18:30:31.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py
+-rw-r--r--   0 root         (0) root         (0)      980 2024-03-17 20:48:31.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/crypto/retrieve.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-04 18:31:47.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/crypto/structure_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/shares/
+-rw-rw-r--   0 root         (0) root         (0)      390 2024-03-22 18:49:35.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/shares/retrieve_one.py
+-rw-rw-r--   0 root         (0) root         (0)      982 2024-03-22 18:48:12.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles/
+-rw-r--r--   0 root         (0) root         (0)     1594 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles_v1/
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        3 2023-12-28 22:53:18.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/symbols/
+-rw-r--r--   0 root         (0) root         (0)      362 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/symbols/array.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/accounts/
+-rw-r--r--   0 root         (0) root         (0)      717 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/accounts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/build_JWT.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/orders/
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/products/
+-rw-r--r--   0 root         (0) root         (0)     3281 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/products/candles.py
+-rw-r--r--   0 root         (0) root         (0)      978 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/products/catalogue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/orders/
+-rw-r--r--   0 root         (0) root         (0)     1543 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/orders/place.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/_status/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-04-04 18:44:17.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/procedures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/procedures/exchanges/
+-rw-rw-r--   0 root         (0) root         (0)       36 2024-04-04 19:14:12.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/procedures/exchanges/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/procedures/options/
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-04-04 19:00:55.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/procedures/options/combine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/lookup/
+-rw-rw-r--   0 root         (0) root         (0)     1134 2024-04-04 19:45:42.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/
+-rw-r--r--   0 root         (0) root         (0)     1234 2024-04-04 19:24:22.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-04-04 20:05:04.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/expirations/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/sensors/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-12-12 05:03:24.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/sensors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals/
+-rw-rw-r--   0 root         (0) root         (0)     3836 2024-03-24 04:00:45.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/
+-rw-rw-r--   0 root         (0) root         (0)     1514 2024-03-31 20:03:17.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/
+-rw-rw-r--   0 root         (0) root         (0)      813 2024-03-22 19:47:25.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py
+-rw-rw-r--   0 root         (0) root         (0)     1829 2024-03-22 19:46:48.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/IRS/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/IRS/taxes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.481856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/IRS/taxes/income/
+-rw-rw-r--   0 root         (0) root         (0)      410 2024-03-27 18:27:21.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/IRS/taxes/income/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/6K/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-11-10 17:23:06.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/6K/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/balance_sheets/
+-rw-r--r--   0 root         (0) root         (0)      496 2023-11-10 17:40:32.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/balance_sheets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/balance_sheets/equity/
+-rw-r--r--   0 root         (0) root         (0)      198 2023-11-10 17:28:03.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/balance_sheets/equity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/income/
+-rw-r--r--   0 root         (0) root         (0)      420 2023-11-10 17:53:32.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/USA/SEC/income/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Yahoo/
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-03-18 19:45:43.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Yahoo/retrieve.py
+-rw-rw-r--   0 root         (0) root         (0)      934 2024-03-22 19:39:27.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Yahoo/retrieve_change.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/clock/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/clock/UTC/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/clock/UTC/ISO.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/clock/UTC/greatness_1.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-11-09 20:46:40.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/format_percentage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/math/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/math/slope/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-11-23 05:19:27.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/math/slope/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.469856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/pandas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/pandas/DF/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/pandas/DF/_status/
+-rw-r--r--   0 root         (0) root         (0)      519 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/pandas/DF/from_list.py
+-rw-r--r--   0 root         (0) root         (0)      326 2024-03-17 21:21:47.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/pandas/DF/to_list.py
+-rw-r--r--   0 root         (0) root         (0)      402 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/ratio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/summation/
+-rw-r--r--   0 root         (0) root         (0)      457 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/summation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      377 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/summation/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.473856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.473856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/
+-rw-r--r--   0 root         (0) root         (0)     2944 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/_status/
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/EMA/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-11-14 05:05:08.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/EMA/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/RSI/
+-rw-r--r--   0 root         (0) root         (0)      782 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/RSI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/SMA/
+-rw-r--r--   0 root         (0) root         (0)      250 2024-01-02 06:36:59.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/SMA/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/TR/
+-rw-r--r--   0 root         (0) root         (0)     1628 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/TR/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/TR/_status/
+-rw-r--r--   0 root         (0) root         (0)      523 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/TR/_status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      792 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/TR/_status/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/VWAP/
+-rw-r--r--   0 root         (0) root         (0)      593 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/VWAP/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/bolinger_bands/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-11-14 04:28:20.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/bolinger_bands/bolinger_bands.r.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.485856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/
+-rw-r--r--   0 root         (0) root         (0)     2832 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1098 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/_status/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-03-18 04:08:14.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/pandas_ta/
+-rw-r--r--   0 root         (0) root         (0)      358 2024-01-06 00:03:10.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/pandas_ta/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend2/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-02 03:30:08.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.473856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AAS/
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AAS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AAS/_status/
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AAS/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AS/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AS/_status/
+-rw-r--r--   0 root         (0) root         (0)      511 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AS/_status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      783 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AS/_status/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/pecdency/
+-rw-r--r--   0 root         (0) root         (0)     1093 2024-01-06 07:15:37.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/pecdency/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/pecdency/__init__v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.473856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/ST/
+-rw-r--r--   0 root         (0) root         (0)     4116 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/ST/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/VDA/
+-rw-r--r--   0 root         (0) root         (0)      433 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/VDA/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/VSA/
+-rw-r--r--   0 root         (0) root         (0)      567 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/VSA/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span/
+-rw-r--r--   0 root         (0) root         (0)     1557 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span/_status/
+-rw-r--r--   0 root         (0) root         (0)      522 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span/_status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      790 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span/_status/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_average/
+-rw-r--r--   0 root         (0) root         (0)     1183 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_average/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_average/_status/
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_reversals/
+-rw-r--r--   0 root         (0) root         (0)     3688 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_reversals/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_roads_v1/
+-rw-r--r--   0 root         (0) root         (0)     3586 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/super_hero_trend/
+-rw-r--r--   0 root         (0) root         (0)     3862 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/super_hero_trend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/super_hero_trend/win_rates/
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/supertrend/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/supertrend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.473856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/AO/
+-rw-r--r--   0 root         (0) root         (0)     1825 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/AO/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/superb/
+-rw-r--r--   0 root         (0) root         (0)     3926 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/superb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/superb/win_rates/
+-rw-r--r--   0 root         (0) root         (0)     1786 2024-03-18 04:08:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.489856 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/
+-rw-rw-r--   0 root         (0) root         (0)     4000 2024-04-04 17:03:41.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/ETF.py
+-rw-rw-r--   0 root         (0) root         (0)        2 2024-04-04 18:06:03.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/REIT.py
+-rw-rw-r--   0 root         (0) root         (0)     2162 2024-04-04 18:22:34.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/TV.py
+-rw-rw-r--   0 root         (0) root         (0)     1411 2024-04-04 17:36:52.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/currency.py
+-rw-rw-r--   0 root         (0) root         (0)       42 2024-04-04 18:06:43.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/penny_stocks.py
+-rw-rw-r--   0 root         (0) root         (0)      415 2024-04-04 18:22:24.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/clique.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/symbol/
+-rw-rw-r--   0 root         (0) root         (0)      119 2024-03-31 19:49:32.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/scans/symbol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_PC_ratio/
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-04-04 18:12:45.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_PC_ratio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/
+-rw-r--r--   0 root         (0) root         (0)      593 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2024-02-28 18:15:52.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-03-31 18:52:09.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/_status/
+-rw-r--r--   0 root         (0) root         (0)     1508 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/_status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      794 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/_status/status_2.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 19:07:37.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/clique.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/show/
+-rw-r--r--   0 root         (0) root         (0)      892 2024-02-28 18:15:51.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/show/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      297 2024-03-31 19:16:52.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/stats/clique.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/options/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/options/movement_calculator/
+-rw-r--r--   0 root         (0) root         (0)     1565 2024-02-28 18:15:52.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/options/movement_calculator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/options/shapes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/options/shapes/shape_1/
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-02-28 18:15:52.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/options/shapes/shape_1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/shares/
+-rw-rw-r--   0 root         (0) root         (0)        7 2024-03-24 04:01:12.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/shares/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.477856 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/shares/shapes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/shares/shapes/shape_1/
+-rw-r--r--   0 root         (0) root         (0)       11 2023-11-21 16:53:15.000000 rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/shares/shapes/shape_1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:16:54.493856 rollercoaster-2.1.0/structures/modules/rollercoaster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3157 2024-04-04 20:16:54.000000 rollercoaster-2.1.0/structures/modules/rollercoaster.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8342 2024-04-04 20:16:54.000000 rollercoaster-2.1.0/structures/modules/rollercoaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-04 20:16:54.000000 rollercoaster-2.1.0/structures/modules/rollercoaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       55 2024-04-04 20:16:54.000000 rollercoaster-2.1.0/structures/modules/rollercoaster.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-04-04 20:16:54.000000 rollercoaster-2.1.0/structures/modules/rollercoaster.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       14 2024-04-04 20:16:54.000000 rollercoaster-2.1.0/structures/modules/rollercoaster.egg-info/top_level.txt
```

### Comparing `rollercoaster-2.0.9/pyproject.toml` & `rollercoaster-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 #
 #	how to publish:
 #
 #		python3 /rollercoaster/structures/modules/rollercoaster/_status/insurance.proc.py
 #		python3 /rollercoaster/structures/modules/rollercoaster/_status/insurance_clouds.proc.py
 #	
-#		cp /rollercoaster/structures/modules/rollercoaster/module.MD readme.md
+#		cp /rollercoaster/structures/modules/rollercoaster/module.MD /rollercoaster/readme.md
 #		(rm -rf dist && python3 -m build && twine upload dist/*)
 #
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rollercoaster"
-version = "2.0.9"
+version = "2.1.0"
 dependencies = [
 	
 	"ramps_galactic",
 	
 	#--
 	
 	"volts",
```

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/_interfaces/clique/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/_interfaces/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/_status/insurance.proc.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/_status/insurance.proc.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/_status/insurance_clouds.proc.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/_status/insurance_clouds.proc.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/autopilot/bt/strategies/example_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/autopilot/bt/strategies/example_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/climate/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/crypto/retrieve.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/crypto/retrieve.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/crypto/structure_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/crypto/structure_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/accounts/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/build_JWT.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/build_JWT.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/products/candles.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/products/candles.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/API/products/catalogue.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/API/products/catalogue.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Coinbase/orders/place.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Coinbase/orders/place.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/procedures/options/combine.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/procedures/options/combine.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Yahoo/retrieve.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Yahoo/retrieve.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/clouds/Yahoo/retrieve_change.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/clouds/Yahoo/retrieve_change.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/clock/UTC/greatness_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/clock/UTC/greatness_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/format_percentage.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/format_percentage.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/ATR/_status/status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/ATR/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/RSI/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/RSI/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/TR/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/TR/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/TR/_status/status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/TR/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/TR/_status/status_2.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/TR/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/VWAP/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/VWAP/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_1/supertrend/_status/status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_1/supertrend/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AAS/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AAS/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AAS/_status/status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AAS/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AS/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AS/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/AS/_status/status_2.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/AS/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/pecdency/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/pecdency/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_2/pecdency/__init__v1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_2/pecdency/__init__v1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/ST/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/ST/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/VSA/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/VSA/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span/_status/status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span/_status/status_2.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_average/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_average/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_reversals/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_reversals/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/super_hero_trend/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/super_hero_trend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_3/supertrend/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_3/supertrend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/AO/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/AO/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/superb/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/superb/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/ETF.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/ETF.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/TV.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/TV.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/scans/_clique/currency.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/scans/_clique/currency.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_PC_ratio/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_PC_ratio/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/_status/status_1.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/_status/status_2.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/stats/aggregate_break_even/show/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/stats/aggregate_break_even/show/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/options/movement_calculator/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/options/movement_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster/treasures/options/shapes/shape_1/__init__.py` & `rollercoaster-2.1.0/structures/modules/rollercoaster/treasures/options/shapes/shape_1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.0.9/structures/modules/rollercoaster.egg-info/SOURCES.txt` & `rollercoaster-2.1.0/structures/modules/rollercoaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

