# Comparing `tmp/guardrails-api-client-0.1.0.tar.gz` & `tmp/guardrails-api-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrails-api-client-0.1.0.tar", last modified: Tue Mar 19 20:20:19 2024, max compression
+gzip compressed data, was "guardrails-api-client-0.1.1.tar", last modified: Fri Apr  5 20:12:13 2024, max compression
```

## Comparing `guardrails-api-client-0.1.0.tar` & `guardrails-api-client-0.1.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.361049 guardrails-api-client-0.1.0/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4296 2024-03-19 20:20:19.360920 guardrails-api-client-0.1.0/PKG-INFO
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4108 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/README.md
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.346850 guardrails-api-client-0.1.0/guardrails_api_client/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)      157 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/__init__.py
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.347653 guardrails-api-client-0.1.0/guardrails_api_client/api/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)       45 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/__init__.py
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.349075 guardrails-api-client-0.1.0/guardrails_api_client/api/default/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/default/__init__.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4002 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/default/delete_ingested_document.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4051 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/default/get_ingested_document.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4004 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/default/get_ingested_document_by_guard_id.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4954 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/default/ingest.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     5310 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/default/update_ingested_document.py
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.350242 guardrails-api-client-0.1.0/guardrails_api_client/api/guard/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/guard/__init__.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3559 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/guard/create_guard.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3479 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/guard/delete_guard.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4387 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/guard/get_guard.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3539 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/guard/get_guards.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3909 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/guard/update_guard.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     5046 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/guard/validate.py
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.351012 guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/__init__.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     6336 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/get_guard_metrics.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4432 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/get_guard_run_metrics.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     6852 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/get_validator_metrics.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     5122 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/get_validator_run_metrics.py
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.351347 guardrails-api-client-0.1.0/guardrails_api_client/api/projections/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/projections/__init__.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4789 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/projections/get_projection.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4785 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/projections/update_projection.py
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.351696 guardrails-api-client-0.1.0/guardrails_api_client/api/service_health/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/service_health/__init__.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3091 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/api/service_health/get_health_check.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)    12131 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/client.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)      546 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/errors.py
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.360584 guardrails-api-client-0.1.0/guardrails_api_client/models/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     2707 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/__init__.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1170 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/any_object.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3232 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/data_type.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1208 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/data_type_children.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     2888 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/document.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1205 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/document_metadata.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1190 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/document_pages.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3746 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/guard.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1248 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/guard_guard_config.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3728 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/guard_metrics.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     2547 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/guard_run_metric_details.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4962 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/guard_run_metrics.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     2403 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/guard_run_step.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1667 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/health_check.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     2131 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/history.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     5939 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/history_event.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1564 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/history_event_prompt.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1241 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/history_event_reasks_item.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3422 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/http_error.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1773 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/http_error_fields.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4430 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/ingestion.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1210 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/ingestion_metadata.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     2850 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/ingestion_payload.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1623 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/json_schema.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1736 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/on_fail.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)      274 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/on_fail_options.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3310 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/projection.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3186 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/rail_spec.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)      140 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/rail_spec_version.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)    25474 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/reask.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     2414 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/schema.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4103 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/schema_element.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)      147 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/status.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3659 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/validate_payload.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)      378 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/validate_payload_llm_api.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1298 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/validate_payload_prompt_params.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3286 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/validation_output.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3822 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/validator_metrics.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     2644 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/validator_run_metric_details.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     1309 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/validator_run_metric_details_parameters.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     5133 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/models/validator_run_metrics.py
--rw-r--r--   0 zaydsimjee   (501) staff       (20)       25 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/py.typed
--rw-r--r--   0 zaydsimjee   (501) staff       (20)      985 2024-03-19 19:59:10.000000 guardrails-api-client-0.1.0/guardrails_api_client/types.py
-drwxr-xr-x   0 zaydsimjee   (501) staff       (20)        0 2024-03-19 20:20:19.347480 guardrails-api-client-0.1.0/guardrails_api_client.egg-info/
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     4296 2024-03-19 20:20:19.000000 guardrails-api-client-0.1.0/guardrails_api_client.egg-info/PKG-INFO
--rw-r--r--   0 zaydsimjee   (501) staff       (20)     3651 2024-03-19 20:20:19.000000 guardrails-api-client-0.1.0/guardrails_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 zaydsimjee   (501) staff       (20)        1 2024-03-19 20:20:19.000000 guardrails-api-client-0.1.0/guardrails_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 zaydsimjee   (501) staff       (20)       62 2024-03-19 20:20:19.000000 guardrails-api-client-0.1.0/guardrails_api_client.egg-info/requires.txt
--rw-r--r--   0 zaydsimjee   (501) staff       (20)       22 2024-03-19 20:20:19.000000 guardrails-api-client-0.1.0/guardrails_api_client.egg-info/top_level.txt
--rw-r--r--   0 zaydsimjee   (501) staff       (20)       75 2024-03-19 20:03:32.000000 guardrails-api-client-0.1.0/pyproject.toml
--rw-r--r--   0 zaydsimjee   (501) staff       (20)       38 2024-03-19 20:20:19.361090 guardrails-api-client-0.1.0/setup.cfg
--rw-r--r--   0 zaydsimjee   (501) staff       (20)      621 2024-03-19 20:03:02.000000 guardrails-api-client-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.339829 guardrails-api-client-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-05 20:12:13.339829 guardrails-api-client-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.327829 guardrails-api-client-0.1.1/guardrails_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.327829 guardrails-api-client-0.1.1/guardrails_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.327829 guardrails-api-client-0.1.1/guardrails_api_client/api/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/default/delete_ingested_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/default/get_ingested_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/default/get_ingested_document_by_guard_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/default/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/default/update_ingested_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.331829 guardrails-api-client-0.1.1/guardrails_api_client/api/guard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/guard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/guard/create_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/guard/delete_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/guard/get_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/guard/get_guards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/guard/update_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/guard/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.331829 guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/get_guard_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/get_guard_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/get_validator_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/get_validator_run_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.331829 guardrails-api-client-0.1.1/guardrails_api_client/api/projections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/projections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/projections/get_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/projections/update_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.331829 guardrails-api-client-0.1.1/guardrails_api_client/api/service_health/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/service_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/api/service_health/get_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.339829 guardrails-api-client-0.1.1/guardrails_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/any_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/data_type_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/document_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/document_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/guard_guard_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/guard_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/guard_run_metric_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/guard_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/guard_run_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/history_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/history_event_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/history_event_reasks_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/http_error_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/ingestion_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/ingestion_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/on_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/on_fail_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/rail_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/rail_spec_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25474 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/reask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/schema_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/validate_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/validate_payload_llm_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/validate_payload_prompt_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/validation_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/validator_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/validator_run_metric_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/validator_run_metric_details_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/models/validator_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/guardrails_api_client/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:12:13.339829 guardrails-api-client-0.1.1/guardrails_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-05 20:12:13.000000 guardrails-api-client-0.1.1/guardrails_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-05 20:12:13.000000 guardrails-api-client-0.1.1/guardrails_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:12:13.000000 guardrails-api-client-0.1.1/guardrails_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 20:12:13.000000 guardrails-api-client-0.1.1/guardrails_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 20:12:13.000000 guardrails-api-client-0.1.1/guardrails_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:12:13.339829 guardrails-api-client-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-05 20:11:59.000000 guardrails-api-client-0.1.1/setup.py
```

### Comparing `guardrails-api-client-0.1.0/PKG-INFO` & `guardrails-api-client-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: guardrails-api-client
-Version: 0.1.0
-Summary: A client library for accessing Guardrails API
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-
 # guardrails-api-client
 A client library for accessing Guardrails API
 
 ## Usage
 First, create a client:
 
 ```python
```

