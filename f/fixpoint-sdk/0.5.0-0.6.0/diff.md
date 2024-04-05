# Comparing `tmp/fixpoint_sdk-0.5.0.tar.gz` & `tmp/fixpoint_sdk-0.6.0.tar.gz`

## Comparing `fixpoint_sdk-0.5.0.tar` & `fixpoint_sdk-0.6.0.tar`

### file list

```diff
@@ -1,176 +1,179 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/.editorconfig
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/.lintstagedrc.json
--rw-r--r--   0        0        0    21691 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/.pylintrc
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/mypy.ini
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/pytest.ini
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/requirements.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/test-requirements.txt
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/.github/workflows/pypi-release-prod.yml
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/.github/workflows/pypi-release-test.yml
--rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/bin/pip-freeze
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/bin/pip-install
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/examples/__init__.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/examples/main.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/examples/streaming.py
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/githooks/pre-commit
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/__init__.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/client.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/compat.py
--rw-r--r--   0        0        0    10547 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/completions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/__init__.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/debugging.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/env.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/exc.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/iterwrapper.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/logging.py
--rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/requests.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.gitignore
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.gitlab-ci.yml
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.openapi-generator-ignore
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.travis.yml
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/README.md
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/git_push.sh
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/pyproject.toml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/setup.cfg
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/setup.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/test-requirements.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/tox.ini
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.github/workflows/python.yml
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/FILES
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/VERSION
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/AppLogLevelType.md
--rw-r--r--   0        0        0    44192 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyApi.md
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatInputLogRequest.md
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatOutputLogRequest.md
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyPostDatasetLogsRequest.md
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyUpdateSpendingTotalsRequest.md
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogChoice.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogUsage.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufAny.md
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufNullValue.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/RpcStatus.md
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecret.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecretProvider.md
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1AppLog.md
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1AttributeFilters.md
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateApiSecretRequest.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsRequest.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsResponse.md
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetRequest.md
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetResponse.md
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesRequest.md
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesResponse.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeRequest.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeResponse.md
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateRoutingConfigRequest.md
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Dataset.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1DatasetFilters.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1DeleteLogAttributeResponse.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1FallbackStrategy.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Like.md
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeFilter.md
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeIngest.md
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListApiSecretsResponse.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListAppLogsResponse.md
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListDatasetsResponse.md
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLikesResponse.md
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLogAttributesResponse.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListOpenAIChatLogsResponse.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListRoutingConfigsResponse.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1LogAttribute.md
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Message.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Mode.md
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Model.md
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatInputLog.md
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLog.md
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLogsFilters.md
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatOutputLog.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OriginType.md
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1PostDatasetLogsResponse.md
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1RelativeDateTimeFilters.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ResetInterval.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1RoutingConfig.md
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1SpendCap.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1TerminalState.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ThumbsReaction.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1UsageTotals.md
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/__init__.py
--rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_client.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_response.py
--rw-r--r--   0        0        0    14511 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/configuration.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/py.typed
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/rest.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/__init__.py
--rw-r--r--   0        0        0   198013 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/llm_proxy_api.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/app_log_level_type.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_input_log_request.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_output_log_request.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_post_dataset_logs_request.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_update_spending_totals_request.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_choice.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_usage.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_any.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_null_value.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/rpc_status.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret_provider.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_app_log.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_attribute_filters.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_api_secret_request.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_request.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_response.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_request.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_response.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_request.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_response.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_request.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_response.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_routing_config_request.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset_filters.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_delete_log_attribute_response.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_fallback_strategy.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_filter.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_ingest.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_api_secrets_response.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_app_logs_response.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_datasets_response.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_likes_response.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_log_attributes_response.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_open_ai_chat_logs_response.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_routing_configs_response.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_log_attribute.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_message.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_mode.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_model.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_input_log.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_log.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_logs_filters.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_output_log.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_origin_type.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_post_dataset_logs_response.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_relative_date_time_filters.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_reset_interval.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_routing_config.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_spend_cap.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_terminal_state.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_thumbs_reaction.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_usage_totals.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/src/fixpoint_sdk/types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/tests/mock_completions.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/tests/test_completions.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/tests/test_types.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/tests/lib/test_iterwrapper.py
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/tests/lib/test_requests.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/LICENSE
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/README.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 fixpoint_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.editorconfig
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.lintstagedrc.json
+-rw-r--r--   0        0        0    21691 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.pylintrc
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/mypy.ini
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/pytest.ini
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/requirements.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/test-requirements.txt
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.github/workflows/pypi-release-prod.yml
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.github/workflows/pypi-release-test.yml
+-rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/bin/pip-freeze
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/bin/pip-install
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/examples/__init__.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/examples/main.py
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/examples/router.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/examples/streaming.py
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/githooks/pre-commit
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/__init__.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/client.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/compat.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/completions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/__init__.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/debugging.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/env.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/exc.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/iterwrapper.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/logging.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/requests.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/exceptions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.gitignore
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.openapi-generator-ignore
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.travis.yml
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/README.md
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/git_push.sh
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/pyproject.toml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/setup.cfg
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/setup.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/test-requirements.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/tox.ini
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.github/workflows/python.yml
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/FILES
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/VERSION
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/AppLogLevelType.md
+-rw-r--r--   0        0        0    44192 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyApi.md
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatInputLogRequest.md
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatOutputLogRequest.md
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyPostDatasetLogsRequest.md
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyUpdateSpendingTotalsRequest.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogChoice.md
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogUsage.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufAny.md
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufNullValue.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/RpcStatus.md
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecret.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecretProvider.md
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1AppLog.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1AttributeFilters.md
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateApiSecretRequest.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsRequest.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsResponse.md
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetRequest.md
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetResponse.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesRequest.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesResponse.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeRequest.md
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeResponse.md
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateRoutingConfigRequest.md
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Dataset.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1DatasetFilters.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1DeleteLogAttributeResponse.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1FallbackStrategy.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Like.md
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeFilter.md
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeIngest.md
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListApiSecretsResponse.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListAppLogsResponse.md
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListDatasetsResponse.md
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLikesResponse.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLogAttributesResponse.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListOpenAIChatLogsResponse.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListRoutingConfigsResponse.md
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LogAttribute.md
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Message.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Mode.md
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Model.md
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatInputLog.md
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLog.md
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLogsFilters.md
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatOutputLog.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OriginType.md
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1PostDatasetLogsResponse.md
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1RelativeDateTimeFilters.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ResetInterval.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1RoutingConfig.md
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1SpendCap.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1TerminalState.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ThumbsReaction.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1UsageTotals.md
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/__init__.py
+-rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_client.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_response.py
+-rw-r--r--   0        0        0    14511 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/configuration.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/py.typed
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/rest.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0   198013 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/llm_proxy_api.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/app_log_level_type.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_input_log_request.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_output_log_request.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_post_dataset_logs_request.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_update_spending_totals_request.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_choice.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_usage.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_any.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_null_value.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/rpc_status.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret_provider.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_app_log.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_attribute_filters.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_api_secret_request.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_request.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_response.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_request.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_response.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_request.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_response.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_request.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_response.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_routing_config_request.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset_filters.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_delete_log_attribute_response.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_fallback_strategy.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_filter.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_ingest.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_api_secrets_response.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_app_logs_response.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_datasets_response.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_likes_response.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_log_attributes_response.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_open_ai_chat_logs_response.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_routing_configs_response.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_log_attribute.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_message.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_mode.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_model.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_input_log.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_log.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_logs_filters.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_output_log.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_origin_type.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_post_dataset_logs_response.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_relative_date_time_filters.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_reset_interval.py
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_routing_config.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_spend_cap.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_terminal_state.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_thumbs_reaction.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_usage_totals.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/mock_completions.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/test_completions.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/test_types.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/lib/test_iterwrapper.py
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/lib/test_requests.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/README.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/PKG-INFO
```

