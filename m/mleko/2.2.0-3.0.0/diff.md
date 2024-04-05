# Comparing `tmp/mleko-2.2.0.tar.gz` & `tmp/mleko-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-2.2.0.tar", max compression
+gzip compressed data, was "mleko-3.0.0.tar", max compression
```

## Comparing `mleko-2.2.0.tar` & `mleko-3.0.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    10947 2024-03-22 17:05:44.140231 mleko-2.2.0/LICENSE
--rw-r--r--   0        0        0     4728 2024-03-22 17:05:44.144232 mleko-2.2.0/README.md
--rw-r--r--   0        0        0     1976 2024-03-22 17:06:10.932299 mleko-2.2.0/mleko/__init__.py
--rw-r--r--   0        0        0      585 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    16986 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0     1563 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1168 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     1012 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
--rw-r--r--   0        0        0     2989 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1333 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/fingerprinters/dict_fingerprinter.py
--rw-r--r--   0        0        0     5578 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
--rw-r--r--   0        0        0    14262 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
--rw-r--r--   0        0        0     1219 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0     1360 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/handlers/__init__.py
--rw-r--r--   0        0        0      650 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/handlers/base_cache_handler.py
--rw-r--r--   0        0        0     1102 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/handlers/joblib_cache_handler.py
--rw-r--r--   0        0        0     1196 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/handlers/pickle_cache_handler.py
--rw-r--r--   0        0        0     1506 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/handlers/vaex_cache_handler.py
--rw-r--r--   0        0        0     8312 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      805 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      492 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1613 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    15173 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     5640 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/data_schema.py
--rw-r--r--   0        0        0     1614 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0    11612 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     7661 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     5156 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5439 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7257 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5803 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      569 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/filter/__init__.py
--rw-r--r--   0        0        0     1615 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/filter/base_filter.py
--rw-r--r--   0        0        0     3927 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/filter/expression_filter.py
--rw-r--r--   0        0        0     7186 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/filter/imblearn_resampling_filter.py
--rw-r--r--   0        0        0     1197 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     6118 2024-03-22 17:05:44.144232 mleko-2.2.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    20008 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0    12998 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      680 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1501 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     4254 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     6732 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1612 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     9362 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     6882 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4743 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0    11498 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3744 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4150 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      388 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/model/__init__.py
--rw-r--r--   0        0        0    14750 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/model/base_model.py
--rw-r--r--   0        0        0    26883 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/model/lgbm_model.py
--rw-r--r--   0        0        0      413 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/model/tune/__init__.py
--rw-r--r--   0        0        0     3767 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/model/tune/base_tuner.py
--rw-r--r--   0        0        0    15426 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/model/tune/optuna_tuner.py
--rw-r--r--   0        0        0      645 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1382 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4497 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     9723 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      874 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     3832 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     6151 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2994 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/filter_step.py
--rw-r--r--   0        0        0     2780 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     7816 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/model_step.py
--rw-r--r--   0        0        0     2903 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     5744 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0     3430 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/pipeline/steps/tune_step.py
--rw-r--r--   0        0        0        0 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/py.typed
--rw-r--r--   0        0        0      766 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     9501 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3431 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0      743 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1414 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     2837 2024-03-22 17:05:44.148232 mleko-2.2.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2608 2024-03-22 17:06:10.932299 mleko-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 mleko-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-04-05 08:27:13.105788 mleko-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4728 2024-04-05 08:27:13.105788 mleko-3.0.0/README.md
+-rw-r--r--   0        0        0     1976 2024-04-05 08:27:41.730234 mleko-3.0.0/mleko/__init__.py
+-rw-r--r--   0        0        0      585 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    16986 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0     1563 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     1012 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
+-rw-r--r--   0        0        0     2989 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1333 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/dict_fingerprinter.py
+-rw-r--r--   0        0        0     5578 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
+-rw-r--r--   0        0        0    14262 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
+-rw-r--r--   0        0        0     1219 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0     1360 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/__init__.py
+-rw-r--r--   0        0        0      650 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/base_cache_handler.py
+-rw-r--r--   0        0        0     1102 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/joblib_cache_handler.py
+-rw-r--r--   0        0        0     1196 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/pickle_cache_handler.py
+-rw-r--r--   0        0        0     1508 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/vaex_cache_handler.py
+-rw-r--r--   0        0        0     8312 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      805 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      492 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1613 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    15173 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     5640 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/data_schema.py
+-rw-r--r--   0        0        0     1614 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0    11612 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     7661 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     5156 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5439 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7257 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5803 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      569 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/filter/__init__.py
+-rw-r--r--   0        0        0     1615 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/filter/base_filter.py
+-rw-r--r--   0        0        0     3927 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/filter/expression_filter.py
+-rw-r--r--   0        0        0     7236 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/filter/imblearn_resampling_filter.py
+-rw-r--r--   0        0        0     1197 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     6118 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    20008 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0    12998 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      680 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     4254 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     6732 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1612 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     9362 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     6882 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4743 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0    11525 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3744 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4150 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      388 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/model/__init__.py
+-rw-r--r--   0        0        0    15073 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/model/base_model.py
+-rw-r--r--   0        0        0    10169 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/model/lgbm_model.py
+-rw-r--r--   0        0        0      413 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/model/tune/__init__.py
+-rw-r--r--   0        0        0     3767 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/model/tune/base_tuner.py
+-rw-r--r--   0        0        0    15426 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/model/tune/optuna_tuner.py
+-rw-r--r--   0        0        0      645 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4497 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     9723 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      874 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     3832 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     6151 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2994 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/filter_step.py
+-rw-r--r--   0        0        0     2780 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     7816 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/model_step.py
+-rw-r--r--   0        0        0     2903 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     5744 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0     3430 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/tune_step.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/py.typed
+-rw-r--r--   0        0        0      766 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     9753 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3431 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      743 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1414 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     2837 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2608 2024-04-05 08:27:41.730234 mleko-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 mleko-3.0.0/PKG-INFO
```

### Comparing `mleko-2.2.0/LICENSE` & `mleko-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/README.md` & `mleko-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/__init__.py` & `mleko-3.0.0/mleko/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 By integrating these features, `mleko` serves as a comprehensive toolkit for machine learning
 practitioners looking to build robust models efficiently.
 """
 
 from __future__ import annotations
 
 
-__version__ = "2.2.0"
+__version__ = "3.0.0"
```

### Comparing `mleko-2.2.0/mleko/cache/__init__.py` & `mleko-3.0.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/cache_mixin.py` & `mleko-3.0.0/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/fingerprinters/__init__.py` & `mleko-3.0.0/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-3.0.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py` & `mleko-3.0.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-3.0.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/fingerprinters/dict_fingerprinter.py` & `mleko-3.0.0/mleko/cache/fingerprinters/dict_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py` & `mleko-3.0.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py` & `mleko-3.0.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-3.0.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/handlers/__init__.py` & `mleko-3.0.0/mleko/cache/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/handlers/base_cache_handler.py` & `mleko-3.0.0/mleko/cache/handlers/base_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/handlers/joblib_cache_handler.py` & `mleko-3.0.0/mleko/cache/handlers/joblib_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/handlers/pickle_cache_handler.py` & `mleko-3.0.0/mleko/cache/handlers/pickle_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/cache/handlers/vaex_cache_handler.py` & `mleko-3.0.0/mleko/cache/handlers/vaex_cache_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     Args:
         cache_file_path: The path of the cache file to be written.
         output: The Vaex DataFrame to be saved in the cache file.
     """
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", "invalid value encountered in cast")
         with tqdm(total=100, desc=f"Writing DataFrame to {cache_file_path.suffix} file") as pbar:
-            output.export_hdf5(
+            output.export_arrow(
                 cache_file_path,
                 progress=set_tqdm_percent_wrapper(pbar),
                 parallel=True,
-                chunk_size=100_000,
+                chunk_size=262_144,
             )
 
 
 VAEX_DATAFRAME_CACHE_HANDLER = CacheHandler(
-    writer=write_vaex_dataframe, reader=read_vaex_dataframe, suffix="hdf5", can_handle_none=False
+    writer=write_vaex_dataframe, reader=read_vaex_dataframe, suffix="arrow", can_handle_none=False
 )
 """A CacheHandler for `vaex` DataFrames."""
```

### Comparing `mleko-2.2.0/mleko/cache/lru_cache_mixin.py` & `mleko-3.0.0/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/__init__.py` & `mleko-3.0.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/convert/base_converter.py` & `mleko-3.0.0/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-3.0.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -346,17 +346,14 @@
                 logger.warning(f"Renaming column {column_name!r} to '_{column_name}'")
                 df.rename(column_name, f"_{column_name}")
 
             if column_name == "":
                 logger.warning(f"Renaming column {column_name!r} to '_empty'")
                 df.rename(column_name, "_empty")
 
-        for column_name in df.get_column_names(dtype="bool"):
-            df[column_name] = get_column(df, column_name).astype("int8")
-
         for column_name in df.get_column_names(dtype=pa.null()):
             df[column_name] = get_column(df, column_name).astype("string")
 
         if self._drop_rows_with_na_columns:
             df = df.dropna(column_names=self._drop_rows_with_na_columns)
 
         ds = DataSchema(
@@ -364,9 +361,12 @@
             categorical=df.get_column_names(dtype="string"),
             boolean=df.get_column_names(dtype="bool"),
             datetime=df.get_column_names(dtype="datetime"),
             timedelta=df.get_column_names(dtype="timedelta"),
         )
         ds.drop_features(self._meta_columns)
 
+        for column_name in df.get_column_names(dtype="bool"):
+            df[column_name] = get_column(df, column_name).astype("int8")
+
         logger.info("Merging chunks into a single DataFrame.")
         return ds, df
```

### Comparing `mleko-2.2.0/mleko/dataset/data_schema.py` & `mleko-3.0.0/mleko/dataset/data_schema.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/feature_select/__init__.py` & `mleko-3.0.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-3.0.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-3.0.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-3.0.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-3.0.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-3.0.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-3.0.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/filter/__init__.py` & `mleko-3.0.0/mleko/dataset/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/filter/base_filter.py` & `mleko-3.0.0/mleko/dataset/filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/filter/expression_filter.py` & `mleko-3.0.0/mleko/dataset/filter/expression_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/filter/imblearn_resampling_filter.py` & `mleko-3.0.0/mleko/dataset/filter/imblearn_resampling_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A module for filtering `vaex` DataFrames using `imblearn` sampling methods."""
 
 from __future__ import annotations
 
+import logging
 from pathlib import Path
 
 import numpy as np
 import pyarrow as pa
 import vaex
 from imblearn.under_sampling.base import BaseSampler
 
@@ -29,30 +30,30 @@
 
     @auto_repr
     def __init__(
         self,
         sampler: BaseSampler,
         target_column: str,
         random_state: int | None = 42,
-        enable_logging: bool = True,
+        verbosity: int = logging.INFO,
         cache_directory: str | Path = "data/imblearn-sampling-filter",
         cache_size: int = 1,
     ) -> None:
         """Initializes the `ImblearnResamplingFilter` with the given `imblearn` sampler and target column.
 
         The `imblearn` sampler should be a sample object that inherits from `BaseSampler`.
         For example, `imblearn.under_sampling.RandomUnderSampler`. Refer to the `imblearn` documentation for more
         information (https://imbalanced-learn.org/stable/introduction.html).
 
         Args:
             sampler: The `imblearn` sampler to be used for sampling.
             target_column: The target column to be used for sampling.
             random_state: The random state to be used for reproducibility, and will recursively set the random state
                 of the sampler and all nested objects if set.
-            enable_logging: If set to True, enables logging.
+            verbosity: The verbosity level of the logger.
             cache_directory: The target directory where the filtered dataframes are to be saved.
             cache_size: The maximum number of cache entries.
 
         Examples:
             >>> import vaex
             >>> from imblearn.under_sampling import RandomUnderSampler
             >>> from mleko.data.filter import ImblearnUnderSamplingFilter
@@ -66,14 +67,15 @@
                 1    2    5
         """
         super().__init__(cache_directory, cache_size)
         self._sampler = sampler
         self._target_column = target_column
         self._random_state = random_state
         self._reset_random_state()
+        logger.set_level(verbosity)
 
     def filter(
         self,
         data_schema: DataSchema,
         dataframe: vaex.DataFrame,
         cache_group: str | None = None,
         force_recompute: bool = False,
```

### Comparing `mleko-2.2.0/mleko/dataset/ingest/__init__.py` & `mleko-3.0.0/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/ingest/base_ingester.py` & `mleko-3.0.0/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-3.0.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-3.0.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/split/__init__.py` & `mleko-3.0.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/split/base_splitter.py` & `mleko-3.0.0/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/split/expression_splitter.py` & `mleko-3.0.0/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/split/random_splitter.py` & `mleko-3.0.0/mleko/dataset/split/random_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/transform/__init__.py` & `mleko-3.0.0/mleko/dataset/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/transform/base_transformer.py` & `mleko-3.0.0/mleko/dataset/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/transform/composite_transformer.py` & `mleko-3.0.0/mleko/dataset/transform/composite_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-3.0.0/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-3.0.0/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         Returns:
             Updated data schema and fitted transformer.
         """
         logger.info(f"Fitting label encoder transformer ({len(self._features)}): {self._features}.")
         for feature in self._features:
             self._ensure_valid_feature_type(feature, data_schema, dataframe)
-            labels = get_column(dataframe, feature).unique(dropna=True)
+            labels: list[str] = get_column(dataframe, feature).unique(dropna=True)  # type: ignore
             if not self._fit_using_label_dict(feature, labels):
                 logger.info(f"Assigning mappings for feature {feature!r}: {labels}.")
                 self._transformer[feature] = {label: i for i, label in enumerate(labels)}
                 self._transformer[feature][None] = -1 if self._encode_null else None
 
         return data_schema, self._transformer
```

### Comparing `mleko-2.2.0/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-3.0.0/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/dataset/transform/min_max_scaler_transformer.py` & `mleko-3.0.0/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/model/base_model.py` & `mleko-3.0.0/mleko/model/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Module for the base model class."""
 
 from __future__ import annotations
 
-import json
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Dict, Hashable, Union
 
 import vaex
 
 from mleko.cache.fingerprinters import DictFingerprinter, VaexFingerprinter
@@ -116,16 +115,22 @@
             ...     },
             ... }
         """
         model, metrics = self._cached_execute(
             lambda_func=lambda: self._fit(data_schema, train_dataframe, validation_dataframe, hyperparameters),
             cache_key_inputs=[
                 self._fingerprint(),
-                json.dumps(self._hyperparameters, sort_keys=True),
-                json.dumps(hyperparameters, sort_keys=True),
+                (
+                    (
+                        {**self._hyperparameters, **hyperparameters}
+                        if hyperparameters is not None
+                        else self._hyperparameters
+                    ),
+                    DictFingerprinter(),
+                ),
                 (data_schema.to_dict(), DictFingerprinter()),
                 (train_dataframe, VaexFingerprinter()),
                 (validation_dataframe, VaexFingerprinter()) if validation_dataframe is not None else "None",
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=JOBLIB_CACHE_HANDLER,
@@ -162,15 +167,15 @@
             logger.error(msg)
             raise RuntimeError(msg)
 
         return self._cached_execute(
             lambda_func=lambda: self._transform(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                json.dumps(self._hyperparameters, sort_keys=True),
+                (self._hyperparameters, DictFingerprinter()),
                 (data_schema.to_dict(), DictFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=VAEX_DATAFRAME_CACHE_HANDLER,
             disable_cache=disable_cache,
@@ -218,16 +223,22 @@
         """
         model, metrics, df_train, df_validation = self._cached_execute(
             lambda_func=lambda: self._fit_transform(
                 data_schema, train_dataframe, validation_dataframe, hyperparameters
             ),
             cache_key_inputs=[
                 self._fingerprint(),
-                json.dumps(self._hyperparameters, sort_keys=True),
-                json.dumps(hyperparameters, sort_keys=True),
+                (
+                    (
+                        {**self._hyperparameters, **hyperparameters}
+                        if hyperparameters is not None
+                        else self._hyperparameters
+                    ),
+                    DictFingerprinter(),
+                ),
                 (data_schema.to_dict(), DictFingerprinter()),
                 (train_dataframe, VaexFingerprinter()),
                 (validation_dataframe, VaexFingerprinter()) if validation_dataframe is not None else None,
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=[
```

### Comparing `mleko-2.2.0/mleko/model/tune/base_tuner.py` & `mleko-3.0.0/mleko/model/tune/base_tuner.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/model/tune/optuna_tuner.py` & `mleko-3.0.0/mleko/model/tune/optuna_tuner.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/__init__.py` & `mleko-3.0.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/data_container.py` & `mleko-3.0.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/pipeline.py` & `mleko-3.0.0/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/pipeline_step.py` & `mleko-3.0.0/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/__init__.py` & `mleko-3.0.0/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/convert_step.py` & `mleko-3.0.0/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-3.0.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/filter_step.py` & `mleko-3.0.0/mleko/pipeline/steps/filter_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/ingest_step.py` & `mleko-3.0.0/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/model_step.py` & `mleko-3.0.0/mleko/pipeline/steps/model_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/split_step.py` & `mleko-3.0.0/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/transform_step.py` & `mleko-3.0.0/mleko/pipeline/steps/transform_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/pipeline/steps/tune_step.py` & `mleko-3.0.0/mleko/pipeline/steps/tune_step.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/utils/__init__.py` & `mleko-3.0.0/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/utils/custom_logger.py` & `mleko-3.0.0/mleko/utils/custom_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,17 @@
             exc_info: Exception information to log.
             stack_info: Whether to add stack information to the log message.
             stacklevel: Level in the stack frame to log the origin of this log record.
             extra: Additional information to log.
         """
         target_stacklevel = stacklevel + 1
         if not isinstance(message, str):
+            if log_level < self.level:  # pragma: no cover
+                return
+
             self.log(
                 log_level,
                 message,
                 *args,
                 exc_info=exc_info,
                 stack_info=stack_info,
                 stacklevel=target_stacklevel,
@@ -264,24 +267,30 @@
 
         match = re.search(r"\[(Debug|Info|Warning|Error|Critical)\]", message, re.IGNORECASE)
 
         if match:
             level_str = match.group(1).upper()
             routed_level = getattr(logging, level_str)
             cleaned_msg = re.sub(rf"\[{level_str}\]\s?", "", message, flags=re.IGNORECASE, count=1)
+            if routed_level < self.level:  # pragma: no cover
+                return
+
             self.log(
                 routed_level,
                 cleaned_msg,
                 *args,
                 exc_info=exc_info,
                 stack_info=stack_info,
                 stacklevel=target_stacklevel,
                 extra=extra,
             )
         else:
+            if log_level < self.level:  # pragma: no cover
+                return
+
             self.log(
                 log_level,
                 message,
                 *args,
                 exc_info=exc_info,
                 stack_info=stack_info,
                 stacklevel=target_stacklevel,
```

### Comparing `mleko-2.2.0/mleko/utils/decorators.py` & `mleko-3.0.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/utils/file_helpers.py` & `mleko-3.0.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/utils/tqdm_helpers.py` & `mleko-3.0.0/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/mleko/utils/vaex_helpers.py` & `mleko-3.0.0/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-2.2.0/pyproject.toml` & `mleko-3.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "2.2.0"
+version = "3.0.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/klarna-incubator/mleko"
 repository = "https://github.com/klarna-incubator/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-2.2.0/PKG-INFO` & `mleko-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 2.2.0
+Version: 3.0.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/klarna-incubator/mleko
 License: Apache-2.0
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.1,<3.11.dev0
 Classifier: Development Status :: 4 - Beta
```