### Comparing `guardrails-api-client-0.1.0/README.md` & `guardrails-api-client-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: guardrails-api-client
+Version: 0.1.1
+Summary: A client library for accessing Guardrails API
+Requires-Python: >=3.8, <4
+Description-Content-Type: text/markdown
+Requires-Dist: httpx<0.28.0,>=0.20.0
+Requires-Dist: attrs>=21.3.0
+Requires-Dist: python-dateutil<3,>=2.8.0
+
 # guardrails-api-client
 A client library for accessing Guardrails API
 
 ## Usage
 First, create a client:
 
 ```python
```

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/default/delete_ingested_document.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/default/delete_ingested_document.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/default/get_ingested_document.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/default/get_ingested_document.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/default/get_ingested_document_by_guard_id.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/default/get_ingested_document_by_guard_id.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/default/ingest.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/default/ingest.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/default/update_ingested_document.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/default/update_ingested_document.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/guard/create_guard.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/guard/create_guard.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/guard/delete_guard.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/guard/delete_guard.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/guard/get_guard.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/guard/get_guard.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/guard/get_guards.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/guard/get_guards.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/guard/update_guard.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/guard/update_guard.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/guard/validate.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/guard/validate.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/get_guard_metrics.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/get_guard_metrics.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/get_guard_run_metrics.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/get_guard_run_metrics.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/get_validator_metrics.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/get_validator_metrics.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/metrics/get_validator_run_metrics.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/metrics/get_validator_run_metrics.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/projections/get_projection.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/projections/get_projection.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/projections/update_projection.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/projections/update_projection.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/api/service_health/get_health_check.py` & `guardrails-api-client-0.1.1/guardrails_api_client/api/service_health/get_health_check.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/client.py` & `guardrails-api-client-0.1.1/guardrails_api_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     Attributes:
         raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
             status code that was not documented in the source OpenAPI document. Can also be provided as a keyword
             argument to the constructor.
     """
 
     raise_on_unexpected_status: bool = field(default=False, kw_only=True)
-    _base_url: str
-    _cookies: Dict[str, str] = field(factory=dict, kw_only=True)
-    _headers: Dict[str, str] = field(factory=dict, kw_only=True)
-    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True)
-    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True)
-    _follow_redirects: bool = field(default=False, kw_only=True)
-    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True)
+    _base_url: str = field(alias="base_url")
+    _cookies: Dict[str, str] = field(factory=dict, kw_only=True, alias="cookies")
+    _headers: Dict[str, str] = field(factory=dict, kw_only=True, alias="headers")
+    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True, alias="timeout")
+    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True, alias="verify_ssl")
+    _follow_redirects: bool = field(default=False, kw_only=True, alias="follow_redirects")
+    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True, alias="httpx_args")
     _client: Optional[httpx.Client] = field(default=None, init=False)
     _async_client: Optional[httpx.AsyncClient] = field(default=None, init=False)
 
     def with_headers(self, headers: Dict[str, str]) -> "Client":
         """Get a new client matching this one with additional headers"""
         if self._client is not None:
             self._client.headers.update(headers)
@@ -161,21 +161,21 @@
             argument to the constructor.
         token: The token to use for authentication
         prefix: The prefix to use for the Authorization header
         auth_header_name: The name of the Authorization header
     """
 
     raise_on_unexpected_status: bool = field(default=False, kw_only=True)
