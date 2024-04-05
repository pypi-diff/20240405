# Comparing `tmp/whylabs-client-0.6.1.tar.gz` & `tmp/whylabs-client-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs-client-0.6.1.tar", last modified: Tue Mar 26 18:14:40 2024, max compression
+gzip compressed data, was "whylabs-client-0.6.2.tar", last modified: Fri Apr  5 00:52:39 2024, max compression
```

## Comparing `whylabs-client-0.6.1.tar` & `whylabs-client-0.6.2.tar`

### file list

```diff
@@ -1,181 +1,189 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:14:40.674342 whylabs-client-0.6.1/
--rw-r--r--   0 root         (0) root         (0)     3400 2024-03-26 18:14:40.674342 whylabs-client-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    29722 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-26 18:14:40.675342 whylabs-client-0.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-03-26 18:14:40.000000 whylabs-client-0.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:14:40.642343 whylabs-client-0.6.1/whylabs_client/
--rw-rw-rw-   0 root         (0) root         (0)      753 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:14:40.646343 whylabs-client-0.6.1/whylabs_client/api/
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/api_key_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5178 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/assets_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6416 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/data_api.py
--rw-rw-rw-   0 root         (0) root         (0)    15394 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/dataset_metadata_api.py
--rw-rw-rw-   0 root         (0) root         (0)    61561 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/dataset_profile_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5992 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/debug_events_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/feature_weights_api.py
--rw-rw-rw-   0 root         (0) root         (0)    17246 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/log_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20538 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/membership_api.py
--rw-rw-rw-   0 root         (0) root         (0)    67193 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/models_api.py
--rw-rw-rw-   0 root         (0) root         (0)    56977 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/monitor_api.py
--rw-rw-rw-   0 root         (0) root         (0)    22628 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/monitor_diagnostics_api.py
--rw-rw-rw-   0 root         (0) root         (0)    56449 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/notification_settings_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/policy_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/schema_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10030 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/security_api.py
--rw-rw-rw-   0 root         (0) root         (0)    35246 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/sessions_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5676 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/traces_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20006 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api/transactions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37531 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:14:40.647343 whylabs-client-0.6.1/whylabs_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17094 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:14:40.674342 whylabs-client-0.6.1/whylabs_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11362 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/account_organization.py
--rw-rw-rw-   0 root         (0) root         (0)    12505 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/account_user.py
--rw-rw-rw-   0 root         (0) root         (0)    11664 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12221 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/activate_azure_subscription_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/activate_azure_subscription_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12110 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/add_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11353 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/admin_report_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11315 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/admin_report_type.py
--rw-rw-rw-   0 root         (0) root         (0)    16926 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analysis_results_record.py
--rw-rw-rw-   0 root         (0) root         (0)    14457 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analysis_results_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11398 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analysis_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13394 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_diagnostic_record.py
--rw-rw-rw-   0 root         (0) root         (0)    13341 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_failure_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11735 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_column_diagnostic_record.py
--rw-rw-rw-   0 root         (0) root         (0)    12179 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_columns_diagnostic_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11628 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_columns_diagnostic_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11892 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_diagnostic_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11584 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_failure_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11774 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_segments_diagnostic_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12144 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzer_segments_diagnostic_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11487 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzers_diagnostic_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12045 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/analyzers_diagnostic_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12419 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/async_log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13478 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/aws_marketplace_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11837 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/azure_marketplace_contact_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    13360 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/azure_marketplace_subscription_details.py
--rw-rw-rw-   0 root         (0) root         (0)    11420 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/batch_log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11811 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/batch_log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11784 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/cache_key_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12758 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/column_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11987 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/create_account_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12589 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/create_dataset_profile_upload_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12449 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/create_reference_profile_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12773 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/create_reference_profile_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/create_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11205 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/create_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11136 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/create_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12492 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/debug_event.py
--rw-rw-rw-   0 root         (0) root         (0)    13384 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/delete_analyzer_result.py
--rw-rw-rw-   0 root         (0) root         (0)    11091 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/delete_analyzer_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11091 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/delete_dataset_profiles_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13387 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/delete_profile.py
--rw-rw-rw-   0 root         (0) root         (0)    11748 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/deletion_status.py
--rw-rw-rw-   0 root         (0) root         (0)    11392 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/diagnostic_interval_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12300 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/diagnostic_interval_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/email_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12349 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/entity_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12718 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/entity_search_result.py
--rw-rw-rw-   0 root         (0) root         (0)    12004 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/entity_weight_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11561 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/entity_weight_record_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11595 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/error_status.py
--rw-rw-rw-   0 root         (0) root         (0)    11465 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/export_trace_partial_success.py
--rw-rw-rw-   0 root         (0) root         (0)    11409 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/export_trace_service_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)    11587 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_account_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11161 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_asset_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11222 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_dataset_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_default_membership_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11365 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_marketplace_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11446 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_notification_settings_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11727 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_profile_observatory_link_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12038 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_profile_observatory_link_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/get_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/list_models_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/list_organization_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11382 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/list_user_api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    11903 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/log_async_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11575 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12344 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/log_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11807 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12791 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11947 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/log_transaction_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/marketplace_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)    11277 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/member.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/membership.py
--rw-rw-rw-   0 root         (0) root         (0)    11852 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/membership_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12260 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/metric_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12785 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/model_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12539 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11629 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/monitor_config_version.py
--rw-rw-rw-   0 root         (0) root         (0)    13161 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    14137 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/notification_action_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/notification_relationship_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11242 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/notification_relationship_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12258 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/notification_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11979 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/notification_settings_day.py
--rw-rw-rw-   0 root         (0) root         (0)    11751 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/notification_sqs_message_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)    14677 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/organization_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11771 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/organization_role_members.py
--rw-rw-rw-   0 root         (0) root         (0)    13324 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/organization_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/pager_duty_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11759 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/patch_account_memberships_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11306 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/post_asset_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11630 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/profile_trace.py
--rw-rw-rw-   0 root         (0) root         (0)    11815 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/profile_traces_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11882 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/provision_new_aws_marketplace_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/provision_new_marketplace_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/provision_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/provision_new_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11241 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/put_account_memberships_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13077 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/reference_profile_item_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11317 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/remove_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/response.py
--rw-rw-rw-   0 root         (0) root         (0)    11163 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/revoke_user_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/role.py
--rw-rw-rw-   0 root         (0) root         (0)    11725 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/schema_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11513 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/search_index_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11787 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/search_index_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11590 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/search_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11239 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/segment.py
--rw-rw-rw-   0 root         (0) root         (0)    11741 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/segment_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/segment_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11563 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/segment_weight.py
--rw-rw-rw-   0 root         (0) root         (0)    11133 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/segments_list_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12108 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/session_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/set_default_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11193 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/slack_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11499 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/sort_order.py
--rw-rw-rw-   0 root         (0) root         (0)    11529 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/status_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11104 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/subscription_product_feature.py
--rw-rw-rw-   0 root         (0) root         (0)    11907 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/subscription_product_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    13683 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/subscription_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11760 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/subscription_tier.py
--rw-rw-rw-   0 root         (0) root         (0)    11886 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/time_period.py
--rw-rw-rw-   0 root         (0) root         (0)    11107 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/transaction_commit_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11921 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/transaction_log_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11160 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/transaction_start_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/transaction_status_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/uber_notification_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)    11706 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/update_account_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11650 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/update_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11747 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    14008 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/user_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    11220 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/user_api_key_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11153 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model/validate_user_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    81897 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:14:40.674342 whylabs-client-0.6.1/whylabs_client/models/
--rw-rw-rw-   0 root         (0) root         (0)    11290 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14199 2024-03-26 18:14:32.000000 whylabs-client-0.6.1/whylabs_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:14:40.642343 whylabs-client-0.6.1/whylabs_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3400 2024-03-26 18:14:40.000000 whylabs-client-0.6.1/whylabs_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7837 2024-03-26 18:14:40.000000 whylabs-client-0.6.1/whylabs_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 18:14:40.000000 whylabs-client-0.6.1/whylabs_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-26 18:14:40.000000 whylabs-client-0.6.1/whylabs_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-26 18:14:40.000000 whylabs-client-0.6.1/whylabs_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.709554 whylabs-client-0.6.2/
+-rw-r--r--   0 root         (0) root         (0)     3400 2024-04-05 00:52:39.709554 whylabs-client-0.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    30686 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-05 00:52:39.711387 whylabs-client-0.6.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.678388 whylabs-client-0.6.2/whylabs_client/
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.682971 whylabs-client-0.6.2/whylabs_client/api/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/api_key_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10305 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/assets_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    12003 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/data_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    15394 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/dataset_metadata_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    61561 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/dataset_profile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5992 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/debug_events_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/feature_weights_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    17246 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/log_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20538 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/membership_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    67193 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/models_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    56977 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/monitor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    22628 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/monitor_diagnostics_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    56449 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/notification_settings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5648 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/policy_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/schema_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10030 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/security_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35246 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/sessions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5676 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/traces_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    24390 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/transactions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37531 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.682971 whylabs-client-0.6.2/whylabs_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17094 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.709554 whylabs-client-0.6.2/whylabs_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11362 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/account_organization.py
+-rw-rw-rw-   0 root         (0) root         (0)    12505 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/account_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12221 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/activate_azure_subscription_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/activate_azure_subscription_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/add_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11326 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/add_policy_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11353 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/admin_report_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11315 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/admin_report_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    16926 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analysis_results_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    14457 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analysis_results_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11398 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analysis_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13394 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_diagnostic_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    13341 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_failure_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11735 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_column_diagnostic_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    12179 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_columns_diagnostic_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11628 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_columns_diagnostic_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11892 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_diagnostic_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11584 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_failure_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11774 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segments_diagnostic_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12144 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segments_diagnostic_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11487 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzers_diagnostic_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12045 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzers_diagnostic_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12419 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/async_log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13478 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/aws_marketplace_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11837 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/azure_marketplace_contact_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    13360 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/azure_marketplace_subscription_details.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/batch_log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11811 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/batch_log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11784 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/cache_key_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12758 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/column_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11987 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_account_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12589 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_dataset_profile_upload_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12449 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_reference_profile_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12773 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_reference_profile_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11205 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12492 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/debug_event.py
+-rw-rw-rw-   0 root         (0) root         (0)    13384 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/delete_analyzer_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    11091 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/delete_analyzer_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11091 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/delete_dataset_profiles_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13387 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/delete_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)    11748 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/deletion_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    11392 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/diagnostic_interval_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12300 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/diagnostic_interval_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/email_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12349 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/entity_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12718 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/entity_search_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    12004 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/entity_weight_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11561 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/entity_weight_record_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11595 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/error_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    11465 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/export_trace_partial_success.py
+-rw-rw-rw-   0 root         (0) root         (0)    11409 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/export_trace_service_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    11587 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_account_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11593 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_asset_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11222 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_dataset_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_default_membership_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11365 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_marketplace_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11446 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_notification_settings_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11727 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_profile_observatory_link_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12038 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_profile_observatory_link_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11733 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/granularity.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/list_models_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/list_organization_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11382 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/list_user_api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    11903 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_async_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11575 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12344 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11807 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12791 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12176 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_transaction_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/marketplace_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11277 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/member.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)    11852 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/membership_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12260 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11624 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    12398 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11375 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12785 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/model_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12539 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11629 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/monitor_config_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    13161 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    14137 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_action_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_relationship_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11242 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_relationship_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12258 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_settings_day.py
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_sqs_message_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14677 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/organization_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11771 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/organization_role_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    13324 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/organization_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/pager_duty_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11759 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/patch_account_memberships_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11512 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/post_asset_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/post_asset_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11630 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/profile_trace.py
+-rw-rw-rw-   0 root         (0) root         (0)    11815 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/profile_traces_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11882 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/provision_new_aws_marketplace_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12226 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/provision_new_marketplace_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/provision_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/provision_new_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11241 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/put_account_memberships_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13077 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/reference_profile_item_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11317 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/remove_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11163 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/revoke_user_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/role.py
+-rw-rw-rw-   0 root         (0) root         (0)    11725 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/schema_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11513 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/search_index_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11787 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/search_index_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11590 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/search_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11239 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11741 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segment_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segment_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11563 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segment_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)    11133 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segments_list_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12108 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/session_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/set_default_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11193 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/slack_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11499 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/sort_order.py
+-rw-rw-rw-   0 root         (0) root         (0)    11529 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/status_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11104 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/subscription_product_feature.py
+-rw-rw-rw-   0 root         (0) root         (0)    11907 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/subscription_product_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    13683 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/subscription_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11760 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/subscription_tier.py
+-rw-rw-rw-   0 root         (0) root         (0)    11886 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/time_period.py
+-rw-rw-rw-   0 root         (0) root         (0)    11107 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/transaction_commit_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11921 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/transaction_log_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11160 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/transaction_start_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/transaction_status_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/uber_notification_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11706 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/update_account_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11650 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/update_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/upload_asset_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/upload_asset_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    14008 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/user_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/user_api_key_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11153 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/validate_user_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    81897 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.709554 whylabs-client-0.6.2/whylabs_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)    11886 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14199 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.679304 whylabs-client-0.6.2/whylabs_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3400 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/top_level.txt
```

### Comparing `whylabs-client-0.6.1/PKG-INFO` & `whylabs-client-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.6.1/README.md` & `whylabs-client-0.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whylabs-client
 WhyLabs API that enables end-to-end AI observability
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1
-- Package version: 0.6.1
+- Package version: 0.6.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://whylabs.ai](https://whylabs.ai)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -95,15 +95,17 @@
 All URIs are relative to *https://api.whylabsapp.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApiKeyApi* | [**create_api_key**](docs/ApiKeyApi.md#create_api_key) | **POST** /v0/organizations/{org_id}/api-key | Generate an API key for a user.
 *ApiKeyApi* | [**revoke_api_key**](docs/ApiKeyApi.md#revoke_api_key) | **DELETE** /v0/organizations/{org_id}/api-key | Revoke the given API Key, removing its ability to access WhyLabs systems
 *AssetsApi* | [**get_asset**](docs/AssetsApi.md#get_asset) | **GET** /v1/assets/{asset_id} | Endpoint to retrieve assets
+*AssetsApi* | [**upload_asset**](docs/AssetsApi.md#upload_asset) | **POST** /v1/assets/{asset_id}/upload | Endpoint to upload an asset
 *DataApi* | [**analysis_results_data**](docs/DataApi.md#analysis_results_data) | **POST** /v0/organizations/{org_id}/dataset/{dataset_id}/data/analysis-results | Endpoint to query analysis results for a dataset
+*DataApi* | [**metric_timeseries_data**](docs/DataApi.md#metric_timeseries_data) | **POST** /v0/organizations/{org_id}/dataset/{dataset_id}/data/metric-timeseries | Endpoint to query a single metric timeseries for a dataset
 *DatasetProfileApi* | [**create_reference_profile**](docs/DatasetProfileApi.md#create_reference_profile) | **POST** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/reference-profile | Returns data needed to uploading the reference profile
 *DatasetProfileApi* | [**delete_analyzer_results**](docs/DatasetProfileApi.md#delete_analyzer_results) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/analyzer-results | Deletes a set of analyzer results
 *DatasetProfileApi* | [**delete_dataset_profiles**](docs/DatasetProfileApi.md#delete_dataset_profiles) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id} | Deletes a set of dataset profiles
 *DatasetProfileApi* | [**delete_reference_profile**](docs/DatasetProfileApi.md#delete_reference_profile) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id} | Delete a single reference profile
 *DatasetProfileApi* | [**get_profile_traces**](docs/DatasetProfileApi.md#get_profile_traces) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/trace/{trace_id} | Returns a list for profile traces matching a trace id
 *DatasetProfileApi* | [**get_reference_profile**](docs/DatasetProfileApi.md#get_reference_profile) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id} | Returns a single reference profile
 *DatasetProfileApi* | [**list_delete_analyzer_results_requests**](docs/DatasetProfileApi.md#list_delete_analyzer_results_requests) | **GET** /v0/organizations/{org_id}/dataset-profiles/delete-requests/analyzer-results | List requests to delete analyzer results
@@ -172,14 +174,15 @@
 *SessionsApi* | [**claim_guest_session**](docs/SessionsApi.md#claim_guest_session) | **POST** /v0/sessions/{session_id}/claim | Claim a guest session, copying its model data into another org and expiring the session.
 *SessionsApi* | [**create_dataset_profile_upload**](docs/SessionsApi.md#create_dataset_profile_upload) | **POST** /v0/sessions/{session_id}/upload | Create an upload for a given session.
 *SessionsApi* | [**create_reference_profile_upload**](docs/SessionsApi.md#create_reference_profile_upload) | **POST** /v0/sessions/{session_id}/reference | Create a reference profile upload for a given session.
 *SessionsApi* | [**create_session**](docs/SessionsApi.md#create_session) | **POST** /v0/sessions | Create a new session that can be used to upload dataset profiles from whylogs for display in whylabs.
 *SessionsApi* | [**get_session**](docs/SessionsApi.md#get_session) | **GET** /v0/sessions/{session_id} | Get information about a session.
 *SessionsApi* | [**get_session_profile_observatory_link**](docs/SessionsApi.md#get_session_profile_observatory_link) | **POST** /v0/sessions/observatory-link/{session_id} | Get observatory links for profiles in a given session. A max of 3 profiles can be viewed a a time.
 *TracesApi* | [**export_traces**](docs/TracesApi.md#export_traces) | **POST** /v1/traces | Export traces into WhyLabs
+*TransactionsApi* | [**abort_transaction**](docs/TransactionsApi.md#abort_transaction) | **POST** /v1/transaction/abort | Abort a transaction which has not yet been committed
 *TransactionsApi* | [**commit_transaction**](docs/TransactionsApi.md#commit_transaction) | **POST** /v1/transaction/commit | Commit a log transaction
 *TransactionsApi* | [**log_transaction**](docs/TransactionsApi.md#log_transaction) | **POST** /v1/transaction/log | Add to a log transaction
 *TransactionsApi* | [**start_transaction**](docs/TransactionsApi.md#start_transaction) | **POST** /v1/transaction | Start a log transaction
 *TransactionsApi* | [**transaction_status**](docs/TransactionsApi.md#transaction_status) | **GET** /v1/transaction | Get the status of a log transaction
 
 
 ## Documentation For Models
@@ -187,14 +190,15 @@
  - [AWSMarketplaceMetadata](docs/AWSMarketplaceMetadata.md)
  - [AccountOrganization](docs/AccountOrganization.md)
  - [AccountUser](docs/AccountUser.md)
  - [ActionType](docs/ActionType.md)
  - [ActivateAzureSubscriptionRequest](docs/ActivateAzureSubscriptionRequest.md)
  - [ActivateAzureSubscriptionResponse](docs/ActivateAzureSubscriptionResponse.md)
  - [AddMembershipRequest](docs/AddMembershipRequest.md)
+ - [AddPolicyResponse](docs/AddPolicyResponse.md)
  - [AdminReportResponse](docs/AdminReportResponse.md)
  - [AdminReportType](docs/AdminReportType.md)
  - [AnalysisResultsRecord](docs/AnalysisResultsRecord.md)
  - [AnalysisResultsRequest](docs/AnalysisResultsRequest.md)
  - [AnalysisResultsResponse](docs/AnalysisResultsResponse.md)
  - [AnalyzerDiagnosticRecord](docs/AnalyzerDiagnosticRecord.md)
  - [AnalyzerFailureRecord](docs/AnalyzerFailureRecord.md)
@@ -244,28 +248,32 @@
  - [GetDefaultMembershipResponse](docs/GetDefaultMembershipResponse.md)
  - [GetMarketplaceMetadataResponse](docs/GetMarketplaceMetadataResponse.md)
  - [GetMembershipsResponse](docs/GetMembershipsResponse.md)
  - [GetNotificationSettingsResponse](docs/GetNotificationSettingsResponse.md)
  - [GetProfileObservatoryLinkRequest](docs/GetProfileObservatoryLinkRequest.md)
  - [GetProfileObservatoryLinkResponse](docs/GetProfileObservatoryLinkResponse.md)
  - [GetSessionResponse](docs/GetSessionResponse.md)
+ - [Granularity](docs/Granularity.md)
  - [ListModelsResponse](docs/ListModelsResponse.md)
  - [ListOrganizationMembershipsResponse](docs/ListOrganizationMembershipsResponse.md)
  - [ListUserApiKeys](docs/ListUserApiKeys.md)
  - [LogAsyncRequest](docs/LogAsyncRequest.md)
  - [LogReferenceRequest](docs/LogReferenceRequest.md)
  - [LogReferenceResponse](docs/LogReferenceResponse.md)
  - [LogResponse](docs/LogResponse.md)
  - [LogSessionReferenceResponse](docs/LogSessionReferenceResponse.md)
  - [LogTransactionMetadata](docs/LogTransactionMetadata.md)
  - [MarketplaceDimensions](docs/MarketplaceDimensions.md)
  - [Member](docs/Member.md)
  - [Membership](docs/Membership.md)
  - [MembershipMetadata](docs/MembershipMetadata.md)
  - [MetricSchema](docs/MetricSchema.md)
+ - [MetricTimeseriesRecord](docs/MetricTimeseriesRecord.md)
+ - [MetricTimeseriesRequest](docs/MetricTimeseriesRequest.md)
+ - [MetricTimeseriesResponse](docs/MetricTimeseriesResponse.md)
  - [ModelMetadataResponse](docs/ModelMetadataResponse.md)
  - [ModelType](docs/ModelType.md)
  - [MonitorConfigVersion](docs/MonitorConfigVersion.md)
  - [NotificationAction](docs/NotificationAction.md)
  - [NotificationActionPayload](docs/NotificationActionPayload.md)
  - [NotificationRelationshipItem](docs/NotificationRelationshipItem.md)
  - [NotificationRelationshipType](docs/NotificationRelationshipType.md)
@@ -274,14 +282,15 @@
  - [NotificationSqsMessageCadence](docs/NotificationSqsMessageCadence.md)
  - [OrganizationMetadata](docs/OrganizationMetadata.md)
  - [OrganizationRoleMembers](docs/OrganizationRoleMembers.md)
  - [OrganizationSummary](docs/OrganizationSummary.md)
  - [PagerDutyNotificationAction](docs/PagerDutyNotificationAction.md)
  - [PatchAccountMembershipsRequest](docs/PatchAccountMembershipsRequest.md)
  - [PostAssetRequest](docs/PostAssetRequest.md)
+ - [PostAssetResponse](docs/PostAssetResponse.md)
  - [ProfileTrace](docs/ProfileTrace.md)
  - [ProfileTracesResponse](docs/ProfileTracesResponse.md)
  - [ProvisionNewAWSMarketplaceUserResponse](docs/ProvisionNewAWSMarketplaceUserResponse.md)
  - [ProvisionNewMarketplaceUserRequest](docs/ProvisionNewMarketplaceUserRequest.md)
  - [ProvisionNewUserRequest](docs/ProvisionNewUserRequest.md)
  - [ProvisionNewUserResponse](docs/ProvisionNewUserResponse.md)
  - [PutAccountMembershipsRequest](docs/PutAccountMembershipsRequest.md)
@@ -312,14 +321,16 @@
  - [TransactionCommitRequest](docs/TransactionCommitRequest.md)
  - [TransactionLogRequest](docs/TransactionLogRequest.md)
  - [TransactionStartRequest](docs/TransactionStartRequest.md)
  - [TransactionStatusResponse](docs/TransactionStatusResponse.md)
  - [UberNotificationSchedule](docs/UberNotificationSchedule.md)
  - [UpdateAccountUserRequest](docs/UpdateAccountUserRequest.md)
  - [UpdateMembershipRequest](docs/UpdateMembershipRequest.md)
+ - [UploadAssetRequest](docs/UploadAssetRequest.md)
+ - [UploadAssetResponse](docs/UploadAssetResponse.md)
  - [User](docs/User.md)
  - [UserApiKey](docs/UserApiKey.md)
  - [UserApiKeyResponse](docs/UserApiKeyResponse.md)
  - [ValidateUserSessionResponse](docs/ValidateUserSessionResponse.md)
 
 
 ## Documentation For Authorization
```

### Comparing `whylabs-client-0.6.1/setup.py` & `whylabs-client-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import setup, find_packages  # noqa: H301
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "RELEASE.md").read_text()
 
 NAME = "whylabs-client"
-VERSION = "0.6.1"
+VERSION = "0.6.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `whylabs-client-0.6.1/whylabs_client/__init__.py` & `whylabs-client-0.6.2/whylabs_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1
     Contact: support@whylabs.ai
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 # import ApiClient
 from whylabs_client.api_client import ApiClient
 
 # import Configuration
 from whylabs_client.configuration import Configuration
```

### Comparing `whylabs-client-0.6.1/whylabs_client/api/api_key_api.py` & `whylabs-client-0.6.2/whylabs_client/api/api_key_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/assets_api.py` & `whylabs-client-0.6.2/whylabs_client/api/schema_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,96 +18,95 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from whylabs_client.model.get_asset_response import GetAssetResponse
 
 
-class AssetsApi(object):
+class SchemaApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_asset_endpoint = _Endpoint(
+        self.get_monitor_config_schema_endpoint = _Endpoint(
             settings={
-                'response_type': (GetAssetResponse,),
+                'response_type': (str,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
-                'endpoint_path': '/v1/assets/{asset_id}',
-                'operation_id': 'get_asset',
+                'endpoint_path': '/v0/organizations/{org_id}/schema/monitor-config',
+                'operation_id': 'get_monitor_config_schema',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'asset_id',
+                    'org_id',
                 ],
                 'required': [
-                    'asset_id',
+                    'org_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'asset_id':
+                    'org_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'asset_id': 'asset_id',
+                    'org_id': 'org_id',
                 },
                 'location_map': {
-                    'asset_id': 'path',
+                    'org_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def get_asset(
+    def get_monitor_config_schema(
         self,
-        asset_id,
+        org_id,
         **kwargs
     ):
-        """Endpoint to retrieve assets  # noqa: E501
+        """Get the current supported schema of the monitor configuration  # noqa: E501
 
-        Endpoint to retrieve assets  # noqa: E501
+        Get the current supported schema of the  monitor configuration  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_asset(asset_id, async_req=True)
+        >>> thread = api.get_monitor_config_schema(org_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            asset_id (str):
+            org_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -126,15 +125,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetAssetResponse
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -151,11 +150,11 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['asset_id'] = \
-            asset_id
-        return self.get_asset_endpoint.call_with_http_info(**kwargs)
+        kwargs['org_id'] = \
+            org_id
+        return self.get_monitor_config_schema_endpoint.call_with_http_info(**kwargs)
```

### Comparing `whylabs-client-0.6.1/whylabs_client/api/data_api.py` & `whylabs-client-0.6.2/whylabs_client/api/policy_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,120 +18,111 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from whylabs_client.model.analysis_results_request import AnalysisResultsRequest
-from whylabs_client.model.analysis_results_response import AnalysisResultsResponse
 
 
-class DataApi(object):
+class PolicyApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.analysis_results_data_endpoint = _Endpoint(
+        self.get_policy_endpoint = _Endpoint(
             settings={
-                'response_type': (AnalysisResultsResponse,),
+                'response_type': (str,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
-                'endpoint_path': '/v0/organizations/{org_id}/dataset/{dataset_id}/data/analysis-results',
-                'operation_id': 'analysis_results_data',
-                'http_method': 'POST',
+                'endpoint_path': '/v1/policy',
+                'operation_id': 'get_policy',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'org_id',
                     'dataset_id',
-                    'analysis_results_request',
+                    'label',
+                    'version',
                 ],
                 'required': [
-                    'org_id',
                     'dataset_id',
-                    'analysis_results_request',
                 ],
                 'nullable': [
+                    'label',
+                    'version',
                 ],
                 'enum': [
                 ],
                 'validation': [
-                    'org_id',
                 ]
             },
             root_map={
                 'validations': {
-                    ('org_id',): {
-                        'max_length': 128,
-                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'org_id':
-                        (str,),
                     'dataset_id':
                         (str,),
-                    'analysis_results_request':
-                        (AnalysisResultsRequest,),
+                    'label':
+                        (str, none_type,),
+                    'version':
+                        (int, none_type,),
                 },
                 'attribute_map': {
-                    'org_id': 'org_id',
                     'dataset_id': 'dataset_id',
+                    'label': 'label',
+                    'version': 'version',
                 },
                 'location_map': {
-                    'org_id': 'path',
-                    'dataset_id': 'path',
-                    'analysis_results_request': 'body',
+                    'dataset_id': 'query',
+                    'label': 'query',
+                    'version': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'application/x-yaml'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
 
-    def analysis_results_data(
+    def get_policy(
         self,
-        org_id,
         dataset_id,
-        analysis_results_request,
         **kwargs
     ):
-        """Endpoint to query analysis results for a dataset  # noqa: E501
+        """Endpoint to get the policy configuration  # noqa: E501
 
-        Returns analysis results for a dataset over a specified interval  # noqa: E501
+        Endpoint to get the policy configuration  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.analysis_results_data(org_id, dataset_id, analysis_results_request, async_req=True)
+        >>> thread = api.get_policy(dataset_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            org_id (str):
             dataset_id (str):
-            analysis_results_request (AnalysisResultsRequest):
 
         Keyword Args:
+            label (str, none_type): [optional]
+            version (int, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -148,15 +139,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            AnalysisResultsResponse
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -173,15 +164,11 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['org_id'] = \
-            org_id
         kwargs['dataset_id'] = \
             dataset_id
-        kwargs['analysis_results_request'] = \
-            analysis_results_request
-        return self.analysis_results_data_endpoint.call_with_http_info(**kwargs)
+        return self.get_policy_endpoint.call_with_http_info(**kwargs)
```

### Comparing `whylabs-client-0.6.1/whylabs_client/api/dataset_metadata_api.py` & `whylabs-client-0.6.2/whylabs_client/api/dataset_metadata_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/dataset_profile_api.py` & `whylabs-client-0.6.2/whylabs_client/api/dataset_profile_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/debug_events_api.py` & `whylabs-client-0.6.2/whylabs_client/api/debug_events_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/feature_weights_api.py` & `whylabs-client-0.6.2/whylabs_client/api/feature_weights_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/log_api.py` & `whylabs-client-0.6.2/whylabs_client/api/log_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/membership_api.py` & `whylabs-client-0.6.2/whylabs_client/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/models_api.py` & `whylabs-client-0.6.2/whylabs_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/monitor_api.py` & `whylabs-client-0.6.2/whylabs_client/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/monitor_diagnostics_api.py` & `whylabs-client-0.6.2/whylabs_client/api/monitor_diagnostics_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/notification_settings_api.py` & `whylabs-client-0.6.2/whylabs_client/api/notification_settings_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/policy_api.py` & `whylabs-client-0.6.2/whylabs_client/api/traces_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,97 +18,107 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
+from whylabs_client.model.export_trace_service_response import ExportTraceServiceResponse
 
 
-class PolicyApi(object):
+class TracesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_policy_endpoint = _Endpoint(
+        self.export_traces_endpoint = _Endpoint(
             settings={
-                'response_type': (str,),
+                'response_type': (ExportTraceServiceResponse,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
-                'endpoint_path': '/v1/policy',
-                'operation_id': 'get_policy',
-                'http_method': 'GET',
+                'endpoint_path': '/v1/traces',
+                'operation_id': 'export_traces',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'dataset_id',
+                    'request_body',
+                    'x_whylabs_resource',
                 ],
                 'required': [
-                    'dataset_id',
+                    'request_body',
                 ],
                 'nullable': [
+                    'x_whylabs_resource',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'dataset_id':
-                        (str,),
+                    'request_body':
+                        ([str],),
+                    'x_whylabs_resource':
+                        (str, none_type,),
                 },
                 'attribute_map': {
-                    'dataset_id': 'dataset_id',
+                    'x_whylabs_resource': 'X-WHYLABS-RESOURCE',
                 },
                 'location_map': {
-                    'dataset_id': 'query',
+                    'request_body': 'body',
+                    'x_whylabs_resource': 'header',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/x-yaml'
+                    'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json',
+                    'application/x-protobuf'
+                ]
             },
             api_client=api_client
         )
 
-    def get_policy(
+    def export_traces(
         self,
-        dataset_id,
+        request_body,
         **kwargs
     ):
-        """Endpoint to get the policy configuration  # noqa: E501
+        """Export traces into WhyLabs  # noqa: E501
 
-        Endpoint to get the policy configuration  # noqa: E501
+        API to export traces into WhyLabs  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_policy(dataset_id, async_req=True)
+        >>> thread = api.export_traces(request_body, async_req=True)
         >>> result = thread.get()
 
         Args:
-            dataset_id (str):
+            request_body ([str]):
 
         Keyword Args:
+            x_whylabs_resource (str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -125,15 +135,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            str
+            ExportTraceServiceResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -150,11 +160,11 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['dataset_id'] = \
-            dataset_id
-        return self.get_policy_endpoint.call_with_http_info(**kwargs)
+        kwargs['request_body'] = \
+            request_body
+        return self.export_traces_endpoint.call_with_http_info(**kwargs)
```

### Comparing `whylabs-client-0.6.1/whylabs_client/api/security_api.py` & `whylabs-client-0.6.2/whylabs_client/api/security_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/sessions_api.py` & `whylabs-client-0.6.2/whylabs_client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/api/transactions_api.py` & `whylabs-client-0.6.2/whylabs_client/api/transactions_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,65 @@
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.abort_transaction_endpoint = _Endpoint(
+            settings={
+                'response_type': (Response,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v1/transaction/abort',
+                'operation_id': 'abort_transaction',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'transaction_id',
+                ],
+                'required': [
+                    'transaction_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'transaction_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'transaction_id': 'transaction_id',
+                },
+                'location_map': {
+                    'transaction_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.commit_transaction_endpoint = _Endpoint(
             settings={
                 'response_type': (Response,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v1/transaction/commit',
@@ -258,14 +309,85 @@
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
+    def abort_transaction(
+        self,
+        transaction_id,
+        **kwargs
+    ):
+        """Abort a transaction which has not yet been committed  # noqa: E501
+
+        Abort a transaction which has not yet been committed  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.abort_transaction(transaction_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            transaction_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['transaction_id'] = \
+            transaction_id
+        return self.abort_transaction_endpoint.call_with_http_info(**kwargs)
+
     def commit_transaction(
         self,
         transaction_id,
         transaction_commit_request,
         **kwargs
     ):
         """Commit a log transaction  # noqa: E501
```

### Comparing `whylabs-client-0.6.1/whylabs_client/api_client.py` & `whylabs-client-0.6.2/whylabs_client/api_client.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/apis/__init__.py` & `whylabs-client-0.6.2/whylabs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/configuration.py` & `whylabs-client-0.6.2/whylabs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.6.1".\
+               "SDK Package Version: 0.6.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `whylabs-client-0.6.1/whylabs_client/exceptions.py` & `whylabs-client-0.6.2/whylabs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/account_organization.py` & `whylabs-client-0.6.2/whylabs_client/model/account_organization.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/account_user.py` & `whylabs-client-0.6.2/whylabs_client/model/account_user.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/action_type.py` & `whylabs-client-0.6.2/whylabs_client/model/action_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/activate_azure_subscription_request.py` & `whylabs-client-0.6.2/whylabs_client/model/activate_azure_subscription_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/activate_azure_subscription_response.py` & `whylabs-client-0.6.2/whylabs_client/model/activate_azure_subscription_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/add_membership_request.py` & `whylabs-client-0.6.2/whylabs_client/model/add_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/admin_report_response.py` & `whylabs-client-0.6.2/whylabs_client/model/admin_report_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/admin_report_type.py` & `whylabs-client-0.6.2/whylabs_client/model/admin_report_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analysis_results_record.py` & `whylabs-client-0.6.2/whylabs_client/model/analysis_results_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analysis_results_request.py` & `whylabs-client-0.6.2/whylabs_client/model/analysis_results_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analysis_results_response.py` & `whylabs-client-0.6.2/whylabs_client/model/analysis_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_diagnostic_record.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_diagnostic_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_failure_record.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_failure_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_column_diagnostic_record.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_column_diagnostic_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_columns_diagnostic_request.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_columns_diagnostic_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_columns_diagnostic_response.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_columns_diagnostic_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_diagnostic_record.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_diagnostic_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_segment_failure_record.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_failure_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_segments_diagnostic_request.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_segments_diagnostic_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzer_segments_diagnostic_response.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzer_segments_diagnostic_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzers_diagnostic_request.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzers_diagnostic_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/analyzers_diagnostic_response.py` & `whylabs-client-0.6.2/whylabs_client/model/analyzers_diagnostic_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/async_log_response.py` & `whylabs-client-0.6.2/whylabs_client/model/async_log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/aws_marketplace_metadata.py` & `whylabs-client-0.6.2/whylabs_client/model/aws_marketplace_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/azure_marketplace_contact_payload.py` & `whylabs-client-0.6.2/whylabs_client/model/azure_marketplace_contact_payload.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/azure_marketplace_subscription_details.py` & `whylabs-client-0.6.2/whylabs_client/model/azure_marketplace_subscription_details.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/batch_log_reference_request.py` & `whylabs-client-0.6.2/whylabs_client/model/batch_log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/batch_log_session_reference_response.py` & `whylabs-client-0.6.2/whylabs_client/model/batch_log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/cache_key_type.py` & `whylabs-client-0.6.2/whylabs_client/model/cache_key_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/column_schema.py` & `whylabs-client-0.6.2/whylabs_client/model/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/create_account_user_request.py` & `whylabs-client-0.6.2/whylabs_client/model/create_account_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/create_dataset_profile_upload_response.py` & `whylabs-client-0.6.2/whylabs_client/model/create_dataset_profile_upload_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/create_reference_profile_request.py` & `whylabs-client-0.6.2/whylabs_client/model/create_reference_profile_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/create_reference_profile_response.py` & `whylabs-client-0.6.2/whylabs_client/model/create_reference_profile_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/create_session_request.py` & `whylabs-client-0.6.2/whylabs_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/create_session_response.py` & `whylabs-client-0.6.2/whylabs_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/create_user_request.py` & `whylabs-client-0.6.2/whylabs_client/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/debug_event.py` & `whylabs-client-0.6.2/whylabs_client/model/debug_event.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/delete_analyzer_result.py` & `whylabs-client-0.6.2/whylabs_client/model/delete_analyzer_result.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/delete_analyzer_results_response.py` & `whylabs-client-0.6.2/whylabs_client/model/delete_analyzer_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/delete_dataset_profiles_response.py` & `whylabs-client-0.6.2/whylabs_client/model/delete_dataset_profiles_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/delete_profile.py` & `whylabs-client-0.6.2/whylabs_client/model/delete_profile.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/deletion_status.py` & `whylabs-client-0.6.2/whylabs_client/model/deletion_status.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/diagnostic_interval_request.py` & `whylabs-client-0.6.2/whylabs_client/model/diagnostic_interval_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/diagnostic_interval_response.py` & `whylabs-client-0.6.2/whylabs_client/model/diagnostic_interval_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/email_notification_action.py` & `whylabs-client-0.6.2/whylabs_client/model/email_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/entity_schema.py` & `whylabs-client-0.6.2/whylabs_client/model/entity_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/entity_search_result.py` & `whylabs-client-0.6.2/whylabs_client/model/entity_search_result.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/entity_weight_record.py` & `whylabs-client-0.6.2/whylabs_client/model/entity_weight_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/entity_weight_record_metadata.py` & `whylabs-client-0.6.2/whylabs_client/model/entity_weight_record_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/error_status.py` & `whylabs-client-0.6.2/whylabs_client/model/error_status.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/export_trace_partial_success.py` & `whylabs-client-0.6.2/whylabs_client/model/export_trace_partial_success.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/export_trace_service_response.py` & `whylabs-client-0.6.2/whylabs_client/model/export_trace_service_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/feature_flags.py` & `whylabs-client-0.6.2/whylabs_client/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_account_memberships_response.py` & `whylabs-client-0.6.2/whylabs_client/model/get_account_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_asset_response.py` & `whylabs-client-0.6.2/whylabs_client/model/segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.segment_tag import SegmentTag
+    globals()['SegmentTag'] = SegmentTag
 
-class GetAssetResponse(ModelNormal):
+
+class Segment(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,53 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'download_url': (str,),  # noqa: E501
+            'tags': ([SegmentTag],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'download_url': 'downloadUrl',  # noqa: E501
+        'tags': 'tags',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, download_url, *args, **kwargs):  # noqa: E501
-        """GetAssetResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, tags, *args, **kwargs):  # noqa: E501
+        """Segment - a model defined in OpenAPI
 
         Args:
-            download_url (str):
+            tags ([SegmentTag]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,15 +167,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.download_url = download_url
+        self.tags = tags
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +188,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, download_url, *args, **kwargs):  # noqa: E501
-        """GetAssetResponse - a model defined in OpenAPI
+    def __init__(self, tags, *args, **kwargs):  # noqa: E501
+        """Segment - a model defined in OpenAPI
 
         Args:
-            download_url (str):
+            tags ([SegmentTag]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,15 +250,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.download_url = download_url
+        self.tags = tags
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_dataset_metadata_response.py` & `whylabs-client-0.6.2/whylabs_client/model/get_dataset_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_default_membership_response.py` & `whylabs-client-0.6.2/whylabs_client/model/get_default_membership_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_marketplace_metadata_response.py` & `whylabs-client-0.6.2/whylabs_client/model/get_marketplace_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_memberships_response.py` & `whylabs-client-0.6.2/whylabs_client/model/get_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_notification_settings_response.py` & `whylabs-client-0.6.2/whylabs_client/model/get_notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_profile_observatory_link_request.py` & `whylabs-client-0.6.2/whylabs_client/model/get_profile_observatory_link_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_profile_observatory_link_response.py` & `whylabs-client-0.6.2/whylabs_client/model/get_profile_observatory_link_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/get_session_response.py` & `whylabs-client-0.6.2/whylabs_client/model/get_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/list_models_response.py` & `whylabs-client-0.6.2/whylabs_client/model/list_models_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/list_organization_memberships_response.py` & `whylabs-client-0.6.2/whylabs_client/model/list_organization_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/list_user_api_keys.py` & `whylabs-client-0.6.2/whylabs_client/model/list_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/log_async_request.py` & `whylabs-client-0.6.2/whylabs_client/model/log_async_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/log_reference_request.py` & `whylabs-client-0.6.2/whylabs_client/model/log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/log_reference_response.py` & `whylabs-client-0.6.2/whylabs_client/model/log_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/log_response.py` & `whylabs-client-0.6.2/whylabs_client/model/log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/log_session_reference_response.py` & `whylabs-client-0.6.2/whylabs_client/model/log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/log_transaction_metadata.py` & `whylabs-client-0.6.2/whylabs_client/model/search_index_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.search_index_type import SearchIndexType
+    globals()['SearchIndexType'] = SearchIndexType
 
-class LogTransactionMetadata(ModelNormal):
+
+class SearchIndexRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,61 +67,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'org_id': (str,),  # noqa: E501
-            'dataset_id': (str,),  # noqa: E501
-            'transaction_id': (str,),  # noqa: E501
-            'expiration_time': (datetime, none_type,),  # noqa: E501
+            'type': (SearchIndexType,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'org_id': 'orgId',  # noqa: E501
-        'dataset_id': 'datasetId',  # noqa: E501
-        'transaction_id': 'transactionId',  # noqa: E501
-        'expiration_time': 'expirationTime',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, dataset_id, transaction_id, *args, **kwargs):  # noqa: E501
-        """LogTransactionMetadata - a model defined in OpenAPI
+    def _from_openapi_data(cls, org_id, type, *args, **kwargs):  # noqa: E501
+        """SearchIndexRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            dataset_id (str):
-            transaction_id (str):
+            type (SearchIndexType):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +143,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            expiration_time (datetime, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,16 +171,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.dataset_id = dataset_id
-        self.transaction_id = transaction_id
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,21 +192,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, dataset_id, transaction_id, *args, **kwargs):  # noqa: E501
-        """LogTransactionMetadata - a model defined in OpenAPI
+    def __init__(self, org_id, type, *args, **kwargs):  # noqa: E501
+        """SearchIndexRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            dataset_id (str):
-            transaction_id (str):
+            type (SearchIndexType):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,15 +230,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            expiration_time (datetime, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,16 +256,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.dataset_id = dataset_id
-        self.transaction_id = transaction_id
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/marketplace_dimensions.py` & `whylabs-client-0.6.2/whylabs_client/model/marketplace_dimensions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/member.py` & `whylabs-client-0.6.2/whylabs_client/model/member.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/membership.py` & `whylabs-client-0.6.2/whylabs_client/model/membership.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/membership_metadata.py` & `whylabs-client-0.6.2/whylabs_client/model/membership_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/metric_schema.py` & `whylabs-client-0.6.2/whylabs_client/model/metric_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/model_metadata_response.py` & `whylabs-client-0.6.2/whylabs_client/model/model_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/model_type.py` & `whylabs-client-0.6.2/whylabs_client/model/model_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/monitor_config_version.py` & `whylabs-client-0.6.2/whylabs_client/model/monitor_config_version.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/notification_action.py` & `whylabs-client-0.6.2/whylabs_client/model/notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/notification_action_payload.py` & `whylabs-client-0.6.2/whylabs_client/model/notification_action_payload.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/notification_relationship_item.py` & `whylabs-client-0.6.2/whylabs_client/model/notification_relationship_item.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/notification_relationship_type.py` & `whylabs-client-0.6.2/whylabs_client/model/notification_relationship_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/notification_settings.py` & `whylabs-client-0.6.2/whylabs_client/model/notification_settings.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/notification_settings_day.py` & `whylabs-client-0.6.2/whylabs_client/model/notification_settings_day.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/notification_sqs_message_cadence.py` & `whylabs-client-0.6.2/whylabs_client/model/notification_sqs_message_cadence.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/organization_metadata.py` & `whylabs-client-0.6.2/whylabs_client/model/organization_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/organization_role_members.py` & `whylabs-client-0.6.2/whylabs_client/model/organization_role_members.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/organization_summary.py` & `whylabs-client-0.6.2/whylabs_client/model/organization_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/pager_duty_notification_action.py` & `whylabs-client-0.6.2/whylabs_client/model/pager_duty_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/patch_account_memberships_request.py` & `whylabs-client-0.6.2/whylabs_client/model/patch_account_memberships_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/post_asset_request.py` & `whylabs-client-0.6.2/whylabs_client/model/subscription_product_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class PostAssetRequest(ModelNormal):
+class SubscriptionProductFeature(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'org_id': (str,),  # noqa: E501
-            's3_uri': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'org_id': 'orgId',  # noqa: E501
-        's3_uri': 's3Uri',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, s3_uri, *args, **kwargs):  # noqa: E501
-        """PostAssetRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """SubscriptionProductFeature - a model defined in OpenAPI
 
         Args:
-            org_id (str):
-            s3_uri (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -164,16 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.org_id = org_id
-        self.s3_uri = s3_uri
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,20 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, s3_uri, *args, **kwargs):  # noqa: E501
-        """PostAssetRequest - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """SubscriptionProductFeature - a model defined in OpenAPI
 
         Args:
-            org_id (str):
-            s3_uri (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -249,16 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.org_id = org_id
-        self.s3_uri = s3_uri
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/profile_trace.py` & `whylabs-client-0.6.2/whylabs_client/model/profile_trace.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/profile_traces_response.py` & `whylabs-client-0.6.2/whylabs_client/model/profile_traces_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/provision_new_aws_marketplace_user_response.py` & `whylabs-client-0.6.2/whylabs_client/model/provision_new_aws_marketplace_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/provision_new_marketplace_user_request.py` & `whylabs-client-0.6.2/whylabs_client/model/provision_new_marketplace_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/provision_new_user_request.py` & `whylabs-client-0.6.2/whylabs_client/model/provision_new_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/provision_new_user_response.py` & `whylabs-client-0.6.2/whylabs_client/model/provision_new_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/put_account_memberships_request.py` & `whylabs-client-0.6.2/whylabs_client/model/put_account_memberships_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/reference_profile_item_response.py` & `whylabs-client-0.6.2/whylabs_client/model/reference_profile_item_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/remove_membership_request.py` & `whylabs-client-0.6.2/whylabs_client/model/remove_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/response.py` & `whylabs-client-0.6.2/whylabs_client/model/response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/revoke_user_session_request.py` & `whylabs-client-0.6.2/whylabs_client/model/revoke_user_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/role.py` & `whylabs-client-0.6.2/whylabs_client/model/role.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/schema_metadata.py` & `whylabs-client-0.6.2/whylabs_client/model/schema_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/search_index_request.py` & `whylabs-client-0.6.2/whylabs_client/model/set_default_membership_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.search_index_type import SearchIndexType
-    globals()['SearchIndexType'] = SearchIndexType
 
-
-class SearchIndexRequest(ModelNormal):
+class SetDefaultMembershipRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,58 +63,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'org_id': (str,),  # noqa: E501
-            'type': (SearchIndexType,),  # noqa: E501
+            'user_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'org_id': 'orgId',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'user_id': 'userId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, type, *args, **kwargs):  # noqa: E501
-        """SearchIndexRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, org_id, user_id, *args, **kwargs):  # noqa: E501
+        """SetDefaultMembershipRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            type (SearchIndexType):
+            user_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +165,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.type = type
+        self.user_id = user_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,20 +186,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, type, *args, **kwargs):  # noqa: E501
-        """SearchIndexRequest - a model defined in OpenAPI
+    def __init__(self, org_id, user_id, *args, **kwargs):  # noqa: E501
+        """SetDefaultMembershipRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            type (SearchIndexType):
+            user_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -256,15 +250,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.type = type
+        self.user_id = user_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/search_index_type.py` & `whylabs-client-0.6.2/whylabs_client/model/search_index_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/search_response.py` & `whylabs-client-0.6.2/whylabs_client/model/search_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/segment.py` & `whylabs-client-0.6.2/whylabs_client/model/segment_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.segment_tag import SegmentTag
-    globals()['SegmentTag'] = SegmentTag
 
-
-class Segment(ModelNormal):
+class SegmentTag(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -59,63 +55,70 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('key',): {
+            'min_length': 1,
+        },
+        ('value',): {
+            'min_length': 1,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'tags': ([SegmentTag],),  # noqa: E501
+            'key': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'tags': 'tags',  # noqa: E501
+        'key': 'key',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, tags, *args, **kwargs):  # noqa: E501
-        """Segment - a model defined in OpenAPI
+    def _from_openapi_data(cls, key, value, *args, **kwargs):  # noqa: E501
+        """SegmentTag - a model defined in OpenAPI
 
         Args:
-            tags ([SegmentTag]):
+            key (str):
+            value (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -167,15 +170,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.tags = tags
+        self.key = key
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -188,19 +192,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, tags, *args, **kwargs):  # noqa: E501
-        """Segment - a model defined in OpenAPI
+    def __init__(self, key, value, *args, **kwargs):  # noqa: E501
+        """SegmentTag - a model defined in OpenAPI
 
         Args:
-            tags ([SegmentTag]):
+            key (str):
+            value (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,15 +255,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.tags = tags
+        self.key = key
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/segment_list_response.py` & `whylabs-client-0.6.2/whylabs_client/model/segment_list_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/segment_tag.py` & `whylabs-client-0.6.2/whylabs_client/model/upload_asset_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class SegmentTag(ModelNormal):
+class UploadAssetRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,20 +55,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('key',): {
-            'min_length': 1,
-        },
-        ('value',): {
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -84,41 +78,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'key': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
+            'file_name': (str,),  # noqa: E501
+            'tag': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'key': 'key',  # noqa: E501
-        'value': 'value',  # noqa: E501
+        'file_name': 'fileName',  # noqa: E501
+        'tag': 'tag',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, key, value, *args, **kwargs):  # noqa: E501
-        """SegmentTag - a model defined in OpenAPI
+    def _from_openapi_data(cls, file_name, *args, **kwargs):  # noqa: E501
+        """UploadAssetRequest - a model defined in OpenAPI
 
         Args:
-            key (str):
-            value (str):
+            file_name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,14 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            tag (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,16 +164,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.key = key
-        self.value = value
+        self.file_name = file_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,20 +185,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, key, value, *args, **kwargs):  # noqa: E501
-        """SegmentTag - a model defined in OpenAPI
+    def __init__(self, file_name, *args, **kwargs):  # noqa: E501
+        """UploadAssetRequest - a model defined in OpenAPI
 
         Args:
-            key (str):
-            value (str):
+            file_name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,14 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            tag (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -255,16 +248,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.key = key
-        self.value = value
+        self.file_name = file_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/segment_weight.py` & `whylabs-client-0.6.2/whylabs_client/model/segment_weight.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/segments_list_request.py` & `whylabs-client-0.6.2/whylabs_client/model/segments_list_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/session_metadata.py` & `whylabs-client-0.6.2/whylabs_client/model/session_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/set_default_membership_request.py` & `whylabs-client-0.6.2/whylabs_client/model/post_asset_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class SetDefaultMembershipRequest(ModelNormal):
+class PostAssetRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -79,40 +79,42 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'org_id': (str,),  # noqa: E501
-            'user_id': (str,),  # noqa: E501
+            's3_uri': (str,),  # noqa: E501
+            'tag': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'org_id': 'orgId',  # noqa: E501
-        'user_id': 'userId',  # noqa: E501
+        's3_uri': 's3Uri',  # noqa: E501
+        'tag': 'tag',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, user_id, *args, **kwargs):  # noqa: E501
-        """SetDefaultMembershipRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, org_id, s3_uri, *args, **kwargs):  # noqa: E501
+        """PostAssetRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            user_id (str):
+            s3_uri (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,14 +139,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            tag (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -165,15 +168,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.user_id = user_id
+        self.s3_uri = s3_uri
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,20 +189,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, user_id, *args, **kwargs):  # noqa: E501
-        """SetDefaultMembershipRequest - a model defined in OpenAPI
+    def __init__(self, org_id, s3_uri, *args, **kwargs):  # noqa: E501
+        """PostAssetRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            user_id (str):
+            s3_uri (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,14 +227,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            tag (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -250,15 +254,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.user_id = user_id
+        self.s3_uri = s3_uri
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/slack_notification_action.py` & `whylabs-client-0.6.2/whylabs_client/model/slack_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/sort_order.py` & `whylabs-client-0.6.2/whylabs_client/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/status_response.py` & `whylabs-client-0.6.2/whylabs_client/model/status_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/subscription_product_feature.py` & `whylabs-client-0.6.2/whylabs_client/model/transaction_status_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class SubscriptionProductFeature(ModelNormal):
+class TransactionStatusResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
+            'files': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
+        'files': 'files',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """SubscriptionProductFeature - a model defined in OpenAPI
+    def _from_openapi_data(cls, files, *args, **kwargs):  # noqa: E501
+        """TransactionStatusResponse - a model defined in OpenAPI
 
         Args:
-            name (str):
+            files ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,15 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.files = files
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """SubscriptionProductFeature - a model defined in OpenAPI
+    def __init__(self, files, *args, **kwargs):  # noqa: E501
+        """TransactionStatusResponse - a model defined in OpenAPI
 
         Args:
-            name (str):
+            files ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,15 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.files = files
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/subscription_product_summary.py` & `whylabs-client-0.6.2/whylabs_client/model/subscription_product_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/subscription_summary.py` & `whylabs-client-0.6.2/whylabs_client/model/subscription_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/subscription_tier.py` & `whylabs-client-0.6.2/whylabs_client/model/subscription_tier.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/time_period.py` & `whylabs-client-0.6.2/whylabs_client/model/time_period.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/transaction_commit_request.py` & `whylabs-client-0.6.2/whylabs_client/model/transaction_commit_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/transaction_log_request.py` & `whylabs-client-0.6.2/whylabs_client/model/transaction_log_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/transaction_start_request.py` & `whylabs-client-0.6.2/whylabs_client/model/transaction_start_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/transaction_status_response.py` & `whylabs-client-0.6.2/whylabs_client/model/add_policy_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class TransactionStatusResponse(ModelNormal):
+class AddPolicyResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'files': ([str],),  # noqa: E501
+            'version': (int,),  # noqa: E501
+            'label': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'files': 'files',  # noqa: E501
+        'version': 'version',  # noqa: E501
+        'label': 'label',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, files, *args, **kwargs):  # noqa: E501
-        """TransactionStatusResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, version, *args, **kwargs):  # noqa: E501
+        """AddPolicyResponse - a model defined in OpenAPI
 
         Args:
-            files ([str]):
+            version (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,14 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            label (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -161,15 +164,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.files = files
+        self.version = version
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +185,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, files, *args, **kwargs):  # noqa: E501
-        """TransactionStatusResponse - a model defined in OpenAPI
+    def __init__(self, version, *args, **kwargs):  # noqa: E501
+        """AddPolicyResponse - a model defined in OpenAPI
 
         Args:
-            files ([str]):
+            version (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,14 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            label (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -244,15 +248,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.files = files
+        self.version = version
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.1/whylabs_client/model/uber_notification_schedule.py` & `whylabs-client-0.6.2/whylabs_client/model/uber_notification_schedule.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/update_account_user_request.py` & `whylabs-client-0.6.2/whylabs_client/model/update_account_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/update_membership_request.py` & `whylabs-client-0.6.2/whylabs_client/model/update_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/user.py` & `whylabs-client-0.6.2/whylabs_client/model/user.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/user_api_key.py` & `whylabs-client-0.6.2/whylabs_client/model/user_api_key.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/user_api_key_response.py` & `whylabs-client-0.6.2/whylabs_client/model/user_api_key_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model/validate_user_session_response.py` & `whylabs-client-0.6.2/whylabs_client/model/validate_user_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/model_utils.py` & `whylabs-client-0.6.2/whylabs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client/models/__init__.py` & `whylabs-client-0.6.2/whylabs_client/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from whylabs_client.model.aws_marketplace_metadata import AWSMarketplaceMetadata
 from whylabs_client.model.account_organization import AccountOrganization
 from whylabs_client.model.account_user import AccountUser
 from whylabs_client.model.action_type import ActionType
 from whylabs_client.model.activate_azure_subscription_request import ActivateAzureSubscriptionRequest
 from whylabs_client.model.activate_azure_subscription_response import ActivateAzureSubscriptionResponse
 from whylabs_client.model.add_membership_request import AddMembershipRequest
+from whylabs_client.model.add_policy_response import AddPolicyResponse
 from whylabs_client.model.admin_report_response import AdminReportResponse
 from whylabs_client.model.admin_report_type import AdminReportType
 from whylabs_client.model.analysis_results_record import AnalysisResultsRecord
 from whylabs_client.model.analysis_results_request import AnalysisResultsRequest
 from whylabs_client.model.analysis_results_response import AnalysisResultsResponse
 from whylabs_client.model.analyzer_diagnostic_record import AnalyzerDiagnosticRecord
 from whylabs_client.model.analyzer_failure_record import AnalyzerFailureRecord
@@ -69,28 +70,32 @@
 from whylabs_client.model.get_default_membership_response import GetDefaultMembershipResponse
 from whylabs_client.model.get_marketplace_metadata_response import GetMarketplaceMetadataResponse
 from whylabs_client.model.get_memberships_response import GetMembershipsResponse
 from whylabs_client.model.get_notification_settings_response import GetNotificationSettingsResponse
 from whylabs_client.model.get_profile_observatory_link_request import GetProfileObservatoryLinkRequest
 from whylabs_client.model.get_profile_observatory_link_response import GetProfileObservatoryLinkResponse
 from whylabs_client.model.get_session_response import GetSessionResponse
+from whylabs_client.model.granularity import Granularity
 from whylabs_client.model.list_models_response import ListModelsResponse
 from whylabs_client.model.list_organization_memberships_response import ListOrganizationMembershipsResponse
 from whylabs_client.model.list_user_api_keys import ListUserApiKeys
 from whylabs_client.model.log_async_request import LogAsyncRequest
 from whylabs_client.model.log_reference_request import LogReferenceRequest
 from whylabs_client.model.log_reference_response import LogReferenceResponse
 from whylabs_client.model.log_response import LogResponse
 from whylabs_client.model.log_session_reference_response import LogSessionReferenceResponse
 from whylabs_client.model.log_transaction_metadata import LogTransactionMetadata
 from whylabs_client.model.marketplace_dimensions import MarketplaceDimensions
 from whylabs_client.model.member import Member
 from whylabs_client.model.membership import Membership
 from whylabs_client.model.membership_metadata import MembershipMetadata
 from whylabs_client.model.metric_schema import MetricSchema
+from whylabs_client.model.metric_timeseries_record import MetricTimeseriesRecord
+from whylabs_client.model.metric_timeseries_request import MetricTimeseriesRequest
+from whylabs_client.model.metric_timeseries_response import MetricTimeseriesResponse
 from whylabs_client.model.model_metadata_response import ModelMetadataResponse
 from whylabs_client.model.model_type import ModelType
 from whylabs_client.model.monitor_config_version import MonitorConfigVersion
 from whylabs_client.model.notification_action import NotificationAction
 from whylabs_client.model.notification_action_payload import NotificationActionPayload
 from whylabs_client.model.notification_relationship_item import NotificationRelationshipItem
 from whylabs_client.model.notification_relationship_type import NotificationRelationshipType
@@ -99,14 +104,15 @@
 from whylabs_client.model.notification_sqs_message_cadence import NotificationSqsMessageCadence
 from whylabs_client.model.organization_metadata import OrganizationMetadata
 from whylabs_client.model.organization_role_members import OrganizationRoleMembers
 from whylabs_client.model.organization_summary import OrganizationSummary
 from whylabs_client.model.pager_duty_notification_action import PagerDutyNotificationAction
 from whylabs_client.model.patch_account_memberships_request import PatchAccountMembershipsRequest
 from whylabs_client.model.post_asset_request import PostAssetRequest
+from whylabs_client.model.post_asset_response import PostAssetResponse
 from whylabs_client.model.profile_trace import ProfileTrace
 from whylabs_client.model.profile_traces_response import ProfileTracesResponse
 from whylabs_client.model.provision_new_aws_marketplace_user_response import ProvisionNewAWSMarketplaceUserResponse
 from whylabs_client.model.provision_new_marketplace_user_request import ProvisionNewMarketplaceUserRequest
 from whylabs_client.model.provision_new_user_request import ProvisionNewUserRequest
 from whylabs_client.model.provision_new_user_response import ProvisionNewUserResponse
 from whylabs_client.model.put_account_memberships_request import PutAccountMembershipsRequest
@@ -137,11 +143,13 @@
 from whylabs_client.model.transaction_commit_request import TransactionCommitRequest
 from whylabs_client.model.transaction_log_request import TransactionLogRequest
 from whylabs_client.model.transaction_start_request import TransactionStartRequest
 from whylabs_client.model.transaction_status_response import TransactionStatusResponse
 from whylabs_client.model.uber_notification_schedule import UberNotificationSchedule
 from whylabs_client.model.update_account_user_request import UpdateAccountUserRequest
 from whylabs_client.model.update_membership_request import UpdateMembershipRequest
+from whylabs_client.model.upload_asset_request import UploadAssetRequest
+from whylabs_client.model.upload_asset_response import UploadAssetResponse
 from whylabs_client.model.user import User
 from whylabs_client.model.user_api_key import UserApiKey
 from whylabs_client.model.user_api_key_response import UserApiKeyResponse
 from whylabs_client.model.validate_user_session_response import ValidateUserSessionResponse
```

### Comparing `whylabs-client-0.6.1/whylabs_client/rest.py` & `whylabs-client-0.6.2/whylabs_client/rest.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.1/whylabs_client.egg-info/PKG-INFO` & `whylabs-client-0.6.2/whylabs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.6.1/whylabs_client.egg-info/SOURCES.txt` & `whylabs-client-0.6.2/whylabs_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 whylabs_client/model/__init__.py
 whylabs_client/model/account_organization.py
 whylabs_client/model/account_user.py
 whylabs_client/model/action_type.py
 whylabs_client/model/activate_azure_subscription_request.py
 whylabs_client/model/activate_azure_subscription_response.py
 whylabs_client/model/add_membership_request.py
+whylabs_client/model/add_policy_response.py
 whylabs_client/model/admin_report_response.py
 whylabs_client/model/admin_report_type.py
 whylabs_client/model/analysis_results_record.py
 whylabs_client/model/analysis_results_request.py
 whylabs_client/model/analysis_results_response.py
 whylabs_client/model/analyzer_diagnostic_record.py
 whylabs_client/model/analyzer_failure_record.py
@@ -94,28 +95,32 @@
 whylabs_client/model/get_default_membership_response.py
 whylabs_client/model/get_marketplace_metadata_response.py
 whylabs_client/model/get_memberships_response.py
 whylabs_client/model/get_notification_settings_response.py
 whylabs_client/model/get_profile_observatory_link_request.py
 whylabs_client/model/get_profile_observatory_link_response.py
 whylabs_client/model/get_session_response.py
+whylabs_client/model/granularity.py
 whylabs_client/model/list_models_response.py
 whylabs_client/model/list_organization_memberships_response.py
 whylabs_client/model/list_user_api_keys.py
 whylabs_client/model/log_async_request.py
 whylabs_client/model/log_reference_request.py
 whylabs_client/model/log_reference_response.py
 whylabs_client/model/log_response.py
 whylabs_client/model/log_session_reference_response.py
 whylabs_client/model/log_transaction_metadata.py
 whylabs_client/model/marketplace_dimensions.py
 whylabs_client/model/member.py
 whylabs_client/model/membership.py
 whylabs_client/model/membership_metadata.py
 whylabs_client/model/metric_schema.py
+whylabs_client/model/metric_timeseries_record.py
+whylabs_client/model/metric_timeseries_request.py
+whylabs_client/model/metric_timeseries_response.py
 whylabs_client/model/model_metadata_response.py
 whylabs_client/model/model_type.py
 whylabs_client/model/monitor_config_version.py
 whylabs_client/model/notification_action.py
 whylabs_client/model/notification_action_payload.py
 whylabs_client/model/notification_relationship_item.py
 whylabs_client/model/notification_relationship_type.py
@@ -124,14 +129,15 @@
 whylabs_client/model/notification_sqs_message_cadence.py
 whylabs_client/model/organization_metadata.py
 whylabs_client/model/organization_role_members.py
 whylabs_client/model/organization_summary.py
 whylabs_client/model/pager_duty_notification_action.py
 whylabs_client/model/patch_account_memberships_request.py
 whylabs_client/model/post_asset_request.py
+whylabs_client/model/post_asset_response.py
 whylabs_client/model/profile_trace.py
 whylabs_client/model/profile_traces_response.py
 whylabs_client/model/provision_new_aws_marketplace_user_response.py
 whylabs_client/model/provision_new_marketplace_user_request.py
 whylabs_client/model/provision_new_user_request.py
 whylabs_client/model/provision_new_user_response.py
 whylabs_client/model/put_account_memberships_request.py
@@ -162,12 +168,14 @@
 whylabs_client/model/transaction_commit_request.py
 whylabs_client/model/transaction_log_request.py
 whylabs_client/model/transaction_start_request.py
 whylabs_client/model/transaction_status_response.py
 whylabs_client/model/uber_notification_schedule.py
 whylabs_client/model/update_account_user_request.py
 whylabs_client/model/update_membership_request.py
+whylabs_client/model/upload_asset_request.py
+whylabs_client/model/upload_asset_response.py
 whylabs_client/model/user.py
 whylabs_client/model/user_api_key.py
 whylabs_client/model/user_api_key_response.py
 whylabs_client/model/validate_user_session_response.py
 whylabs_client/models/__init__.py
```