### Comparing `fixpoint_sdk-0.5.0/.pylintrc` & `fixpoint_sdk-0.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/mypy.ini` & `fixpoint_sdk-0.6.0/mypy.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [mypy]
-exclude = (examples/|venv/|src/fixpoint_sdk/openapi)
+exclude = (venv/|src/fixpoint_sdk/openapi/gen)
 # Start off with these
 warn_unused_configs = True
 warn_redundant_casts = True
 warn_unused_ignores = True
 
 # Getting these passing should be easy
 strict_equality = True
@@ -20,14 +20,16 @@
 
 # These next few are various gradations of forcing use of type annotations
 disallow_untyped_calls = False
 disallow_incomplete_defs = True
 disallow_untyped_defs = True
 
 # This one isn't too hard to get passing, but return on investment is lower
-no_implicit_reexport = True
+no_implicit_reexport = False
 
 # This one can be tricky to get passing if you use a lot of untyped libraries
 warn_return_any = True
 
 # It's ok if our third party imports are not typed
 ignore_missing_imports = True
+
+plugins = pydantic.mypy
```

### Comparing `fixpoint_sdk-0.5.0/requirements.txt` & `fixpoint_sdk-0.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/.github/workflows/ci.yml` & `fixpoint_sdk-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/.github/workflows/pypi-release-prod.yml` & `fixpoint_sdk-0.6.0/.github/workflows/pypi-release-prod.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/.github/workflows/pypi-release-test.yml` & `fixpoint_sdk-0.6.0/.github/workflows/pypi-release-test.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/bin/pip-freeze` & `fixpoint_sdk-0.6.0/bin/pip-freeze`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/examples/streaming.py` & `fixpoint_sdk-0.6.0/examples/streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     # You can iterate via `resp.completions`, like below, or via `resp` directly like:
     #
     #     for chunk in resp:
     #         ...
     #
     # Pylint is getting this wrong
     # pylint: disable=not-an-iterable
-    for chunk in resp.completions:
+    for chunk in resp.completion:
         content = chunk.choices[0].delta.content
         if content:
             text_contents.append(content)
     print(f"Output text: {''.join(text_contents)}")
     output_log = resp.output_log
     assert output_log is not None
     print(f"Logged output with ID/name: {output_log['name']}")
```

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/client.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,112 @@
 """Defines the Fixpoint client, which is the main interface for the SDK."""
 
 import typing
 
 from openai import OpenAI
 
