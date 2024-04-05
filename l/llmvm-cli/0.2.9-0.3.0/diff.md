# Comparing `tmp/llmvm_cli-0.2.9.tar.gz` & `tmp/llmvm_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmvm_cli-0.2.9.tar", max compression
+gzip compressed data, was "llmvm_cli-0.3.0.tar", max compression
```

## Comparing `llmvm_cli-0.2.9.tar` & `llmvm_cli-0.3.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0     1495 2023-08-25 00:38:50.285349 llmvm_cli-0.2.9/LICENSE
--rw-r--r--   0        0        0    28302 2024-03-24 21:27:31.080227 llmvm_cli-0.2.9/README.md
--rw-r--r--   0        0        0      106 2024-02-19 19:15:49.498636 llmvm_cli-0.2.9/llmvm/client/__main__.py
--rw-r--r--   0        0        0    65054 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/client/awesome_prompts.csv
--rw-r--r--   0        0        0    75466 2024-03-24 23:48:03.697862 llmvm_cli-0.2.9/llmvm/client/client.py
--rw-r--r--   0        0        0        0 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/common/__init__.py
--rw-r--r--   0        0        0    18387 2024-03-24 23:53:05.635163 llmvm_cli-0.2.9/llmvm/common/anthropic_executor.py
--rw-r--r--   0        0        0     3828 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/common/container.py
--rw-r--r--   0        0        0     7735 2024-03-23 20:37:13.889331 llmvm_cli-0.2.9/llmvm/common/gemini_executor.py
--rw-r--r--   0        0        0    39682 2024-03-16 21:48:48.336279 llmvm_cli-0.2.9/llmvm/common/helpers.py
--rw-r--r--   0        0        0     7472 2024-03-09 18:34:25.824843 llmvm_cli-0.2.9/llmvm/common/logging_helpers.py
--rw-r--r--   0        0        0     7100 2024-03-23 20:32:11.140212 llmvm_cli-0.2.9/llmvm/common/mistral_executor.py
--rw-r--r--   0        0        0     3852 2024-03-17 05:28:38.556759 llmvm_cli-0.2.9/llmvm/common/object_transformers.py
--rw-r--r--   0        0        0    28425 2024-03-23 20:37:11.425322 llmvm_cli-0.2.9/llmvm/common/objects.py
--rw-r--r--   0        0        0    10068 2024-03-23 20:24:42.394521 llmvm_cli-0.2.9/llmvm/common/openai_executor.py
--rw-r--r--   0        0        0     6563 2024-03-16 21:40:48.365800 llmvm_cli-0.2.9/llmvm/common/pdf.py
--rw-r--r--   0        0        0    10201 2024-03-23 20:33:11.888437 llmvm_cli-0.2.9/llmvm/common/perf.py
--rw-r--r--   0        0        0      457 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/common/singleton.py
--rw-r--r--   0        0        0     1608 2024-03-17 08:21:55.736230 llmvm_cli-0.2.9/llmvm/config.yaml
--rw-r--r--   0        0        0    76737 2024-03-16 22:18:47.282337 llmvm_cli-0.2.9/llmvm/model_prices_and_context_window.json
--rw-r--r--   0        0        0        0 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/__init__.py
--rw-r--r--   0        0        0      106 2024-02-19 19:16:42.270867 llmvm_cli-0.2.9/llmvm/server/__main__.py
--rw-r--r--   0        0        0     5977 2024-03-09 18:34:25.824843 llmvm_cli-0.2.9/llmvm/server/ast_parser.py
--rw-r--r--   0        0        0     2255 2024-03-16 03:31:58.989238 llmvm_cli-0.2.9/llmvm/server/base_library/content_downloader.py
--rw-r--r--   0        0        0    13460 2024-03-23 20:03:01.496961 llmvm_cli-0.2.9/llmvm/server/base_library/function_bindable.py
--rw-r--r--   0        0        0    16053 2024-03-23 20:03:01.512961 llmvm_cli-0.2.9/llmvm/server/base_library/searcher.py
--rw-r--r--   0        0        0     5457 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/base_library/source.py
--rw-r--r--   0        0        0     6006 2024-03-23 20:03:01.512961 llmvm_cli-0.2.9/llmvm/server/base_library/source_project.py
--rw-r--r--   0        0        0      607 2024-03-15 23:56:01.794321 llmvm_cli-0.2.9/llmvm/server/bcl.py
--rw-r--r--   0        0        0     1731 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/persistent_cache.py
--rw-r--r--   0        0        0        0 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/__init__.py
--rw-r--r--   0        0        0      160 2024-03-17 08:20:46.961242 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      176 2024-02-18 20:46:27.585460 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1148 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer.prompt
--rw-r--r--   0        0        0     4983 2024-03-17 20:55:58.695953 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer_error_correction.prompt
--rw-r--r--   0        0        0     1339 2024-03-17 21:23:27.214324 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer_nocontext.prompt
--rw-r--r--   0        0        0      362 2024-03-09 18:34:25.828843 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer_primitive.prompt
--rw-r--r--   0        0        0     5532 2024-03-17 21:44:34.840485 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer_regen_code_or_rewrite.prompt
--rw-r--r--   0        0        0       84 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/assistant_result.prompt
--rw-r--r--   0        0        0     1463 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/code_get_source_summary.prompt
--rw-r--r--   0        0        0      380 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/code_method_definition.prompt
--rw-r--r--   0        0        0      810 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/coerce.prompt
--rw-r--r--   0        0        0      788 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/document_chunk.prompt
--rw-r--r--   0        0        0       81 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/foreach_result.prompt
--rw-r--r--   0        0        0      343 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/function_call_result.prompt
--rw-r--r--   0        0        0      320 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/functionmeta_result.prompt
--rw-r--r--   0        0        0      215 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/list_result.prompt
--rw-r--r--   0        0        0      757 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_error_correction.prompt
--rw-r--r--   0        0        0     1544 2024-03-18 01:20:28.422176 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_global.prompt
--rw-r--r--   0        0        0      935 2024-02-07 01:05:05.227736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_list.prompt
--rw-r--r--   0        0        0      784 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_local.prompt
--rw-r--r--   0        0        0      862 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_old.prompt
--rw-r--r--   0        0        0      556 2024-03-09 18:34:25.828843 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_call.prompt
--rw-r--r--   0        0        0      167 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_call_result.prompt
--rw-r--r--   0        0        0      545 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_loop_bind.prompt
--rw-r--r--   0        0        0      876 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/map_reduce_map.prompt
--rw-r--r--   0        0        0      783 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/map_reduce_reduce.prompt
--rw-r--r--   0        0        0      592 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/pandas_bind.prompt
--rw-r--r--   0        0        0      641 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/pdf_content.prompt
--rw-r--r--   0        0        0     2639 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/query_understanding.prompt
--rw-r--r--   0        0        0      762 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/search_classifier.prompt
--rw-r--r--   0        0        0      458 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/search_expander.prompt
--rw-r--r--   0        0        0     1003 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/search_location.prompt
--rw-r--r--   0        0        0      746 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/search_ranker.prompt
--rw-r--r--   0        0        0     8200 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_code_insights.prompt
--rw-r--r--   0        0        0     4940 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_code_prompt_old.prompt
--rw-r--r--   0        0        0    12639 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_continuation_execution.prompt
--rw-r--r--   0        0        0     4927 2024-03-17 05:45:59.593830 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_error_correction.prompt
--rw-r--r--   0        0        0    15324 2024-03-17 05:45:45.041749 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_tool_execution.prompt
--rw-r--r--   0        0        0      156 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/prompts/starlark/str_result.prompt
--rw-r--r--   0        0        0    23395 2024-03-17 22:50:41.916006 llmvm_cli-0.2.9/llmvm/server/server.py
--rw-r--r--   0        0        0    37254 2024-03-23 20:08:27.966392 llmvm_cli-0.2.9/llmvm/server/starlark_execution_controller.py
--rw-r--r--   0        0        0    40722 2024-03-23 20:03:01.488961 llmvm_cli-0.2.9/llmvm/server/starlark_runtime.py
--rw-r--r--   0        0        0    11120 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/tools/browser.py
--rw-r--r--   0        0        0     6327 2024-03-16 02:14:12.501375 llmvm_cli-0.2.9/llmvm/server/tools/edgar.py
--rw-r--r--   0        0        0    12020 2024-03-17 21:30:40.436550 llmvm_cli-0.2.9/llmvm/server/tools/firefox.py
--rw-r--r--   0        0        0        0 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/tools/legacy.py
--rw-r--r--   0        0        0     1872 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/tools/market.py
--rw-r--r--   0        0        0     4270 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/tools/scraper.py
--rw-r--r--   0        0        0     6839 2024-02-19 19:10:51.453449 llmvm_cli-0.2.9/llmvm/server/tools/search.py
--rw-r--r--   0        0        0     8704 2024-02-07 01:05:05.231736 llmvm_cli-0.2.9/llmvm/server/tools/search_hn.py
--rw-r--r--   0        0        0     4369 2024-03-16 19:27:38.094307 llmvm_cli-0.2.9/llmvm/server/tools/webhelpers.py
--rw-r--r--   0        0        0     9391 2024-03-16 19:24:49.413325 llmvm_cli-0.2.9/llmvm/server/vector_search.py
--rw-r--r--   0        0        0     6848 2024-02-19 23:04:49.110110 llmvm_cli-0.2.9/llmvm/server/vector_store.py
--rw-r--r--   0        0        0     1562 2024-03-24 23:53:23.447240 llmvm_cli-0.2.9/pyproject.toml
--rw-r--r--   0        0        0    30688 1970-01-01 00:00:00.000000 llmvm_cli-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1495 2024-01-03 07:02:07.545205 llmvm_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0    28302 2024-04-02 06:01:38.458668 llmvm_cli-0.3.0/README.md
+-rw-r--r--   0        0        0      106 2024-02-25 23:41:30.071592 llmvm_cli-0.3.0/llmvm/client/__main__.py
+-rw-r--r--   0        0        0    65054 2024-02-07 02:24:12.376520 llmvm_cli-0.3.0/llmvm/client/awesome_prompts.csv
+-rw-r--r--   0        0        0    76135 2024-04-05 17:39:11.686252 llmvm_cli-0.3.0/llmvm/client/client.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:24:12.376988 llmvm_cli-0.3.0/llmvm/common/__init__.py
+-rw-r--r--   0        0        0    19995 2024-04-05 04:13:18.903735 llmvm_cli-0.3.0/llmvm/common/anthropic_executor.py
+-rw-r--r--   0        0        0     3828 2024-02-07 02:24:12.377381 llmvm_cli-0.3.0/llmvm/common/container.py
+-rw-r--r--   0        0        0     7735 2024-04-02 06:01:38.459780 llmvm_cli-0.3.0/llmvm/common/gemini_executor.py
+-rw-r--r--   0        0        0    40120 2024-04-05 04:13:18.904346 llmvm_cli-0.3.0/llmvm/common/helpers.py
+-rw-r--r--   0        0        0     7472 2024-03-01 18:22:41.276981 llmvm_cli-0.3.0/llmvm/common/logging_helpers.py
+-rw-r--r--   0        0        0     7100 2024-04-02 06:01:38.460105 llmvm_cli-0.3.0/llmvm/common/mistral_executor.py
+-rw-r--r--   0        0        0     3861 2024-04-05 04:13:18.904513 llmvm_cli-0.3.0/llmvm/common/object_transformers.py
+-rw-r--r--   0        0        0    28450 2024-04-05 17:39:11.686652 llmvm_cli-0.3.0/llmvm/common/objects.py
+-rw-r--r--   0        0        0    10655 2024-04-05 17:39:11.686930 llmvm_cli-0.3.0/llmvm/common/openai_executor.py
+-rw-r--r--   0        0        0     7404 2024-04-05 04:13:18.905099 llmvm_cli-0.3.0/llmvm/common/pdf.py
+-rw-r--r--   0        0        0    10711 2024-04-02 06:01:38.460644 llmvm_cli-0.3.0/llmvm/common/perf.py
+-rw-r--r--   0        0        0      457 2024-02-07 02:24:12.378504 llmvm_cli-0.3.0/llmvm/common/singleton.py
+-rw-r--r--   0        0        0     1608 2024-03-18 05:16:30.191195 llmvm_cli-0.3.0/llmvm/config.yaml
+-rw-r--r--   0        0        0    76737 2024-04-02 06:01:38.460972 llmvm_cli-0.3.0/llmvm/model_prices_and_context_window.json
+-rw-r--r--   0        0        0        0 2024-02-07 02:24:12.378662 llmvm_cli-0.3.0/llmvm/server/__init__.py
+-rw-r--r--   0        0        0      106 2024-02-25 23:41:30.074183 llmvm_cli-0.3.0/llmvm/server/__main__.py
+-rw-r--r--   0        0        0     5977 2024-03-01 18:22:41.278186 llmvm_cli-0.3.0/llmvm/server/ast_parser.py
+-rw-r--r--   0        0        0    20300 2024-04-02 06:01:38.461151 llmvm_cli-0.3.0/llmvm/server/base_library/browser.py
+-rw-r--r--   0        0        0     2255 2024-03-18 05:16:30.191315 llmvm_cli-0.3.0/llmvm/server/base_library/content_downloader.py
+-rw-r--r--   0        0        0    13460 2024-04-02 06:01:38.461337 llmvm_cli-0.3.0/llmvm/server/base_library/function_bindable.py
+-rw-r--r--   0        0        0    16053 2024-04-02 06:01:38.461512 llmvm_cli-0.3.0/llmvm/server/base_library/searcher.py
+-rw-r--r--   0        0        0     5457 2024-03-18 05:16:30.191913 llmvm_cli-0.3.0/llmvm/server/base_library/source.py
+-rw-r--r--   0        0        0     6006 2024-04-02 06:01:38.461658 llmvm_cli-0.3.0/llmvm/server/base_library/source_project.py
+-rw-r--r--   0        0        0      607 2024-03-18 05:16:30.192200 llmvm_cli-0.3.0/llmvm/server/bcl.py
+-rw-r--r--   0        0        0     1731 2024-02-07 02:24:12.379056 llmvm_cli-0.3.0/llmvm/server/persistent_cache.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:24:12.379148 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/__init__.py
+-rw-r--r--   0        0        0     1148 2024-02-07 02:24:12.379247 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer.prompt
+-rw-r--r--   0        0        0     4983 2024-03-18 05:16:30.192346 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_error_correction.prompt
+-rw-r--r--   0        0        0     1339 2024-03-18 05:16:30.192471 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_nocontext.prompt
+-rw-r--r--   0        0        0      362 2024-03-18 05:16:30.192566 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_primitive.prompt
+-rw-r--r--   0        0        0     5532 2024-03-18 05:16:30.192634 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_regen_code_or_rewrite.prompt
+-rw-r--r--   0        0        0       84 2024-02-07 02:24:12.379686 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/assistant_result.prompt
+-rw-r--r--   0        0        0     2542 2024-04-02 06:01:38.461773 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/browser_execute_plan.prompt
+-rw-r--r--   0        0        0     1883 2024-04-02 06:01:38.461872 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/browser_generate_plan.prompt
+-rw-r--r--   0        0        0     1463 2024-02-07 02:24:12.384341 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/code_get_source_summary.prompt
+-rw-r--r--   0        0        0      380 2024-02-07 02:24:12.384491 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/code_method_definition.prompt
+-rw-r--r--   0        0        0      810 2024-02-07 02:24:12.384600 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/coerce.prompt
+-rw-r--r--   0        0        0      788 2024-02-07 02:24:12.384694 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/document_chunk.prompt
+-rw-r--r--   0        0        0       81 2024-02-07 02:24:12.384782 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/foreach_result.prompt
+-rw-r--r--   0        0        0      343 2024-02-07 02:24:12.384857 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/function_call_result.prompt
+-rw-r--r--   0        0        0      320 2024-02-07 02:24:12.384939 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/functionmeta_result.prompt
+-rw-r--r--   0        0        0      215 2024-02-07 02:24:12.385017 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/list_result.prompt
+-rw-r--r--   0        0        0      757 2024-02-07 02:24:12.385103 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_error_correction.prompt
+-rw-r--r--   0        0        0     1544 2024-03-18 05:16:30.192749 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_global.prompt
+-rw-r--r--   0        0        0      935 2024-02-07 02:24:12.385254 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_list.prompt
+-rw-r--r--   0        0        0      784 2024-02-07 02:24:12.385408 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_local.prompt
+-rw-r--r--   0        0        0      862 2024-02-07 02:24:12.385520 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_old.prompt
+-rw-r--r--   0        0        0      556 2024-03-18 05:16:30.192871 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_call.prompt
+-rw-r--r--   0        0        0      167 2024-02-07 02:24:12.385701 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_call_result.prompt
+-rw-r--r--   0        0        0      545 2024-02-07 02:24:12.385794 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_loop_bind.prompt
+-rw-r--r--   0        0        0      876 2024-02-07 02:24:12.385890 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/map_reduce_map.prompt
+-rw-r--r--   0        0        0      783 2024-02-07 02:24:12.387514 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/map_reduce_reduce.prompt
+-rw-r--r--   0        0        0      592 2024-02-07 02:24:12.387584 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/pandas_bind.prompt
+-rw-r--r--   0        0        0      641 2024-02-07 02:24:12.387647 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/pdf_content.prompt
+-rw-r--r--   0        0        0     2639 2024-02-07 02:24:12.387730 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/query_understanding.prompt
+-rw-r--r--   0        0        0      762 2024-02-07 02:24:12.387793 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_classifier.prompt
+-rw-r--r--   0        0        0      458 2024-02-07 02:24:12.387857 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_expander.prompt
+-rw-r--r--   0        0        0     1003 2024-02-07 02:24:12.387923 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_location.prompt
+-rw-r--r--   0        0        0      746 2024-02-07 02:24:12.388003 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_ranker.prompt
+-rw-r--r--   0        0        0     8200 2024-02-07 02:24:12.388113 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_code_insights.prompt
+-rw-r--r--   0        0        0     4940 2024-02-07 02:24:12.388202 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_code_prompt_old.prompt
+-rw-r--r--   0        0        0    12639 2024-02-07 02:24:12.388275 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_continuation_execution.prompt
+-rw-r--r--   0        0        0     4927 2024-03-18 05:16:30.193009 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_error_correction.prompt
+-rw-r--r--   0        0        0    15324 2024-03-18 05:16:30.193153 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_tool_execution.prompt
+-rw-r--r--   0        0        0      156 2024-02-07 02:24:12.388557 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/str_result.prompt
+-rw-r--r--   0        0        0    23395 2024-03-18 05:16:30.193315 llmvm_cli-0.3.0/llmvm/server/server.py
+-rw-r--r--   0        0        0    37254 2024-04-02 06:01:38.462118 llmvm_cli-0.3.0/llmvm/server/starlark_execution_controller.py
+-rw-r--r--   0        0        0    40722 2024-04-02 06:01:38.462363 llmvm_cli-0.3.0/llmvm/server/starlark_runtime.py
+-rw-r--r--   0        0        0     6327 2024-03-18 05:16:30.194183 llmvm_cli-0.3.0/llmvm/server/tools/edgar.py
+-rw-r--r--   0        0        0    13091 2024-04-02 06:01:38.462546 llmvm_cli-0.3.0/llmvm/server/tools/firefox.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:24:12.389702 llmvm_cli-0.3.0/llmvm/server/tools/legacy.py
+-rw-r--r--   0        0        0     1872 2024-02-07 02:24:12.389891 llmvm_cli-0.3.0/llmvm/server/tools/market.py
+-rw-r--r--   0        0        0     4270 2024-02-07 02:24:12.390078 llmvm_cli-0.3.0/llmvm/server/tools/scraper.py
+-rw-r--r--   0        0        0     6839 2024-02-25 23:41:30.075967 llmvm_cli-0.3.0/llmvm/server/tools/search.py
+-rw-r--r--   0        0        0     8704 2024-02-07 02:24:12.390266 llmvm_cli-0.3.0/llmvm/server/tools/search_hn.py
+-rw-r--r--   0        0        0     4603 2024-04-02 06:01:38.462796 llmvm_cli-0.3.0/llmvm/server/tools/webhelpers.py
+-rw-r--r--   0        0        0     9391 2024-03-18 05:16:30.194621 llmvm_cli-0.3.0/llmvm/server/vector_search.py
+-rw-r--r--   0        0        0     6848 2024-02-25 23:41:30.076167 llmvm_cli-0.3.0/llmvm/server/vector_store.py
+-rw-r--r--   0        0        0     1562 2024-04-05 17:39:25.432631 llmvm_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    30688 1970-01-01 00:00:00.000000 llmvm_cli-0.3.0/PKG-INFO
```

### Comparing `llmvm_cli-0.2.9/LICENSE` & `llmvm_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/README.md` & `llmvm_cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/client/awesome_prompts.csv` & `llmvm_cli-0.3.0/llmvm/client/awesome_prompts.csv`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/client/client.py` & `llmvm_cli-0.3.0/llmvm/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,49 @@
         sub_messages = parse_message_actions(type(parsed_message), content)
         for sub_message in sub_messages:
             messages.append(sub_message)
         message = message[len(role) + len(content):]
     return messages
 
 
-def parse_path(ctx, param, value, raise_parse_exception=False) -> List[str]:
+def parse_path(ctx, param, value) -> List[str]:
+    def parse_helper(value, exclusions):
+        files = []
+        # deal with ~
+        item = os.path.expanduser(value)
+        # shell escaping
+        item = item.replace('\\', '')
+
+        if os.path.isdir(item):
+            # If it's a directory, add all files within
+            for dirpath, dirnames, filenames in os.walk(item):
+                for filename in filenames:
+                    files.append(os.path.join(dirpath, filename))
+
+                if not Helpers.is_glob_recursive(item):
+                    dirnames.clear()
+        elif os.path.isfile(item):
+            # If it's a file, add it to the list
+            files.append(item)
+        # check for glob
+        elif Helpers.is_glob_pattern(item):
+            # check for !
+            if item.startswith('!'):
+                for filepath in glob.glob(item[1:], recursive=Helpers.is_glob_recursive(item)):
+                    exclusions.append(filepath)
+            elif any('{' in item and '}' in item for item in value):
+                brace_items = Helpers.flatten([Helpers.glob_brace(item) for item in value if '{' in item and '}' in item])
+                files = files + brace_items
+            else:
+                for filepath in glob.glob(item, recursive=Helpers.is_glob_recursive(item)):
+                    files.append(filepath)
+        elif item.startswith('http'):
+            files.append(item)
+        return files
+
     if not value:
         return []
 
     if (
         (isinstance(value, str))
         and (value.startswith('"') or value.startswith("'"))
         and (value.endswith("'") or value.endswith('"'))
@@ -140,71 +174,34 @@
         value = value[1:-1]
 
     files = []
 
     if not value:
         return files
 
-    if isinstance(value, str) and not Helpers.is_glob_pattern(value) and ',' in value:
-        value = value.split(',')
-
     if isinstance(value, str):
         value = [value]
 
     if isinstance(value, tuple):
         value = list(value)
 
     # see if there are any brace glob patterns, and if so, expand them
     # and include them in the value array
     if any('{' in item and '}' in item for item in value):
         brace_globs = [Helpers.glob_brace(item) for item in value if '{' in item and '}' in item]
         brace_globs = Helpers.flatten(brace_globs)
-        value += tuple(brace_globs)
+        value += list(brace_globs)
 
     # split by ' '
-    value = Helpers.flatten([item.split(' ') for item in value])
+    # value = Helpers.flatten([item.split(' ') for item in value])
 
     exclusions = []
 
     for item in value:
-        # deal with ~
-        item = os.path.expanduser(item)
-        # shell escaping
-        item = item.replace('\\', '')
-
-        if os.path.isdir(item):
-            # If it's a directory, add all files within
-            for dirpath, dirnames, filenames in os.walk(item):
-                for filename in filenames:
-                    files.append(os.path.join(dirpath, filename))
-
-                if not Helpers.is_glob_recursive(item):
-                    dirnames.clear()
-        elif os.path.isfile(item):
-            # If it's a file, add it to the list
-            files.append(item)
-        # check for glob
-        elif Helpers.is_glob_pattern(item):
-            # check for !
-            if item.startswith('!'):
-                for filepath in glob.glob(item[1:], recursive=Helpers.is_glob_recursive(item)):
-                    exclusions.append(filepath)
-            elif any('{' in item and '}' in item for item in value):
-                brace_items = Helpers.flatten([Helpers.glob_brace(item) for item in value if '{' in item and '}' in item])
-                files = files + brace_items
-            else:
-                for filepath in glob.glob(item, recursive=Helpers.is_glob_recursive(item)):
-                    files.append(filepath)
-        elif item.startswith('http'):
-            files.append(item)
-        else:
-            if raise_parse_exception:
-                raise MissingParameter(f'Unable to parse path: {item}')
-            else:
-                return []
+        files.extend(parse_helper(item, exclusions))
 
     # deal with exclusions
     files = [file for file in files if file not in exclusions]
     return files
 
 
 def parse_command_string(s, command):
@@ -236,15 +233,15 @@
             path_part = ''
             # special case path because of strange shell behavior with " "
             if part == '-p' or part == '--path':
                 z = i
                 while (
                     (z + 1 < len(parts))
                     and (
-                        parse_path(None, None, parts[z + 1], raise_parse_exception=False)
+                        parse_path(None, None, parts[z + 1])
                         or Helpers.glob_brace(parts[z + 1])
                         or parts[z + 1].startswith('!')
                     )
                 ):
                     path_part += parts[z + 1] + ' '
                     # tokens.append(parts[z + 1])
                     skip_n += 1
@@ -685,33 +682,14 @@
     elif isinstance(message, bytes):
         user_message = User(Content(message.decode('utf-8')))
     elif isinstance(message, Message):
         user_message = message
 
     context_messages_list = list(context_messages)
 
-    if not sys.stdin.isatty():
-        # input is coming from a pipe, could be binary or text
-        if not message: message = ''
-
-        file_content = sys.stdin.buffer.read()
-
-        with io.BytesIO(file_content) as bytes_buffer:
-            if Helpers.is_image(bytes_buffer):
-                image_bytes = Helpers.load_resize_save(bytes_buffer.getvalue(), 'PNG')
-                StreamPrinter('user').display_image(image_bytes)
-                context_messages_list.insert(0, User(ImageContent(image_bytes, url='cli')))
-            elif Helpers.is_pdf(bytes_buffer):
-                with tempfile.NamedTemporaryFile(delete=False, suffix='.pdf') as temp_file:
-                    temp_file.write(bytes_buffer.read())
-                    temp_file.flush()
-                    context_messages_list.insert(0, User(PdfContent(bytes_buffer.read(), url=temp_file.name)))
-            else:
-                context_messages_list.insert(0, User(Content(bytes_buffer.read().decode('utf-8', errors='ignore'))))
-
     clear_thread = False
     # if the incoming message is a thread, parse it and send it through
     role_strings = ['Assistant: ', 'System: ', 'User: ']
     action_strings = ['ImageContent(', 'PdfContent(', 'FileContent(']
 
     if isinstance(message, str) and any(role_string in message for role_string in role_strings):
         all_messages = parse_message_thread(message)
@@ -1307,15 +1285,15 @@
             except Exception:
                 console.print_exception(max_frames=10)
 
 
 @click.group(
     cls=DefaultGroup,
     default='message',
-    default_if_no_args=False,
+    default_if_no_args=True,
 )
 @click.pass_context
 def cli(ctx):
     global invoke_context
     global renderer
 
     if ctx.invoked_subcommand is None:
@@ -1825,15 +1803,15 @@
     model: str,
     compression: str,
     escape: bool,
     context_messages: Sequence[Message] = [],
 ):
     global thread_id
     global last_thread
-    # context_messages: Sequence[Message] = []
+    context_messages = list(context_messages)
 
     if mode == 'code' and not path:
         raise MissingParameter('path')
 
     if not escape and not sys.stdin.isatty():
         escape = True
 
@@ -1861,14 +1839,53 @@
             context_messages.insert(0, User(Content(c)))
 
     # if we have files, but no message, grab the last file and use it as the message
     if not message and context_messages:
         message = context_messages[-1]
         context_messages = context_messages[:-1]
 
+    # input is coming from a pipe, could be binary or text
+    if not sys.stdin.isatty():
+        import select
+        ready, _, _ = select.select([sys.stdin], [], [], 1)
+
+        if ready:
+            lines = []
+            while True:
+                line = sys.stdin.buffer.readline()
+                if not line:
+                    break
+                lines.append(line)
+            # file_content = sys.stdin.buffer.read()
+            file_content = b''.join(lines)
+            with io.BytesIO(file_content) as bytes_buffer:
+                if Helpers.is_image(bytes_buffer):
+                    image_bytes = Helpers.load_resize_save(bytes_buffer.getvalue(), 'PNG')
+                    StreamPrinter('user').display_image(image_bytes)
+                    tty_message = User(ImageContent(image_bytes, url='cli'))
+                    if message:
+                        context_messages.insert(0, tty_message)
+                    else:
+                        message = tty_message
+                elif Helpers.is_pdf(bytes_buffer):
+                    with tempfile.NamedTemporaryFile(delete=False, suffix='.pdf') as temp_file:
+                        temp_file.write(bytes_buffer.read())
+                        temp_file.flush()
+                        tty_message = User(PdfContent(bytes_buffer.read(), url=temp_file.name))
+                        if message:
+                            context_messages.insert(0, tty_message)
+                        else:
+                            message = tty_message
+                else:
+                    tty_message = User(Content(bytes_buffer.read().decode('utf-8', errors='ignore')))
+                    if message:
+                        context_messages.insert(0, tty_message)
+                    else:
+                        message = tty_message
+
     if message:
         if isinstance(message, str) and (
             (message.startswith('"') and message.endswith('"'))
             or (message.startswith("'") and message.endswith("'"))
         ):
             message = message[1:-1]
 
@@ -1909,21 +1926,23 @@
 
         if not escape: StreamPrinter('').write_string('\n')
         print_response([MessageModel.to_message(thread.messages[-1])], escape)
         if not escape: StreamPrinter('').write_string('\n')
         last_thread = thread
         thread_id = thread.id
         return thread
+    else:
+        rich.print('No message to send.')
 
 
 if __name__ == '__main__':
     # special case the hijacking of --help
     if len(sys.argv) == 2 and (sys.argv[1] == '--help' or sys.argv[1] == '-h'):
         Repl().help()
         sys.exit(0)
 
-    if len(sys.argv) <= 1:
+    if len(sys.argv) <= 1 and sys.stdin.isatty():
         repl_inst = Repl()
         loop = asyncio.get_event_loop()
         loop.run_until_complete(repl_inst.repl())
     else:
         cli()
```

