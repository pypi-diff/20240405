# Comparing `tmp/investing_algorithm_framework-3.4.0.tar.gz` & `tmp/investing_algorithm_framework-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-3.4.0.tar", max compression
+gzip compressed data, was "investing_algorithm_framework-3.4.1.tar", max compression
```

## Comparing `investing_algorithm_framework-3.4.0.tar` & `investing_algorithm_framework-3.4.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0    11343 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/LICENSE
--rw-r--r--   0        0        0    19512 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/README.md
--rw-r--r--   0        0        0     2084 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/__init__.py
--rw-r--r--   0        0        0      501 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0        0        0    34948 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0        0        0    31166 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/app.py
--rw-r--r--   0        0        0     1092 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/__init__.py
--rw-r--r--   0        0        0     2362 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0        0        0      154 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0        0        0      451 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0        0        0     1062 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0        0        0     1085 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0        0        0     3750 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/strategy.py
--rw-r--r--   0        0        0      963 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/task.py
--rw-r--r--   0        0        0      134 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/__init__.py
--rw-r--r--   0        0        0      587 2024-04-04 14:04:05.929424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0        0        0      693 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0        0        0      727 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0        0        0      617 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0        0        0      506 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0        0        0     2020 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0        0        0      585 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0        0        0      158 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/run_strategies.py
--rw-r--r--   0        0        0      361 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0        0        0      442 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0        0        0      743 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0        0        0      437 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0        0        0       80 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0        0        0      603 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/create_app.py
--rw-r--r--   0        0        0     6312 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/dependency_container.py
--rw-r--r--   0        0        0     3913 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/config.py
--rw-r--r--   0        0        0     2293 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0        0        0      962 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/data_structures.py
--rw-r--r--   0        0        0      823 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/decimal_parsing.py
--rw-r--r--   0        0        0     1628 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/exceptions.py
--rw-r--r--   0        0        0     1121 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0        0        0      812 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/app_mode.py
--rw-r--r--   0        0        0      253 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/backtesting/__init__.py
--rw-r--r--   0        0        0     2374 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
--rw-r--r--   0        0        0    13604 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
--rw-r--r--   0        0        0      674 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
--rw-r--r--   0        0        0      659 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/base_model.py
--rw-r--r--   0        0        0       87 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/market/__init__.py
--rw-r--r--   0        0        0      779 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/market/market_credential.py
--rw-r--r--   0        0        0      237 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0        0        0    10194 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0        0        0     1110 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order_fee.py
--rw-r--r--   0        0        0      814 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0        0        0      937 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0        0        0      751 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order_type.py
--rw-r--r--   0        0        0      230 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0        0        0     2495 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1752 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
--rw-r--r--   0        0        0     3141 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      123 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0        0        0     1131 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/position/position_snapshot.py
--rw-r--r--   0        0        0     4598 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/strategy_profile.py
--rw-r--r--   0        0        0     2659 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0        0        0     2798 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0        0        0     2011 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0        0        0       99 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trade/__init__.py
--rw-r--r--   0        0        0     6819 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trade/trade.py
--rw-r--r--   0        0        0      807 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trade/trade_status.py
--rw-r--r--   0        0        0     1119 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0        0        0     6791 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0        0        0      634 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/__init__.py
--rw-r--r--   0        0        0     1047 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/market_credential_service.py
--rw-r--r--   0        0        0     9941 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/market_data_sources.py
--rw-r--r--   0        0        0     3520 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/market_service.py
--rw-r--r--   0        0        0      115 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/portfolios/__init__.py
--rw-r--r--   0        0        0      320 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0      699 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/rounding_service.py
--rw-r--r--   0        0        0      258 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0        0        0      156 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0        0        0     1805 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/strategy.py
--rw-r--r--   0        0        0      700 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0        0        0    10969 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/backtesting.py
--rw-r--r--   0        0        0     2746 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0        0        0      275 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0        0        0      417 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0        0        0      608 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0        0        0      253 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/synchronized.py
--rw-r--r--   0        0        0     1361 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/__init__.py
--rw-r--r--   0        0        0      176 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0        0        0     1386 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
--rw-r--r--   0        0        0      732 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0        0        0      327 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/decimal_parser.py
--rw-r--r--   0        0        0      437 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
--rw-r--r--   0        0        0    17466 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
--rw-r--r--   0        0        0     5472 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
--rw-r--r--   0        0        0      142 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/model_extension.py
--rw-r--r--   0        0        0      102 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0        0        0     4877 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/order/order.py
--rw-r--r--   0        0        0      847 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py
--rw-r--r--   0        0        0      141 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0        0        0     3226 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1238 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      135 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0        0        0     1898 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/position/position.py
--rw-r--r--   0        0        0      842 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
--rw-r--r--   0        0        0      567 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      487 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
--rw-r--r--   0        0        0     3352 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0        0        0     1073 2024-04-04 14:04:05.933424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0        0        0     1967 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
--rw-r--r--   0        0        0     1994 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0        0        0      680 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
--rw-r--r--   0        0        0     7661 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/repository.py
--rw-r--r--   0        0        0      163 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0        0        0       91 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
--rw-r--r--   0        0        0    15303 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
--rw-r--r--   0        0        0      195 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
--rw-r--r--   0        0        0       43 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
--rw-r--r--   0        0        0    11932 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
--rw-r--r--   0        0        0     1318 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0        0        0      191 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/backtesting/__init__.py
--rw-r--r--   0        0        0     1025 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
--rw-r--r--   0        0        0    15007 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/backtesting/backtest_service.py
--rw-r--r--   0        0        0      624 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/configuration_service.py
--rw-r--r--   0        0        0      820 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/market_credential_service.py
--rw-r--r--   0        0        0      235 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/market_data_source_service/__init__.py
--rw-r--r--   0        0        0     5213 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
--rw-r--r--   0        0        0     6267 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
--rw-r--r--   0        0        0      159 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/order_service/__init__.py
--rw-r--r--   0        0        0     7644 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/order_service/order_backtest_service.py
--rw-r--r--   0        0        0    27823 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/order_service/order_service.py
--rw-r--r--   0        0        0      510 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/__init__.py
--rw-r--r--   0        0        0      825 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
--rw-r--r--   0        0        0     2055 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
--rw-r--r--   0        0        0     4493 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/portfolio_service.py
--rw-r--r--   0        0        0     1984 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
--rw-r--r--   0        0        0    16126 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0     1052 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0        0        0      525 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/position_snapshot_service.py
--rw-r--r--   0        0        0      995 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0        0        0     8075 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0        0        0       68 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/trade_service/__init__.py
--rw-r--r--   0        0        0    14761 2024-04-04 14:04:05.937424 investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/trade_service/trade_service.py
--rw-r--r--   0        0        0      742 2024-04-04 14:04:14.889416 investing_algorithm_framework-3.4.0/pyproject.toml
--rw-r--r--   0        0        0    20584 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-05 09:57:22.868679 investing_algorithm_framework-3.4.1/LICENSE
+-rw-r--r--   0        0        0    19512 2024-04-05 09:57:22.868679 investing_algorithm_framework-3.4.1/README.md
+-rw-r--r--   0        0        0     2084 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0        0        0    34948 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0        0        0    31166 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/app.py
+-rw-r--r--   0        0        0     1092 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/__init__.py
+-rw-r--r--   0        0        0     2362 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0        0        0      451 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0        0        0     1062 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0        0        0     1085 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0        0        0     3750 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0        0        0      963 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/task.py
+-rw-r--r--   0        0        0      134 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0        0        0      693 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0        0        0      727 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0        0        0      617 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0        0        0      506 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0        0        0     2020 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0        0        0      585 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0        0        0      158 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/run_strategies.py
+-rw-r--r--   0        0        0      361 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0        0        0      743 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0        0        0      437 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0        0        0       80 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0        0        0      603 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/create_app.py
+-rw-r--r--   0        0        0     6312 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/dependency_container.py
+-rw-r--r--   0        0        0     3913 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0        0        0     2293 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0        0        0      962 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/data_structures.py
+-rw-r--r--   0        0        0      823 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/decimal_parsing.py
+-rw-r--r--   0        0        0     1628 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/exceptions.py
+-rw-r--r--   0        0        0     1121 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/app_mode.py
+-rw-r--r--   0        0        0      253 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/backtesting/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
+-rw-r--r--   0        0        0    13604 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
+-rw-r--r--   0        0        0      674 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
+-rw-r--r--   0        0        0      659 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/base_model.py
+-rw-r--r--   0        0        0       87 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/market/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/market/market_credential.py
+-rw-r--r--   0        0        0      237 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0        0        0    10194 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0        0        0     1110 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order_fee.py
+-rw-r--r--   0        0        0      814 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0        0        0      937 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0        0        0      751 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order_type.py
+-rw-r--r--   0        0        0      230 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     2495 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1752 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+-rw-r--r--   0        0        0     3141 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      123 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0        0        0     1131 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/position/position_snapshot.py
+-rw-r--r--   0        0        0     4598 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/strategy_profile.py
+-rw-r--r--   0        0        0     2659 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0        0        0     2798 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0        0        0     2011 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0        0        0       99 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trade/__init__.py
+-rw-r--r--   0        0        0     7112 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trade/trade.py
+-rw-r--r--   0        0        0      807 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trade/trade_status.py
+-rw-r--r--   0        0        0     1119 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0        0        0     6791 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0        0        0      634 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/market_credential_service.py
+-rw-r--r--   0        0        0     9941 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/market_data_sources.py
+-rw-r--r--   0        0        0     3520 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/market_service.py
+-rw-r--r--   0        0        0      115 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0      699 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/rounding_service.py
+-rw-r--r--   0        0        0      258 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0        0        0      156 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0        0        0     1805 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/strategy.py
+-rw-r--r--   0        0        0      700 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0        0        0    10969 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/backtesting.py
+-rw-r--r--   0        0        0     2746 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0        0        0      275 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0        0        0      417 2024-04-05 09:57:22.872679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0        0        0      608 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0        0        0      253 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/synchronized.py
+-rw-r--r--   0        0        0     1361 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0        0        0     1386 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+-rw-r--r--   0        0        0      732 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/decimal_parser.py
+-rw-r--r--   0        0        0      437 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
+-rw-r--r--   0        0        0    17466 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
+-rw-r--r--   0        0        0     5472 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
+-rw-r--r--   0        0        0      142 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/model_extension.py
+-rw-r--r--   0        0        0      102 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0        0        0     4877 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0        0        0      847 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py
+-rw-r--r--   0        0        0      141 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     3226 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1238 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      135 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0        0        0      842 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
+-rw-r--r--   0        0        0      567 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      487 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
+-rw-r--r--   0        0        0     3352 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0        0        0     1073 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0        0        0     1967 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
+-rw-r--r--   0        0        0     1994 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0        0        0      680 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
+-rw-r--r--   0        0        0     7661 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/repository.py
+-rw-r--r--   0        0        0      163 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
+-rw-r--r--   0        0        0    15303 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
+-rw-r--r--   0        0        0      195 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
+-rw-r--r--   0        0        0    11932 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
+-rw-r--r--   0        0        0     1318 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/backtesting/__init__.py
+-rw-r--r--   0        0        0     1025 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
+-rw-r--r--   0        0        0    15007 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/backtesting/backtest_service.py
+-rw-r--r--   0        0        0      624 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/configuration_service.py
+-rw-r--r--   0        0        0      820 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/market_credential_service.py
+-rw-r--r--   0        0        0      235 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/market_data_source_service/__init__.py
+-rw-r--r--   0        0        0     5213 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
+-rw-r--r--   0        0        0     6267 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
+-rw-r--r--   0        0        0      159 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/order_service/__init__.py
+-rw-r--r--   0        0        0     8010 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/order_service/order_backtest_service.py
+-rw-r--r--   0        0        0    27823 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/order_service/order_service.py
+-rw-r--r--   0        0        0      510 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
+-rw-r--r--   0        0        0     2055 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
+-rw-r--r--   0        0        0     4493 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/portfolio_service.py
+-rw-r--r--   0        0        0     1984 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
+-rw-r--r--   0        0        0    16126 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0     1052 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0        0        0      525 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/position_snapshot_service.py
+-rw-r--r--   0        0        0      995 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0        0        0     8075 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0        0        0       68 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/trade_service/__init__.py
+-rw-r--r--   0        0        0    14761 2024-04-05 09:57:22.876679 investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/trade_service/trade_service.py
+-rw-r--r--   0        0        0      742 2024-04-05 09:57:31.664750 investing_algorithm_framework-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0    20584 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.4.1/PKG-INFO
```

### Comparing `investing_algorithm_framework-3.4.0/LICENSE` & `investing_algorithm_framework-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/README.md` & `investing_algorithm_framework-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/algorithm.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/task.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/task.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/create_app.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/create_app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/dependency_container.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/config.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/constants.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/data_structures.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/data_structures.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/decimal_parsing.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/decimal_parsing.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/app_mode.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/app_mode.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/backtesting/backtest_position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/backtesting/backtest_report.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/market/market_credential.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/market/market_credential.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order_fee.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order_status.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/position/position.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/position/position_snapshot.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/strategy_profile.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/strategy_profile.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trade/trade.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trade/trade.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,20 +205,29 @@
             stop_loss_price = self.open_price * \
                               (1 - stop_loss_percentage / 100)
             return current_price <= stop_loss_price
         else:
             # If dataframes are provided, we use the dataframe to calculate
             # the stop loss price
             if ohlcv_df is not None:
-                filtered_df = ohlcv_df.filter(
-                    pl.col('Datetime') >= self.opened_at.strftime(
-                        DATETIME_FORMAT
+                column_type = ohlcv_df['Datetime'].dtype
+
+                if isinstance(column_type, pl.Datetime):
+                    filtered_df = ohlcv_df.filter(
+                        pl.col('Datetime') >= self.opened_at
+                    )
+                else:
+                    filtered_df = ohlcv_df.filter(
+                        pl.col('Datetime') >= self.opened_at.strftime(
+                            DATETIME_FORMAT
+                        )
                     )
-                )
+
                 prices = filtered_df['Close'].to_numpy()
+
             highest_price = max(prices)
             stop_loss_price = highest_price * (1 - stop_loss_percentage / 100)
             return current_price <= stop_loss_price
 
     def __repr__(self):
         return self.repr(
             target_symbol=self.target_symbol,
```

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trade/trade_status.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trade/trade_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/market_credential_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/market_data_sources.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/market_data_sources.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/market_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/services/rounding_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/services/rounding_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/backtesting.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/backtesting.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/order/order.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/backtesting/backtest_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/backtesting/backtest_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/configuration_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/market_credential_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/order_service/order_backtest_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/order_service/order_backtest_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 import pandas as pd
+import polars as pl
 
 from investing_algorithm_framework.domain import BACKTESTING_INDEX_DATETIME, \
     OrderStatus, BACKTESTING_PENDING_ORDER_CHECK_INTERVAL, \
     OperationalException, OrderSide, Order
 from investing_algorithm_framework.services.market_data_source_service \
     import BacktestMarketDataSourceService
 from .order_service import OrderService
@@ -156,17 +157,26 @@
         :return: True if the order has executed, False otherwise
         """
 
         # Extract attributes from the order object
         created_at = order.get_created_at()
         order_side = order.get_order_side()
         order_price = order.get_price()
+        column_type = ohlcv_data_frame['Datetime'].dtype
 
-        # Filter OHLCV data after the order creation time
-        ohlcv_data_after_order = ohlcv_data_frame.loc[created_at:]
+        if isinstance(column_type, pl.Datetime):
+            ohlcv_data_after_order = ohlcv_data_frame.filter(
+                pl.col('Datetime') >= created_at
+            )
+        else:
+            ohlcv_data_after_order = ohlcv_data_frame.filter(
+                pl.col('Datetime') >= created_at.strftime(
+                    self.configuration_service.config["DATETIME_FORMAT"]
+                )
+            )
 
         # Check if the order execution conditions are met
         if OrderSide.BUY.equals(order_side):
             # Check if the low price drops below or equals the order price
             if (ohlcv_data_after_order['Low'] <= order_price).any():
                 return True
         elif OrderSide.SELL.equals(order_side):
```

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/order_service/order_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/portfolio_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/position_snapshot_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/position_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/investing_algorithm_framework/services/trade_service/trade_service.py` & `investing_algorithm_framework-3.4.1/investing_algorithm_framework/services/trade_service/trade_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.0/pyproject.toml` & `investing_algorithm_framework-3.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investing-algorithm-framework"
-version = "v3.4.0"
+version = "v3.4.1"
 description = "A framework for creating trading bots"
 authors = ["MDUYN"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 wrapt = "^1.16.0"
```

### Comparing `investing_algorithm_framework-3.4.0/PKG-INFO` & `investing_algorithm_framework-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing-algorithm-framework
-Version: 3.4.0
+Version: 3.4.1
 Summary: A framework for creating trading bots
 Author: MDUYN
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.4.0
+Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.4.1
 Summary: A framework for creating trading bots Author: MDUYN Requires-Python:
 >=3.8.1,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.9,<4.0.0) Requires-Dist: Flask-Migrate
 (>=2.6.0,<3.0.0) Requires-Dist: MarkupSafe (>=2.1.2,<3.0.0) Requires-Dist:
```