-from fixpoint_sdk.openapi.gen.openapi_client.configuration import Configuration
-from fixpoint_sdk.openapi.gen.openapi_client.api_client import ApiClient
-from fixpoint_sdk.openapi.gen.openapi_client.api.llm_proxy_api import LLMProxyApi
+from .openapi.gen.openapi_client.configuration import Configuration
+from .openapi.gen.openapi_client.api_client import ApiClient
+from .openapi.gen.openapi_client.api.llm_proxy_api import LLMProxyApi
 
 from .lib.env import get_fixpoint_api_key, get_api_base_url
 from .lib.requests import Requester
 from . import types
 from .completions import Chat, ChatWithRouter
 
 
-class ChatRouterClient:
-    """The ChatRouterClient lets you interact with the Fixpoint API and the OpenAI API."""
-
+class _FixpointClientBase:
     def __init__(
         self,
-        *args: typing.Any,
+        *,
         fixpoint_api_key: typing.Optional[str] = None,
         openai_api_key: typing.Optional[str] = None,
         api_base_url: typing.Optional[str] = None,
         **kwargs: typing.Any,
     ):
         # Check that the environment variable FIXPOINT_API_KEY is set
         _api_key = get_fixpoint_api_key(fixpoint_api_key)
 
         self._api_key = _api_key
         self._requester = Requester(self._api_key, get_api_base_url(api_base_url))
         if openai_api_key:
             kwargs = dict(kwargs, api_key=openai_api_key)
-        self.client = OpenAI(*args, **kwargs)
-        self.chat = ChatWithRouter(self._requester, self.client)
+        self.fixpoint = _Fixpoint(self._requester)
+
 
+class ChatRouterClient(_FixpointClientBase):
+    """The ChatRouterClient lets you interact with the Fixpoint API and the OpenAI API."""
 
-class FixpointClient:
+    def __init__(
+        self,
+        *,
+        fixpoint_api_key: typing.Optional[str] = None,
+        openai_api_key: typing.Optional[str] = None,
+        api_base_url: typing.Optional[str] = None,
+        **kwargs: typing.Any,
+    ):
+        super().__init__(
+            fixpoint_api_key=fixpoint_api_key,
+            openai_api_key=openai_api_key,
+            api_base_url=api_base_url,
+            **kwargs,
+        )
+        client = OpenAI(**kwargs)
+        self.chat = ChatWithRouter(self._requester, client)
+
+
+class FixpointClient(_FixpointClientBase):
     """The FixpointClient lets you interact with the Fixpoint API."""
 
     def __init__(
         self,
-        *args: typing.Any,
+        *,
         fixpoint_api_key: typing.Optional[str] = None,
         openai_api_key: typing.Optional[str] = None,
         api_base_url: typing.Optional[str] = None,
         **kwargs: typing.Any,
     ):
