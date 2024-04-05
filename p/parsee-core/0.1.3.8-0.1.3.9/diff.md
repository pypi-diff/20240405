# Comparing `tmp/parsee_core-0.1.3.8.tar.gz` & `tmp/parsee_core-0.1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsee_core-0.1.3.8.tar", max compression
+gzip compressed data, was "parsee_core-0.1.3.9.tar", max compression
```

## Comparing `parsee_core-0.1.3.8.tar` & `parsee_core-0.1.3.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      485 2024-02-14 17:01:39.100086 parsee_core-0.1.3.8/parsee/__init__.py
--rw-r--r--   0        0        0     2768 2024-03-13 08:58:10.546792 parsee_core-0.1.3.8/parsee/cloud/api.py
--rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.3.8/parsee/converters/__init__.py
--rw-r--r--   0        0        0     6035 2024-02-14 15:27:25.505875 parsee_core-0.1.3.8/parsee/converters/html_extraction.py
--rw-r--r--   0        0        0      344 2024-02-14 09:53:17.700535 parsee_core-0.1.3.8/parsee/converters/interfaces.py
--rw-r--r--   0        0        0     1800 2024-02-14 11:04:57.276847 parsee_core-0.1.3.8/parsee/converters/json_to_raw.py
--rw-r--r--   0        0        0     1063 2024-03-12 10:43:02.953449 parsee_core-0.1.3.8/parsee/converters/langchain.py
--rw-r--r--   0        0        0     2512 2024-03-14 12:40:05.729568 parsee_core-0.1.3.8/parsee/converters/main.py
--rw-r--r--   0        0        0     4339 2024-03-07 12:02:27.214681 parsee_core-0.1.3.8/parsee/converters/pdf_extraction.py
--rw-r--r--   0        0        0     6706 2024-02-28 09:39:54.651652 parsee_core-0.1.3.8/parsee/datasets/dataset_dataclasses.py
--rw-r--r--   0        0        0     6419 2024-03-11 17:39:35.687707 parsee_core-0.1.3.8/parsee/datasets/evaluation/main.py
--rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.3.8/parsee/datasets/main.py
--rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.3.8/parsee/datasets/readers/disk_reader.py
--rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.3.8/parsee/datasets/readers/interfaces.py
--rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.3.8/parsee/datasets/writers/disk_writer.py
--rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.3.8/parsee/datasets/writers/interfaces.py
--rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.3.8/parsee/extraction/__init__.py
--rw-r--r--   0        0        0     4072 2024-03-13 08:33:25.399204 parsee_core-0.1.3.8/parsee/extraction/extractor_dataclasses.py
--rw-r--r--   0        0        0    26486 2024-03-12 10:43:02.953830 parsee_core-0.1.3.8/parsee/extraction/extractor_elements.py
--rw-r--r--   0        0        0     9405 2024-02-14 09:53:17.695285 parsee_core-0.1.3.8/parsee/extraction/final_structuring.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.3.8/parsee/extraction/models/__init__.py
--rw-r--r--   0        0        0     1390 2024-03-15 10:50:04.142839 parsee_core-0.1.3.8/parsee/extraction/models/helpers.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.3.8/parsee/extraction/models/llm_models/__init__.py
--rw-r--r--   0        0        0     1988 2024-03-15 10:50:04.143286 parsee_core-0.1.3.8/parsee/extraction/models/llm_models/anthropic_model.py
--rw-r--r--   0        0        0     2107 2024-03-15 10:50:04.143625 parsee_core-0.1.3.8/parsee/extraction/models/llm_models/chatgpt_model.py
--rw-r--r--   0        0        0      787 2024-02-22 09:42:26.224225 parsee_core-0.1.3.8/parsee/extraction/models/llm_models/llm_base_model.py
--rw-r--r--   0        0        0      785 2024-02-19 16:48:56.158120 parsee_core-0.1.3.8/parsee/extraction/models/llm_models/prompts.py
--rw-r--r--   0        0        0     1936 2024-03-15 10:50:04.143967 parsee_core-0.1.3.8/parsee/extraction/models/llm_models/replicate_model.py
--rw-r--r--   0        0        0     7759 2024-03-12 16:24:07.618641 parsee_core-0.1.3.8/parsee/extraction/models/llm_models/structuring_schema.py
--rw-r--r--   0        0        0      882 2024-02-14 09:53:17.731629 parsee_core-0.1.3.8/parsee/extraction/models/model_dataclasses.py
--rw-r--r--   0        0        0     8011 2024-03-15 10:50:04.144186 parsee_core-0.1.3.8/parsee/extraction/models/model_loader.py
--rw-r--r--   0        0        0     3508 2024-02-22 09:49:50.419488 parsee_core-0.1.3.8/parsee/extraction/run.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.8/parsee/extraction/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.8/parsee/extraction/tasks/element_classification/__init__.py
--rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.3.8/parsee/extraction/tasks/element_classification/element_model.py
--rw-r--r--   0        0        0     2207 2024-02-22 09:52:47.321926 parsee_core-0.1.3.8/parsee/extraction/tasks/element_classification/element_model_llm.py
--rw-r--r--   0        0        0     7994 2024-03-08 10:22:59.229776 parsee_core-0.1.3.8/parsee/extraction/tasks/element_classification/features.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/__init__.py
--rw-r--r--   0        0        0     4811 2024-03-01 11:50:42.255522 parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/features.py
--rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/mapping_model.py
--rw-r--r--   0        0        0     1944 2024-02-22 09:52:47.320729 parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/mapping_model_llm.py
--rw-r--r--   0        0        0      928 2024-02-14 09:52:23.276265 parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/utils.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.3.8/parsee/extraction/tasks/meta_info_structuring/__init__.py
--rw-r--r--   0        0        0    13012 2024-03-01 12:05:20.644356 parsee_core-0.1.3.8/parsee/extraction/tasks/meta_info_structuring/features.py
--rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.3.8/parsee/extraction/tasks/meta_info_structuring/meta_info.py
--rw-r--r--   0        0        0     2619 2024-02-22 09:52:47.325111 parsee_core-0.1.3.8/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.3.8/parsee/extraction/tasks/questions/__init__.py
--rw-r--r--   0        0        0     5600 2024-03-15 10:50:04.144602 parsee_core-0.1.3.8/parsee/extraction/tasks/questions/features.py
--rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.3.8/parsee/extraction/tasks/questions/question_model.py
--rw-r--r--   0        0        0     3941 2024-03-12 16:27:29.550990 parsee_core-0.1.3.8/parsee/extraction/tasks/questions/question_model_llm.py
--rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.3.8/parsee/extraction/tasks/questions/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.3.8/parsee/storage/__init__.py
--rw-r--r--   0        0        0     2284 2024-02-22 09:42:26.247730 parsee_core-0.1.3.8/parsee/storage/in_memory_storage.py
--rw-r--r--   0        0        0      989 2024-03-04 17:06:27.482788 parsee_core-0.1.3.8/parsee/storage/interfaces.py
--rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.3.8/parsee/storage/vector_stores/interfaces.py
--rw-r--r--   0        0        0     3005 2024-02-21 09:37:29.119873 parsee_core-0.1.3.8/parsee/storage/vector_stores/simple_faiss.py
--rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.3.8/parsee/templates/__init__.py
--rw-r--r--   0        0        0     1293 2024-02-22 09:42:26.225885 parsee_core-0.1.3.8/parsee/templates/element_schema.py
--rw-r--r--   0        0        0      238 2024-01-26 09:00:34.050000 parsee_core-0.1.3.8/parsee/templates/export_schema.py
--rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.3.8/parsee/templates/general_structuring_schema.py
--rw-r--r--   0        0        0     3740 2024-02-22 09:42:26.221745 parsee_core-0.1.3.8/parsee/templates/helpers.py
--rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.3.8/parsee/templates/job_template.py
--rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.3.8/parsee/templates/mappings.py
--rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.3.8/parsee/templates/template_from_json.py
--rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.3.8/parsee/utils/__init__.py
--rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.3.8/parsee/utils/constants.py
--rw-r--r--   0        0        0      741 2024-03-15 10:50:04.144816 parsee_core-0.1.3.8/parsee/utils/enums.py
--rw-r--r--   0        0        0     5552 2024-03-14 12:47:20.873826 parsee_core-0.1.3.8/parsee/utils/helper.py
--rw-r--r--   0        0        0      781 2024-03-15 10:50:14.226945 parsee_core-0.1.3.8/pyproject.toml
--rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 parsee_core-0.1.3.8/PKG-INFO
+-rw-r--r--   0        0        0      485 2024-02-14 17:01:39.100086 parsee_core-0.1.3.9/parsee/__init__.py
+-rw-r--r--   0        0        0     2768 2024-03-13 08:58:10.546792 parsee_core-0.1.3.9/parsee/cloud/api.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.3.9/parsee/converters/__init__.py
+-rw-r--r--   0        0        0     6035 2024-02-14 15:27:25.505875 parsee_core-0.1.3.9/parsee/converters/html_extraction.py
+-rw-r--r--   0        0        0      344 2024-02-14 09:53:17.700535 parsee_core-0.1.3.9/parsee/converters/interfaces.py
+-rw-r--r--   0        0        0     1800 2024-02-14 11:04:57.276847 parsee_core-0.1.3.9/parsee/converters/json_to_raw.py
+-rw-r--r--   0        0        0     1063 2024-03-12 10:43:02.953449 parsee_core-0.1.3.9/parsee/converters/langchain.py
+-rw-r--r--   0        0        0     2512 2024-03-14 12:40:05.729568 parsee_core-0.1.3.9/parsee/converters/main.py
+-rw-r--r--   0        0        0     4339 2024-03-07 12:02:27.214681 parsee_core-0.1.3.9/parsee/converters/pdf_extraction.py
+-rw-r--r--   0        0        0     6706 2024-02-28 09:39:54.651652 parsee_core-0.1.3.9/parsee/datasets/dataset_dataclasses.py
+-rw-r--r--   0        0        0     6419 2024-03-11 17:39:35.687707 parsee_core-0.1.3.9/parsee/datasets/evaluation/main.py
+-rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.3.9/parsee/datasets/main.py
+-rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.3.9/parsee/datasets/readers/disk_reader.py
+-rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.3.9/parsee/datasets/readers/interfaces.py
+-rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.3.9/parsee/datasets/writers/disk_writer.py
+-rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.3.9/parsee/datasets/writers/interfaces.py
+-rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.3.9/parsee/extraction/__init__.py
+-rw-r--r--   0        0        0     4072 2024-03-13 08:33:25.399204 parsee_core-0.1.3.9/parsee/extraction/extractor_dataclasses.py
+-rw-r--r--   0        0        0    26486 2024-03-12 10:43:02.953830 parsee_core-0.1.3.9/parsee/extraction/extractor_elements.py
+-rw-r--r--   0        0        0     9405 2024-02-14 09:53:17.695285 parsee_core-0.1.3.9/parsee/extraction/final_structuring.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.3.9/parsee/extraction/models/__init__.py
+-rw-r--r--   0        0        0     1390 2024-03-15 10:50:04.142839 parsee_core-0.1.3.9/parsee/extraction/models/helpers.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/__init__.py
+-rw-r--r--   0        0        0     1995 2024-03-15 12:24:39.438997 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/anthropic_model.py
+-rw-r--r--   0        0        0     2107 2024-03-15 10:50:04.143625 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/chatgpt_model.py
+-rw-r--r--   0        0        0      787 2024-02-22 09:42:26.224225 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/llm_base_model.py
+-rw-r--r--   0        0        0      785 2024-02-19 16:48:56.158120 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/prompts.py
+-rw-r--r--   0        0        0     1936 2024-03-15 10:50:04.143967 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/replicate_model.py
+-rw-r--r--   0        0        0     7759 2024-03-12 16:24:07.618641 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/structuring_schema.py
+-rw-r--r--   0        0        0      882 2024-02-14 09:53:17.731629 parsee_core-0.1.3.9/parsee/extraction/models/model_dataclasses.py
+-rw-r--r--   0        0        0     8011 2024-03-15 10:50:04.144186 parsee_core-0.1.3.9/parsee/extraction/models/model_loader.py
+-rw-r--r--   0        0        0     3508 2024-02-22 09:49:50.419488 parsee_core-0.1.3.9/parsee/extraction/run.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.9/parsee/extraction/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/__init__.py
+-rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/element_model.py
+-rw-r--r--   0        0        0     2207 2024-02-22 09:52:47.321926 parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/element_model_llm.py
+-rw-r--r--   0        0        0     7994 2024-03-08 10:22:59.229776 parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/features.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/__init__.py
+-rw-r--r--   0        0        0     4811 2024-03-01 11:50:42.255522 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/features.py
+-rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/mapping_model.py
+-rw-r--r--   0        0        0     1944 2024-02-22 09:52:47.320729 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/mapping_model_llm.py
+-rw-r--r--   0        0        0      928 2024-02-14 09:52:23.276265 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/utils.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/__init__.py
+-rw-r--r--   0        0        0    13012 2024-03-01 12:05:20.644356 parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/features.py
+-rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/meta_info.py
+-rw-r--r--   0        0        0     2619 2024-02-22 09:52:47.325111 parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/__init__.py
+-rw-r--r--   0        0        0     5600 2024-03-15 10:50:04.144602 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/features.py
+-rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/question_model.py
+-rw-r--r--   0        0        0     3941 2024-03-12 16:27:29.550990 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/question_model_llm.py
+-rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.3.9/parsee/storage/__init__.py
+-rw-r--r--   0        0        0     2284 2024-02-22 09:42:26.247730 parsee_core-0.1.3.9/parsee/storage/in_memory_storage.py
+-rw-r--r--   0        0        0      989 2024-03-04 17:06:27.482788 parsee_core-0.1.3.9/parsee/storage/interfaces.py
+-rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.3.9/parsee/storage/vector_stores/interfaces.py
+-rw-r--r--   0        0        0     3005 2024-02-21 09:37:29.119873 parsee_core-0.1.3.9/parsee/storage/vector_stores/simple_faiss.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.3.9/parsee/templates/__init__.py
+-rw-r--r--   0        0        0     1293 2024-02-22 09:42:26.225885 parsee_core-0.1.3.9/parsee/templates/element_schema.py
+-rw-r--r--   0        0        0      238 2024-01-26 09:00:34.050000 parsee_core-0.1.3.9/parsee/templates/export_schema.py
+-rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.3.9/parsee/templates/general_structuring_schema.py
+-rw-r--r--   0        0        0     3740 2024-02-22 09:42:26.221745 parsee_core-0.1.3.9/parsee/templates/helpers.py
+-rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.3.9/parsee/templates/job_template.py
+-rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.3.9/parsee/templates/mappings.py
+-rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.3.9/parsee/templates/template_from_json.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.3.9/parsee/utils/__init__.py
+-rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.3.9/parsee/utils/constants.py
+-rw-r--r--   0        0        0      741 2024-03-15 10:50:04.144816 parsee_core-0.1.3.9/parsee/utils/enums.py
+-rw-r--r--   0        0        0     5552 2024-03-14 12:47:20.873826 parsee_core-0.1.3.9/parsee/utils/helper.py
+-rw-r--r--   0        0        0      781 2024-03-15 12:24:39.443961 parsee_core-0.1.3.9/pyproject.toml
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 parsee_core-0.1.3.9/PKG-INFO
```

### Comparing `parsee_core-0.1.3.8/parsee/cloud/api.py` & `parsee_core-0.1.3.9/parsee/cloud/api.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/converters/html_extraction.py` & `parsee_core-0.1.3.9/parsee/converters/html_extraction.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/converters/json_to_raw.py` & `parsee_core-0.1.3.9/parsee/converters/json_to_raw.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/converters/langchain.py` & `parsee_core-0.1.3.9/parsee/converters/langchain.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/converters/main.py` & `parsee_core-0.1.3.9/parsee/converters/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/converters/pdf_extraction.py` & `parsee_core-0.1.3.9/parsee/converters/pdf_extraction.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/datasets/dataset_dataclasses.py` & `parsee_core-0.1.3.9/parsee/datasets/dataset_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/datasets/evaluation/main.py` & `parsee_core-0.1.3.9/parsee/datasets/evaluation/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/datasets/main.py` & `parsee_core-0.1.3.9/parsee/datasets/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/datasets/readers/disk_reader.py` & `parsee_core-0.1.3.9/parsee/datasets/readers/disk_reader.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/datasets/readers/interfaces.py` & `parsee_core-0.1.3.9/parsee/datasets/readers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/datasets/writers/disk_writer.py` & `parsee_core-0.1.3.9/parsee/datasets/writers/disk_writer.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/datasets/writers/interfaces.py` & `parsee_core-0.1.3.9/parsee/datasets/writers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/extractor_dataclasses.py` & `parsee_core-0.1.3.9/parsee/extraction/extractor_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/extractor_elements.py` & `parsee_core-0.1.3.9/parsee/extraction/extractor_elements.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/final_structuring.py` & `parsee_core-0.1.3.9/parsee/extraction/final_structuring.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/helpers.py` & `parsee_core-0.1.3.9/parsee/extraction/models/helpers.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/llm_models/anthropic_model.py` & `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/anthropic_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 temperature=0,
                 messages=[
                     {"role": "user", "content": prompt}
                 ]
             )
 
             answer = message.content[0].text if len(message.content) > 0 else ""
