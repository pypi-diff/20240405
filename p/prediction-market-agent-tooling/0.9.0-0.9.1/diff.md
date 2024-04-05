# Comparing `tmp/prediction_market_agent_tooling-0.9.0.tar.gz` & `tmp/prediction_market_agent_tooling-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prediction_market_agent_tooling-0.9.0.tar", max compression
+gzip compressed data, was "prediction_market_agent_tooling-0.9.1.tar", max compression
```

## Comparing `prediction_market_agent_tooling-0.9.0.tar` & `prediction_market_agent_tooling-0.9.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     7650 2024-04-04 11:57:12.147864 prediction_market_agent_tooling-0.9.0/LICENSE
--rw-r--r--   0        0        0     2992 2024-04-04 11:57:12.147864 prediction_market_agent_tooling-0.9.0/README.md
--rw-r--r--   0        0        0     9578 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json
--rw-r--r--   0        0        0    11406 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json
--rw-r--r--   0        0        0     9841 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json
--rw-r--r--   0        0        0     4777 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json
--rw-r--r--   0        0        0     7315 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json
--rw-r--r--   0        0        0     1775 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json
--rw-r--r--   0        0        0    15953 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json
--rw-r--r--   0        0        0     6055 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/wxdai.abi.json
--rw-r--r--   0        0        0        0 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/__init__.py
--rw-r--r--   0        0        0     3737 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/agents.py
--rw-r--r--   0        0        0    21237 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/benchmark.py
--rw-r--r--   0        0        0     2748 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/utils.py
--rw-r--r--   0        0        0     2596 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/config.py
--rw-r--r--   0        0        0     7621 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/agent.py
--rw-r--r--   0        0        0      621 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/agent_example.py
--rw-r--r--   0        0        0       82 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/constants.py
--rw-r--r--   0        0        0     3739 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/gcp/deploy.py
--rw-r--r--   0        0        0     5255 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/gcp/utils.py
--rw-r--r--   0        0        0     2526 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/gtypes.py
--rw-r--r--   0        0        0     4488 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/agent_market.py
--rw-r--r--   0        0        0     1026 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/categorize.py
--rw-r--r--   0        0        0      763 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/data_models.py
--rw-r--r--   0        0        0        0 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/__init__.py
--rw-r--r--   0        0        0     6882 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/api.py
--rw-r--r--   0        0        0     5357 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/data_models.py
--rw-r--r--   0        0        0     3402 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/manifold.py
--rw-r--r--   0        0        0      513 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/utils.py
--rw-r--r--   0        0        0     1550 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/markets.py
--rw-r--r--   0        0        0        0 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/__init__.py
--rw-r--r--   0        0        0    10800 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/data_models.py
--rw-r--r--   0        0        0    27589 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen.py
--rw-r--r--   0        0        0    19354 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py
--rw-r--r--   0        0        0     7399 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_replicate.py
--rw-r--r--   0        0        0    11382 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py
--rw-r--r--   0        0        0    15423 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py
--rw-r--r--   0        0        0     4188 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/api.py
--rw-r--r--   0        0        0     4199 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/data_models.py
--rw-r--r--   0        0        0    10863 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/data_models_web.py
--rw-r--r--   0        0        0     2652 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py
--rw-r--r--   0        0        0     1960 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/utils.py
--rw-r--r--   0        0        0     2503 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/manifold.py
--rw-r--r--   0        0        0     2419 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/omen.py
--rw-r--r--   0        0        0     2413 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/polymarket.py
--rw-r--r--   0        0        0    11465 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/monitor.py
--rw-r--r--   0        0        0     4045 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/monitor_app.py
--rw-r--r--   0        0        0        0 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/py.typed
--rw-r--r--   0        0        0      625 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/balances.py
--rw-r--r--   0        0        0     3520 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py
--rw-r--r--   0        0        0     4367 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py
--rw-r--r--   0        0        0      422 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/minimum_bet_to_win.py
--rw-r--r--   0        0        0      429 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/stretch_bet_between.py
--rw-r--r--   0        0        0      499 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/cache.py
--rw-r--r--   0        0        0     5879 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/contract.py
--rw-r--r--   0        0        0      660 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/gnosis_rpc.py
--rw-r--r--   0        0        0     1761 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/google.py
--rw-r--r--   0        0        0     2037 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/hexbytes_custom.py
--rw-r--r--   0        0        0     2613 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/is_predictable.py
--rw-r--r--   0        0        0      733 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/parallelism.py
--rw-r--r--   0        0        0      729 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/singleton.py
--rw-r--r--   0        0        0     4674 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/utils.py
--rw-r--r--   0        0        0     5314 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/web3_utils.py
--rw-r--r--   0        0        0     1355 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 prediction_market_agent_tooling-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     7650 2024-04-05 08:50:05.815609 prediction_market_agent_tooling-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2992 2024-04-05 08:50:05.815609 prediction_market_agent_tooling-0.9.1/README.md
+-rw-r--r--   0        0        0     9578 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_dxdao.abi.json
+-rw-r--r--   0        0        0    11406 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm.abi.json
+-rw-r--r--   0        0        0     9841 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json
+-rw-r--r--   0        0        0     4777 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json
+-rw-r--r--   0        0        0     7315 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_kleros.abi.json
+-rw-r--r--   0        0        0     1775 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_oracle.abi.json
+-rw-r--r--   0        0        0    15953 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_realitio.abi.json
+-rw-r--r--   0        0        0     6055 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/wxdai.abi.json
+-rw-r--r--   0        0        0        0 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/__init__.py
+-rw-r--r--   0        0        0     3737 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/agents.py
+-rw-r--r--   0        0        0    21237 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2748 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/utils.py
+-rw-r--r--   0        0        0     2596 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/config.py
+-rw-r--r--   0        0        0     7621 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/agent.py
+-rw-r--r--   0        0        0      621 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/agent_example.py
+-rw-r--r--   0        0        0       82 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/constants.py
+-rw-r--r--   0        0        0     3739 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/gcp/deploy.py
+-rw-r--r--   0        0        0     5255 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/gcp/utils.py
+-rw-r--r--   0        0        0     2526 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/gtypes.py
+-rw-r--r--   0        0        0     4488 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/agent_market.py
+-rw-r--r--   0        0        0     1026 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/categorize.py
+-rw-r--r--   0        0        0      763 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/data_models.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/__init__.py
+-rw-r--r--   0        0        0     6882 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/api.py
+-rw-r--r--   0        0        0     5357 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/data_models.py
+-rw-r--r--   0        0        0     3402 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/manifold.py
+-rw-r--r--   0        0        0      513 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/utils.py
+-rw-r--r--   0        0        0     1550 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/markets.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/__init__.py
+-rw-r--r--   0        0        0    10800 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/data_models.py
+-rw-r--r--   0        0        0    27589 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen.py
+-rw-r--r--   0        0        0    19354 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_contracts.py
+-rw-r--r--   0        0        0     7399 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_replicate.py
+-rw-r--r--   0        0        0    11382 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py
+-rw-r--r--   0        0        0    15716 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py
+-rw-r--r--   0        0        0     4188 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/api.py
+-rw-r--r--   0        0        0     4199 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/data_models.py
+-rw-r--r--   0        0        0    10863 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/data_models_web.py
+-rw-r--r--   0        0        0     2652 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/polymarket.py
+-rw-r--r--   0        0        0     1960 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/utils.py
+-rw-r--r--   0        0        0     2503 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/manifold.py
+-rw-r--r--   0        0        0     2419 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/omen.py
+-rw-r--r--   0        0        0     2413 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/polymarket.py
+-rw-r--r--   0        0        0    11465 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/monitor.py
+-rw-r--r--   0        0        0     4045 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/monitor_app.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/py.typed
+-rw-r--r--   0        0        0      625 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/balances.py
+-rw-r--r--   0        0        0     3520 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py
+-rw-r--r--   0        0        0     4367 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py
+-rw-r--r--   0        0        0      422 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/minimum_bet_to_win.py
+-rw-r--r--   0        0        0      429 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/stretch_bet_between.py
+-rw-r--r--   0        0        0      499 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/cache.py
+-rw-r--r--   0        0        0     5879 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/contract.py
+-rw-r--r--   0        0        0      660 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/gnosis_rpc.py
+-rw-r--r--   0        0        0     1761 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/google.py
+-rw-r--r--   0        0        0     2037 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/hexbytes_custom.py
+-rw-r--r--   0        0        0     2613 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/is_predictable.py
+-rw-r--r--   0        0        0      733 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/parallelism.py
+-rw-r--r--   0        0        0      729 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/singleton.py
+-rw-r--r--   0        0        0     4674 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/utils.py
+-rw-r--r--   0        0        0     5314 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/web3_utils.py
+-rw-r--r--   0        0        0     1355 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 prediction_market_agent_tooling-0.9.1/PKG-INFO
```

### Comparing `prediction_market_agent_tooling-0.9.0/LICENSE` & `prediction_market_agent_tooling-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/README.md` & `prediction_market_agent_tooling-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_dxdao.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_kleros.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_oracle.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_realitio.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/wxdai.abi.json` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/wxdai.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/agents.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/agents.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/benchmark.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/utils.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/config.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/config.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/agent.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/agent.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/agent_example.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/agent_example.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/gcp/deploy.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/gcp/deploy.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/gcp/utils.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/gtypes.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/gtypes.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/agent_market.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/agent_market.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/categorize.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/categorize.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/data_models.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/api.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/api.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/data_models.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/manifold.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/manifold.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/utils.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/markets.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/markets.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/data_models.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_contracts.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_replicate.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_replicate.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import typing as t
-from datetime import datetime
+from datetime import datetime, timedelta
 
 from eth_typing import ChecksumAddress
 from subgrounds import FieldPath, Subgrounds
 
 from prediction_market_agent_tooling.gtypes import HexAddress, HexBytes, Wei
 from prediction_market_agent_tooling.markets.agent_market import FilterBy, SortBy
 from prediction_market_agent_tooling.markets.omen.data_models import (
@@ -18,15 +18,14 @@
 )
 from prediction_market_agent_tooling.tools.singleton import SingletonMeta
 from prediction_market_agent_tooling.tools.utils import to_int_timestamp, utcnow
 from prediction_market_agent_tooling.tools.web3_utils import ZERO_BYTES
 
 
 class OmenSubgraphHandler(metaclass=SingletonMeta):
-
     """
     Class responsible for handling interactions with Omen subgraphs (trades, conditionalTokens).
     """
 
     OMEN_TRADES_SUBGRAPH = "https://api.thegraph.com/subgraphs/name/protofire/omen-xdai"
     CONDITIONAL_TOKENS_SUBGRAPH = (
         "https://api.thegraph.com/subgraphs/name/gnosis/conditional-tokens-gc"
@@ -148,30 +147,27 @@
 
         if created_after:
             where_stms["creationTimestamp_gt"] = to_int_timestamp(created_after)
 
         if opened_before:
             where_stms["openingTimestamp_lt"] = to_int_timestamp(opened_before)
 
-        if opened_after:
-            where_stms["openingTimestamp_gt"] = to_int_timestamp(opened_after)
-
         if liquidity_bigger_than is not None:
             where_stms["liquidityMeasure_gt"] = liquidity_bigger_than
 
         if condition_id_in is not None:
             where_stms["condition_"]["id_in"] = [x.hex() for x in condition_id_in]
 
         if filter_by == FilterBy.RESOLVED:
             finalized = True
             resolved = True
         elif filter_by == FilterBy.OPEN:
-            where_stms["currentAnswer"] = None
-            finalized = False
-            resolved = False
+            # We can not use `resolved=False` + `finalized=False` here,
+            # because even closed markets don't need to be resolved yet (e.g. if someone forgot to finalize the question on reality).
+            opened_after = utcnow() + timedelta(seconds=42)
         elif filter_by == FilterBy.NONE:
             pass
         else:
             raise ValueError(f"Unknown filter_by: {filter_by}")
 
         if resolved is not None:
             if resolved:
@@ -181,14 +177,17 @@
 
         if finalized is not None:
             if finalized:
                 where_stms["answerFinalizedTimestamp_not"] = None
             else:
                 where_stms["answerFinalizedTimestamp"] = None
 
+        if opened_after:
+            where_stms["openingTimestamp_gt"] = to_int_timestamp(opened_after)
+
         if finalized_before:
             where_stms["answerFinalizedTimestamp_lt"] = to_int_timestamp(
                 finalized_before
             )
 
         excluded_question_titles = [""]
         if excluded_questions is not None:
@@ -198,15 +197,16 @@
         return where_stms
 
     def _build_sort_direction(self, sort_by: SortBy) -> str:
         match sort_by:
             case SortBy.NEWEST:
                 sort_direction = "desc"
             case SortBy.CLOSING_SOONEST:
-                sort_direction = "asc"
+                # `desc` feel unintuitive, but really if we use `asc`, we are getting markets closing in 2030, 2026, etc.
+                sort_direction = "desc"
             case SortBy.NONE:
                 sort_direction = "desc"
             case _:
                 raise ValueError(f"Unknown sort_by: {sort_by}")
 
         return sort_direction
```

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/api.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/api.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/data_models.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/data_models_web.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/data_models_web.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/polymarket.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/utils.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/manifold.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/manifold.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/omen.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/omen.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/polymarket.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/polymarket.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/monitor.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/monitor_app.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/monitor_app.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/balances.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/balances.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/contract.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/contract.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/gnosis_rpc.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/gnosis_rpc.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/google.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/google.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/hexbytes_custom.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/hexbytes_custom.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/is_predictable.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/is_predictable.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/parallelism.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/parallelism.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/singleton.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/singleton.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/utils.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/web3_utils.py` & `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/web3_utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.0/pyproject.toml` & `prediction_market_agent_tooling-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prediction-market-agent-tooling"
-version = "0.9.0"
+version = "0.9.1"
 description = "Tools to benchmark, deploy and monitor prediction market agents."
 authors = ["Gnosis"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 buy_omen = "scripts.bet_omen:buy"
 sell_omen = "scripts.bet_omen:sell"
```

### Comparing `prediction_market_agent_tooling-0.9.0/PKG-INFO` & `prediction_market_agent_tooling-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prediction-market-agent-tooling
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools to benchmark, deploy and monitor prediction market agents.
 Author: Gnosis
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
```

