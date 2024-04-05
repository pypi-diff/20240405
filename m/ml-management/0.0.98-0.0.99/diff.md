# Comparing `tmp/ml-management-0.0.98.tar.gz` & `tmp/ml-management-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.98.tar", last modified: Fri Mar 29 11:38:31 2024, max compression
+gzip compressed data, was "ml-management-0.0.99.tar", last modified: Fri Apr  5 11:45:25 2024, max compression
```

## Comparing `ml-management-0.0.98.tar` & `ml-management-0.0.99.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.314700 ml-management-0.0.98/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-02-22 09:53:17.000000 ml-management-0.0.98/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.218699 ml-management-0.0.98/ML_management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.222699 ml-management-0.0.98/ML_management/collectors/
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/collectors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1100 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/collectors/collector_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/collectors/collectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.226699 ml-management-0.0.98/ML_management/collectors/dummy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/collectors/dummy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/collectors/dummy/dummy_collector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.226699 ml-management-0.0.98/ML_management/collectors/s3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/collectors/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9953 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/collectors/s3/s3collector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.234699 ml-management-0.0.98/ML_management/collectors/topic_markers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/collectors/topic_markers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   331440 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3169 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.238699 ml-management-0.0.98/ML_management/dataset_loader_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/dataset_loader_template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.242699 ml-management-0.0.98/ML_management/executor_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/executor_template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.250699 ml-management-0.0.98/ML_management/executor_template/default_executors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.254699 ml-management-0.0.98/ML_management/executor_template/default_executors/eval/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/eval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/eval/conda.yaml
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/eval/eval_executor.py
--rw-r--r--   0 root         (0) root         (0)      883 2024-03-25 09:30:44.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/eval_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.258699 ml-management-0.0.98/ML_management/executor_template/default_executors/finetune/
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/finetune/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/finetune/conda.yaml
--rw-rw-rw-   0 root         (0) root         (0)      902 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/finetune/finetune_executor.py
--rw-r--r--   0 root         (0) root         (0)      902 2024-03-25 09:30:44.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/finetune_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.262699 ml-management-0.0.98/ML_management/executor_template/default_executors/train/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/train/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/train/conda.yaml
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/train/train_executor.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-03-25 09:30:44.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/train_executor.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-03-25 09:30:44.000000 ml-management-0.0.98/ML_management/executor_template/default_executors/upload.py
--rw-rw-rw-   0 root         (0) root         (0)     2875 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/executor_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/executor_template/multi_model_executor_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)     4938 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/executor_template/no_model_executor_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/executor_template/upload_model_mode.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.262699 ml-management-0.0.98/ML_management/loader/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2146 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/loader/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.282699 ml-management-0.0.98/ML_management/mlmanagement/
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/mlmanagement/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5861 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/abstract_mlflow_client.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/base_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3482 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/jsonschema_inference.py
--rw-r--r--   0 root         (0) root         (0)    32128 2024-03-29 11:38:29.000000 ml-management-0.0.98/ML_management/mlmanagement/mlmanagement.py
--rw-r--r--   0 root         (0) root         (0)    13055 2024-03-29 11:38:29.000000 ml-management-0.0.98/ML_management/mlmanagement/mlmanager.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)     4169 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/module_finder.py
--rw-rw-rw-   0 root         (0) root         (0)     5762 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4410 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/session.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/singleton_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/mlmanagement/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2024-03-20 12:25:21.000000 ml-management-0.0.98/ML_management/mlmanagement/variables.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/mlmanagement/visibility_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.286700 ml-management-0.0.98/ML_management/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/models/model_type_to_methods_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.298700 ml-management-0.0.98/ML_management/models/patterns/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/models/patterns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/models/patterns/evaluable_model.py
--rw-r--r--   0 root         (0) root         (0)     6915 2024-03-29 11:38:29.000000 ml-management-0.0.98/ML_management/models/patterns/model_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/models/patterns/model_with_losses.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/models/patterns/retrainable_model.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/models/patterns/target_layer.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/models/patterns/torch_model.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/models/patterns/trainable_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.302700 ml-management-0.0.98/ML_management/registry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3362 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/registry/abstract_registry_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4585 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/registry/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4264 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/registry/registry_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.306700 ml-management-0.0.98/ML_management/sdk/
--rw-r--r--   0 root         (0) root         (0)     1273 2024-03-29 11:38:29.000000 ml-management-0.0.98/ML_management/sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98458 2024-03-29 11:38:29.000000 ml-management-0.0.98/ML_management/sdk/schema.py
--rw-r--r--   0 root         (0) root         (0)    45509 2024-03-29 11:38:29.000000 ml-management-0.0.98/ML_management/sdk/sdk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.306700 ml-management-0.0.98/ML_management/test_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/test_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7971 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/test_sdk/test_sdk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.310700 ml-management-0.0.98/ML_management/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/tests/test_jsonschema_inference.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/tests/test_s3_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.310700 ml-management-0.0.98/ML_management/uploader_data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 11:38:27.000000 ml-management-0.0.98/ML_management/uploader_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2102 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/uploader_data/s3_uploader.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2024-02-22 09:53:17.000000 ml-management-0.0.98/ML_management/uploader_data/utils.py
--rw-r--r--   0 root         (0) root         (0)      367 2024-03-29 11:38:31.314700 ml-management-0.0.98/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-02-22 09:53:17.000000 ml-management-0.0.98/README.md
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-29 11:38:29.000000 ml-management-0.0.98/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 11:38:31.314700 ml-management-0.0.98/ml_management.egg-info/
--rw-r--r--   0 root         (0) root         (0)      367 2024-03-29 11:38:30.000000 ml-management-0.0.98/ml_management.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4039 2024-03-29 11:38:30.000000 ml-management-0.0.98/ml_management.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 11:38:30.000000 ml-management-0.0.98/ml_management.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      143 2024-03-29 11:38:30.000000 ml-management-0.0.98/ml_management.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-29 11:38:30.000000 ml-management-0.0.98/ml_management.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-29 11:38:31.314700 ml-management-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1080 2024-03-29 11:38:29.000000 ml-management-0.0.98/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.435853 ml-management-0.0.99/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-04 13:12:56.000000 ml-management-0.0.99/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.395853 ml-management-0.0.99/ML_management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.395853 ml-management-0.0.99/ML_management/collectors/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/collectors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/collectors/collector_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/collectors/collectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.395853 ml-management-0.0.99/ML_management/collectors/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/collectors/dummy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/collectors/dummy/dummy_collector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.399853 ml-management-0.0.99/ML_management/collectors/s3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/collectors/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9953 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/collectors/s3/s3collector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.399853 ml-management-0.0.99/ML_management/collectors/topic_markers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   331440 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.403853 ml-management-0.0.99/ML_management/dataset_loader_template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/dataset_loader_template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.407853 ml-management-0.0.99/ML_management/executor_template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/executor_template/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.407853 ml-management-0.0.99/ML_management/executor_template/default_executors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.411853 ml-management-0.0.99/ML_management/executor_template/default_executors/eval/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/eval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/eval/conda.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/eval/eval_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/eval_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.411853 ml-management-0.0.99/ML_management/executor_template/default_executors/finetune/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/finetune/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/finetune/conda.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      902 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/finetune/finetune_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)      902 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/finetune_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.411853 ml-management-0.0.99/ML_management/executor_template/default_executors/train/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/train/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/train/conda.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/train/train_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/executor_template/default_executors/upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/executor_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/multi_model_executor_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)     4938 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/no_model_executor_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/executor_template/upload_model_mode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.411853 ml-management-0.0.99/ML_management/loader/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/loader/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.423853 ml-management-0.0.99/ML_management/mlmanagement/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5861 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/abstract_mlflow_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/base_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3482 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-rw-   0 root         (0) root         (0)    32160 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-rw-   0 root         (0) root         (0)    13055 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/mlmanagement/mlmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/module_finder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5762 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4410 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/singleton_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/variables.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/mlmanagement/visibility_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.423853 ml-management-0.0.99/ML_management/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/models/model_type_to_methods_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.427853 ml-management-0.0.99/ML_management/models/patterns/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/models/patterns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/models/patterns/evaluable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     6915 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/models/patterns/model_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/models/patterns/model_with_losses.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/models/patterns/retrainable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/models/patterns/target_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/models/patterns/torch_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/models/patterns/trainable_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.427853 ml-management-0.0.99/ML_management/registry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3362 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/registry/abstract_registry_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4585 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/registry/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4264 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/registry/registry_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.431853 ml-management-0.0.99/ML_management/sdk/
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    98458 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/sdk/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    45509 2024-04-04 13:30:57.000000 ml-management-0.0.99/ML_management/sdk/sdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.431853 ml-management-0.0.99/ML_management/test_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/test_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7971 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/test_sdk/test_sdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.431853 ml-management-0.0.99/ML_management/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/tests/test_s3_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.435853 ml-management-0.0.99/ML_management/uploader_data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 11:45:12.000000 ml-management-0.0.99/ML_management/uploader_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2102 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/uploader_data/s3_uploader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-04-04 13:12:56.000000 ml-management-0.0.99/ML_management/uploader_data/utils.py
+-rw-r--r--   0 root         (0) root         (0)      367 2024-04-05 11:45:25.435853 ml-management-0.0.99/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-04 13:12:56.000000 ml-management-0.0.99/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-05 11:45:24.000000 ml-management-0.0.99/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:45:25.435853 ml-management-0.0.99/ml_management.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      367 2024-04-05 11:45:25.000000 ml-management-0.0.99/ml_management.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4039 2024-04-05 11:45:25.000000 ml-management-0.0.99/ml_management.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 11:45:25.000000 ml-management-0.0.99/ml_management.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      143 2024-04-05 11:45:25.000000 ml-management-0.0.99/ml_management.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-05 11:45:25.000000 ml-management-0.0.99/ml_management.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 11:45:25.435853 ml-management-0.0.99/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-04-04 13:30:57.000000 ml-management-0.0.99/setup.py
```

### Comparing `ml-management-0.0.98/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.99/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/collectors/collectors.py` & `ml-management-0.0.99/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.99/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.99/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.99/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.99/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/default_executors/eval/eval_executor.py` & `ml-management-0.0.99/ML_management/executor_template/default_executors/eval/eval_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/default_executors/eval_executor.py` & `ml-management-0.0.99/ML_management/executor_template/default_executors/eval_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/default_executors/finetune/finetune_executor.py` & `ml-management-0.0.99/ML_management/executor_template/default_executors/finetune/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.99/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/default_executors/train/train_executor.py` & `ml-management-0.0.99/ML_management/executor_template/default_executors/train/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.99/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/default_executors/upload.py` & `ml-management-0.0.99/ML_management/executor_template/default_executors/upload.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.99/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/multi_model_executor_pattern.py` & `ml-management-0.0.99/ML_management/executor_template/multi_model_executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/executor_template/no_model_executor_pattern.py` & `ml-management-0.0.99/ML_management/executor_template/no_model_executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/loader/loader.py` & `ml-management-0.0.99/ML_management/loader/loader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.99/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/abstract_mlflow_client.py` & `ml-management-0.0.99/ML_management/mlmanagement/abstract_mlflow_client.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/base_exceptions.py` & `ml-management-0.0.99/ML_management/mlmanagement/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.99/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.99/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.99/ML_management/mlmanagement/mlmanagement.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
     periodic_type,
     cron_expression,
     executor_params_json,
     model_params_json,
     data_params_json,
     collector_name,
     gpu,