-    _base_url: str
-    _cookies: Dict[str, str] = field(factory=dict, kw_only=True)
-    _headers: Dict[str, str] = field(factory=dict, kw_only=True)
-    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True)
-    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True)
-    _follow_redirects: bool = field(default=False, kw_only=True)
-    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True)
+    _base_url: str = field(alias="base_url")
+    _cookies: Dict[str, str] = field(factory=dict, kw_only=True, alias="cookies")
+    _headers: Dict[str, str] = field(factory=dict, kw_only=True, alias="headers")
+    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True, alias="timeout")
+    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True, alias="verify_ssl")
+    _follow_redirects: bool = field(default=False, kw_only=True, alias="follow_redirects")
+    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True, alias="httpx_args")
     _client: Optional[httpx.Client] = field(default=None, init=False)
     _async_client: Optional[httpx.AsyncClient] = field(default=None, init=False)
 
     token: str
     prefix: str = "Bearer"
     auth_header_name: str = "Authorization"
```

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/errors.py` & `guardrails-api-client-0.1.1/guardrails_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/__init__.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/any_object.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/any_object.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/data_type.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/data_type.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/data_type_children.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/data_type_children.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/document.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/document.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/document_metadata.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/document_metadata.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/document_pages.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/document_pages.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/guard.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/guard.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/guard_guard_config.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/guard_guard_config.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/guard_metrics.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/guard_metrics.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/guard_run_metric_details.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/guard_run_metric_details.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/guard_run_metrics.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/guard_run_metrics.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/guard_run_step.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/guard_run_step.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/health_check.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/health_check.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/history.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/history.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/history_event.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/history_event.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/history_event_prompt.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/history_event_prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/history_event_reasks_item.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/history_event_reasks_item.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/http_error.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/http_error.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/http_error_fields.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/http_error_fields.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/ingestion.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/ingestion.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/ingestion_metadata.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/ingestion_metadata.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/ingestion_payload.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/ingestion_payload.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/json_schema.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/json_schema.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/on_fail.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/on_fail.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/projection.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/projection.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/rail_spec.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/rail_spec.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/reask.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/reask.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/schema.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/schema.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/schema_element.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/schema_element.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 
 @_attrs_define
 class SchemaElement:
     """
     Attributes:
         type (str):
-        name (str):
+        name (Union[Unset, str]):
         description (Union[Unset, str]):
         strict (Union[Unset, bool]):
         date_format (Union[Unset, str]):
         time_format (Union[Unset, str]):
         on_fail (Union[Unset, str]):
         on_fails (Union[Unset, List['OnFail']]):
         model (Union[Unset, str]):
     """
 
     type: str
-    name: str
+    name: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     strict: Union[Unset, bool] = UNSET
     date_format: Union[Unset, str] = UNSET
     time_format: Union[Unset, str] = UNSET
     on_fail: Union[Unset, str] = UNSET
     on_fails: Union[Unset, List["OnFail"]] = UNSET
     model: Union[Unset, str] = UNSET
@@ -63,17 +63,18 @@
         model = self.model
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "type": type,
-                "name": name,
             }
         )
+        if name is not UNSET:
+            field_dict["name"] = name
         if description is not UNSET:
             field_dict["description"] = description
         if strict is not UNSET:
             field_dict["strict"] = strict
         if date_format is not UNSET:
             field_dict["dateFormat"] = date_format
         if time_format is not UNSET:
@@ -90,15 +91,15 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.on_fail import OnFail
 
         d = src_dict.copy()
         type = d.pop("type")
 
-        name = d.pop("name")
+        name = d.pop("name", UNSET)
 
         description = d.pop("description", UNSET)
 
         strict = d.pop("strict", UNSET)
 
         date_format = d.pop("dateFormat", UNSET)
```

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/validate_payload.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/validate_payload.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/validate_payload_prompt_params.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/validate_payload_prompt_params.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/validator_metrics.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/validator_metrics.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/validator_run_metric_details.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/validator_run_metric_details.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/validator_run_metric_details_parameters.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/validator_run_metric_details_parameters.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/models/validator_run_metrics.py` & `guardrails-api-client-0.1.1/guardrails_api_client/models/validator_run_metrics.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client/types.py` & `guardrails-api-client-0.1.1/guardrails_api_client/types.py`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client.egg-info/PKG-INFO` & `guardrails-api-client-0.1.1/guardrails_api_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: guardrails-api-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A client library for accessing Guardrails API
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
+Requires-Dist: httpx<0.28.0,>=0.20.0
+Requires-Dist: attrs>=21.3.0
+Requires-Dist: python-dateutil<3,>=2.8.0
 
 # guardrails-api-client
 A client library for accessing Guardrails API
 
 ## Usage
 First, create a client:
```

### Comparing `guardrails-api-client-0.1.0/guardrails_api_client.egg-info/SOURCES.txt` & `guardrails-api-client-0.1.1/guardrails_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guardrails-api-client-0.1.0/setup.py` & `guardrails-api-client-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="guardrails-api-client",
-    version="0.1.0",
+    version="0.1.1",
     description="A client library for accessing Guardrails API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     python_requires=">=3.8, <4",
     install_requires=["httpx >= 0.20.0, < 0.28.0", "attrs >= 21.3.0", "python-dateutil >= 2.8.0, < 3"],
     package_data={"guardrails_api_client": ["py.typed"]},
```