### Comparing `llmvm_cli-0.2.9/llmvm/common/anthropic_executor.py` & `llmvm_cli-0.3.0/llmvm/common/anthropic_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import base64
 import os
 from typing import Any, Awaitable, Callable, Dict, List, Optional, cast
 
 from anthropic import AI_PROMPT, HUMAN_PROMPT, AsyncAnthropic
+from anthropic.types.message import Message as AnthropicMessage
 
 from llmvm.common.container import Container
 from llmvm.common.helpers import Helpers
 from llmvm.common.logging_helpers import messages_trace, setup_logging
 from llmvm.common.object_transformers import ObjectTransformers
 from llmvm.common.objects import (Assistant, AstNode, Content, Executor,
                                   FileContent, ImageContent, MarkdownContent,
@@ -22,24 +23,24 @@
     def __init__(
         self,
         api_key: str,
         default_model: str = 'claude-3-sonnet-20240229',
         api_endpoint: str = 'https://api.anthropic.com',
         default_max_token_len: int = 200000,
         default_max_output_len: int = 4096,
-        beta: bool = True,
+        messages_api: bool = True,
     ):
         super().__init__(
             default_model=default_model,
             api_endpoint=api_endpoint,
             default_max_token_len=default_max_token_len,
             default_max_output_len=default_max_output_len,
         )
         self.client = AsyncAnthropic(api_key=api_key, base_url=api_endpoint)
-        self.beta = beta
+        self.messages_api = messages_api
 
     def from_dict(self, message: Dict[str, Any]) -> 'Message':
         role = message['role']
         message_content = message['content']
 
         url = message['url'] if 'url' in message else ''
         content_type = message['content_type'] if 'content_type' in message else ''
@@ -77,14 +78,17 @@
         elif role == 'system':
             return System(content)
         elif role == 'assistant':
             return Assistant(content)
         raise ValueError(f'role not found or not supported: {message}')
 
     def wrap_messages(self, messages: List[Message]) -> List[Dict[str, str]]:
+        # todo: this logic is wrong -- if called from execute_direct
+        # it'll unpack the pdf/markdown but not do it properly
+        # as those functions will return multiple messages
         def wrap_message(index: int, content: Content) -> str:
             if isinstance(content, FileContent):
                 return f"<file url={content.url}>{content.get_str()}</file>"
             elif isinstance(content, PdfContent):
                 # return f"<pdf url={content.url}>{content.get_str()}</pdf>"
                 return f"<pdf url={content.url}>{ObjectTransformers.transform_pdf_content(content, self)}</pdf>"
             elif isinstance(content, MarkdownContent):
@@ -148,14 +152,23 @@
                                     "data": base64.b64encode(Helpers.anthropic_resize(messages[i].message.sequence)).decode('utf-8')  # type: ignore
                                 }
                         }]
                     })
             elif isinstance(messages[i], User) and i < len(messages) - 1:  # is not last message, context messages
                 wrapped.append({'role': 'user', 'content': wrap_message(counter, messages[i].message)})
                 counter += 1
