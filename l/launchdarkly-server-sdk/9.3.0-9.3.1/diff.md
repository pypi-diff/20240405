# Comparing `tmp/launchdarkly_server_sdk-9.3.0.tar.gz` & `tmp/launchdarkly_server_sdk-9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchdarkly_server_sdk-9.3.0.tar", max compression
+gzip compressed data, was "launchdarkly_server_sdk-9.3.1.tar", max compression
```

## Comparing `launchdarkly_server_sdk-9.3.0.tar` & `launchdarkly_server_sdk-9.3.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0      556 2024-03-14 17:32:11.465419 launchdarkly_server_sdk-9.3.0/LICENSE.txt
--rw-r--r--   0        0        0     4706 2024-03-14 17:32:11.465419 launchdarkly_server_sdk-9.3.0/README.md
--rw-r--r--   0        0        0     3152 2024-03-14 17:32:11.465419 launchdarkly_server_sdk-9.3.0/ldclient/__init__.py
--rw-r--r--   0        0        0    29033 2024-03-14 17:32:11.465419 launchdarkly_server_sdk-9.3.0/ldclient/client.py
--rw-r--r--   0        0        0    21742 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/config.py
--rw-r--r--   0        0        0    40947 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/context.py
--rw-r--r--   0        0        0     8450 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/evaluation.py
--rw-r--r--   0        0        0     8126 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/feature_store.py
--rw-r--r--   0        0        0     6186 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/feature_store_helpers.py
--rw-r--r--   0        0        0       76 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/__init__.py
--rw-r--r--   0        0        0     5323 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/big_segments.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/__init__.py
--rw-r--r--   0        0        0     1932 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/feature_requester.py
--rw-r--r--   0        0        0     4188 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/polling.py
--rw-r--r--   0        0        0     6268 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/status.py
--rw-r--r--   0        0        0    10847 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/streaming.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/datastore/__init__.py
--rw-r--r--   0        0        0     1767 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/datastore/status.py
--rw-r--r--   0        0        0     4548 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/dependency_tracker.py
--rw-r--r--   0        0        0    22768 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/events/__init__.py
--rw-r--r--   0        0        0     4678 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/events/diagnostics.py
--rw-r--r--   0        0        0     4674 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/events/event_context_formatter.py
--rw-r--r--   0        0        0    22719 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/events/event_processor.py
--rw-r--r--   0        0        0     3384 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/events/event_summarizer.py
--rw-r--r--   0        0        0     7096 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/events/types.py
--rw-r--r--   0        0        0     1916 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/fixed_thread_pool.py
--rw-r--r--   0        0        0     1691 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/flag_tracker.py
--rw-r--r--   0        0        0     3122 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/http.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/consul/__init__.py
--rw-r--r--   0        0        0     5727 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/consul/consul_feature_store.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/dynamodb/__init__.py
--rw-r--r--   0        0        0     2782 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/dynamodb/dynamodb_big_segment_store.py
--rw-r--r--   0        0        0     8515 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/dynamodb/dynamodb_feature_store.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/files/__init__.py
--rw-r--r--   0        0        0     7928 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/files/file_data_source.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/redis/__init__.py
--rw-r--r--   0        0        0     2196 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/redis/redis_big_segment_store.py
--rw-r--r--   0        0        0     4256 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/redis/redis_feature_store.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/test_data/__init__.py
--rw-r--r--   0        0        0      969 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/test_data/test_data_source.py
--rw-r--r--   0        0        0     1155 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/listeners.py
--rw-r--r--   0        0        0      897 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/lru_cache.py
--rw-r--r--   0        0        0      154 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/__init__.py
--rw-r--r--   0        0        0     3322 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/attribute_ref.py
--rw-r--r--   0        0        0     2546 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/clause.py
--rw-r--r--   0        0        0      505 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/encoder.py
--rw-r--r--   0        0        0     4057 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/entity.py
--rw-r--r--   0        0        0     5798 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/feature_flag.py
--rw-r--r--   0        0        0     4105 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/segment.py
--rw-r--r--   0        0        0     2189 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/value_parsing.py
--rw-r--r--   0        0        0     2142 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/model/variation_or_rollout.py
--rw-r--r--   0        0        0     5015 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/operators.py
--rw-r--r--   0        0        0     1691 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/repeating_task.py
--rw-r--r--   0        0        0     1111 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/rwlock.py
--rw-r--r--   0        0        0      503 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/sampler.py
--rw-r--r--   0        0        0      655 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/stubs.py
--rw-r--r--   0        0        0     7421 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/impl/util.py
--rw-r--r--   0        0        0    14255 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/integrations/__init__.py
--rw-r--r--   0        0        0    27679 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/integrations/test_data.py
--rw-r--r--   0        0        0    41033 2024-03-14 17:32:11.469419 launchdarkly_server_sdk-9.3.0/ldclient/interfaces.py
--rw-r--r--   0        0        0      296 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/ldclient/migrations/__init__.py
--rw-r--r--   0        0        0    13756 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/ldclient/migrations/migrator.py
--rw-r--r--   0        0        0     8524 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/ldclient/migrations/tracker.py
--rw-r--r--   0        0        0     7206 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/ldclient/migrations/types.py
--rw-r--r--   0        0        0        1 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/ldclient/py.typed
--rw-r--r--   0        0        0       45 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/ldclient/version.py
--rw-r--r--   0        0        0     2993 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/ldclient/versioned_data_kind.py
--rw-r--r--   0        0        0     2504 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/pyproject.toml
--rw-r--r--   0        0        0       56 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/__init__.py
--rw-r--r--   0        0        0     7914 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/builders.py
--rw-r--r--   0        0        0     5136 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/feature_store_test_base.py
--rw-r--r--   0        0        0     6002 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/http_util.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/datasource/__init__.py
--rw-r--r--   0        0        0     5408 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/datasource/test_feature_requester.py
--rw-r--r--   0        0        0     4767 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/datasource/test_polling_processor.py
--rw-r--r--   0        0        0    18044 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/datasource/test_streaming.py
--rw-r--r--   0        0        0     3007 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/evaluator_util.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/events/__init__.py
--rw-r--r--   0        0        0     6606 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/events/test_diagnostics.py
--rw-r--r--   0        0        0     3732 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/events/test_event_context_formatter.py
--rw-r--r--   0        0        0     2658 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/events/test_event_factory.py
--rw-r--r--   0        0        0    34501 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/events/test_event_processor.py
--rw-r--r--   0        0        0     1978 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/events/test_event_summarizer.py
--rw-r--r--   0        0        0     1815 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_attribute_ref.py
--rw-r--r--   0        0        0     7183 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_big_segments.py
--rw-r--r--   0        0        0    11415 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_data_sink.py
--rw-r--r--   0        0        0     6025 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator.py
--rw-r--r--   0        0        0     3769 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_big_segment.py
--rw-r--r--   0        0        0     5874 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_bucketing.py
--rw-r--r--   0        0        0     3295 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_clause.py
--rw-r--r--   0        0        0     3944 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_prerequisites.py
--rw-r--r--   0        0        0     7093 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_segment.py
--rw-r--r--   0        0        0     3595 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_target.py
--rw-r--r--   0        0        0     2396 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_flag_tracker.py
--rw-r--r--   0        0        0     1145 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_listeners.py
--rw-r--r--   0        0        0     1009 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_lru_cache.py
--rw-r--r--   0        0        0     2115 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_model_decode.py
--rw-r--r--   0        0        0      403 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_model_encoder.py
--rw-r--r--   0        0        0     4508 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_operators.py
--rw-r--r--   0        0        0     1477 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_repeating_task.py
--rw-r--r--   0        0        0      678 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/impl/test_sampler.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/integrations/__init__.py
--rw-r--r--   0        0        0     4483 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/integrations/big_segment_store_test_base.py
--rw-r--r--   0        0        0     4377 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/integrations/persistent_feature_store_test_base.py
--rw-r--r--   0        0        0     1564 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/integrations/test_consul.py
--rw-r--r--   0        0        0     7245 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/integrations/test_dynamodb.py
--rw-r--r--   0        0        0     4554 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/integrations/test_redis.py
--rw-r--r--   0        0        0    14039 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/integrations/test_test_data_source.py
--rw-r--r--   0        0        0        0 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/migrations/__init__.py
--rw-r--r--   0        0        0    20199 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/migrations/test_migrator.py
--rw-r--r--   0        0        0     2195 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/migrations/test_migrator_builder.py
--rw-r--r--   0        0        0    10674 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/migrations/test_op_tracker.py
--rw-r--r--   0        0        0     1453 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/mock_components.py
--rw-r--r--   0        0        0     3092 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/proxy_test_util.py
--rw-r--r--   0        0        0      227 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/selfsigned.key
--rw-r--r--   0        0        0      554 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/selfsigned.pem
--rw-r--r--   0        0        0     4831 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/stub_util.py
--rw-r--r--   0        0        0      377 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/sync_util.py
--rw-r--r--   0        0        0     2674 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_config.py
--rw-r--r--   0        0        0    12587 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_context.py
--rw-r--r--   0        0        0     2653 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_feature_store_client_wrapper.py
--rw-r--r--   0        0        0    12727 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_feature_store_helpers.py
--rw-r--r--   0        0        0     9134 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_file_data_source.py
--rw-r--r--   0        0        0     3127 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_flags_state.py
--rw-r--r--   0        0        0      653 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_in_memory_feature_store.py
--rw-r--r--   0        0        0      787 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_init.py
--rw-r--r--   0        0        0     7293 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_ldclient.py
--rw-r--r--   0        0        0     6899 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_ldclient_end_to_end.py
--rw-r--r--   0        0        0    13214 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_ldclient_evaluation.py
--rw-r--r--   0        0        0    11139 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_ldclient_events.py
--rw-r--r--   0        0        0     2621 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_ldclient_listeners.py
--rw-r--r--   0        0        0     2330 2024-03-14 17:32:11.473419 launchdarkly_server_sdk-9.3.0/testing/test_ldclient_migration_variation.py
--rw-r--r--   0        0        0     2779 2024-03-14 17:32:11.477419 launchdarkly_server_sdk-9.3.0/testing/test_ldclient_singleton.py
--rw-r--r--   0        0        0     1080 2024-03-14 17:32:11.477419 launchdarkly_server_sdk-9.3.0/testing/test_util.py
--rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 launchdarkly_server_sdk-9.3.0/PKG-INFO
+-rw-r--r--   0        0        0      556 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     4706 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/README.md
+-rw-r--r--   0        0        0     3152 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/__init__.py
+-rw-r--r--   0        0        0    29033 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/client.py
+-rw-r--r--   0        0        0    21742 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/config.py
+-rw-r--r--   0        0        0    40947 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/context.py
+-rw-r--r--   0        0        0     8450 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/evaluation.py
+-rw-r--r--   0        0        0     8126 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/feature_store.py
+-rw-r--r--   0        0        0     6186 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/feature_store_helpers.py
+-rw-r--r--   0        0        0       76 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/__init__.py
+-rw-r--r--   0        0        0     5323 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/big_segments.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/feature_requester.py
+-rw-r--r--   0        0        0     4188 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/polling.py
+-rw-r--r--   0        0        0     6268 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/status.py
+-rw-r--r--   0        0        0    10847 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/streaming.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/datastore/__init__.py
+-rw-r--r--   0        0        0     1767 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/datastore/status.py
+-rw-r--r--   0        0        0     4548 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/dependency_tracker.py
+-rw-r--r--   0        0        0    22768 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/evaluator.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/events/__init__.py
+-rw-r--r--   0        0        0     4678 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/events/diagnostics.py
+-rw-r--r--   0        0        0     4674 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/events/event_context_formatter.py
+-rw-r--r--   0        0        0    22719 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/events/event_processor.py
+-rw-r--r--   0        0        0     3384 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/events/event_summarizer.py
+-rw-r--r--   0        0        0     7096 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/events/types.py
+-rw-r--r--   0        0        0     1916 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/fixed_thread_pool.py
+-rw-r--r--   0        0        0     1691 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/flag_tracker.py
+-rw-r--r--   0        0        0     3122 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/http.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/consul/__init__.py
+-rw-r--r--   0        0        0     5727 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/consul/consul_feature_store.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/dynamodb/__init__.py
+-rw-r--r--   0        0        0     2782 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/dynamodb/dynamodb_big_segment_store.py
+-rw-r--r--   0        0        0     8515 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/dynamodb/dynamodb_feature_store.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/files/__init__.py
+-rw-r--r--   0        0        0     7928 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/files/file_data_source.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.357473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/redis/__init__.py
+-rw-r--r--   0        0        0     2196 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/redis/redis_big_segment_store.py
+-rw-r--r--   0        0        0     4256 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/redis/redis_feature_store.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/test_data/__init__.py
+-rw-r--r--   0        0        0      969 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/test_data/test_data_source.py
+-rw-r--r--   0        0        0     1155 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/listeners.py
+-rw-r--r--   0        0        0      897 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/lru_cache.py
+-rw-r--r--   0        0        0      154 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/__init__.py
+-rw-r--r--   0        0        0     3322 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/attribute_ref.py
+-rw-r--r--   0        0        0     2546 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/clause.py
+-rw-r--r--   0        0        0      505 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/encoder.py
+-rw-r--r--   0        0        0     4057 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/entity.py
+-rw-r--r--   0        0        0     5798 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/feature_flag.py
+-rw-r--r--   0        0        0     4105 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/segment.py
+-rw-r--r--   0        0        0     2189 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/value_parsing.py
+-rw-r--r--   0        0        0     2142 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/model/variation_or_rollout.py
+-rw-r--r--   0        0        0     5015 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/operators.py
+-rw-r--r--   0        0        0     1691 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/repeating_task.py
+-rw-r--r--   0        0        0     1111 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/rwlock.py
+-rw-r--r--   0        0        0      503 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/sampler.py
+-rw-r--r--   0        0        0      655 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/stubs.py
+-rw-r--r--   0        0        0     7421 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/impl/util.py
+-rw-r--r--   0        0        0    14255 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/integrations/__init__.py
+-rw-r--r--   0        0        0    27679 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/integrations/test_data.py
+-rw-r--r--   0        0        0    41033 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/interfaces.py
+-rw-r--r--   0        0        0      296 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/migrations/__init__.py
+-rw-r--r--   0        0        0    13756 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/migrations/migrator.py
+-rw-r--r--   0        0        0     8524 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/migrations/tracker.py
+-rw-r--r--   0        0        0     7206 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/migrations/types.py
+-rw-r--r--   0        0        0        1 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/py.typed
+-rw-r--r--   0        0        0       56 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/__init__.py
+-rw-r--r--   0        0        0     7914 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/builders.py
+-rw-r--r--   0        0        0     5133 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/feature_store_test_base.py
+-rw-r--r--   0        0        0     6020 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/http_util.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/datasource/__init__.py
+-rw-r--r--   0        0        0     5426 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/datasource/test_feature_requester.py
+-rw-r--r--   0        0        0     4794 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/datasource/test_polling_processor.py
+-rw-r--r--   0        0        0    18089 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/datasource/test_streaming.py
+-rw-r--r--   0        0        0     3016 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/evaluator_util.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/__init__.py
+-rw-r--r--   0        0        0     6606 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_diagnostics.py
+-rw-r--r--   0        0        0     3732 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_event_context_formatter.py
+-rw-r--r--   0        0        0     2667 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_event_factory.py
+-rw-r--r--   0        0        0    34528 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_event_processor.py
+-rw-r--r--   0        0        0     1987 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_event_summarizer.py
+-rw-r--r--   0        0        0     1815 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_attribute_ref.py
+-rw-r--r--   0        0        0     7152 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_big_segments.py
+-rw-r--r--   0        0        0    11433 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_data_sink.py
+-rw-r--r--   0        0        0     6039 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator.py
+-rw-r--r--   0        0        0     3783 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_big_segment.py
+-rw-r--r--   0        0        0     5868 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_bucketing.py
+-rw-r--r--   0        0        0     3313 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_clause.py
+-rw-r--r--   0        0        0     3962 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_prerequisites.py
+-rw-r--r--   0        0        0     7111 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_segment.py
+-rw-r--r--   0        0        0     3597 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_target.py
+-rw-r--r--   0        0        0     2405 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_flag_tracker.py
+-rw-r--r--   0        0        0     1145 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_listeners.py
+-rw-r--r--   0        0        0     1009 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_lru_cache.py
+-rw-r--r--   0        0        0     2124 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_model_decode.py
+-rw-r--r--   0        0        0      403 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_model_encoder.py
+-rw-r--r--   0        0        0     4517 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_operators.py
+-rw-r--r--   0        0        0     1477 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_repeating_task.py
+-rw-r--r--   0        0        0      678 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_sampler.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/__init__.py
+-rw-r--r--   0        0        0     4483 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/big_segment_store_test_base.py
+-rw-r--r--   0        0        0     4384 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/persistent_feature_store_test_base.py
+-rw-r--r--   0        0        0     1582 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/test_consul.py
+-rw-r--r--   0        0        0     7252 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/test_dynamodb.py
+-rw-r--r--   0        0        0     4577 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/test_redis.py
+-rw-r--r--   0        0        0    14039 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/test_test_data_source.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:25:34.361473 launchdarkly_server_sdk-9.3.1/ldclient/testing/migrations/__init__.py
+-rw-r--r--   0        0        0    20217 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/migrations/test_migrator.py
+-rw-r--r--   0        0        0     2195 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/migrations/test_migrator_builder.py
+-rw-r--r--   0        0        0    10692 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/migrations/test_op_tracker.py
+-rw-r--r--   0        0        0     1453 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/mock_components.py
+-rw-r--r--   0        0        0     3101 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/proxy_test_util.py
+-rw-r--r--   0        0        0      227 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/selfsigned.key
+-rw-r--r--   0        0        0      554 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/selfsigned.pem
+-rw-r--r--   0        0        0     4840 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/stub_util.py
+-rw-r--r--   0        0        0      377 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/sync_util.py
+-rw-r--r--   0        0        0     2674 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_config.py
+-rw-r--r--   0        0        0    12587 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_context.py
+-rw-r--r--   0        0        0     2653 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_feature_store_client_wrapper.py
+-rw-r--r--   0        0        0    12727 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_feature_store_helpers.py
+-rw-r--r--   0        0        0     9152 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_file_data_source.py
+-rw-r--r--   0        0        0     3127 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_flags_state.py
+-rw-r--r--   0        0        0      662 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_in_memory_feature_store.py
+-rw-r--r--   0        0        0      787 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_init.py
+-rw-r--r--   0        0        0     7311 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient.py
+-rw-r--r--   0        0        0     6926 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_end_to_end.py
+-rw-r--r--   0        0        0    13250 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_evaluation.py
+-rw-r--r--   0        0        0    11166 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_events.py
+-rw-r--r--   0        0        0     2648 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_listeners.py
+-rw-r--r--   0        0        0     2348 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_migration_variation.py
+-rw-r--r--   0        0        0     2806 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_singleton.py
+-rw-r--r--   0        0        0     1080 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/testing/test_util.py
+-rw-r--r--   0        0        0       45 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/version.py
+-rw-r--r--   0        0        0     2993 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/ldclient/versioned_data_kind.py
+-rw-r--r--   0        0        0     2536 2024-04-05 14:25:34.365473 launchdarkly_server_sdk-9.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 launchdarkly_server_sdk-9.3.1/PKG-INFO
```

### Comparing `launchdarkly_server_sdk-9.3.0/LICENSE.txt` & `launchdarkly_server_sdk-9.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/README.md` & `launchdarkly_server_sdk-9.3.1/README.md`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/__init__.py` & `launchdarkly_server_sdk-9.3.1/ldclient/__init__.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/client.py` & `launchdarkly_server_sdk-9.3.1/ldclient/client.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/config.py` & `launchdarkly_server_sdk-9.3.1/ldclient/config.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/context.py` & `launchdarkly_server_sdk-9.3.1/ldclient/context.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/evaluation.py` & `launchdarkly_server_sdk-9.3.1/ldclient/evaluation.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/feature_store.py` & `launchdarkly_server_sdk-9.3.1/ldclient/feature_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/feature_store_helpers.py` & `launchdarkly_server_sdk-9.3.1/ldclient/feature_store_helpers.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/big_segments.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/big_segments.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/feature_requester.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/feature_requester.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/polling.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/polling.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/status.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/status.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/datasource/streaming.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/datasource/streaming.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/datastore/status.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/datastore/status.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/dependency_tracker.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/dependency_tracker.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/evaluator.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/evaluator.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/events/diagnostics.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/events/diagnostics.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/events/event_context_formatter.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/events/event_context_formatter.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/events/event_processor.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/events/event_processor.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/events/event_summarizer.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/events/event_summarizer.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/events/types.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/events/types.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/fixed_thread_pool.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/fixed_thread_pool.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/flag_tracker.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/flag_tracker.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/http.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/http.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/consul/consul_feature_store.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/consul/consul_feature_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/dynamodb/dynamodb_big_segment_store.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/dynamodb/dynamodb_big_segment_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/dynamodb/dynamodb_feature_store.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/dynamodb/dynamodb_feature_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/files/file_data_source.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/files/file_data_source.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/redis/redis_big_segment_store.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/redis/redis_big_segment_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/redis/redis_feature_store.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/redis/redis_feature_store.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/integrations/test_data/test_data_source.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/integrations/test_data/test_data_source.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/listeners.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/listeners.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/lru_cache.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/lru_cache.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/model/attribute_ref.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/model/attribute_ref.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/model/clause.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/model/clause.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/model/entity.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/model/entity.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/model/feature_flag.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/model/feature_flag.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/model/segment.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/model/segment.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/model/value_parsing.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/model/value_parsing.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/model/variation_or_rollout.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/model/variation_or_rollout.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/operators.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/operators.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/repeating_task.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/repeating_task.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/rwlock.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/rwlock.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/stubs.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/stubs.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/impl/util.py` & `launchdarkly_server_sdk-9.3.1/ldclient/impl/util.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/integrations/__init__.py` & `launchdarkly_server_sdk-9.3.1/ldclient/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/integrations/test_data.py` & `launchdarkly_server_sdk-9.3.1/ldclient/integrations/test_data.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/interfaces.py` & `launchdarkly_server_sdk-9.3.1/ldclient/interfaces.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/migrations/migrator.py` & `launchdarkly_server_sdk-9.3.1/ldclient/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/migrations/tracker.py` & `launchdarkly_server_sdk-9.3.1/ldclient/migrations/tracker.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/migrations/types.py` & `launchdarkly_server_sdk-9.3.1/ldclient/migrations/types.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/ldclient/versioned_data_kind.py` & `launchdarkly_server_sdk-9.3.1/ldclient/versioned_data_kind.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/pyproject.toml` & `launchdarkly_server_sdk-9.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "launchdarkly-server-sdk"
-version = "9.3.0"
+version = "9.3.1"
 description = "LaunchDarkly SDK for Python"
 authors = ["LaunchDarkly <dev@launchdarkly.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://docs.launchdarkly.com/sdk/server-side/python"
 repository = "https://github.com/launchdarkly/python-server-sdk"
 documentation = "https://launchdarkly-python-sdk.readthedocs.io/en/latest/"
@@ -17,17 +17,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
 ]
-packages = [
-    { include = "ldclient" },
-    { include = "testing" },
+packages = [ { include = "ldclient" } ]
+exclude = [
+    { path = "ldclient/testing", format = "wheel" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 certifi = ">=2018.4.16"
 expiringdict = ">=1.1.4"
 pyRFC3339 = ">=1.0"
@@ -47,15 +47,15 @@
 dynamodb = ["boto3"]
 test-filesource = ["pyyaml", "watchdog"]
 
 
 [tool.poetry.group.dev.dependencies]
 mock = ">=2.0.0"
 pytest = ">=2.8"
-redis = ">=2.10.5,<3.0.0"
+redis = ">=2.10.5,<5.0.0"
 boto3 = ">=1.9.71,<2.0.0"
 coverage = ">=4.4"
 jsonpickle = ">1.4.1"
 pytest-cov = ">=2.4.0"
 pytest-mypy = "==0.10.3"
 mypy = "==1.8.0"
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/builders.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/builders.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/feature_store_test_base.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/feature_store_test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ldclient.interfaces import FeatureStore
 from ldclient.versioned_data_kind import FEATURES
 
-from testing.builders import *
+from ldclient.testing.builders import *
 
 from abc import abstractmethod
 import pytest
 
 # The basic test suite to be run against all feature store implementations.
 #
 # FeatureStoreTestBase and FeatureStoreTester are used only by test_in_memory_feature_store. For all
@@ -17,19 +17,19 @@
     def create_feature_store(self) -> FeatureStore:
         pass
 
 
 class StoreTestScope:
     def __init__(self, store: FeatureStore):
         self.__store = store
-    
+
     @property
     def store(self) -> FeatureStore:
         return self.__store
-    
+
     # These magic methods allow the scope to be automatically cleaned up in a "with" block
     def __enter__(self):
         return self.__store
 
     def __exit__(self, type, value, traceback):
         if hasattr(self.store, "stop"):  # stop was not originally required for all feature store implementations
             self.__store.stop()
@@ -55,15 +55,15 @@
         scope.store.init({
             FEATURES: {
                 'foo': self.make_feature('foo', 10).to_json_dict(),
                 'bar': self.make_feature('bar', 10).to_json_dict(),
             }
         })
         return scope
-    
+
     @staticmethod
     def make_feature(key, ver):
         return FlagBuilder(key).version(ver).on(True).variations(True, False).salt('abc').build()
 
     def test_not_initialized_before_init(self, tester):
         with self.store(tester) as store:
             assert store.initialized is False
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/http_util.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/http_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def __init__(self, port, secure):
         Thread.__init__(self)
         self.port = port
         self.uri = '%s://localhost:%d' % ('https' if secure else 'http', port)
         self.server = HTTPServer(('localhost', port), MockServerRequestHandler)
         if secure:
             context = SSLContext(PROTOCOL_TLSv1_2)
-            context.load_cert_chain('./testing/selfsigned.pem', './testing/selfsigned.key')
+            context.load_cert_chain('./ldclient/testing/selfsigned.pem', './ldclient/testing/selfsigned.key')
             self.server.socket = context.wrap_socket(
                 self.server.socket,
                 server_side=True
             )
         self.server.server_wrapper = self
         self.matchers = {}
         self.requests = queue.Queue()
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/datasource/test_feature_requester.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/datasource/test_feature_requester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ldclient.config import Config
 from ldclient.impl.datasource.feature_requester import FeatureRequesterImpl
 from ldclient.version import VERSION
 from ldclient.versioned_data_kind import FEATURES, SEGMENTS
-from testing.http_util import start_server, BasicResponse, JsonResponse
-from testing.proxy_test_util import do_proxy_tests
+from ldclient.testing.http_util import start_server, BasicResponse, JsonResponse
+from ldclient.testing.proxy_test_util import do_proxy_tests
 
 def test_get_all_data_returns_data():
     with start_server() as server:
         config = Config(sdk_key = 'sdk-key', base_uri = server.uri)
         fr = FeatureRequesterImpl(config)
 
         flags = { 'flag1': { 'key': 'flag1' } }
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/datasource/test_polling_processor.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/datasource/test_polling_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from ldclient.impl.datasource.polling import PollingUpdateProcessor
 from ldclient.impl.datasource.status import DataSourceUpdateSinkImpl
 from ldclient.impl.listeners import Listeners
 from ldclient.impl.util import UnsuccessfulResponseException
 from ldclient.interfaces import DataSourceStatus, DataSourceState, DataSourceErrorKind
 from ldclient.versioned_data_kind import FEATURES, SEGMENTS
 
-from testing.builders import *
-from testing.stub_util import MockFeatureRequester, MockResponse
-from testing.test_util import SpyListener
+from ldclient.testing.builders import *
+from ldclient.testing.stub_util import MockFeatureRequester, MockResponse
+from ldclient.testing.test_util import SpyListener
 
 pp = None
 mock_requester = None
 store = None
 ready = None
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/datasource/test_streaming.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/datasource/test_streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from ldclient.impl.events.diagnostics import _DiagnosticAccumulator
 from ldclient.impl.listeners import Listeners
 from ldclient.version import VERSION
 from ldclient.versioned_data_kind import FEATURES, SEGMENTS
 from ldclient.interfaces import DataSourceStatus, DataSourceState, DataSourceErrorKind
 from ldclient.impl.datasource.status import DataSourceUpdateSinkImpl
 
-from testing.builders import *
-from testing.http_util import start_server, BasicResponse, CauseNetworkError, SequentialHandler
-from testing.proxy_test_util import do_proxy_tests
-from testing.stub_util import make_delete_event, make_patch_event, make_put_event, make_invalid_put_event, stream_content
-from testing.test_util import SpyListener
+from ldclient.testing.builders import *
+from ldclient.testing.http_util import start_server, BasicResponse, CauseNetworkError, SequentialHandler
+from ldclient.testing.proxy_test_util import do_proxy_tests
+from ldclient.testing.stub_util import make_delete_event, make_patch_event, make_put_event, make_invalid_put_event, stream_content
+from ldclient.testing.test_util import SpyListener
 
 brief_delay = 0.001
 
 # These long timeouts are necessary because of a problem in the Windows CI environment where HTTP requests to
 # the test server running at localhost tests are *extremely* slow. It looks like a similar issue to what's
 # described at https://stackoverflow.com/questions/2617615/slow-python-http-server-on-localhost but we had no
 # luck with the advice that was given there.
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/evaluator_util.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/evaluator_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ldclient import Context
 from ldclient.evaluation import BigSegmentsStatus
 from ldclient.impl.evaluator import Evaluator, _make_big_segment_ref
 from ldclient.impl.events.types import EventFactory
 from ldclient.impl.model import *
-from testing.builders import *
+from ldclient.testing.builders import *
 
 from typing import Any, Optional, Tuple, Union
 
 basic_user = Context.create('user-key')
 fake_timestamp = 0
 event_factory = EventFactory(False, lambda: fake_timestamp)
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/events/test_diagnostics.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/events/test_event_context_formatter.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_event_context_formatter.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/events/test_event_factory.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_event_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ldclient.context import Context
 from ldclient.evaluation import EvaluationDetail
 from ldclient.impl.events.types import EventFactory
 
-from testing.builders import *
+from ldclient.testing.builders import *
 
 _event_factory_default = EventFactory(False)
 _user = Context.create('x')
 
 def make_basic_flag_with_rules(kind, should_track_events):
     rule_builder = FlagRuleBuilder().rollout({
         'variations': [
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/events/test_event_processor.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_event_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from ldclient.impl.events.event_processor import DefaultEventProcessor
 from ldclient.migrations.types import Operation, Origin, Stage
 from ldclient.migrations.tracker import MigrationOpEvent
 from ldclient.impl.events.types import EventInput, EventInputCustom, EventInputEvaluation, EventInputIdentify
 from ldclient.impl.util import timedelta_millis
 from ldclient.impl.events.event_context_formatter import EventContextFormatter
 
-from testing.builders import *
-from testing.proxy_test_util import do_proxy_tests
-from testing.stub_util import MockHttp
+from ldclient.testing.builders import *
+from ldclient.testing.proxy_test_util import do_proxy_tests
+from ldclient.testing.stub_util import MockHttp
 
 
 default_config = Config("fake_sdk_key")
 context = Context.builder('userkey').name('Red').build()
 flag = FlagBuilder('flagkey').version(2).build()
 flag_with_0_sampling_ratio = FlagBuilder('flagkey').version(3).sampling_ratio(0).build()
 flag_excluded_from_summaries = FlagBuilder('flagkey').version(4).exclude_from_summaries(True).build()
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/events/test_event_summarizer.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/events/test_event_summarizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ldclient.context import Context
 from ldclient.impl.events.event_summarizer import EventSummarizer, EventSummaryCounter, EventSummaryFlag
 from ldclient.impl.events.types import *
 
-from testing.builders import *
+from ldclient.testing.builders import *
 
 
 user = Context.create('user1')
 flag1 = FlagBuilder('flag1').version(11).build()
 flag2 = FlagBuilder('flag2').version(22).build()
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_attribute_ref.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_attribute_ref.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_big_segments.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_big_segments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ldclient.config import BigSegmentsConfig
 from ldclient.evaluation import BigSegmentsStatus
 from ldclient.impl.big_segments import BigSegmentStoreManager, _hash_for_user_key
 from ldclient.interfaces import BigSegmentStoreMetadata
-from testing.mock_components import MockBigSegmentStore
+from ldclient.testing.mock_components import MockBigSegmentStore
 
 from queue import Queue
 import time
 
 user_key = 'user-key'
 user_hash = _hash_for_user_key(user_key)
 
@@ -104,37 +104,37 @@
 
     try:
         result1 = manager.get_user_membership(user_key_1)
         result2 = manager.get_user_membership(user_key_2)
         result3 = manager.get_user_membership(user_key_3)
 
         assert store.membership_queries == [user_hash_1, user_hash_2, user_hash_3]
-        
+
         # Since the capacity is only 2 and user_key_1 was the least recently used, that key should be
         # evicted by the user_key_3 query. Now only user_key_2 and user_key_3 are in the cache, and
         # querying them again should not cause a new query to the store.
         result2a = manager.get_user_membership(user_key_2)
         result3a = manager.get_user_membership(user_key_3)
         assert result2a == result2
         assert result3a == result3
-        
+
         assert store.membership_queries == [user_hash_1, user_hash_2, user_hash_3]
-        
+
         result1a = manager.get_user_membership(user_key_1)
         assert result1a == result1
-        
+
         assert store.membership_queries == [user_hash_1, user_hash_2, user_hash_3, user_hash_1]
     finally:
         manager.stop()
 
 def test_status_polling_detects_store_unavailability():
     store = MockBigSegmentStore()
     store.setup_metadata_always_up_to_date()
     statuses = Queue()
-    
+
     manager = BigSegmentStoreManager(BigSegmentsConfig(store=store, status_poll_interval=0.01))
 
     try:
         manager.status_provider.add_listener(lambda status: statuses.put(status))
 
         status1 = manager.status_provider.status
         assert status1.available == True
@@ -151,15 +151,15 @@
     finally:
         manager.stop()
 
 def test_status_polling_detects_stale_status():
     store = MockBigSegmentStore()
     store.setup_metadata_always_up_to_date()
     statuses = Queue()
-    
+
     manager = BigSegmentStoreManager(BigSegmentsConfig(store=store, status_poll_interval=0.01))
 
     try:
         manager.status_provider.add_listener(lambda status: statuses.put(status))
 
         status1 = manager.status_provider.status
         assert status1.stale == False
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_data_sink.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_data_sink.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from ldclient.impl.datasource.status import DataSourceUpdateSinkImpl
 from ldclient.feature_store import InMemoryFeatureStore
 from ldclient.interfaces import DataSourceState, DataSourceErrorKind
 from ldclient.impl.listeners import Listeners
 from ldclient.versioned_data_kind import FEATURES, SEGMENTS
 
-from testing.test_util import SpyListener
-from testing.builders import FlagBuilder, FlagRuleBuilder, make_clause, SegmentBuilder, SegmentRuleBuilder
+from ldclient.testing.test_util import SpyListener
+from ldclient.testing.builders import FlagBuilder, FlagRuleBuilder, make_clause, SegmentBuilder, SegmentRuleBuilder
 
 
 @pytest.fixture
 def basic_data() -> Dict:
     flag1 = FlagBuilder('flag1').version(1).on(False).build()
     flag2 = FlagBuilder('flag2').version(1).on(False).build()
     flag3 = FlagBuilder('flag3').version(1).rules(
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ldclient.client import Context
 from ldclient.evaluation import EvaluationDetail
-from testing.builders import *
-from testing.impl.evaluator_util import *
+from ldclient.testing.builders import *
+from ldclient.testing.impl.evaluator_util import *
 
 
 def test_flag_returns_off_variation_if_flag_is_off():
     flag = FlagBuilder('feature').on(False).off_variation(1).variations('a', 'b', 'c').build()
     user = Context.create('x')
     detail = EvaluationDetail('b', 1, {'kind': 'OFF'})
     assert_eval_result(basic_evaluator.evaluate(flag, user, event_factory), detail, None)
@@ -96,9 +96,9 @@
 
     assert evaluator.evaluate(flag, user, event_factory).detail.value == True
 
 def test_segment_match_clause_falls_through_with_no_errors_if_segment_not_found():
     user = Context.create('foo')
     flag = make_boolean_flag_with_clauses(make_clause_matching_segment_key('segkey'))
     evaluator = EvaluatorBuilder().with_unknown_segment('segkey').build()
-    
+
     assert evaluator.evaluate(flag, user, event_factory).detail.value == False
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_big_segment.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_big_segment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from ldclient.evaluation import BigSegmentsStatus
-from testing.builders import *
-from testing.impl.evaluator_util import *
+from ldclient.testing.builders import *
+from ldclient.testing.impl.evaluator_util import *
 
 
 def test_big_segment_with_no_generation_is_not_matched():
     segment = SegmentBuilder('key').version(1) \
         .included(basic_user.key) \
         .unbounded(True) \
         .build()
@@ -26,15 +26,15 @@
     _test_matched_with_include(True, True)
 
 def _test_matched_with_include(non_default_kind: bool, multi_kind_context: bool):
     target_key = 'contextkey'
     single_kind_context = Context.create(target_key, 'kind1') if non_default_kind else Context.create(target_key)
     eval_context = Context.create_multi(single_kind_context, Context.create('key2', 'kind2')) if multi_kind_context \
         else single_kind_context
-    
+
     segment = SegmentBuilder('key').version(1) \
         .unbounded(True) \
         .unbounded_context_kind('kind1' if non_default_kind else None) \
         .generation(2) \
         .build()
     flag = make_boolean_flag_matching_segment(segment)
     evaluator = EvaluatorBuilder().with_segment(segment).with_big_segment_for_key(target_key, segment, True).build()
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_bucketing.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_bucketing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ldclient.client import Context
 from ldclient.impl.evaluator import _bucket_context, _variation_index_for_context
 from ldclient.impl.model import *
 
-from testing.builders import *
-from testing.impl.evaluator_util import *
+from ldclient.testing.builders import *
+from ldclient.testing.impl.evaluator_util import *
 
 import math
 import pytest
 
 
 def assert_match_clause(clause: dict, context: Context, should_match: bool):
     assert_match(basic_evaluator, make_boolean_flag_with_clauses(clause), context, should_match)
@@ -18,15 +18,15 @@
         user = Context.create('userkey')
         flag = FlagBuilder('key').salt('salt').build()
 
         # First verify that with our test inputs, the bucket value will be greater than zero and less than 100000,
         # so we can construct a rollout whose second bucket just barely contains that value
         bucket_value = math.trunc(_bucket_context(None, user, None, flag.key, flag.salt, None) * 100000)
         assert bucket_value > 0 and bucket_value < 100000
-        
+
         bad_variation_a = 0
         matched_variation = 1
         bad_variation_b = 2
         rule = VariationOrRollout({
             'rollout': {
                 'variations': [
                     { 'variation': bad_variation_a, 'weight': bucket_value }, # end of bucket range is not inclusive, so it will *not* match the target value
@@ -40,25 +40,25 @@
 
     def test_last_bucket_is_used_if_bucket_value_equals_total_weight(self):
         user = Context.create('userkey')
         flag = FlagBuilder('key').salt('salt').build()
 
         # We'll construct a list of variations that stops right at the target bucket value
         bucket_value = math.trunc(_bucket_context(None, user, None, flag.key, flag.salt, None) * 100000)
-        
+
         rule = VariationOrRollout({
             'rollout': {
                 'variations': [
                     { 'variation': 0, 'weight': bucket_value }
                 ]
             }
         })
         result_variation = _variation_index_for_context(flag, rule, user)
         assert result_variation == (0, False)
-        
+
     def test_bucket_by_user_key(self):
         user = Context.create('userKeyA')
         bucket = _bucket_context(None, user, None, 'hashKey', 'saltyA', None)
         assert bucket == pytest.approx(0.42157587)
 
         user = Context.create('userKeyB')
         bucket = _bucket_context(None, user, None, 'hashKey', 'saltyA', None)
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_clause.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_clause.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ldclient.client import Context
-from testing.builders import *
-from testing.impl.evaluator_util import *
+from ldclient.testing.builders import *
+from ldclient.testing.impl.evaluator_util import *
 
 
 def assert_match_clause(clause: dict, context: Context, should_match: bool):
     assert_match(basic_evaluator, make_boolean_flag_with_clauses(clause), context, should_match)
 
 
 class TestEvaluatorClause:
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_prerequisites.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_prerequisites.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from ldclient.client import Context
 from ldclient.evaluation import EvaluationDetail
 from ldclient.impl.events.types import EventInputEvaluation
 
-from testing.builders import *
-from testing.impl.evaluator_util import *
+from ldclient.testing.builders import *
+from ldclient.testing.impl.evaluator_util import *
 
 
 def test_flag_returns_off_variation_if_prerequisite_not_found():
     flag = FlagBuilder('feature').on(True).off_variation(1).variations('a', 'b', 'c').fallthrough_variation(1) \
         .prerequisite('badfeature', 1).build()
     evaluator = EvaluatorBuilder().with_unknown_flag('badfeature').build()
     user = Context.create('x')
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_segment.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from ldclient import Context
 from ldclient.impl.evaluator import _bucket_context
-from testing.builders import *
-from testing.impl.evaluator_util import *
+from ldclient.testing.builders import *
+from ldclient.testing.impl.evaluator_util import *
 
 
 def _segment_matches_context(segment: Segment, context: Context) -> bool:
     e = EvaluatorBuilder().with_segment(segment).build()
     flag = make_boolean_flag_matching_segment(segment)
     result = e.evaluate(flag, context, event_factory)
     return result.detail.value
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_evaluator_target.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_evaluator_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ldclient.client import Context
-from testing.builders import *
-from testing.impl.evaluator_util import *
+from ldclient.testing.builders import *
+from ldclient.testing.impl.evaluator_util import *
 
 
 FALLTHROUGH_VAR = 0
 MATCH_VAR_1 = 1
 MATCH_VAR_2 = 2
 VARIATIONS = ['fallthrough', 'match1', 'match2']
 
@@ -30,15 +30,15 @@
 
 class TestEvaluatorTarget:
     def test_user_targets_only(self):
         flag = base_flag_builder() \
             .target(MATCH_VAR_1, 'c') \
             .target(MATCH_VAR_2, 'b', 'a') \
             .build()
-        
+
         expect_match(flag, Context.create('a'), MATCH_VAR_2)
         expect_match(flag, Context.create('b'), MATCH_VAR_2)
         expect_match(flag, Context.create('c'), MATCH_VAR_1)
         expect_fallthrough(flag, Context.create('z'))
 
         # in a multi-kind context, these targets match only the key for the user kind
         expect_match(flag,
@@ -57,15 +57,15 @@
             .target(MATCH_VAR_1, 'c') \
             .target(MATCH_VAR_2, 'b', 'a') \
             .context_target('dog', MATCH_VAR_1, 'a', 'b') \
             .context_target('dog', MATCH_VAR_2, 'c') \
             .context_target(Context.DEFAULT_KIND, MATCH_VAR_1) \
             .context_target(Context.DEFAULT_KIND, MATCH_VAR_2) \
             .build()
-        
+
         expect_match(flag, Context.create('a'), MATCH_VAR_2)
         expect_match(flag, Context.create('b'), MATCH_VAR_2)
         expect_match(flag, Context.create('c'), MATCH_VAR_1)
         expect_fallthrough(flag, Context.create('z'))
 
         expect_match(flag,
             Context.create_multi(Context.create('b', 'dog'), Context.create('a')),
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_flag_tracker.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_flag_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ldclient.impl.flag_tracker import FlagTrackerImpl
-from testing.test_util import SpyListener
+from ldclient.testing.test_util import SpyListener
 from ldclient.impl.listeners import Listeners
 from ldclient.interfaces import FlagChange
 
 
 def test_can_add_and_remove_listeners():
     spy = SpyListener()
     listeners = Listeners()
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_listeners.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_listeners.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_lru_cache.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_model_decode.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_model_decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import re
 from semver import VersionInfo
 
 from ldclient.impl.model import *
 
-from testing.builders import *
+from ldclient.testing.builders import *
 
 
 def test_flag_targets_are_stored_as_sets():
     flag = FlagBuilder("key") \
         .target(0, "a", "b") \
         .context_target("kind1", 0, "c", "d") \
         .build()
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_operators.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from ldclient.impl import operators
 
-from testing.builders import *
+from ldclient.testing.builders import *
 
 
 @pytest.mark.parametrize("op,context_value,clause_value,expected", [
     # numeric comparisons
     [ "in",                 99,      99,      True ],
     [ "in",                 99.0001, 99.0001, True ],
     [ "in",                 99,      99.0001, False ],
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_repeating_task.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_repeating_task.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/impl/test_sampler.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/impl/test_sampler.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/integrations/big_segment_store_test_base.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/big_segment_store_test_base.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/integrations/persistent_feature_store_test_base.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/persistent_feature_store_test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from abc import abstractmethod, abstractproperty
 import pytest
 
 from ldclient.feature_store import CacheConfig
 from ldclient.interfaces import FeatureStore
 from ldclient.versioned_data_kind import FEATURES
 
-from testing.feature_store_test_base import FeatureStoreTestBase, FeatureStoreTester, StoreTestScope
-from testing.test_util import skip_database_tests
+from ldclient.testing.feature_store_test_base import FeatureStoreTestBase, FeatureStoreTester, StoreTestScope
+from ldclient.testing.test_util import skip_database_tests
 
 
 # The standard test suite to be run against all persistent feature store implementations. See
-# testing.feature_store_test_base for the basic model being used here. For each database integration,
+# ldclient.testing.feature_store_test_base for the basic model being used here. For each database integration,
 # we must define a subclass of PersistentFeatureStoreTester which overrides its abstract methods as
 # appropriate for that database, and then define a subclass of PersistentFeatureStoreTestBase which
 # simply specifies what tester subclass to use.
 
 
 class PersistentFeatureStoreTester(FeatureStoreTester):
     def __init__(self):
@@ -25,15 +25,15 @@
     def create_persistent_feature_store(self, prefix: str, caching: CacheConfig) -> FeatureStore:
         """
         Override this method to create a feature store instance.
         :param prefix: the prefix parameter for the store constructor - may be None or empty to use the default
         :param caching: caching parameters for the store constructor
         """
         pass
-    
+
     @abstractmethod
     def clear_data(self, prefix: str):
         """
         Override this method to clear any existing data from the database for the specified prefix.
         """
         pass
 
@@ -70,20 +70,20 @@
         tester_a = self.tester_class()
         tester_a.prefix = "a"
         tester_a.clear_data(tester_a.prefix)
 
         tester_b = self.tester_class()
         tester_b.prefix = "b"
         tester_b.clear_data(tester_b.prefix)
-        
+
         flag_a1 = { 'key': 'flagA1', 'version': 1 }
         flag_a2 = { 'key': 'flagA2', 'version': 1 }
         flag_b1 = { 'key': 'flagB1', 'version': 1 }
         flag_b2 = { 'key': 'flagB2', 'version': 1 }
-        
+
         with StoreTestScope(tester_a.create_feature_store()) as store_a:
             with StoreTestScope(tester_b.create_feature_store()) as store_b:
                 store_a.init({ FEATURES: { 'flagA1': flag_a1 } })
                 store_a.upsert(FEATURES, flag_a2)
 
                 store_b.init({ FEATURES: { 'flagB1': flag_b1 } })
                 store_b.upsert(FEATURES, flag_b2)
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/integrations/test_consul.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/test_consul.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ldclient.integrations import Consul
 
-from testing.integrations.persistent_feature_store_test_base import *
-from testing.test_util import skip_database_tests
+from ldclient.testing.integrations.persistent_feature_store_test_base import *
+from ldclient.testing.test_util import skip_database_tests
 import pytest
 
 have_consul = False
 try:
     import consul
     have_consul = True
 except ImportError:
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/integrations/test_dynamodb.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/test_dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ldclient.impl.integrations.dynamodb.dynamodb_big_segment_store import _DynamoDBBigSegmentStore
 from ldclient.impl.integrations.dynamodb.dynamodb_feature_store import _DynamoDBFeatureStoreCore, _DynamoDBHelpers
 from ldclient.integrations import DynamoDB
 from ldclient.interfaces import UpdateProcessor
 
-from testing.integrations.big_segment_store_test_base import *
-from testing.integrations.persistent_feature_store_test_base import *
-from testing.test_util import skip_database_tests
+from ldclient.testing.integrations.big_segment_store_test_base import *
+from ldclient.testing.integrations.persistent_feature_store_test_base import *
+from ldclient.testing.test_util import skip_database_tests
 
 import time
 
 have_dynamodb = False
 try:
     import boto3
     have_dynamodb = True
@@ -46,15 +46,15 @@
         'endpoint_url': 'http://localhost:8000',
         'region_name': 'us-east-1'
     }
 
     @staticmethod
     def make_client():
         return boto3.client('dynamodb', **DynamoDBTestHelper.options)
-    
+
     def clear_data_for_prefix(prefix):
         client = DynamoDBTestHelper.make_client()
         delete_requests = []
         req = {
             'TableName': DynamoDBTestHelper.table_name,
             'ConsistentRead': True,
             'ProjectionExpression': '#namespace, #key',
@@ -115,28 +115,28 @@
                 time.sleep(0.5)
 
 
 class DynamoDBFeatureStoreTester(PersistentFeatureStoreTester):
     def __init__(self):
         super().__init__()
         DynamoDBTestHelper.ensure_table_created()
-        
+
     def create_persistent_feature_store(self, prefix, caching) -> FeatureStore:
         return DynamoDB.new_feature_store(DynamoDBTestHelper.table_name,
             prefix=prefix, caching=caching, dynamodb_opts=DynamoDBTestHelper.options)
 
     def clear_data(self, prefix):
         DynamoDBTestHelper.clear_data_for_prefix(prefix)
 
 
 class DynamoDBBigSegmentTester(BigSegmentStoreTester):
     def __init__(self):
         super().__init__()
         DynamoDBTestHelper.ensure_table_created()
-        
+
     def create_big_segment_store(self, prefix) -> BigSegmentStore:
         return DynamoDB.new_big_segment_store(DynamoDBTestHelper.table_name,
             prefix=prefix, dynamodb_opts=DynamoDBTestHelper.options)
 
     def clear_data(self, prefix):
         DynamoDBTestHelper.clear_data_for_prefix(prefix)
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/integrations/test_redis.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/test_redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ldclient.impl.integrations.redis.redis_big_segment_store import _RedisBigSegmentStore
 from ldclient.integrations import Redis
 from ldclient.versioned_data_kind import FEATURES
 
-from testing.integrations.big_segment_store_test_base import *
-from testing.integrations.persistent_feature_store_test_base import *
-from testing.test_util import skip_database_tests
+from ldclient.testing.integrations.big_segment_store_test_base import *
+from ldclient.testing.integrations.persistent_feature_store_test_base import *
+from ldclient.testing.test_util import skip_database_tests
 
 import pytest
 import json
 
 have_redis = False
 try:
     import redis
@@ -51,15 +51,15 @@
     def clear_data(self, prefix):
         RedisTestHelper.clear_data_for_prefix(prefix or Redis.DEFAULT_PREFIX)
 
 
 class RedisBigSegmentStoreTester(BigSegmentStoreTester):
     def create_big_segment_store(self, prefix) -> BigSegmentStore:
         return Redis.new_big_segment_store(prefix=prefix)
-    
+
     def clear_data(self, prefix):
         RedisTestHelper.clear_data_for_prefix(prefix or Redis.DEFAULT_PREFIX)
 
     def set_metadata(self, prefix: str, metadata: BigSegmentStoreMetadata):
         r = RedisTestHelper.make_client()
         r.set((prefix or Redis.DEFAULT_PREFIX) + _RedisBigSegmentStore.KEY_LAST_UP_TO_DATE,
             "" if metadata.last_up_to_date is None else str(metadata.last_up_to_date))
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/integrations/test_test_data_source.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/integrations/test_test_data_source.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/migrations/test_migrator.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/migrations/test_migrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from ldclient import Result
 from ldclient.migrations.types import Stage, Origin, MigratorFn, ExecutionOrder
 from ldclient.migrations.migrator import Migrator
 from ldclient.migrations.tracker import MigrationOpEvent
 from ldclient.versioned_data_kind import FEATURES
 from ldclient.impl.events.types import EventInputEvaluation
 from ldclient.impl.util import timedelta_millis
-from testing.builders import FlagBuilder
-from testing.test_ldclient import make_client, user
+from ldclient.testing.builders import FlagBuilder
+from ldclient.testing.test_ldclient import make_client, user
 from typing import List
 from time import sleep
 
 
 def success(payload) -> Result:
     return Result.success(True)
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/migrations/test_migrator_builder.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/migrations/test_migrator_builder.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/migrations/test_op_tracker.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/migrations/test_op_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from datetime import timedelta
 from ldclient import Context
 from ldclient.migrations import OpTracker, Stage, Operation, Origin, MigrationOpEvent
 from ldclient.evaluation import EvaluationDetail
-from testing.builders import build_off_flag_with_value, MigrationSettingsBuilder
-from testing.test_ldclient import user
+from ldclient.testing.builders import build_off_flag_with_value, MigrationSettingsBuilder
+from ldclient.testing.test_ldclient import user
 
 
 @pytest.fixture
 def bare_tracker() -> OpTracker:
     flag = build_off_flag_with_value("flag", True).build()
     detail = EvaluationDetail('value', 0, {'kind': 'OFF'})
     tracker = OpTracker("flag", flag, user, detail, Stage.LIVE)
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/mock_components.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/mock_components.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/proxy_test_util.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/proxy_test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ldclient.config import Config, HTTPConfig
-from testing.http_util import start_server, BasicResponse, JsonResponse
+from ldclient.testing.http_util import start_server, BasicResponse, JsonResponse
 
 # Runs tests of all of our supported proxy server configurations: secure or insecure, configured
 # by Config.http_proxy or by an environment variable, with or without authentication. The action
 # parameter is a function that takes three parameters: server, config, secure; the expectation is
 # that it causes an HTTP/HTTPS request to be made via the configured proxy. The caller must pass
 # in the monkeypatch fixture from pytest.
 def do_proxy_tests(action, action_method, monkeypatch):
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/selfsigned.pem` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/selfsigned.pem`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/stub_util.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/stub_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from email.utils import formatdate
 import json
 
 from ldclient.impl.model import ModelEntity
 from ldclient.interfaces import EventProcessor, FeatureRequester, FeatureStore, UpdateProcessor
 
-from testing.http_util import ChunkedResponse, JsonResponse
+from ldclient.testing.http_util import ChunkedResponse, JsonResponse
 
 
 def item_as_json(item):
     return item.to_json_dict() if isinstance(item, ModelEntity) else item
 
 def make_items_map(items = []):
     ret = {}
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_config.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_config.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_context.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_context.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_feature_store_client_wrapper.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_feature_store_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_feature_store_helpers.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_feature_store_helpers.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_file_data_source.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_file_data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ldclient.feature_store import InMemoryFeatureStore
 from ldclient.impl.datasource.status import DataSourceUpdateSinkImpl
 from ldclient.impl.listeners import Listeners
 from ldclient.integrations import Files
 from ldclient.interfaces import DataSourceStatus, DataSourceState, DataSourceErrorKind
 from ldclient.versioned_data_kind import FEATURES, SEGMENTS
 
-from testing.test_util import SpyListener
+from ldclient.testing.test_util import SpyListener
 
 have_yaml = False
 try:
     import yaml
     have_yaml = True
 except ImportError:
     pass
@@ -291,15 +291,15 @@
 def test_does_not_allow_unsafe_yaml():
     if not have_yaml:
         pytest.skip("skipping file source test with YAML because pyyaml isn't available")
 
     # This extended syntax defined by pyyaml allows arbitrary code execution. We should be using
     # yaml.safe_load() which does not support such things.
     unsafe_yaml = '''
-!!python/object/apply:testing.test_file_data_source.arbitrary_method_called_from_yaml ["hi"]
+!!python/object/apply:ldclient.testing.test_file_data_source.arbitrary_method_called_from_yaml ["hi"]
 '''
     path = make_temp_file(unsafe_yaml)
     try:
         factory = Files.new_data_source(paths = path)
         client = LDClient(config=Config('SDK_KEY', update_processor_class = factory, send_events = False))
     finally:
         os.remove(path)
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_flags_state.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_flags_state.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_in_memory_feature_store.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_in_memory_feature_store.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from ldclient.feature_store import InMemoryFeatureStore
 from ldclient.interfaces import FeatureStore
 
-from testing.feature_store_test_base import FeatureStoreTestBase, FeatureStoreTester
+from ldclient.testing.feature_store_test_base import FeatureStoreTestBase, FeatureStoreTester
 
 def test_in_memory_status_checks():
     store = InMemoryFeatureStore()
 
     assert store.is_monitoring_enabled() is False
     assert store.is_available() is True
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_init.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_init.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_ldclient.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from ldclient.impl.datasource.polling import PollingUpdateProcessor
 from ldclient.impl.datasource.streaming import StreamingUpdateProcessor
 from ldclient.impl.stubs import NullUpdateProcessor
 from ldclient.interfaces import UpdateProcessor
 from ldclient.versioned_data_kind import FEATURES, SEGMENTS
 
 import pytest
-from testing.builders import *
-from testing.stub_util import CapturingFeatureStore, MockEventProcessor, MockUpdateProcessor
+from ldclient.testing.builders import *
+from ldclient.testing.stub_util import CapturingFeatureStore, MockEventProcessor, MockUpdateProcessor
 
 
 unreachable_uri="http://fake"
 
 
 context = Context.builder('xyz').set('bizzle', 'def').build()
 user = Context.from_dict({
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_ldclient_end_to_end.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_end_to_end.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ldclient.client import LDClient, Context
 from ldclient.config import Config, HTTPConfig
-from testing.http_util import BasicResponse, SequentialHandler, start_secure_server, start_server
-from testing.stub_util import make_put_event, poll_content, stream_content
+from ldclient.testing.http_util import BasicResponse, SequentialHandler, start_secure_server, start_server
+from ldclient.testing.stub_util import make_put_event, poll_content, stream_content
 
 import json
 import pytest
 import sys
 
 sdk_key = 'sdk-key'
 user = Context.from_dict({ 'key': 'userkey', 'kind': 'user' })
@@ -144,11 +144,11 @@
     with start_secure_server() as server:
         server.for_path('/sdk/latest-all', poll_content())
         config = Config(
             sdk_key = 'sdk_key',
             base_uri = server.uri,
             stream = False,
             send_events = False,
-            http = HTTPConfig(ca_certs = './testing/selfsigned.pem')
+            http = HTTPConfig(ca_certs = './ldclient/testing/selfsigned.pem')
         )
         with LDClient(config = config) as client:
             assert client.is_initialized()
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_ldclient_evaluation.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from ldclient.evaluation import BigSegmentsStatus, EvaluationDetail
 from ldclient.feature_store import InMemoryFeatureStore
 from ldclient.impl.big_segments import _hash_for_user_key
 from ldclient.impl.evaluator import _make_big_segment_ref
 from ldclient.interfaces import FeatureStore
 from ldclient.versioned_data_kind import FEATURES, SEGMENTS
 
-from testing.builders import *
-from testing.mock_components import MockBigSegmentStore
-from testing.stub_util import MockEventProcessor, MockUpdateProcessor
-from testing.test_ldclient import make_client, user
+from ldclient.testing.builders import *
+from ldclient.testing.mock_components import MockBigSegmentStore
+from ldclient.testing.stub_util import MockEventProcessor, MockUpdateProcessor
+from ldclient.testing.test_ldclient import make_client, user
 
 
 flag1 = {
     'key': 'key1',
     'version': 100,
     'on': False,
     'offVariation': 0,
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_ldclient_events.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from ldclient.feature_store import InMemoryFeatureStore
 from ldclient.impl.events.types import EventInputCustom, EventInputEvaluation, EventInputIdentify
 from ldclient.migrations.tracker import MigrationOpEvent
 from ldclient.impl.stubs import NullEventProcessor
 from ldclient.versioned_data_kind import FEATURES
 from ldclient.migrations import OpTracker, Stage, Operation, Origin
 
-from testing.builders import *
-from testing.stub_util import MockUpdateProcessor
-from testing.test_ldclient import context, make_client, make_ldd_client, make_offline_client, unreachable_uri, user
+from ldclient.testing.builders import *
+from ldclient.testing.stub_util import MockUpdateProcessor
+from ldclient.testing.test_ldclient import context, make_client, make_ldd_client, make_offline_client, unreachable_uri, user
 
 
 def get_first_event(c):
     e = c._event_processor._events.pop(0)
     c._event_processor._events = []
     return e
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_ldclient_listeners.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_listeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ldclient.client import LDClient, Config
 from ldclient.interfaces import DataSourceState
 from ldclient.config import BigSegmentsConfig
-from testing.mock_components import MockBigSegmentStore
-from testing.stub_util import MockEventProcessor, MockUpdateProcessor, make_put_event, stream_content
-from testing.http_util import start_server
+from ldclient.testing.mock_components import MockBigSegmentStore
+from ldclient.testing.stub_util import MockEventProcessor, MockUpdateProcessor, make_put_event, stream_content
+from ldclient.testing.http_util import start_server
 
 from queue import Queue
 
 
 def test_big_segment_store_status_unavailable():
     config=Config(
         sdk_key='SDK_KEY',
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_ldclient_migration_variation.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_migration_variation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from ldclient.feature_store import InMemoryFeatureStore
 from ldclient.versioned_data_kind import FEATURES
 from ldclient.migrations import Stage, Operation, Origin
 
-from testing.builders import FlagBuilder
-from testing.test_ldclient import make_client, user
+from ldclient.testing.builders import FlagBuilder
+from ldclient.testing.test_ldclient import make_client, user
 
 
 def test_uses_default_if_flag_not_found():
     store = InMemoryFeatureStore()
     client = make_client(store)
 
     stage, tracker = client.migration_variation('key', user, Stage.LIVE)
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_ldclient_singleton.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_ldclient_singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ldclient
 from ldclient import _reset_client
 from ldclient.config import Config
-from testing.http_util import start_server, BasicResponse
-from testing.stub_util import make_put_event, stream_content
-from testing.sync_util import wait_until
+from ldclient.testing.http_util import start_server, BasicResponse
+from ldclient.testing.stub_util import make_put_event, stream_content
+from ldclient.testing.sync_util import wait_until
 import json
 
 sdk_key = 'sdk-key'
 
 # These are end-to-end tests like test_ldclient_end_to_end, but less detailed in terms of the client's
 # network behavior because what we're really testing is the singleton mechanism.
```

### Comparing `launchdarkly_server_sdk-9.3.0/testing/test_util.py` & `launchdarkly_server_sdk-9.3.1/ldclient/testing/test_util.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_server_sdk-9.3.0/PKG-INFO` & `launchdarkly_server_sdk-9.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchdarkly-server-sdk
-Version: 9.3.0
+Version: 9.3.1
 Summary: LaunchDarkly SDK for Python
 Home-page: https://docs.launchdarkly.com/sdk/server-side/python
 License: Apache-2.0
 Author: LaunchDarkly
 Author-email: dev@launchdarkly.com
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
```