-        # Check that the environment variable FIXPOINT_API_KEY is set
-        _api_key = get_fixpoint_api_key(fixpoint_api_key)
+        super().__init__(
+            fixpoint_api_key=fixpoint_api_key,
+            openai_api_key=openai_api_key,
+            api_base_url=api_base_url,
+            **kwargs,
+        )
+        client = OpenAI(**kwargs)
+        self.chat = Chat(self._requester, client)
+
+
+class _Fixpoint:
+    def __init__(self, requester: Requester):
+        self.user_feedback = self._UserFeedback(requester)
+        self.attributes = self._Attributes(requester)
+
+        configuration = Configuration(
+            host=get_api_base_url(requester.base_url),
+        )
+
+        api_client = ApiClient(
+            configuration,
+            header_name="Authorization",
+            header_value=f"Bearer {requester.api_key}",
+        )
+        self.proxy_client = LLMProxyApi(api_client)
 
-        self._api_key = _api_key
-        self._requester = Requester(self._api_key, get_api_base_url(api_base_url))
-        if openai_api_key:
-            kwargs = dict(kwargs, api_key=openai_api_key)
-        self.client = OpenAI(*args, **kwargs)
-        self.chat = Chat(self._requester, self.client)
-        self.fixpoint = self._Fixpoint(self._requester)
+    class _UserFeedback:
+        def __init__(self, requester: Requester):
+            self._requester = requester
+
+        def create(
+            self, request: types.CreateUserFeedbackRequest
+        ) -> types.CreateUserFeedbackResponse:
+            """Attach user feedback to an LLM log."""
+            return self._requester.create_user_feedback(request)
 
-    class _Fixpoint:
+    class _Attributes:
         def __init__(self, requester: Requester):
-            self.user_feedback = self._UserFeedback(requester)
-            self.attributes = self._Attributes(requester)
+            self._requester = requester
 