-            final_cost = (Decimal(message.usage.input_tokens+message.usage.output_tokens) * (self.model.price_per_1k_tokens/1000)) if self.model.price_per_1k_tokens is not None else Decimal(0)
+            final_cost = (Decimal(message.usage.input_tokens+message.usage.output_tokens) * Decimal(self.model.price_per_1k_tokens/1000)) if self.model.price_per_1k_tokens is not None else Decimal(0)
             return answer, final_cost
         except Exception as e:
             if retries < self.max_retries:
                 time.sleep(wait * 2 ** retries)
                 return self._call_api(prompt, retries + 1)
             else:
                 return "", Decimal(0)
```

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/llm_models/chatgpt_model.py` & `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/chatgpt_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/llm_models/llm_base_model.py` & `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/llm_base_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/llm_models/prompts.py` & `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/prompts.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/llm_models/replicate_model.py` & `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/replicate_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/llm_models/structuring_schema.py` & `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/model_dataclasses.py` & `parsee_core-0.1.3.9/parsee/extraction/models/model_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/models/model_loader.py` & `parsee_core-0.1.3.9/parsee/extraction/models/model_loader.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/run.py` & `parsee_core-0.1.3.9/parsee/extraction/run.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/element_classification/element_model.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/element_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/element_classification/element_model_llm.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/element_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/element_classification/features.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/features.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/mapping_model.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/mapping_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/mapping_model_llm.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/mapping_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/mappings/utils.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/meta_info_structuring/features.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/meta_info_structuring/meta_info.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/meta_info.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/questions/features.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/questions/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/questions/question_model.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/questions/question_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/questions/question_model_llm.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/questions/question_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/extraction/tasks/questions/utils.py` & `parsee_core-0.1.3.9/parsee/extraction/tasks/questions/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/storage/in_memory_storage.py` & `parsee_core-0.1.3.9/parsee/storage/in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/storage/interfaces.py` & `parsee_core-0.1.3.9/parsee/storage/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/storage/vector_stores/simple_faiss.py` & `parsee_core-0.1.3.9/parsee/storage/vector_stores/simple_faiss.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/templates/element_schema.py` & `parsee_core-0.1.3.9/parsee/templates/element_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/templates/general_structuring_schema.py` & `parsee_core-0.1.3.9/parsee/templates/general_structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/templates/helpers.py` & `parsee_core-0.1.3.9/parsee/templates/helpers.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/templates/job_template.py` & `parsee_core-0.1.3.9/parsee/templates/job_template.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/templates/mappings.py` & `parsee_core-0.1.3.9/parsee/templates/mappings.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/utils/enums.py` & `parsee_core-0.1.3.9/parsee/utils/enums.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/parsee/utils/helper.py` & `parsee_core-0.1.3.9/parsee/utils/helper.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.8/pyproject.toml` & `parsee_core-0.1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsee-core"
-version = "0.1.3.8"
+version = "0.1.3.9"
 description = ""
 authors = ["Parsee.ai <info@parsee.ai>"]
 homepage = "https://parsee.ai"
 packages = [{include = "parsee"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
```

### Comparing `parsee_core-0.1.3.8/PKG-INFO` & `parsee_core-0.1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsee-core
-Version: 0.1.3.8
+Version: 0.1.3.9
 Summary: 
 Home-page: https://parsee.ai
 Author: Parsee.ai
 Author-email: info@parsee.ai
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