+            elif (
+                isinstance(messages[i], User)
+                and i == len(messages) - 1
+                and (
+                    isinstance(messages[i].message, PdfContent)
+                    or isinstance(messages[i].message, ImageContent)
+                )
+            ):  # is the last message, and it's a pdf or image
+                wrapped.append({'role': 'user', 'content': wrap_message(counter, messages[i].message)})
             elif isinstance(messages[i], User) and i == len(messages) - 1:  # is the last message
                 wrapped.append({'role': 'user', 'content': messages[i].message.get_str()})
             else:
                 wrapped.append({'role': messages[i].role(), 'content': messages[i].message.get_str()})
 
         messages_list = []
 
@@ -166,27 +179,27 @@
         #         elif wrapped[i]['role'] == 'assistant':
         #             messages_list.append({'role': 'user', 'content': 'Thanks. Read for your next message.'})
         #     messages_list.append(wrapped[i])
 
         return wrapped
 
     def user_token(self):
-        if self.beta:
+        if self.messages_api:
             return 'User'
         else:
             return HUMAN_PROMPT.replace(':', '').replace('\n', '')
 
     def assistant_token(self) -> str:
-        if self.beta:
+        if self.messages_api:
             return 'Assistant'
         else:
             return AI_PROMPT.replace(':', '').replace('\n', '')
 
     def append_token(self) -> str:
-        if self.beta:
+        if self.messages_api:
             return ''
         else:
             return AI_PROMPT
 
     def count_tokens(
         self,
         messages: List[Message] | List[Dict[str, str]] | str,
@@ -231,15 +244,15 @@
                 prompt += f"""{AI_PROMPT} {message['content']}\n\n"""
             elif message['role'] == 'user':
                 prompt += f"""{HUMAN_PROMPT} {message['content']}\n\n"""
 
         prompt += f"""{AI_PROMPT}"""
         return prompt
 
-    async def __aexecute_direct(
+    async def aexecute_direct(
         self,
         messages: List[Dict[str, Any]],
         functions: List[Dict[str, str]] = [],
         model: Optional[str] = None,
         max_output_tokens: int = 2048,
         temperature: float = 0.0,
     ) -> TokenStreamManager:
@@ -301,19 +314,19 @@
         # todo, this is a busted hack. if a helper function returns nothing, then usually that
         # message get stripped away
         if messages_list[0]['role'] != 'system' and messages_list[0]['role'] != 'user':
             messages_list.insert(0, {'role': 'user', 'content': 'None.'})
 
         messages_trace(messages_list)
 
-        token_trace = TokenPerf('__aexecute_direct', 'anthropic', model, prompt_len=message_tokens)  # type: ignore
+        token_trace = TokenPerf('aexecute_direct', 'anthropic', model)  # type: ignore
         token_trace.start()
 
         try:
-            if self.beta:
+            if self.messages_api:
                 # AsyncStreamManager[AsyncMessageStream]
                 stream = self.client.messages.stream(
                     max_tokens=max_output_tokens,
                     messages=messages_list,  # type: ignore
                     model=model,
                     system=system_message,
                     temperature=temperature,
@@ -350,23 +363,32 @@
 
         # find the system message and append to the front
         system_message = last(lambda x: x.role() == 'system', messages)
 
         if not system_message:
             system_message = System(Content('You are a helpful assistant.'))
 
+        expanded_messages = []
+        for message in messages:
+            if isinstance(message, User) and isinstance(message.message, PdfContent):
+                expanded_messages.extend(ObjectTransformers.transform_pdf_content(message.message, self))
+            elif isinstance(message, User) and isinstance(message.message, MarkdownContent):
+                expanded_messages.extend(ObjectTransformers.transform_markdown_content(message.message, self))
+            else:
+                expanded_messages.append(message)
+
         # fresh message list
-        messages_list: List[Dict[str, str]] = self.wrap_messages(messages)
+        messages_list: List[Dict[str, str]] = self.wrap_messages(expanded_messages)
 
         if messages_list[0]['role'] == 'system' and messages_list[1]['role'] != 'user':
             logging.error(f'First message must be from the user after a system prompt: {messages_list}')
         elif messages_list[0]['role'] == 'assistant':
             logging.error(f'First message must be from the user, not assistant: {messages_list}')
 
-        stream = self.__aexecute_direct(
+        stream = self.aexecute_direct(
             messages_list,
             max_output_tokens=max_output_tokens,
             model=model,
             temperature=temperature,
         )
 
         text_response = ''
@@ -375,16 +397,21 @@
         async with await stream as stream_async:  # type: ignore
             async for text in stream_async:
                 await stream_handler(Content(text))
                 text_response += text
             await stream_handler(TokenStopNode())
             perf = stream_async.perf
 
-        if self.beta:
-            _ = await stream_async.get_final_message()  # type: ignore
+        if self.messages_api:
+            final_message = await stream_async.get_final_message()  # type: ignore
+            # anthropic API does the proper accounting of input/output tokens, so set them here.
+            if final_message:
+                perf._prompt_len = final_message.usage.input_tokens
+                perf._sample_len = final_message.usage.output_tokens
+                perf.object = final_message  # type: ignore
         else:
             async for completion in await stream:  # type: ignore
                 s = completion.completion
                 await stream_handler(Content(s))
                 text_response += s
             await stream_handler(TokenStopNode())
```

### Comparing `llmvm_cli-0.2.9/llmvm/common/container.py` & `llmvm_cli-0.3.0/llmvm/common/container.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/common/gemini_executor.py` & `llmvm_cli-0.3.0/llmvm/common/gemini_executor.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/common/helpers.py` & `llmvm_cli-0.3.0/llmvm/common/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from enum import Enum, IntEnum
 from functools import reduce
 from importlib import resources
 from itertools import cycle, islice
 from logging import Logger
 from typing import Any, Callable, Dict, Generator, List, Optional
 from urllib.parse import urlparse
+import zlib
 from zoneinfo import ZoneInfo
 
 import httpx
 import nest_asyncio
 import psutil
 from dateutil.relativedelta import relativedelta
 from docstring_parser import parse
@@ -401,14 +402,24 @@
 
             with Image.open(io.BytesIO(byte_stream)) as im:
                 return True
         except Exception:
             return False
 
     @staticmethod
+    def decompress_if_compressed(byte_stream):
+        try:
+            # Attempt to decompress to see if it's zlib compressed
+            decompressed_data = zlib.decompress(byte_stream)
+            return True, decompressed_data
+        except zlib.error as e:
+            # If decompression fails, it's likely not zlib compressed or the data is corrupted/incomplete
+            return False, byte_stream
+
+    @staticmethod
     def image_size(byte_stream: bytes) -> tuple[int, int]:
         try:
             if isinstance(byte_stream, io.BytesIO):
                 byte_stream = byte_stream.getvalue()
 
             with Image.open(io.BytesIO(byte_stream)) as im:
                 return im.size
```

### Comparing `llmvm_cli-0.2.9/llmvm/common/logging_helpers.py` & `llmvm_cli-0.3.0/llmvm/common/logging_helpers.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/common/mistral_executor.py` & `llmvm_cli-0.3.0/llmvm/common/mistral_executor.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/common/object_transformers.py` & `llmvm_cli-0.3.0/llmvm/common/object_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         if not content.sequence and content.is_local():
             content.sequence = open(content.url, 'rb').read()
 
         if content.original_sequence is None and Container.get_config_variable('LLMVM_FULL_PROCESSING', default=False):
             # avoid circular import
             pdf = Pdf(executor=executor)
             result = pdf.get_pdf_content(content)
-            content.original = content.sequence
+            content.original_sequence = content.sequence
             content.sequence = result
             cache.set(content.url, content)
 
             return [User(content) for content in result]
         else:
             result = PdfHelpers.parse_pdf_bytes(cast(bytes, content.sequence))
             return [User(Content(result))]
```

### Comparing `llmvm_cli-0.2.9/llmvm/common/objects.py` & `llmvm_cli-0.3.0/llmvm/common/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
 
     def b64encode(self) -> str:
         if isinstance(self.sequence, bytes):
             return base64.b64encode(self.sequence).decode('utf-8')
         elif isinstance(self.sequence, str):
             return base64.b64encode(self.sequence.encode('utf-8')).decode('utf-8')
         elif isinstance(self.sequence, list) and len(self.sequence) > 0 and isinstance(self.sequence[0], Content):
-            return base64.b64encode(self.original).decode('utf-8')
+            return base64.b64encode(self.original_sequence).decode('utf-8')  # type: ignore
         else:
             raise ValueError(f'unknown sequence: {self.sequence}')
 
     @staticmethod
     def decode(base64_str: str):
         return base64.b64decode(base64_str)
```

### Comparing `llmvm_cli-0.2.9/llmvm/common/openai_executor.py` & `llmvm_cli-0.3.0/llmvm/common/openai_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import tiktoken
 from openai import AsyncOpenAI
 from openai.types.chat import ChatCompletionMessageParam
 from openai.types.chat.completion_create_params import Function
 from PIL import Image
 
 from llmvm.common.logging_helpers import messages_trace, setup_logging
-from llmvm.common.objects import (Assistant, AstNode, Content, Executor,
-                                  Message, System, TokenStopNode, User,
+from llmvm.common.object_transformers import ObjectTransformers
+from llmvm.common.objects import (Assistant, AstNode, Content, Executor, MarkdownContent,
+                                  Message, PdfContent, System, TokenStopNode, User,
                                   awaitable_none)
 from llmvm.common.perf import TokenPerf, TokenStreamManager
 
 logging = setup_logging()
 
 class OpenAIExecutor(Executor):
     def __init__(
@@ -127,59 +128,59 @@
         return 'openai'
 
     async def __aexecute_direct(
         self,
         messages: List[Dict[str, str]],
         functions: List[Dict[str, str]] = [],
         model: Optional[str] = None,
-        max_completion_tokens: int = 4096,
+        max_output_tokens: int = 4096,
         temperature: float = 0.0,
     ) -> TokenStreamManager:
         model = model if model else self.default_model
 
         # only works if profiling or LLMVM_PROFILING is set to true
         message_tokens = self.count_tokens(messages, model=model)
-        if message_tokens > self.max_input_tokens(max_completion_tokens, model=model):
+        if message_tokens > self.max_input_tokens(max_output_tokens, model=model):
             raise Exception('Prompt too long. prompt tokens: {}, completion tokens: {}, total: {}, max context window: {}'
                             .format(message_tokens,
-                                    max_completion_tokens,
-                                    message_tokens + max_completion_tokens,
+                                    max_output_tokens,
+                                    message_tokens + max_output_tokens,
                                     self.max_tokens(model)))
 
         messages_cast = cast(List[ChatCompletionMessageParam], messages)
         functions_cast = cast(List[Function], functions)
 
         token_trace = TokenPerf('__aexecute_direct', 'openai', model, prompt_len=message_tokens)  # type: ignore
         token_trace.start()
 
         if functions:
             response = await self.aclient.chat.completions.create(
                 model=model,
                 temperature=temperature,
-                max_tokens=max_completion_tokens,
+                max_tokens=max_output_tokens,
                 functions=functions_cast,
                 messages=messages_cast,
                 stream=True
             )
             return TokenStreamManager(response, token_trace) # type: ignore
         else:
             # for whatever reason, [] functions generates an InvalidRequestError
             response = await self.aclient.chat.completions.create(
                 model=model if model else self.default_model,
                 temperature=temperature,
-                max_tokens=max_completion_tokens,
+                max_tokens=max_output_tokens,
                 messages=messages_cast,
                 stream=True
             )
         return TokenStreamManager(response, token_trace)  # type: ignore
 
     async def aexecute(
         self,
         messages: List[Message],
-        max_completion_tokens: int = 4096,
+        max_output_tokens: int = 4096,
         temperature: float = 0.0,
         model: Optional[str] = None,
         stream_handler: Callable[[AstNode], Awaitable[None]] = awaitable_none,
     ) -> Assistant:
         model = model if model else self.default_model
 
         def last(predicate, iterable):
@@ -190,24 +191,33 @@
 
         # find the system message and append to the front
         system_message = last(lambda x: x.role() == 'system', messages)
 
         if not system_message:
             system_message = System(Content('You are a helpful assistant.'))
 
+        expanded_messages = []
+        for message in messages:
+            if isinstance(message, User) and isinstance(message.message, PdfContent):
+                expanded_messages.extend(ObjectTransformers.transform_pdf_content(message.message, self))
+            elif isinstance(message, User) and isinstance(message.message, MarkdownContent):
+                expanded_messages.extend(ObjectTransformers.transform_markdown_content(message.message, self))
+            else:
+                expanded_messages.append(message)
+
         # fresh message list
         messages_list: List[Dict[str, str]] = []
 
         messages_list.append(Message.to_dict(system_message))
-        for message in [m for m in messages if m.role() != 'system']:
+        for message in [m for m in expanded_messages if m.role() != 'system']:
             messages_list.append(Message.to_dict(message))
 
         stream = self.__aexecute_direct(
             messages_list,
-            max_completion_tokens=max_completion_tokens,
+            max_output_tokens=max_output_tokens,
             model=model if model else self.default_model,
             temperature=temperature,
         )
 
         text_response = ''
 
         async with await stream as stream_async:  # type: ignore
@@ -227,17 +237,17 @@
         messages_trace(messages_list)
 
         return assistant
 
     def execute(
         self,
         messages: List[Message],
-        max_completion_tokens: int = 2048,
+        max_output_tokens: int = 2048,
         temperature: float = 0.0,
         model: Optional[str] = None,
         stream_handler: Optional[Callable[[AstNode], None]] = None,
     ) -> Assistant:
         async def stream_pipe(node: AstNode):
             if stream_handler:
                 stream_handler(node)
 
-        return asyncio.run(self.aexecute(messages, max_completion_tokens, temperature, model, stream_pipe))
+        return asyncio.run(self.aexecute(messages, max_output_tokens, temperature, model, stream_pipe))
```

### Comparing `llmvm_cli-0.2.9/llmvm/common/pdf.py` & `llmvm_cli-0.3.0/llmvm/common/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List, cast
 from urllib.parse import urlparse
 
 import pdf2image
 import pdfplumber
 import pytesseract
 from pdfminer.high_level import extract_text_to_fp
+from pdfminer.image import ImageWriter
 from PIL import Image
 from pytesseract import Output
 
 from llmvm.common.helpers import Helpers, write_client_stream
 from llmvm.common.logging_helpers import setup_logging
 from llmvm.common.objects import (Content, Executor, ImageContent, LLMCall,
                                   PdfContent, StreamNode, User)
@@ -164,20 +165,31 @@
             text = page.extract_text(x_tolerance=x_tolerance)
             if text:
                 page_content.append(Content(text))
 
             images = page.images
             for img in images:
                 raw_data = img['stream'].get_rawdata()
+                _, raw_data = Helpers.decompress_if_compressed(raw_data)
                 if Helpers.is_image(raw_data):
                     img_stream = BytesIO(img['stream'].get_rawdata())
                     im = Image.open(img_stream)
                     buf = io.BytesIO()
                     im.save(buf, format='PNG')
-                    page_content.append(ImageContent(buf.getvalue(), url=url_or_file))
+                    with tempfile.NamedTemporaryFile(suffix='.png', delete=False) as temp_file:
+                        im.save(temp_file.name, format='PNG')
+                        page_content.append(ImageContent(buf.getvalue(), url=temp_file.name))
+                else:
+                    with tempfile.NamedTemporaryFile(suffix='.png', delete=False) as temp_file:
+                        image_bbox = (img['x0'], page.height - img['y1'], img['x1'], page.height - img['y0'])
+                        page.crop(image_bbox).to_image().save(temp_file.name, format='PNG')
+                        im = Image.open(temp_file.name)
+                        buf = io.BytesIO()
+                        im.save(buf, format='PNG')
+                        page_content.append(ImageContent(buf.getvalue(), url=temp_file.name))
 
             content.extend(page_content)
 
         write_client_stream(
             StreamNode(
                 return_image.getvalue(),
                 type='bytes',
```

### Comparing `llmvm_cli-0.2.9/llmvm/common/perf.py` & `llmvm_cli-0.3.0/llmvm/common/perf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime as dt
 import inspect
 import os
 import time
-from typing import List, cast
+from typing import Any, List, Optional, cast
 
 import openai
 from anthropic import AsyncMessageStream, AsyncMessageStreamManager
 from anthropic import AsyncStream as AnthropicAsyncStream
 from anthropic.types import Completion as AnthropicCompletion
+from anthropic.types import Message as AnthropicMessage
 from google.generativeai.types.generation_types import \
     AsyncGenerateContentResponse as AsyncGeminiStream
 from google.generativeai.types.generation_types import \
     GenerateContentResponse as GeminiCompletion
 from mistralai.models.chat_completion import \
     ChatCompletionStreamResponse as MistralCompletion
 from openai.types.chat.chat_completion_chunk import \
@@ -42,19 +43,21 @@
     ):
         self._name: str = name
         self._executor: str = executor_name
         self._model: str = model_name
         self._start: float = 0.0
         self._stop: float = 0.0
         self._prompt_len: int = prompt_len
+        self._sample_len: int = 0
         self._ticks: List[float] = []
         self.enabled = enabled
         self.log_file = log_file
         self.calculator = TokenPriceCalculator()
         self.request_id = request_id
+        self.object = None
 
     def start(self):
         if self.enabled:
             self._start = time.perf_counter()
 
     def stop(self):
         if self.enabled:
@@ -85,15 +88,15 @@
                 'name': self._name,
                 'executor': self._executor,
                 'model': self._model,
                 'total_time': total_time,
                 'prompt_time': prompt_time,
                 'sample_time': sample_time,
                 'prompt_len': self._prompt_len,
-                'sample_len': len(self._ticks),
+                'sample_len': self._sample_len if self._sample_len > 0 else len(self._ticks),
                 's_tok_sec': s_tok_sec,
                 'p_tok_sec': p_tok_sec,
                 'p_cost': self._prompt_len * self.calculator.input_price(self._model, self._executor),
                 's_cost': len(self._ticks) * self.calculator.output_price(self._model, self._executor),
                 'request_id': self.request_id,
                 'ticks': self.ticks()
             }
@@ -121,15 +124,15 @@
     def debug(self):
         if self.enabled:
             res = self.result()
             # output \n to the debug stream without using logging.debug
             import sys
             sys.stderr.write('\n')
             logging.debug(f"total_time: {res['total_time']:.2f} prompt_time: {res['prompt_time']:.2f} sample_time: {res['sample_time']:.2f}")
-            logging.debug(f"prompt_len: {res['prompt_len']} sample_len: {len(res['ticks'])}")
+            logging.debug(f"prompt_len: {res['prompt_len']} sample_len: {res['sample_len']}")
             logging.debug(f"p_tok_sec: {res['p_tok_sec']:.2f} s_tok_sec: {res['s_tok_sec']:.2f}")
             logging.debug(f"p_cost: ${res['p_cost']:.5f} s_cost: ${res['s_cost']:.5f} request_id: {res['request_id']}")
 
     def log(self):
         if self.enabled:
             self.debug()
             if not os.path.exists(os.path.expanduser(self.log_file)):
@@ -192,29 +195,33 @@
     def __init__(
         self,
         original_stream,
         token_perf: 'TokenPerf'
     ):
         self.stream = original_stream
         self.perf = token_perf
+        self.object: Optional[Any] = None  # used for Anthropic's AsyncMessageStream needed for get_final_message()
 
     def __aiter__(self):
         return LoggingAsyncIterator(self.stream, self.perf)
 
     # act as a proxy to self.original_stream for any other methods that are called
     def __getattr__(self, name):
         if name == 'text_stream':
             return self
         else:
             return getattr(self.stream, name)
 
     # we're proxying the .text_stream, which doesn't have get_final_message()
     # but we don't need it as we're streaming
-    async def get_final_message(self):
-        return ''
+    async def get_final_message(self) -> Optional[AnthropicMessage]:
+        if isinstance(self.object, AsyncMessageStream):
+            return await self.object.get_final_message()
+        else:
+            return None
 
 
 class TokenStreamManager:
     def __init__(
         self,
         stream: AsyncMessageStreamManager | AnthropicAsyncStream[AnthropicCompletion] | openai.AsyncStream,  # type: ignore
         token_perf: 'TokenPerf'
@@ -230,14 +237,16 @@
             result: AsyncMessageStream = await self.stream.__aenter__()
             # special anthropic debugging
             self.perf.request_id = result.response.headers['request-id']
             if Container().get_config_variable('LLMVM_SHARE', default=''):
                 with open(os.path.expanduser(Container().get_config_variable('LLMVM_SHARE') + f'/{self.perf.request_id}.json'), 'w') as f:
                     f.write(result.response._request._content.decode('utf-8'))  # type: ignore
             self.token_perf_wrapper = TokenStreamWrapper(result.text_stream, self.perf)  # type: ignore
+            self.token_perf_wrapper.object = result
+
             return self.token_perf_wrapper
         elif isinstance(self.stream, openai.AsyncStream):
             self.token_perf_wrapper = TokenStreamWrapper(self.stream, self.perf)
             return self.token_perf_wrapper
         elif isinstance(self.stream, AsyncGeminiStream):
             self.token_perf_wrapper = TokenStreamWrapper(self.stream, self.perf)
             return self.token_perf_wrapper
```

### Comparing `llmvm_cli-0.2.9/llmvm/config.yaml` & `llmvm_cli-0.3.0/llmvm/config.yaml`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/model_prices_and_context_window.json` & `llmvm_cli-0.3.0/llmvm/model_prices_and_context_window.json`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/ast_parser.py` & `llmvm_cli-0.3.0/llmvm/server/ast_parser.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/base_library/content_downloader.py` & `llmvm_cli-0.3.0/llmvm/server/base_library/content_downloader.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/base_library/function_bindable.py` & `llmvm_cli-0.3.0/llmvm/server/base_library/function_bindable.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/base_library/searcher.py` & `llmvm_cli-0.3.0/llmvm/server/base_library/searcher.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/base_library/source.py` & `llmvm_cli-0.3.0/llmvm/server/base_library/source.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/base_library/source_project.py` & `llmvm_cli-0.3.0/llmvm/server/base_library/source_project.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/bcl.py` & `llmvm_cli-0.3.0/llmvm/server/bcl.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/persistent_cache.py` & `llmvm_cli-0.3.0/llmvm/server/persistent_cache.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer_error_correction.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_error_correction.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer_nocontext.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_nocontext.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/answer_regen_code_or_rewrite.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_regen_code_or_rewrite.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/code_get_source_summary.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/code_get_source_summary.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/coerce.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/coerce.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/document_chunk.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/document_chunk.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_error_correction.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_error_correction.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_global.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_global.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_list.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_list.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_local.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_local.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_bind_old.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_old.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_call.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_call.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/llm_loop_bind.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_loop_bind.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/map_reduce_map.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/map_reduce_map.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/map_reduce_reduce.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/map_reduce_reduce.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/pandas_bind.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/pandas_bind.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/pdf_content.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/pdf_content.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/query_understanding.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/query_understanding.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/search_classifier.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_classifier.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/search_location.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_location.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/search_ranker.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_ranker.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_code_insights.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_code_insights.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_code_prompt_old.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_code_prompt_old.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_continuation_execution.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_continuation_execution.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_error_correction.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_error_correction.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/prompts/starlark/starlark_tool_execution.prompt` & `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_tool_execution.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/server.py` & `llmvm_cli-0.3.0/llmvm/server/server.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/starlark_execution_controller.py` & `llmvm_cli-0.3.0/llmvm/server/starlark_execution_controller.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/starlark_runtime.py` & `llmvm_cli-0.3.0/llmvm/server/starlark_runtime.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/tools/browser.py` & `llmvm_cli-0.3.0/llmvm/server/tools/firefox.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,253 @@
 import asyncio
 import concurrent
 import concurrent.futures
 import datetime as dt
 import os
 import threading
 import time
-from typing import Any, Awaitable, Callable, Dict, List, cast
+from typing import Dict, List, cast
+from urllib.parse import urlparse
 
 import aiofiles
 import httpx
 import nest_asyncio
-from PIL import Image
-from playwright.async_api import Error, Page, async_playwright
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-from selenium.webdriver.firefox.options import Options as FirefoxOptions
-from selenium.webdriver.firefox.webdriver import WebDriver
-from selenium.webdriver.remote.webelement import WebElement
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.wait import WebDriverWait
-from yfinance import download
-
-from container import Container
-from helpers.helpers import Helpers, write_client_stream
-from helpers.logging_helpers import setup_logging
-from helpers.singleton import Singleton
-from objects import StreamNode
+from playwright.async_api import ElementHandle, Error, Page, async_playwright
+
+from llmvm.common.container import Container
+from llmvm.common.helpers import write_client_stream
+from llmvm.common.logging_helpers import setup_logging
+from llmvm.common.objects import StreamNode
+from llmvm.common.singleton import Singleton
 
 nest_asyncio.apply()
 logging = setup_logging()
 
+def read_netscape_cookies(cookies_txt_filename: str):
+    cookies = []
+    with open(cookies_txt_filename, 'r') as file:
+        for line in file.readlines():
+            if not line.startswith('#') and line.strip():  # Ignore comments and empty lines
+                try:
+                    domain, _, path, secure, expires_value, name, value = line.strip().split('\t')
+
+                    if int(expires_value) != -1 and int(expires_value) < 0:
+                        continue  # Skip invalid cookies
+
+                    dt_object = dt.datetime.fromtimestamp(int(expires_value))
+                    if dt_object.date() < dt.datetime.now().date():
+                        continue
+
+                    cookies.append({
+                        "name": name,
+                        "value": value,
+                        "domain": domain,
+                        "path": path,
+                        "expires": int(expires_value),
+                        "httpOnly": False,
+                        "secure": secure == "TRUE"
+                    })
+                except Exception as ex:
+                    pass
+    return cookies
+
+
+class FirefoxHelpers():
+    def __init__(self, cookies: List[Dict] = []):
+        self.loop = asyncio.SelectorEventLoop()
+        self.thread = threading.Thread(target=self._run_event_loop, daemon=True)
+        self.thread.start()
+        self.firefox = FirefoxHelpersInternal(cookies=cookies)
+
+    @staticmethod
+    async def check_installed() -> bool:
+        try:
+            playwright = await async_playwright().start()
+            browser = await playwright.firefox.launch(headless=True)
+            await browser.close()
+            return True
+        except Exception as ex:
+            logging.debug(f'FirefoxHelpers.check_installed() failed with: {ex}')
+            return False
 
-class BrowserPageInternal():
-    def __init__(self, internals: 'BrowserHelperInternal', page: Page):
-        self.internals = internals
-        self._page = page
+    def _run_event_loop(self):
+        asyncio.set_event_loop(self.loop)
+        self.loop.run_forever()
+
+    def run_in_loop(self, coro):
+        future = concurrent.futures.Future()
+
+        async def wrapped():
+            try:
+                result = await coro
+                future.set_result(result)
+            except Exception as e:
+                future.set_exception(e)
+
+        asyncio.run_coroutine_threadsafe(wrapped(), self.loop)
+        return future
+
+    def set_cookies(self, cookies: List[Dict]):
+        self.firefox.set_cookies(cookies)
+
+    async def close(self) -> None:
+        return self.run_in_loop(self.firefox.close()).result()
+
+    async def goto(self, url: str):
+        return self.run_in_loop(self.firefox.goto(url)).result()
+
+    async def wait(self, milliseconds: int) -> None:
+        return self.run_in_loop(self.firefox.wait(milliseconds)).result()
+
+    async def wait_until(self, selector: str) -> None:
+        return self.run_in_loop(self.firefox.wait_until(selector)).result()
+
+    async def wait_until_text(self, selector: str) -> None:
+        return self.run_in_loop(self.firefox.wait_until_text(selector)).result()
+
+    async def get_html(self) -> str:
+        return self.run_in_loop(self.firefox.get_html()).result()
+
+    async def screenshot(self) -> bytes:
+        return self.run_in_loop(self.firefox.screenshot()).result()
+
+    async def get_url(self, url: str):
+        result = self.run_in_loop(self.firefox.get_url(url)).result()
+        write_client_stream(
+            StreamNode(
+                obj=await self.screenshot(),
+                type='bytes',
+                metadata={'type': 'bytes', 'url': url}
+            ))
+        return result
+
+    async def pdf(self) -> str:
+        return self.run_in_loop(self.firefox.pdf()).result()
+
+    async def pdf_url(self, url: str) -> str:
+        return self.run_in_loop(self.firefox.pdf_url(url)).result()
+
+    async def clickable(self) -> List[str]:
+        return self.run_in_loop(self.firefox.clickable()).result()
+
+    async def click(self, element) -> None:
+        return self.run_in_loop(self.firefox.click(element)).result()
+
+    async def get_input_elements(self) -> List[ElementHandle]:
+        return self.run_in_loop(self.firefox.get_input_elements()).result()
+
+    async def get_clickable_elements(self) -> List[ElementHandle]:
+        return self.run_in_loop(self.firefox.get_clickable_elements()).result()
+
+    async def fill(self, element: ElementHandle, value: str) -> None:
+        return self.run_in_loop(self.firefox.fill(element, value)).result()
+
+class FirefoxHelpersInternal():
+    def __init__(self, cookies: List[Dict] = []):
+        self.prefs = {
+            "print.always_print_silent": True,
+            "print.printer_Mozilla_Save_to_PDF.print_to_file": True,
+            "print_printer": "Mozilla Save to PDF",
+            "browser.download.dir": Container().get('firefox_download_directory', default=os.path.expanduser('~')),
+            "browser.download.folderList": 2,
+            "browser.helperApps.neverAsk.saveToDisk": "text/plain, application/vnd.ms-excel, text/csv, text/comma-separated-values, application/octet-stream",
+        }
+
+        profile_directory = Container().get('firefox_profile_directory', '')
+        if os.path.exists(profile_directory):
+            self.prefs.update({"profile": profile_directory})
+
+        self.cookies = cookies
+        self._context = None
+        self._page = None
+        self.playwright = None
+        self.browser = None
+        self.wait_fors = {
+            'twitter.com': lambda page: self.wait(1500),
+            'techmeme.com': lambda page: self.wait(1500)
+        }
+
+    def set_cookies(self, cookies: List[Dict]):
+        self.cookies = cookies
+
+    async def __new_page(self, cookies: List[Dict] = []) -> Page:
+        if self.playwright is None or self.browser is None:
+            self.playwright = await async_playwright().start()
+            self.browser = await self.playwright.firefox.launch(
+                headless=Container().get('firefox_headless', default=True),
+                firefox_user_prefs=self.prefs
+            )
+
+        self._context = await self.browser.new_context(accept_downloads=True)
+        cookie_file = Container().get('firefox_cookies', '')
+        if os.path.exists(cookie_file):
+            result = read_netscape_cookies(cookie_file)
+            await self._context.add_cookies(result)
+
+        if self.cookies:
+            await self._context.add_cookies(self.cookies)  # type: ignore
+        return await self._context.new_page()
 
     async def page(self) -> Page:
-        return self._page  # type: ignore
+        if self._page is None:
+            self._page = await self.__new_page()
+            return self._page
+        else:
+            return cast(Page, self._page)
+
+    async def close(self) -> None:
+        if self._page is not None:
+            await (await self.page()).close()
+        if self.browser is not None:
+            await self.browser.close()
 
     async def goto(self, url: str):
         try:
             if (await self.page()).url != url:
                 await (await self.page()).goto(url)
-        except Error as ex:
+
+                domain = urlparse(url).netloc
+                if domain in self.wait_fors:
+                    wait_for_lambda = self.wait_fors[domain]
+                    await wait_for_lambda(await self.page())
+
+        except Error as _:
             # try new page
-            self._page = await self.internals.page()
+            self._page = await self.__new_page()
             await (await self.page()).goto(url)
 
-    async def set_cookies(self, cookies: List[Dict[str, Any]]):
-        await (await self.page()).context.add_cookies(cookies)  # type: ignore
-
     async def wait(self, milliseconds: int) -> None:
         await (await self.page()).evaluate("() => { setTimeout(function() { return; }, 0); }")
         await (await self.page()).wait_for_timeout(milliseconds)
 
     async def wait_until(self, selector: str) -> None:
         element = await (await self.page()).wait_for_selector(selector)
 
     async def wait_until_text(self, selector: str) -> None:
         element = await (await self.page()).wait_for_selector(f'*:has-text("{selector}")', timeout=5000)
 
     async def get_html(self) -> str:
         return await (await self.page()).content()
 
     async def screenshot(self) -> bytes:
-        screenshot_data = await (await self.page()).screenshot(type='png')
-        return screenshot_data
+        try:
+            return await asyncio.wait_for((await self.page()).screenshot(type='png'), timeout=2)
+        except asyncio.TimeoutError as ex:
+            logging.debug(f'screenshot timed out with: {ex}')
+            return b''
 
     async def get_url(self, url: str):
         await self.goto(url)
 
         try:
             html = await self.get_html()
             return html
         except Error as ex:
             # try new page
-            self._page = await self.internals.page()
+            self._page = await self.__new_page()
             await self.goto(url)
             await self._page.wait_for_load_state('networkidle')
             html = await self.get_html()
             return html
 
     async def pdf(self) -> str:
         await (await self.page()).evaluate("() => { setTimeout(function() { return; }, 0); }")
@@ -158,135 +325,21 @@
         for element in clickable_elements:
             unique_ids.add(element)
         return list(unique_ids)
 
     async def click(self, element) -> None:
         await element.click()
 
-    async def close(self) -> None:
-        await (await self.page()).close()
-        self._page = None
-
-
-class BrowserHelperInternal(metaclass=Singleton):
-    def __init__(self):
-        self.prefs = {
-            "print.always_print_silent": True,
-            "print.printer_Mozilla_Save_to_PDF.print_to_file": True,
-            "print_printer": "Mozilla Save to PDF",
-            "browser.download.dir": Container().get('browser_download_directory', default=os.path.expanduser('~')),
-            "browser.download.folderList": 2,
-            "browser.helperApps.neverAsk.saveToDisk": "text/plain, application/vnd.ms-excel, text/csv, text/comma-separated-values, application/octet-stream",
-        }
-
-        self._context = None
-        self.playwright = None
-        self.browser = None
-        self.init_lock = asyncio.Lock()
-
-    async def initialize_browser(self):
-        async with self.init_lock:
-            self.playwright = await async_playwright().start()
-            self.browser = await self.playwright.firefox.launch(
-                headless=Container().get('browser_headless', default=False),
-                firefox_user_prefs=self.prefs
-            )
-
-            self._context = await self.browser.new_context(accept_downloads=True)
-            cookie_file = Container().get('browser_cookies', '')
-            if os.path.exists(cookie_file):
-                result = Helpers.read_netscape_cookies(open(cookie_file, 'r').read())
-                await self._context.add_cookies(result)  # type: ignore
-
-    async def page(self) -> Page:
-        await self.initialize_browser()
-        context = await self.browser.new_context(accept_downloads=True)  # type: ignore
-        page = await context.new_page()
-        return page
-
-    async def browser_page(self) -> 'BrowserPageInternal':
-        await self.initialize_browser()
-        return BrowserPageInternal(self, await self.page())
-
-
-class BrowserHelper(metaclass=Singleton):
-    _is_initialized = False
-
-    def __init__(self):
-        if not self._is_initialized:
-            self.loop = asyncio.SelectorEventLoop()
-            self.thread = threading.Thread(target=self._run_event_loop, daemon=True)
-            self.thread.start()
-            self.firefox = BrowserHelperInternal()
-            BrowserHelper._is_initialized = True
-
-    def _run_event_loop(self):
-        asyncio.set_event_loop(self.loop)
-        self.loop.run_forever()
-
-    def run_in_loop(self, coro):
-        future = concurrent.futures.Future()
-
-        async def wrapped():
-            try:
-                result = await coro
-                future.set_result(result)
-            except Exception as e:
-                future.set_exception(e)
-
-        asyncio.run_coroutine_threadsafe(wrapped(), self.loop)
-        return future
-
-    def browser_page(self, cookies_file_content: str = '') -> 'BrowserPage':
-        return BrowserPage(self)
-
-
-class BrowserPage():
-    def __init__(self, browser_helper: BrowserHelper):
-        self.helper = browser_helper
-        self.browser_page = BrowserPageInternal(self.helper.firefox, self.helper.run_in_loop(self.helper.firefox.page()).result())
-
-    async def goto(self, url: str):
-        return self.helper.run_in_loop(self.browser_page.goto(url)).result()
-
-    async def wait(self, milliseconds: int) -> None:
-        return self.helper.run_in_loop(self.browser_page.wait(milliseconds)).result()
-
-    async def wait_until(self, selector: str) -> None:
-        return self.helper.run_in_loop(self.browser_page.wait_until(selector)).result()
-
-    async def wait_until_text(self, selector: str) -> None:
-        return self.helper.run_in_loop(self.browser_page.wait_until_text(selector)).result()
-
-    async def get_html(self) -> str:
-        return self.helper.run_in_loop(self.browser_page.get_html()).result()
-
-    async def screenshot(self) -> bytes:
-        return self.helper.run_in_loop(self.browser_page.screenshot()).result()
-
-    async def set_cookies(self, cookies: List[Dict[str, Any]]):
-        return self.helper.run_in_loop(self.browser_page.set_cookies(cookies)).result()
-
-    async def get_url(self, url: str):
-        result = self.helper.run_in_loop(self.browser_page.get_url(url)).result()
-        write_client_stream(
-            StreamNode(
-                obj=await self.screenshot(),
-                type='bytes',
-                metadata={'type': 'bytes', 'url': url}
-            ))
-        return result
-
-    async def pdf(self) -> str:
-        return self.helper.run_in_loop(self.browser_page.pdf()).result()
-
-    async def pdf_url(self, url: str) -> str:
-        return self.helper.run_in_loop(self.browser_page.pdf_url(url)).result()
-
-    async def clickable(self) -> List[str]:
-        return self.helper.run_in_loop(self.browser_page.clickable()).result()
+    async def get_clickable_elements(self) -> List[ElementHandle]:
+        clickable_elements = await (await self.page()).query_selector_all(
+            "a, button, input[type='submit'], input[type='button']"
+        )
+        return clickable_elements
 
-    async def click(self, element) -> None:
-        return self.helper.run_in_loop(self.browser_page.click(element)).result()
+    async def get_input_elements(self) -> List[ElementHandle]:
+        input_elements = await (await self.page()).query_selector_all(
+            "input[type='text'], input[type='email'], input[type='password'], textarea"
+        )
+        return input_elements
 
-    async def close(self) -> None:
-        return self.helper.run_in_loop(self.browser_page.close()).result()
+    async def fill(self, element: ElementHandle, value: str) -> None:
+        await element.fill(value)
```

### Comparing `llmvm_cli-0.2.9/llmvm/server/tools/edgar.py` & `llmvm_cli-0.3.0/llmvm/server/tools/edgar.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/tools/market.py` & `llmvm_cli-0.3.0/llmvm/server/tools/market.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/tools/scraper.py` & `llmvm_cli-0.3.0/llmvm/server/tools/scraper.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/tools/search.py` & `llmvm_cli-0.3.0/llmvm/server/tools/search.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/tools/search_hn.py` & `llmvm_cli-0.3.0/llmvm/server/tools/search_hn.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/tools/webhelpers.py` & `llmvm_cli-0.3.0/llmvm/server/tools/webhelpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,26 @@
 from llmvm.common.logging_helpers import setup_logging
 from llmvm.common.objects import Content, MarkdownContent
 from llmvm.server.tools.firefox import FirefoxHelpers
 from llmvm.server.tools.search import SerpAPISearcher
 
 logging = setup_logging()
 
-class IgnoringScriptConverter(MarkdownConverter):
+class VerboseConverter(MarkdownConverter):
     def convert_script(self, el, text, convert_as_inline):
         return ''
 
+    def convert_input(self, el, text, convert_as_inline):
+        return str(el)
+
+    def convert_textarea(self, el, text, convert_as_inline):
+        return str(el)
+
+    def convert_label(self, el, text, convert_as_inline):
+        return str(el)
 
 class WebHelpers():
     @staticmethod
     def convert_html_to_markdown(html: str, url: str = '') -> MarkdownContent:
         def clean_markdown(markdown_text: str) -> str:
             lines = []
             blank_counter = 0
@@ -57,15 +65,15 @@
 
         logging.debug(f'WebHelpers.convert_html_to_markdown_soup: {html[:25]}')
         soup = BeautifulSoup(html, features='lxml')
 
         for data in soup(['style', 'script']):
             data.decompose()
 
-        result = IgnoringScriptConverter().convert_soup(soup)
+        result = VerboseConverter().convert_soup(soup)
         cleaned_result = clean_markdown(result)
         return MarkdownContent(sequence=unicodedata.normalize('NFKD', cleaned_result), url=url)
 
     @staticmethod
     def get_linkedin_profile(linkedin_url: str) -> str:
         from llmvm.common.pdf import PdfHelpers
         """Extracts the career information from a person's LinkedIn profile from a given LinkedIn url"""
```

### Comparing `llmvm_cli-0.2.9/llmvm/server/vector_search.py` & `llmvm_cli-0.3.0/llmvm/server/vector_search.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/llmvm/server/vector_store.py` & `llmvm_cli-0.3.0/llmvm/server/vector_store.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.2.9/pyproject.toml` & `llmvm_cli-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llmvm-cli"
-version = "0.2.9"
+version = "0.3.0"
 description = "Command Line LLM with client-side tools support."
 authors = ["9600 devs <contact@9600.dev>"]
 readme = "README.md"
 packages = [ {include = "llmvm"} ]
 include = ["llmvm/client/awesome_prompts.csv", "llmvm/model_prices_and_context_window.json", "llmvm/server/prompts/**/*", "llmvm/config.yaml"]
 homepage = "https://github.com/9600dev/llmvm"
 repository = "https://github.com/9600dev/llmvm"
```

### Comparing `llmvm_cli-0.2.9/PKG-INFO` & `llmvm_cli-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmvm-cli
-Version: 0.2.9
+Version: 0.3.0
 Summary: Command Line LLM with client-side tools support.
 Home-page: https://github.com/9600dev/llmvm
 Author: 9600 devs
 Author-email: contact@9600.dev
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