-            configuration = Configuration(
-                host=get_api_base_url(requester.base_url),
-            )
-
-            api_client = ApiClient(
-                configuration,
-                header_name="Authorization",
-                header_value=f"Bearer {requester.api_key}",
-            )
-            self.proxy_client = LLMProxyApi(api_client)
-
-        class _UserFeedback:
-            def __init__(self, requester: Requester):
-                self._requester = requester
-
-            def create(
-                self, request: types.CreateUserFeedbackRequest
-            ) -> types.CreateUserFeedbackResponse:
-                """Attach user feedback to an LLM log."""
-                return self._requester.create_user_feedback(request)
-
-        class _Attributes:
-            def __init__(self, requester: Requester):
-                self._requester = requester
-
-            def create(
-                self, request: types.CreateLogAttributeRequest
-            ) -> types.LogAttribute:
-                """Attach a log attribute to an LLM log."""
-                return self._requester.create_attribute(request)
+        def create(
+            self, request: types.CreateLogAttributeRequest
+        ) -> types.LogAttribute:
+            """Attach a log attribute to an LLM log."""
+            return self._requester.create_attribute(request)
```

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/compat.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/compat.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/completions.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/completions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,48 @@
 """Code for chat completions."""
 
 import typing
-from typing import Optional, Literal, Generator
+from typing import Optional, Literal, List, Generator
 from dataclasses import dataclass
 
 from openai import OpenAI
 from openai._streaming import Stream
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 from openai.types.chat.chat_completion import Choice
 from openai.types.chat.chat_completion_message import ChatCompletionMessage
+from openai.types.chat.chat_completion_message_param import ChatCompletionMessageParam
 
 from .lib.requests import Requester
 from .lib.debugging import dprint
 from .lib.iterwrapper import IterWrapper
 from .lib.logging import logger
 from . import types
 
 
+Model = typing.Union[
+    str,
+    Literal[
+        "gpt-4-1106-preview",
+        "gpt-4-vision-preview",
+        "gpt-4",
+        "gpt-4-0314",
+        "gpt-4-0613",
+        "gpt-4-32k",
+        "gpt-4-32k-0314",
+        "gpt-4-32k-0613",
+        "gpt-3.5-turbo",
+        "gpt-3.5-turbo-16k",
+        "gpt-3.5-turbo-0301",
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-1106",
+        "gpt-3.5-turbo-16k-0613",
+    ],
+]
+
+
 @dataclass
 class FixpointChatRoutedCompletion:
     """Wraps the OpenAI chat completion with logging data."""
 
     completion: types.ChatCompletion
 
 
@@ -97,19 +119,26 @@
 
     # pylint: disable=use-yield-from
     def __iter__(self) -> typing.Iterator[ChatCompletionChunk]:
         """Yield the chat completion chunks."""
         return self
 
     @property
-    def completions(self) -> Generator[ChatCompletionChunk, None, None]:
+    def completion(self) -> Generator[ChatCompletionChunk, None, None]:
         """Yield the chat completion chunks."""
         for chunk in self:
             yield chunk
 
+    # This function is deprecated, because `completion` exists on all inference
+    # response types while `completions` only exists on streaming response.
+    @property
+    def completions(self) -> Generator[ChatCompletionChunk, None, None]:
+        """Yield the chat completion chunks."""
+        return self.completion
+
     @property
     def output_log(self) -> typing.Optional[types.OutputLog]:
         """Returns the output log if we have streamed all output chunks."""
         if not self._all_streamed:
             logger.warning(
                 "\n".join(
                     [
@@ -188,105 +217,129 @@
     def __init__(self, requester: Requester, client: OpenAI):
         self.client = client
         self._requester = requester
 
     @typing.overload
     def create(
         self,
-        *args: typing.Any,
-        mode: Optional[types.ModeArg] = None,
-        stream: Optional[Literal[False]] = None,
+        *,
+        messages: List[ChatCompletionMessageParam],
+        model: Model,
+        stream: Optional[Literal[False]],
         **kwargs: typing.Any,
     ) -> FixpointChatCompletion: ...
 
     @typing.overload
     def create(
         self,
-        *args: typing.Any,
-        mode: Optional[types.ModeArg] = None,
+        *,
+        messages: List[ChatCompletionMessageParam],
+        model: Model,
         stream: Literal[True],
         **kwargs: typing.Any,
     ) -> FixpointChatCompletionStream: ...
 
+    @typing.overload
     def create(
         self,
-        *args: typing.Any,
+        *,
+        messages: List[ChatCompletionMessageParam],
+        model: Model,
+        stream: bool,
+        **kwargs: typing.Any,
+    ) -> typing.Union[FixpointChatCompletion, FixpointChatCompletionStream]: ...
+
+    @typing.overload
+    def create(
+        self,
+        *,
+        messages: List[ChatCompletionMessageParam],
+        model: Model,
+        stream: typing.Union[Optional[Literal[False]], Literal[True]] = None,
+        **kwargs: typing.Any,
+    ) -> typing.Union[FixpointChatCompletion, FixpointChatCompletionStream]: ...
+
+    def create(
+        self,
+        *,
+        messages: List[ChatCompletionMessageParam],
+        model: Model,
+        stream: typing.Union[Optional[Literal[False]], Literal[True]] = None,
         mode: Optional[types.ModeArg] = "unspecified",
         **kwargs: typing.Any,
     ) -> typing.Union[FixpointChatCompletion, FixpointChatCompletionStream]:
         """Create an OpenAI completion and log the LLM input and output."""
         # Do not mutate the input kwargs. That is an unexpected behavior for
         # our caller.
         kwargs = kwargs.copy()
         # Extract trace_id from kwargs, if it exists, otherwise set it to None
         trace_id = kwargs.pop("trace_id", None)
         mode_type = types.parse_mode_type(mode)
 
         # Deep copy the kwargs to avoid modifying the original
         req_copy = kwargs.copy()
-        if "model" not in req_copy:
-            raise ValueError("model needs to be passed in as a kwarg")
-        req_copy["model_name"] = req_copy.pop("model")
+        req_copy["model_name"] = model
+        req_copy["messages"] = messages
 
         # Send HTTP request before calling create
         input_resp = self._requester.create_openai_input_log(
             req_copy["model_name"],
             # TODO(dbmikus) fix sloppy typing
             typing.cast(types.OpenAILLMInputLog, req_copy),
             trace_id=trace_id,
             mode=mode_type,
         )
         dprint(f'Created an input log: {input_resp["name"]}')
 
-        stream = kwargs.get("stream", False)
-        # Make create call to OPEN AI
-        openai_response = self.client.chat.completions.create(*args, **kwargs)
         if stream:
-            dprint("Received an openai response stream")
-        else:
-            dprint(f"Received an openai response: {openai_response.id}")
-
-        if not stream:
-            # Send HTTP request after calling create
-            output_resp = self._requester.create_openai_output_log(
-                req_copy["model_name"],
-                input_resp,
-                openai_response,
-                trace_id=trace_id,
-                mode=mode_type,
+            openai_response = self.client.chat.completions.create(
+                messages=messages, model=model, stream=stream, **kwargs
             )
-            dprint(f"Created an output log: {output_resp['name']}")
-            return FixpointChatCompletion(
-                completion=openai_response,
+            dprint("Received an openai response stream")
+            return FixpointChatCompletionStream(
+                stream=openai_response,
                 input_log=input_resp,
-                output_log=output_resp,
+                mode_type=mode_type,
+                requester=self._requester,
+                trace_id=trace_id,
+                model_name=req_copy["model_name"],
             )
 
-        return FixpointChatCompletionStream(
-            stream=openai_response,
-            input_log=input_resp,
-            mode_type=mode_type,
-            requester=self._requester,
+        openai_response = self.client.chat.completions.create(
+            messages=messages, model=model, stream=stream, **kwargs
+        )
+        dprint(f"Received an openai response: {openai_response.id}")
+        # Send HTTP request after calling create
+        output_resp = self._requester.create_openai_output_log(
+            req_copy["model_name"],
+            input_resp,
+            openai_response,
             trace_id=trace_id,
-            model_name=req_copy["model_name"],
+            mode=mode_type,
+        )
+        dprint(f"Created an output log: {output_resp['name']}")
+        return FixpointChatCompletion(
+            completion=openai_response,
+            input_log=input_resp,
+            output_log=output_resp,
         )
 
 
 class RoutedCompletions:
     """Create chat completion inferences and log them."""
 
     def __init__(self, requester: Requester, client: OpenAI):
         self._requester = requester
         self._client = client
 
     def create(
         self,
         mode: Optional[types.ModeArg] = "unspecified",
         **kwargs: typing.Any,
-    ) -> typing.Union[FixpointChatRoutedCompletion]:
+    ) -> FixpointChatRoutedCompletion:
         """Create an OpenAI completion and log the LLM input and output."""
         # Prepare the request
         req_copy = kwargs.copy()
         trace_id = kwargs.pop("trace_id", None)
 
         routed_log_resp = self._requester.create_openai_routed_log(
             typing.cast(types.OpenAILLMInputLog, req_copy),
```

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/debugging.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/debugging.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/env.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/env.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/iterwrapper.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/lib/requests.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 
 import requests
 from openai.types.chat import ChatCompletion
 
 from .debugging import debug_log_function_io
 from .. import types