+    additional_system_packages,
 ):
     """Add job metainfo on job registration. For internal use only."""
     return request_for_function(inspect.currentframe())
 
 
 def _add_job_start_metainfo(
     job_name,
```

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.99/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/module_finder.py` & `ml-management-0.0.99/ML_management/mlmanagement/module_finder.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.99/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/session.py` & `ml-management-0.0.99/ML_management/mlmanagement/session.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/utils.py` & `ml-management-0.0.99/ML_management/mlmanagement/utils.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/mlmanagement/variables.py` & `ml-management-0.0.99/ML_management/mlmanagement/variables.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.99/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.99/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.99/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/registry/abstract_registry_manager.py` & `ml-management-0.0.99/ML_management/registry/abstract_registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/registry/exceptions.py` & `ml-management-0.0.99/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/registry/registry_manager.py` & `ml-management-0.0.99/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/sdk/__init__.py` & `ml-management-0.0.99/ML_management/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/sdk/schema.py` & `ml-management-0.0.99/ML_management/sdk/schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/sdk/sdk.py` & `ml-management-0.0.99/ML_management/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/test_sdk/test_sdk.py` & `ml-management-0.0.99/ML_management/test_sdk/test_sdk.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.99/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.99/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.99/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ML_management/uploader_data/utils.py` & `ml-management-0.0.99/ML_management/uploader_data/utils.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.99/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.98/setup.py` & `ml-management-0.0.99/setup.py`

 * *Files identical despite different names*

