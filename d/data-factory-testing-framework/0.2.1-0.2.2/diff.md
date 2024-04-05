# Comparing `tmp/data_factory_testing_framework-0.2.1.tar.gz` & `tmp/data_factory_testing_framework-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_factory_testing_framework-0.2.1.tar", max compression
+gzip compressed data, was "data_factory_testing_framework-0.2.2.tar", max compression
```

## Comparing `data_factory_testing_framework-0.2.1.tar` & `data_factory_testing_framework-0.2.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1141 2024-03-31 09:18:21.737989 data_factory_testing_framework-0.2.1/LICENSE
--rw-r--r--   0        0        0     5591 2024-03-31 09:18:21.737989 data_factory_testing_framework-0.2.1/README.md
--rw-r--r--   0        0        0     2053 2024-03-31 09:20:05.036770 data_factory_testing_framework-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      260 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/__init__.py
--rw-r--r--   0        0        0      794 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/_deserializer_base.py
--rw-r--r--   0        0        0      496 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/_deserializer_data_factory.py
--rw-r--r--   0        0        0      539 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/_deserializer_fabric.py
--rw-r--r--   0        0        0        0 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/shared/__init__.py
--rw-r--r--   0        0        0     2753 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/shared/_activity_deserializer.py
--rw-r--r--   0        0        0     2077 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/shared/_data_factory_element_replacer.py
--rw-r--r--   0        0        0       13 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/__init__.py
--rw-r--r--   0        0        0       96 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/__init__.py
--rw-r--r--   0        0        0     1051 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/exceptions.py
--rw-r--r--   0        0        0     7135 2024-03-31 09:18:21.741989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/expression_evaluator.py
--rw-r--r--   0        0        0     3387 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/expression_rule_transformer.py
--rw-r--r--   0        0        0     3204 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/expression_terminal_transformer.py
--rw-r--r--   0        0        0     2105 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/__init__.py
--rw-r--r--   0        0        0     1351 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/activity_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1898 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/branch_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1484 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/dataset_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1681 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/evaluation_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1227 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/expression_parameter_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1990 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/expression_rule_evaluator.py
--rw-r--r--   0        0        0     3226 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/function_call_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1113 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/item_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1467 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/linked_service_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1192 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/literal_evaluation_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1477 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/literal_interpolation_expression_rule_evaluator.py
--rw-r--r--   0        0        0     2896 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/logical_bool_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1685 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/pipeline_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1514 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/system_variable_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1335 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/variable_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     5937 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_collection_implementation.py
--rw-r--r--   0        0        0     5437 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_conversion_implementation.py
--rw-r--r--   0        0        0    10102 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_date_implementation.py
--rw-r--r--   0        0        0     1679 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_logical_implementation.py
--rw-r--r--   0        0        0     2131 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_math_implementation.py
--rw-r--r--   0        0        0     4936 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_repository.py
--rw-r--r--   0        0        0     4190 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_string_implementation.py
--rw-r--r--   0        0        0       97 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_pythonnet/__init__.py
--rw-r--r--   0        0        0     3386 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_pythonnet/csharp_datetime.py
--rw-r--r--   0        0        0        0 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/__init__.py
--rw-r--r--   0        0        0      568 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/_factories/base_repository_factory.py
--rw-r--r--   0        0        0      900 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/_factories/data_factory_repository_factory.py
--rw-r--r--   0        0        0     3164 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/_factories/fabric_repository_factory.py
--rw-r--r--   0        0        0     1365 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/data_factory_repository.py
--rw-r--r--   0        0        0     8967 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_test_framework.py
--rw-r--r--   0        0        0     1815 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/__init__.py
--rw-r--r--   0        0        0      304 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_activity_not_found_error.py
--rw-r--r--   0        0        0      471 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_activity_output_field_not_found_error.py
--rw-r--r--   0        0        0      361 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_data_factory_element_evaluation_error.py
--rw-r--r--   0        0        0      607 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_function_call_invalid_arguments_count_error.py
--rw-r--r--   0        0        0      325 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_parameter_not_found_error.py
--rw-r--r--   0        0        0      705 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_pipeline_activities_circular_dependency_error.py
--rw-r--r--   0        0        0      301 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_pipeline_not_found_error.py
--rw-r--r--   0        0        0      272 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_state_iteration_item_not_set_error.py
--rw-r--r--   0        0        0      301 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_unsupported_function_error.py
--rw-r--r--   0        0        0      120 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_user_error.py
--rw-r--r--   0        0        0      349 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_variable_being_evaluated_does_not_exist_error.py
--rw-r--r--   0        0        0      293 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_variable_not_found_error.py
--rw-r--r--   0        0        0      329 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/__init__.py
--rw-r--r--   0        0        0     1490 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/_data_factory_element.py
--rw-r--r--   0        0        0      126 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/_data_factory_object_type.py
--rw-r--r--   0        0        0     3687 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/_pipeline.py
--rw-r--r--   0        0        0      895 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/__init__.py
--rw-r--r--   0        0        0     4084 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_activity.py
--rw-r--r--   0        0        0      650 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_activity_dependency.py
--rw-r--r--   0        0        0     1272 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_append_variable_activity.py
--rw-r--r--   0        0        0      784 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_control_activity.py
--rw-r--r--   0        0        0     2626 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_execute_pipeline_activity.py
--rw-r--r--   0        0        0      789 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_fail_activity.py
--rw-r--r--   0        0        0     1263 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_filter_activity.py
--rw-r--r--   0        0        0     1670 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_for_each_activity.py
--rw-r--r--   0        0        0     1980 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_if_condition_activity.py
--rw-r--r--   0        0        0     1707 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_set_variable_activity.py
--rw-r--r--   0        0        0     2395 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_switch_activity.py
--rw-r--r--   0        0        0     1917 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_until_activity.py
--rw-r--r--   0        0        0        0 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/py.typed
--rw-r--r--   0        0        0      505 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/__init__.py
--rw-r--r--   0        0        0      751 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_activity_result.py
--rw-r--r--   0        0        0      279 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_dependency_condition.py
--rw-r--r--   0        0        0     8339 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_pipeline_run_state.py
--rw-r--r--   0        0        0      544 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_pipeline_run_variable.py
--rw-r--r--   0        0        0      656 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_run_parameter.py
--rw-r--r--   0        0        0      647 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_run_parameter_type.py
--rw-r--r--   0        0        0      534 2024-03-31 09:18:21.745989 data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_run_state.py
--rw-r--r--   0        0        0     6526 1970-01-01 00:00:00.000000 data_factory_testing_framework-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1141 2024-04-05 13:53:00.744238 data_factory_testing_framework-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5642 2024-04-05 13:53:00.744238 data_factory_testing_framework-0.2.2/README.md
+-rw-r--r--   0        0        0     2053 2024-04-05 13:54:43.008480 data_factory_testing_framework-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      260 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/__init__.py
+-rw-r--r--   0        0        0      794 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/_deserializer_base.py
+-rw-r--r--   0        0        0      496 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/_deserializer_data_factory.py
+-rw-r--r--   0        0        0      539 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/_deserializer_fabric.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/shared/__init__.py
+-rw-r--r--   0        0        0     2753 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/shared/_activity_deserializer.py
+-rw-r--r--   0        0        0     2077 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/shared/_data_factory_element_replacer.py
+-rw-r--r--   0        0        0       13 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/__init__.py
+-rw-r--r--   0        0        0     1051 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/exceptions.py
+-rw-r--r--   0        0        0     7135 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/expression_evaluator.py
+-rw-r--r--   0        0        0     3387 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/expression_rule_transformer.py
+-rw-r--r--   0        0        0     3204 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/expression_terminal_transformer.py
+-rw-r--r--   0        0        0     2105 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/__init__.py
+-rw-r--r--   0        0        0     1351 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/activity_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1898 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/branch_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1484 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/dataset_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1681 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/evaluation_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1227 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/expression_parameter_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1990 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/expression_rule_evaluator.py
+-rw-r--r--   0        0        0     3226 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/function_call_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1113 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/item_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1467 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/linked_service_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1192 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/literal_evaluation_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1477 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/literal_interpolation_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     2896 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/logical_bool_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1685 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/pipeline_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1514 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/system_variable_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1335 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/variable_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     5937 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_collection_implementation.py
+-rw-r--r--   0        0        0     5437 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_conversion_implementation.py
+-rw-r--r--   0        0        0    10102 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_date_implementation.py
+-rw-r--r--   0        0        0     1679 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_logical_implementation.py
+-rw-r--r--   0        0        0     2131 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_math_implementation.py
+-rw-r--r--   0        0        0     4936 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_repository.py
+-rw-r--r--   0        0        0     4190 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_string_implementation.py
+-rw-r--r--   0        0        0       97 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_pythonnet/__init__.py
+-rw-r--r--   0        0        0     3386 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_pythonnet/csharp_datetime.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/__init__.py
+-rw-r--r--   0        0        0      568 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/_factories/base_repository_factory.py
+-rw-r--r--   0        0        0      900 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/_factories/data_factory_repository_factory.py
+-rw-r--r--   0        0        0     3164 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/_factories/fabric_repository_factory.py
+-rw-r--r--   0        0        0     1365 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/data_factory_repository.py
+-rw-r--r--   0        0        0     8967 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_test_framework.py
+-rw-r--r--   0        0        0     1815 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/__init__.py
+-rw-r--r--   0        0        0      304 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_activity_not_found_error.py
+-rw-r--r--   0        0        0      471 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_activity_output_field_not_found_error.py
+-rw-r--r--   0        0        0      361 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_data_factory_element_evaluation_error.py
+-rw-r--r--   0        0        0      607 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_function_call_invalid_arguments_count_error.py
+-rw-r--r--   0        0        0      325 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_parameter_not_found_error.py
+-rw-r--r--   0        0        0      705 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_pipeline_activities_circular_dependency_error.py
+-rw-r--r--   0        0        0      301 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_pipeline_not_found_error.py
+-rw-r--r--   0        0        0      272 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_state_iteration_item_not_set_error.py
+-rw-r--r--   0        0        0      301 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_unsupported_function_error.py
+-rw-r--r--   0        0        0      120 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_user_error.py
+-rw-r--r--   0        0        0      349 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_variable_being_evaluated_does_not_exist_error.py
+-rw-r--r--   0        0        0      293 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_variable_not_found_error.py
+-rw-r--r--   0        0        0      329 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/__init__.py
+-rw-r--r--   0        0        0     1490 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/_data_factory_element.py
+-rw-r--r--   0        0        0      126 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/_data_factory_object_type.py
+-rw-r--r--   0        0        0     3687 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/_pipeline.py
+-rw-r--r--   0        0        0      895 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/__init__.py
+-rw-r--r--   0        0        0     4084 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_activity.py
+-rw-r--r--   0        0        0      650 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_activity_dependency.py
+-rw-r--r--   0        0        0     1272 2024-04-05 13:53:00.748238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_append_variable_activity.py
+-rw-r--r--   0        0        0      784 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_control_activity.py
+-rw-r--r--   0        0        0     2626 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_execute_pipeline_activity.py
+-rw-r--r--   0        0        0      789 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_fail_activity.py
+-rw-r--r--   0        0        0     1263 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_filter_activity.py
+-rw-r--r--   0        0        0     1670 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_for_each_activity.py
+-rw-r--r--   0        0        0     1980 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_if_condition_activity.py
+-rw-r--r--   0        0        0     1707 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_set_variable_activity.py
+-rw-r--r--   0        0        0     2395 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_switch_activity.py
+-rw-r--r--   0        0        0     1917 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_until_activity.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/py.typed
+-rw-r--r--   0        0        0      505 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/__init__.py
+-rw-r--r--   0        0        0      751 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_activity_result.py
+-rw-r--r--   0        0        0      279 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_dependency_condition.py
+-rw-r--r--   0        0        0     8339 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_pipeline_run_state.py
+-rw-r--r--   0        0        0      544 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_pipeline_run_variable.py
+-rw-r--r--   0        0        0      656 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_run_parameter.py
+-rw-r--r--   0        0        0      647 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_run_parameter_type.py
+-rw-r--r--   0        0        0      534 2024-04-05 13:53:00.752238 data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_run_state.py
+-rw-r--r--   0        0        0     6577 1970-01-01 00:00:00.000000 data_factory_testing_framework-0.2.2/PKG-INFO
```

### Comparing `data_factory_testing_framework-0.2.1/LICENSE` & `data_factory_testing_framework-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/README.md` & `data_factory_testing_framework-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Data Factory - Testing Framework :hammer_and_wrench:
 
 A stand-alone test framework that allows to write unit tests for Data Factory pipelines on [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/data-factory/) and [Azure Data Factory](https://learn.microsoft.com/en-us/azure/data-factory/concepts-pipelines-activities?tabs=data-factory).
 
+> The framework is currently in _Public Preview_ and is not officially supported by Microsoft.
+
 ## Features :rocket:
 
 The framework evaluates pipeline and activity definitions which can be asserted. It does so by providing the following features:
 
 1. Evaluate expressions by using the framework's internal expression parser. It supports all the functions and arguments that are available in the Data Factory expression language.
 2. Test an activity with a specific state and assert the evaluated expressions.
 3. Test a pipeline run by verifying the execution flow of activities for specific input parameters and assert the evaluated expressions of each activity.
@@ -78,37 +80,37 @@
 1. [Batch job example](examples/fabric/batch_job/README.md)
 
 Azure Data Factory:
 
 1. [Copy blobs example](examples/data_factory/copy_blobs/README.md)
 2. [Batch job example](examples/data_factory/batch_job/README.md)
 
+## Limitations :warning:
+
+The framework has the following limitations at the moment:
+
+1. The framework reimplements the Data Factory expression language in Python. This means that it might not be 100% accurate with the actual Data Factory language, especially when it comes to xml functions.
+2. The framework does not support automatic type conversion of arguments passed to functions in expressions.
+
+> These limitations are top priority to be resolved in the future.
+
 ## Contributing :handshake:
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit <https://cla.opensource.microsoft.com>.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
 a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
 provided by the bot. You will only need to do this once across all repos using our CLA.
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
-## Disclaimer :warning:
-
-This unit test framework is not officially supported.
-It is currently in an experimental state and has not been tested with every single data factory resource.
-It should support all activities out-of-the-box but has not been thoroughly tested,
-please report any issues in the issues section and include an example of the pipeline that is not working as expected.
-
-If there's a lot of interest in this framework, then we will continue to improve it and move it to a production-ready state.
-
 ## Trademarks :tm:
 
 This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
 trademarks or logos is subject to and must follow
 [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
 Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
 Any use of third-party trademarks or logos are subject to those third-party's policies.
```

### Comparing `data_factory_testing_framework-0.2.1/pyproject.toml` & `data_factory_testing_framework-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-factory-testing-framework"
-version = "0.2.1"
+version = "0.2.2"
 description = "A stand-alone test framework that allows to write unit tests for Data Factory pipelines on Microsoft Fabric and Azure Data Factory."
 authors = ["Arjen Kroezen <arjenkroezen@microsoft.com>", "Yennifer Santos <ysantos@microsoft.com>", "Jaya Kumar <kumarjaya@microsoft.com>", "Leonard Herold <lherold@microsoft.com>"]
 readme = "README.md"
 license = "MIT"
 include = [ "README.md", "LICENSE" ]
 keywords = ["fabric", "datafactory", "unit-testing", "functional-testing", "azure"]
```

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/_deserializer_base.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/_deserializer_base.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/_deserializer_fabric.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/_deserializer_fabric.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/shared/_activity_deserializer.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/shared/_activity_deserializer.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_deserializers/shared/_data_factory_element_replacer.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_deserializers/shared/_data_factory_element_replacer.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/exceptions.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/exceptions.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/expression_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/expression_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/expression_rule_transformer.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/expression_rule_transformer.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/expression_terminal_transformer.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/expression_terminal_transformer.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/__init__.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/activity_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/activity_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/branch_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/branch_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/dataset_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/dataset_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/evaluation_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/evaluation_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/expression_parameter_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/expression_parameter_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/function_call_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/function_call_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/item_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/item_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/linked_service_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/linked_service_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/literal_evaluation_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/literal_evaluation_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/literal_interpolation_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/literal_interpolation_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/logical_bool_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/logical_bool_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/pipeline_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/pipeline_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/system_variable_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/system_variable_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/evaluator/rules/variable_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/evaluator/rules/variable_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_collection_implementation.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_collection_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_conversion_implementation.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_conversion_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_date_implementation.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_date_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_logical_implementation.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_logical_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_math_implementation.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_math_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_repository.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_repository.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_functions/functions_string_implementation.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_functions/functions_string_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_pythonnet/csharp_datetime.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_pythonnet/csharp_datetime.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/_factories/base_repository_factory.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/_factories/base_repository_factory.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/_factories/data_factory_repository_factory.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/_factories/data_factory_repository_factory.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/_factories/fabric_repository_factory.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/_factories/fabric_repository_factory.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_repositories/data_factory_repository.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_repositories/data_factory_repository.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/_test_framework.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/_test_framework.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/__init__.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_function_call_invalid_arguments_count_error.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_function_call_invalid_arguments_count_error.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/exceptions/_pipeline_activities_circular_dependency_error.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/exceptions/_pipeline_activities_circular_dependency_error.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/_data_factory_element.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/_data_factory_element.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/_pipeline.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/_pipeline.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/__init__.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/__init__.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_activity_dependency.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_activity_dependency.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_append_variable_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_append_variable_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_control_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_control_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_execute_pipeline_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_execute_pipeline_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_fail_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_fail_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_filter_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_filter_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_for_each_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_for_each_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_if_condition_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_if_condition_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_set_variable_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_set_variable_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_switch_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_switch_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/models/activities/_until_activity.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/models/activities/_until_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_activity_result.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_activity_result.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_pipeline_run_state.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_pipeline_run_state.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_pipeline_run_variable.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_pipeline_run_variable.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_run_parameter.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_run_parameter.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_run_parameter_type.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_run_parameter_type.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/src/data_factory_testing_framework/state/_run_state.py` & `data_factory_testing_framework-0.2.2/src/data_factory_testing_framework/state/_run_state.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.1/PKG-INFO` & `data_factory_testing_framework-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-factory-testing-framework
-Version: 0.2.1
+Version: 0.2.2
 Summary: A stand-alone test framework that allows to write unit tests for Data Factory pipelines on Microsoft Fabric and Azure Data Factory.
 License: MIT
 Keywords: fabric,datafactory,unit-testing,functional-testing,azure
 Author: Arjen Kroezen
 Author-email: arjenkroezen@microsoft.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,16 @@
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # Data Factory - Testing Framework :hammer_and_wrench:
 
 A stand-alone test framework that allows to write unit tests for Data Factory pipelines on [Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/data-factory/) and [Azure Data Factory](https://learn.microsoft.com/en-us/azure/data-factory/concepts-pipelines-activities?tabs=data-factory).
 
+> The framework is currently in _Public Preview_ and is not officially supported by Microsoft.
+
 ## Features :rocket:
 
 The framework evaluates pipeline and activity definitions which can be asserted. It does so by providing the following features:
 
 1. Evaluate expressions by using the framework's internal expression parser. It supports all the functions and arguments that are available in the Data Factory expression language.
 2. Test an activity with a specific state and assert the evaluated expressions.
 3. Test a pipeline run by verifying the execution flow of activities for specific input parameters and assert the evaluated expressions of each activity.
@@ -100,37 +102,37 @@
 1. [Batch job example](examples/fabric/batch_job/README.md)
 
 Azure Data Factory:
 
 1. [Copy blobs example](examples/data_factory/copy_blobs/README.md)
 2. [Batch job example](examples/data_factory/batch_job/README.md)
 
+## Limitations :warning:
+
+The framework has the following limitations at the moment:
+
+1. The framework reimplements the Data Factory expression language in Python. This means that it might not be 100% accurate with the actual Data Factory language, especially when it comes to xml functions.
+2. The framework does not support automatic type conversion of arguments passed to functions in expressions.
+
+> These limitations are top priority to be resolved in the future.
+
 ## Contributing :handshake:
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit <https://cla.opensource.microsoft.com>.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
 a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
 provided by the bot. You will only need to do this once across all repos using our CLA.
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
-## Disclaimer :warning:
-
-This unit test framework is not officially supported.
-It is currently in an experimental state and has not been tested with every single data factory resource.
-It should support all activities out-of-the-box but has not been thoroughly tested,
-please report any issues in the issues section and include an example of the pipeline that is not working as expected.
-
-If there's a lot of interest in this framework, then we will continue to improve it and move it to a production-ready state.
-
 ## Trademarks :tm:
 
 This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
 trademarks or logos is subject to and must follow
 [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
 Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
 Any use of third-party trademarks or logos are subject to those third-party's policies.
```