+from ..lib import exc
 
 DEFAULT_TIMEOUT_S = 60
 
 ApiCallback = typing.Callable[[str, typing.Any, typing.Any], None]
 
 
 class Requester:
@@ -202,11 +203,14 @@
         headers = {
             "Accept": "application/json",
             "Authorization": f"Bearer {self.api_key}",
         }
         resp = requests.post(
             url, headers=headers, json=req_or_resp_obj, timeout=self.timeout_s
         )
-        resp.raise_for_status()
+        try:
+            resp.raise_for_status()
+        except requests.HTTPError as e:
+            raise exc.ApiException(e.response.status_code, e.response.text) from e
         if self._on_api_call:
             self._on_api_call(url, req_or_resp_obj, resp.json())
         return resp
```

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.gitignore` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.gitignore`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.gitlab-ci.yml` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.openapi-generator-ignore` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/README.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/README.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/git_push.sh` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/git_push.sh`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/pyproject.toml` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/setup.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/setup.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.github/workflows/python.yml` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/FILES` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/FILES`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyApi.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyApi.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatInputLogRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatInputLogRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatOutputLogRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatOutputLogRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyPostDatasetLogsRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyPostDatasetLogsRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyUpdateSpendingTotalsRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyUpdateSpendingTotalsRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogChoice.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogChoice.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogUsage.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogUsage.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufAny.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufAny.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/RpcStatus.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/RpcStatus.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecret.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecret.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1AppLog.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1AppLog.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1AttributeFilters.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1AttributeFilters.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateApiSecretRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateApiSecretRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateRoutingConfigRequest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateRoutingConfigRequest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Dataset.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Dataset.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1DatasetFilters.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1DatasetFilters.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1DeleteLogAttributeResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1DeleteLogAttributeResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Like.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Like.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeFilter.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeFilter.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeIngest.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeIngest.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListApiSecretsResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListApiSecretsResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListAppLogsResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListAppLogsResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListDatasetsResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListDatasetsResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLikesResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLikesResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLogAttributesResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLogAttributesResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListOpenAIChatLogsResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListOpenAIChatLogsResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1ListRoutingConfigsResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListRoutingConfigsResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1LogAttribute.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LogAttribute.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Message.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Message.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1Model.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Model.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatInputLog.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatInputLog.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLog.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLog.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLogsFilters.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLogsFilters.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatOutputLog.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatOutputLog.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1PostDatasetLogsResponse.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1PostDatasetLogsResponse.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1RelativeDateTimeFilters.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1RelativeDateTimeFilters.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1RoutingConfig.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1RoutingConfig.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1SpendCap.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1SpendCap.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/docs/V1UsageTotals.md` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1UsageTotals.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/__init__.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_client.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/configuration.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/exceptions.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/rest.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/llm_proxy_api.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/llm_proxy_api.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/__init__.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/app_log_level_type.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/app_log_level_type.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_input_log_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_input_log_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_output_log_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_output_log_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_post_dataset_logs_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_post_dataset_logs_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_update_spending_totals_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_update_spending_totals_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_choice.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_choice.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_usage.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_usage.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_any.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_null_value.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/rpc_status.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret_provider.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret_provider.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_app_log.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_app_log.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_attribute_filters.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_attribute_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_api_secret_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_api_secret_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_routing_config_request.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_routing_config_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset_filters.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_delete_log_attribute_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_delete_log_attribute_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_fallback_strategy.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_fallback_strategy.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_filter.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_filter.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_ingest.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_ingest.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_api_secrets_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_api_secrets_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_app_logs_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_app_logs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_datasets_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_likes_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_likes_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_log_attributes_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_log_attributes_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_open_ai_chat_logs_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_open_ai_chat_logs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_routing_configs_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_routing_configs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_log_attribute.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_log_attribute.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_message.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_message.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_mode.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_mode.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_model.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_model.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_input_log.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_input_log.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_log.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_log.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_logs_filters.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_logs_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_output_log.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_output_log.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_origin_type.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_origin_type.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_post_dataset_logs_response.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_post_dataset_logs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_relative_date_time_filters.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_relative_date_time_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_reset_interval.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_reset_interval.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_routing_config.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_routing_config.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_spend_cap.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_spend_cap.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_terminal_state.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_terminal_state.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_thumbs_reaction.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_thumbs_reaction.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_usage_totals.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_usage_totals.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/src/fixpoint_sdk/types/__init__.py` & `fixpoint_sdk-0.6.0/src/fixpoint_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/tests/mock_completions.py` & `fixpoint_sdk-0.6.0/tests/mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/tests/test_completions.py` & `fixpoint_sdk-0.6.0/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/tests/test_types.py` & `fixpoint_sdk-0.6.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/tests/lib/test_iterwrapper.py` & `fixpoint_sdk-0.6.0/tests/lib/test_iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/tests/lib/test_requests.py` & `fixpoint_sdk-0.6.0/tests/lib/test_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/LICENSE` & `fixpoint_sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/README.md` & `fixpoint_sdk-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.5.0/pyproject.toml` & `fixpoint_sdk-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fixpoint_sdk"
-version = "0.5.0"
+version = "0.6.0"
 
 authors = [
 { name="Jakub Cichon", email="jakub@fixpoint.co" },
 { name="Dylan Mikus", email="dylan@fixpoint.co" },
 ]
 description = "Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter"
 readme = "README.md"
```

### Comparing `fixpoint_sdk-0.5.0/PKG-INFO` & `fixpoint_sdk-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fixpoint_sdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter
 Project-URL: Homepage, https://github.com/gofixpoint/python-sdk
 Project-URL: Issues, https://github.com/gofixpoint/python-sdk/issues
 Author-email: Jakub Cichon <jakub@fixpoint.co>, Dylan Mikus <dylan@fixpoint.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

