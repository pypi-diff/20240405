# Comparing `tmp/r2r-0.1.29.tar.gz` & `tmp/r2r-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.1.29.tar", max compression
+gzip compressed data, was "r2r-0.1.31.tar", max compression
```

## Comparing `r2r-0.1.29.tar` & `r2r-0.1.31.tar`

### file list

```diff
@@ -1,85 +1,87 @@
--rw-r--r--   0        0        0     1082 2024-04-04 17:32:45.964493 r2r-0.1.29/LICENSE.md
--rw-r--r--   0        0        0     6625 2024-04-04 17:32:45.964493 r2r-0.1.29/README.md
--rw-r--r--   0        0        0      680 2024-04-04 17:32:45.964493 r2r-0.1.29/config.json
--rw-r--r--   0        0        0     2252 2024-04-04 17:32:45.980493 r2r-0.1.29/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/__init__.py
--rw-r--r--   0        0        0       53 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/client/__init__.py
--rw-r--r--   0        0        0     5956 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/client/base.py
--rw-r--r--   0        0        0     1123 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/__init__.py
--rw-r--r--   0        0        0      110 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      781 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/abstractions/output.py
--rw-r--r--   0        0        0      249 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/adapters/__init__.py
--rw-r--r--   0        0        0     2928 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/adapters/advanced/reducto.py
--rw-r--r--   0        0        0     2797 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/adapters/base.py
--rw-r--r--   0        0        0     2407 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/embedding.py
--rw-r--r--   0        0        0     1334 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/eval.py
--rw-r--r--   0        0        0     2175 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/ingestion.py
--rw-r--r--   0        0        0     1515 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/pipeline.py
--rw-r--r--   0        0        0     6227 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/rag.py
--rw-r--r--   0        0        0      935 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/embedding.py
--rw-r--r--   0        0        0      789 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/eval.py
--rw-r--r--   0        0        0     1773 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/llm.py
--rw-r--r--   0        0        0    11873 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/logging.py
--rw-r--r--   0        0        0     1249 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/prompt.py
--rw-r--r--   0        0        0     3833 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/vector_db.py
--rw-r--r--   0        0        0      256 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      176 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/utils/base.py
--rw-r--r--   0        0        0       95 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66651 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      203 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     1676 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/embeddings/modal/base.py
--rw-r--r--   0        0        0     3311 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/embeddings/openai/base.py
--rw-r--r--   0        0        0     1923 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/embeddings/setence_transformer/base.py
--rw-r--r--   0        0        0      139 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/eval/deepeval/base.py
--rw-r--r--   0        0        0     2676 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/eval/parea/base.py
--rw-r--r--   0        0        0        0 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/clients/__init__.py
--rw-r--r--   0        0        0     3135 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/clients/run_basic_client.py
--rw-r--r--   0        0        0     4063 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/clients/run_basic_client_old.py
--rw-r--r--   0        0        0     1625 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/clients/run_synthetic_query_client.py
--rw-r--r--   0        0        0   802904 2024-04-04 17:32:45.988493 r2r-0.1.29/r2r/examples/data/meditations.pdf
--rw-r--r--   0        0        0    14812 2024-04-04 17:32:45.988493 r2r-0.1.29/r2r/examples/data/test.pdf
--rw-r--r--   0        0        0  1307590 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/data/the_republic.pdf
--rw-r--r--   0        0        0        0 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/__init__.py
--rw-r--r--   0        0        0      526 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/basic_pipeline.py
--rw-r--r--   0        0        0      533 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/reducto_pipeline.py
--rw-r--r--   0        0        0     6746 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/synthetic_query_pipeline.py
--rw-r--r--   0        0        0      504 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/web_search_pipeline.py
--rw-r--r--   0        0        0      101 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/integrations/exa.py
--rw-r--r--   0        0        0     1184 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3905 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/integrations/serper.py
--rw-r--r--   0        0        0      276 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3602 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/litellm/base.py
--rw-r--r--   0        0        0     4419 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/llamacpp/base.py
--rw-r--r--   0        0        0        0 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/llamacpp/model/__init__.py
--rw-r--r--   0        0        0     3794 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/openai/base.py
--rw-r--r--   0        0        0      217 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/__init__.py
--rw-r--r--   0        0        0    16236 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/app.py
--rw-r--r--   0        0        0     4966 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/factory.py
--rw-r--r--   0        0        0     3280 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/models.py
--rw-r--r--   0        0        0    10797 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/utils.py
--rw-r--r--   0        0        0      541 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/__init__.py
--rw-r--r--   0        0        0     5948 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/embedding.py
--rw-r--r--   0        0        0     1767 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/eval.py
--rw-r--r--   0        0        0     2978 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/ingestion.py
--rw-r--r--   0        0        0     1002 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/prompt_provider.py
--rw-r--r--   0        0        0     3079 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/rag.py
--rw-r--r--   0        0        0     2392 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/web_search/rag.py
--rw-r--r--   0        0        0     6035 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/tests/end_to_end.py
--rw-r--r--   0        0        0    14812 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/tests/test.pdf
--rw-r--r--   0        0        0      539 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3269 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5299 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     9298 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/client.py
--rw-r--r--   0        0        0    35441 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/exc.py
--rw-r--r--   0        0        0      166 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     5881 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vector_dbs/local/base.py
--rw-r--r--   0        0        0     5607 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vector_dbs/pg_vector/base.py
--rw-r--r--   0        0        0     7125 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vector_dbs/qdrant/base.py
--rw-r--r--   0        0        0     9094 1970-01-01 00:00:00.000000 r2r-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-05 21:53:39.847457 r2r-0.1.31/LICENSE.md
+-rw-r--r--   0        0        0     6828 2024-04-05 21:53:39.847457 r2r-0.1.31/README.md
+-rw-r--r--   0        0        0      680 2024-04-05 21:53:39.847457 r2r-0.1.31/config.json
+-rw-r--r--   0        0        0     2252 2024-04-05 21:53:39.883458 r2r-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/client/__init__.py
+-rw-r--r--   0        0        0     5956 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/client/base.py
+-rw-r--r--   0        0        0     1123 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      781 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/abstractions/output.py
+-rw-r--r--   0        0        0      249 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2928 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/adapters/advanced/reducto.py
+-rw-r--r--   0        0        0     2797 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/adapters/base.py
+-rw-r--r--   0        0        0     2407 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/embedding.py
+-rw-r--r--   0        0        0     1334 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/eval.py
+-rw-r--r--   0        0        0     2175 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/ingestion.py
+-rw-r--r--   0        0        0     1515 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/pipeline.py
+-rw-r--r--   0        0        0     6227 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/rag.py
+-rw-r--r--   0        0        0      935 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/embedding.py
+-rw-r--r--   0        0        0     1015 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/eval.py
+-rw-r--r--   0        0        0     1808 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/llm.py
+-rw-r--r--   0        0        0    11873 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/logging.py
+-rw-r--r--   0        0        0     1249 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/prompt.py
+-rw-r--r--   0        0        0     3833 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/vector_db.py
+-rw-r--r--   0        0        0      256 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/utils/base.py
+-rw-r--r--   0        0        0       95 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66651 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      203 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     1676 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/embeddings/modal/base.py
+-rw-r--r--   0        0        0     3311 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/embeddings/openai/base.py
+-rw-r--r--   0        0        0     1923 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/embeddings/setence_transformer/base.py
+-rw-r--r--   0        0        0      139 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2169 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/eval/deepeval/base.py
+-rw-r--r--   0        0        0     2707 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/eval/parea/base.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/clients/__init__.py
+-rw-r--r--   0        0        0     3244 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/clients/run_basic_client.py
+-rw-r--r--   0        0        0     4249 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/clients/run_basic_client_old.py
+-rw-r--r--   0        0        0     1625 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/clients/run_synthetic_query_client.py
+-rw-r--r--   0        0        0      689 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/configs/local_llama_cpp.json
+-rw-r--r--   0        0        0      687 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/configs/local_ollama.json
+-rw-r--r--   0        0        0   802904 2024-04-05 21:53:39.887458 r2r-0.1.31/r2r/examples/data/meditations.pdf
+-rw-r--r--   0        0        0    14812 2024-04-05 21:53:39.887458 r2r-0.1.31/r2r/examples/data/test.pdf
+-rw-r--r--   0        0        0  1307590 2024-04-05 21:53:39.891458 r2r-0.1.31/r2r/examples/data/the_republic.pdf
+-rw-r--r--   0        0        0        0 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0     1223 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/basic_pipeline.py
+-rw-r--r--   0        0        0      533 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/reducto_pipeline.py
+-rw-r--r--   0        0        0     6746 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/synthetic_query_pipeline.py
+-rw-r--r--   0        0        0      504 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/web_search_pipeline.py
+-rw-r--r--   0        0        0      101 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1184 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3905 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      277 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3602 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/litellm/base.py
+-rw-r--r--   0        0        0     4467 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/llama_cpp/base.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/llama_cpp/model/__init__.py
+-rw-r--r--   0        0        0     3794 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/openai/base.py
+-rw-r--r--   0        0        0      217 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/__init__.py
+-rw-r--r--   0        0        0    16236 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/app.py
+-rw-r--r--   0        0        0     5108 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/factory.py
+-rw-r--r--   0        0        0     3280 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/models.py
+-rw-r--r--   0        0        0    10797 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/utils.py
+-rw-r--r--   0        0        0      541 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/__init__.py
+-rw-r--r--   0        0        0     5948 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/embedding.py
+-rw-r--r--   0        0        0     1827 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/eval.py
+-rw-r--r--   0        0        0     2978 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/ingestion.py
+-rw-r--r--   0        0        0     1002 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/prompt_provider.py
+-rw-r--r--   0        0        0     3079 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/rag.py
+-rw-r--r--   0        0        0     2392 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/web_search/rag.py
+-rw-r--r--   0        0        0     6035 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/tests/end_to_end.py
+-rw-r--r--   0        0        0    14812 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/tests/test.pdf
+-rw-r--r--   0        0        0      539 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3269 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5299 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9298 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/client.py
+-rw-r--r--   0        0        0    35441 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      166 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     5881 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vector_dbs/local/base.py
+-rw-r--r--   0        0        0     5607 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vector_dbs/pg_vector/base.py
+-rw-r--r--   0        0        0     7125 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vector_dbs/qdrant/base.py
+-rw-r--r--   0        0        0     9297 1970-01-01 00:00:00.000000 r2r-0.1.31/PKG-INFO
```

### Comparing `r2r-0.1.29/LICENSE.md` & `r2r-0.1.31/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/README.md` & `r2r-0.1.31/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 
 [`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This **client script** should be executed subsequent to the server startup above. It facilitates the upload of text entries and PDFs to the server using the Python client and demonstrates the management of document and user-level vectors through its built-in features.
 
    ```bash
    # run the client
    python -m r2r.examples.clients.run_basic_client
    ```
+### Running Basic Local RAG
+
+[Refer here](https://r2r-docs.sciphi.ai/tutorials/local-rag) for a tutorial on how to modify the commands above to use local providers.
 
 ## Synthetic Queries Example
 
 [`synthetic_query_pipeline.py`](r2r/examples/servers/synthetic_query_pipeline.py): Execute this script to start a backend server equipped with an advanced pipeline. This pipeline is designed to create synthetic queries, enhancing the RAG system's learning and performance.
 
    ```bash
    # launch the server
@@ -96,15 +99,15 @@
 [`run_synthetic_query_client.py`](r2r/examples/clients/run_synthetic_query_client.py): Use this client script after the synthetic query pipeline is running. It's tailored for use with the synthetic query pipeline, demonstrating the improved features of the RAG system.
 
    ```bash
    # run the client
    python -m r2r.examples.clients.run_synthetic_query_client
    ```
 
-## Extras Examples
+## Extra Examples
 
 [`reducto_pipeline.py`](r2r/examples/servers/reducto_pipeline.py): Launch this script to activate a backend server that integrates a Reducto adapter for enhanced PDF ingestion.
 
    ```bash
    # launch the server
    python -m r2r.examples.servers.reducto_pipeline
    ```
@@ -116,16 +119,16 @@
    python -m r2r.examples.servers.web_search_pipeline
    ```
 
 ## Core Abstractions
 
 The framework primarily revolves around three core abstractions:
 
-- The **Ingestion Pipeline**: Facilitates the preparation of embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.). The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/ingestion).
+- The **Ingestion Pipeline**: Facilitates the preparation of embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.). The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/deep-dive/ingestion).
 
-- The **Embedding Pipeline**: Manages the transformation of text into stored vector embeddings, interacting with embedding and vector database providers through a series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks, etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/embedding.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/embedding).
+- The **Embedding Pipeline**: Manages the transformation of text into stored vector embeddings, interacting with embedding and vector database providers through a series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks, etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/embedding.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/deep-dive/embedding).
 
-- The **RAG Pipeline**: Works similarly to the embedding pipeline but incorporates an LLM provider to produce text completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/rag.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/rag).
+- The **RAG Pipeline**: Works similarly to the embedding pipeline but incorporates an LLM provider to produce text completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/rag.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/deep-dive/rag).
 
-- The **Eval Pipeline**: Samples some subset of rag_completion calls for evaluation. Currently [DeepEval](https://github.com/confident-ai/deepeval) is supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/eval).
+- The **Eval Pipeline**: Samples some subset of rag_completion calls for evaluation. Currently [DeepEval](https://github.com/confident-ai/deepeval) and [Parea](https://github.com/parea-ai/parea-sdk-py) are supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/deep-dive/eval).
 
 Each pipeline incorporates a logging database for operation tracking and observability.
```

#### html2text {}

```diff
@@ -34,46 +34,50 @@
 encompasses ingestion, embedding, and RAG processes, all accessible via
 FastAPI. ```bash # launch the server python -
 m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
 clients/run_basic_client.py): This **client script** should be executed
 subsequent to the server startup above. It facilitates the upload of text
 entries and PDFs to the server using the Python client and demonstrates the
 management of document and user-level vectors through its built-in features.
-```bash # run the client python -m r2r.examples.clients.run_basic_client ``` ##
-Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/examples/servers/
-synthetic_query_pipeline.py): Execute this script to start a backend server
-equipped with an advanced pipeline. This pipeline is designed to create
-synthetic queries, enhancing the RAG system's learning and performance. ```bash
-# launch the server python -m r2r.examples.servers.synthetic_query_pipeline ```
+```bash # run the client python -m r2r.examples.clients.run_basic_client ```
+### Running Basic Local RAG [Refer here](https://r2r-docs.sciphi.ai/tutorials/
+local-rag) for a tutorial on how to modify the commands above to use local
+providers. ## Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/
+examples/servers/synthetic_query_pipeline.py): Execute this script to start a
+backend server equipped with an advanced pipeline. This pipeline is designed to
+create synthetic queries, enhancing the RAG system's learning and performance.
+```bash # launch the server python -
+m r2r.examples.servers.synthetic_query_pipeline ```
 [`run_synthetic_query_client.py`](r2r/examples/clients/
 run_synthetic_query_client.py): Use this client script after the synthetic
 query pipeline is running. It's tailored for use with the synthetic query
 pipeline, demonstrating the improved features of the RAG system. ```bash # run
 the client python -m r2r.examples.clients.run_synthetic_query_client ``` ##
-Extras Examples [`reducto_pipeline.py`](r2r/examples/servers/
+Extra Examples [`reducto_pipeline.py`](r2r/examples/servers/
 reducto_pipeline.py): Launch this script to activate a backend server that
 integrates a Reducto adapter for enhanced PDF ingestion. ```bash # launch the
 server python -m r2r.examples.servers.reducto_pipeline ```
 [`web_search_pipeline.py`](r2r/examples/servers/web_search_pipeline.py): This
 script sets up a backend server that includes a `WebSearchRAGPipeline`, adding
 web search functionality to your RAG setup. ```bash # launch the server python
 -m r2r.examples.servers.web_search_pipeline ``` ## Core Abstractions The
 framework primarily revolves around three core abstractions: - The **Ingestion
 Pipeline**: Facilitates the preparation of embeddable 'Documents' from various
 data formats (json, txt, pdf, html, etc.). The abstraction can be found in
 [`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is
-available [here](https://r2r-docs.sciphi.ai/core-features/ingestion). - The
+available [here](https://r2r-docs.sciphi.ai/deep-dive/ingestion). - The
 **Embedding Pipeline**: Manages the transformation of text into stored vector
 embeddings, interacting with embedding and vector database providers through a
 series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks,
 etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/
 embedding.py) and relevant documentation is available [here](https://r2r-
-docs.sciphi.ai/core-features/embedding). - The **RAG Pipeline**: Works
-similarly to the embedding pipeline but incorporates an LLM provider to produce
-text completions. The abstraction can be found in [`rag.py`](r2r/core/
-pipelines/rag.py) and relevant documentation is available [here](https://r2r-
-docs.sciphi.ai/core-features/rag). - The **Eval Pipeline**: Samples some subset
-of rag_completion calls for evaluation. Currently [DeepEval](https://
-github.com/confident-ai/deepeval) is supported. The abstraction can be found in
-[`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available
-[here](https://r2r-docs.sciphi.ai/core-features/eval). Each pipeline
-incorporates a logging database for operation tracking and observability.
+docs.sciphi.ai/deep-dive/embedding). - The **RAG Pipeline**: Works similarly to
+the embedding pipeline but incorporates an LLM provider to produce text
+completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/
+rag.py) and relevant documentation is available [here](https://r2r-
+docs.sciphi.ai/deep-dive/rag). - The **Eval Pipeline**: Samples some subset of
+rag_completion calls for evaluation. Currently [DeepEval](https://github.com/
+confident-ai/deepeval) and [Parea](https://github.com/parea-ai/parea-sdk-py)
+are supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/
+eval.py) and relevant documentation is available [here](https://r2r-
+docs.sciphi.ai/deep-dive/eval). Each pipeline incorporates a logging database
+for operation tracking and observability.
```

### Comparing `r2r-0.1.29/config.json` & `r2r-0.1.31/config.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/pyproject.toml` & `r2r-0.1.31/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "r2r"
-version = "0.1.29"
+version = "0.1.31"
 description = "SciPhi R2R"
 authors = ["Owen Colegrove <owen@sciphi.ai>"]
 license = "MIT"
 readme = "README.md"
 include = ["config.json"]
 
 [tool.poetry.dependencies]
```

### Comparing `r2r-0.1.29/r2r/client/base.py` & `r2r-0.1.31/r2r/client/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/__init__.py` & `r2r-0.1.31/r2r/core/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/abstractions/output.py` & `r2r-0.1.31/r2r/core/abstractions/output.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/adapters/advanced/reducto.py` & `r2r-0.1.31/r2r/core/adapters/advanced/reducto.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/adapters/base.py` & `r2r-0.1.31/r2r/core/adapters/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/pipelines/embedding.py` & `r2r-0.1.31/r2r/core/pipelines/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/pipelines/eval.py` & `r2r-0.1.31/r2r/core/pipelines/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/pipelines/ingestion.py` & `r2r-0.1.31/r2r/core/pipelines/ingestion.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/pipelines/pipeline.py` & `r2r-0.1.31/r2r/core/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/pipelines/rag.py` & `r2r-0.1.31/r2r/core/pipelines/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/providers/embedding.py` & `r2r-0.1.31/r2r/core/providers/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/providers/eval.py` & `r2r-0.1.31/r2r/core/providers/eval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import random
 from abc import ABC, abstractmethod
-from typing import Optional
+from typing import Optional, Union
 
 
 class EvalProvider(ABC):
-    providers = ["deepeval", "parea"]
+    providers = ["deepeval", "parea", "none"]
 
     def __init__(self, provider: str, sampling_fraction: float = 1.0):
         if provider not in self.providers:
             raise ValueError(f"Provider {provider} not supported.")
+        if provider == "none" and sampling_fraction != 0.0:
+            raise ValueError(
+                f"Sampling fraction must be 0.0 when setting evaluation provider to None."
+            )
+
         self.provider = provider
         self.sampling_fraction = sampling_fraction
 
     def evaluate(
         self, query: str, context: str, completion: str
     ) -> Optional[dict]:
         if random.random() < self.sampling_fraction:
-            return self.evaluate(query, context, completion)
+            return self._evaluate(query, context, completion)
         return None
 
     @abstractmethod
     def _evaluate(
         self, query: str, context: str, completion: str
-    ) -> dict[str, dict[str, str]]:
+    ) -> dict[str, dict[str, Union[str, float]]]:
         pass
```

### Comparing `r2r-0.1.29/r2r/core/providers/llm.py` & `r2r-0.1.31/r2r/core/providers/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     skip_special_tokens: bool = False
     stop_token: Optional[str] = None
     num_beams: int = 1
     do_sample: bool = True
     # Additional args to pass to the generation config
     add_generation_kwargs: dict = field(default_factory=dict)
     generate_with_chat: bool = False
+    api_base: Optional[str] = None
 
 
 class LLMProvider(ABC):
     """An abstract class to provide a common interface for LLMs."""
 
     def __init__(
         self,
```

### Comparing `r2r-0.1.29/r2r/core/providers/logging.py` & `r2r-0.1.31/r2r/core/providers/logging.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/providers/prompt.py` & `r2r-0.1.31/r2r/core/providers/prompt.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/providers/vector_db.py` & `r2r-0.1.31/r2r/core/providers/vector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/core/utils/splitter/text.py` & `r2r-0.1.31/r2r/core/utils/splitter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/embeddings/modal/base.py` & `r2r-0.1.31/r2r/embeddings/modal/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/embeddings/openai/base.py` & `r2r-0.1.31/r2r/embeddings/openai/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/embeddings/setence_transformer/base.py` & `r2r-0.1.31/r2r/embeddings/setence_transformer/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/eval/deepeval/base.py` & `r2r-0.1.31/r2r/eval/deepeval/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/eval/parea/base.py` & `r2r-0.1.31/r2r/eval/parea/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import Union
 
 from r2r.core.providers.eval import EvalProvider
 
 
 class PareaEvalProvider(EvalProvider):
     def __init__(self, provider: str, sampling_fraction: float = 1.0):
         super().__init__(provider, sampling_fraction)
@@ -41,15 +42,15 @@
         if not os.getenv("OPENAI_API_KEY"):
             raise ValueError(
                 "Please set the `OPENAI_API_KEY` environment variable to run with Parea."
             )
 
     def _evaluate(
         self, query: str, context: str, completion: str
-    ) -> dict[str, dict[str, str | float]]:
+    ) -> dict[str, dict[str, Union[str, float]]]:
         log = self._create_log(query, context, completion)
 
         answer_relevancy_score = self.answer_relevancy(log)
         context_query_relevancy_score = self.context_query_relevancy(log)
         context_ranking_pointwise_score = self.context_ranking_pointwise(log)
         answer_context_faithfulness_statement_level_score = (
             self.answer_context_faithfulness_statement_level(log)
```

### Comparing `r2r-0.1.29/r2r/examples/clients/run_basic_client.py` & `r2r-0.1.31/r2r/examples/clients/run_basic_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import glob
 import os
-import uuid
 
 import fire
 
 from r2r.client import R2RClient
 from r2r.core.utils import generate_id_from_label
 
 
@@ -19,15 +18,14 @@
             # uncomment the following line to add more documents
             # "the_republic.pdf": "Title: The Republic - Plato",
         }
 
     def ingest(self):
         current_file_directory = os.path.dirname(os.path.abspath(__file__))
         data_path = os.path.join(current_file_directory, "..", "data")
-
         for file_path in glob.glob(os.path.join(data_path, "*.pdf")):
             file_name = file_path.split(os.path.sep)[-1]
             if file_name in self.titles:
                 document_id = generate_id_from_label(file_path)
                 metadata = {
                     "user_id": self.user_id,
                     "chunk_prefix": self.titles[file_name],
@@ -47,29 +45,30 @@
         for i, response in enumerate(search_response):
             text = response["metadata"]["text"]
             title, body = text.split("\n", 1)
             print(f"Result {i + 1}: {title}")
             print(body[:500])
             print("\n")
 
-    def rag_completion(self, query):
+    def rag_completion(self, query, model="gpt-4-turbo-preview"):
         rag_response = self.client.rag_completion(
             query,
             5,
             filters={"user_id": self.user_id},
+            generation_config={"model": model},
         )
         print("rag_response = ", rag_response)
 
-    def rag_completion_streaming(self, query):
+    def rag_completion_streaming(self, query, model="gpt-4-turbo-preview"):
         async def stream_rag_completion():
             async for chunk in self.client.stream_rag_completion(
                 query,
                 5,
                 filters={"user_id": self.user_id},
-                generation_config={"stream": True},
+                generation_config={"stream": True, "model": model},
             ):
                 print(chunk, end="", flush=True)
 
         asyncio.run(stream_rag_completion())
 
     def delete_document(self, document_path: str):
         document_id = generate_id_from_label(document_path)
```

### Comparing `r2r-0.1.29/r2r/examples/clients/run_basic_client_old.py` & `r2r-0.1.31/r2r/examples/clients/run_basic_client_old.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,119 +19,119 @@
     {"txt": "This is a test entry"},
     {"tags": ["example", "test"]},
     do_upsert=True,
 )
 print(f"Upsert entry response:\n{entry_response}\n\n")
 
 
-entry_response = client.add_entry(
-    generate_id_from_label("doc 1"),
-    {"txt": "This is a test entry"},
-    {"tags": ["example", "test"]},
-    do_upsert=False,
-)
-print(f"Copy same entry response:\n{entry_response}\n\n")
-
-
-print("Upserting entries to remote db...")
-# Upsert multiple entries
-entries = [
-    {
-        "document_id": generate_id_from_label("doc 2"),
-        "blobs": {"txt": "Second test entry"},
-        "metadata": {"tags": "bulk"},
-    },
-    {
-        "document_id": generate_id_from_label("doc 3"),
-        "blobs": {"txt": "Third test entry"},
-        "metadata": {"tags": "example"},
-    },
-]
-bulk_upsert_response = client.add_entries(entries, do_upsert=True)
-print(f"Upsert entries response:\n{bulk_upsert_response}\n\n")
-
-# Perform a search
-print("Searching remote db...")
-search_response = client.search("test", 5)
-print(f"Search response:\n{search_response}\n\n")
-
-print("Searching remote db with filter...")
-# Perform a search w/ filter
-filtered_search_response = client.search("test", 5, filters={"tags": "bulk"})
-print(f"Search response w/ filter:\n{filtered_search_response}\n\n")
-
-print("Deleting sample document in remote db...")
-# Delete a document
-response = client.filtered_deletion(
-    "document_id", generate_id_from_label("doc 2")
-)
-print(f"Deletion response:\n{response}\n\n")
-
-print("Searching remote db with filter after deletion...")
-# Perform a search w/ filter after deletion
-post_deletion_filtered_search_response = client.search(
-    "test", 5, filters={"tags": "bulk"}
-)
-print(
-    f"Search response w/ filter+deletion:\n{post_deletion_filtered_search_response}\n\n"
-)
-
-# Example file path for upload
-# get file directory
-current_file_directory = os.path.dirname(os.path.realpath(__file__))
-
-file_path = os.path.join(current_file_directory, "..", "data", "test.pdf")
-
-print(f"Uploading and processing file: {file_path}...")
-# # Upload and process a file
-metadata = {"tags": ["example", "test"]}
-upload_pdf_response = client.upload_and_process_file(
-    generate_id_from_label("pdf 1"), file_path, metadata, None
-)
-print(f"Upload test pdf response:\n{upload_pdf_response}\n\n")
-
-print("Searching remote db after upload...")
-# Perform a search on this file
-pdf_filtered_search_response = client.search(
-    "what is a cool physics equation?",
-    5,
-    filters={"document_id": generate_id_from_label("pdf 1")},
-)
-print(
-    f"Search response w/ uploaded pdf filter:\n{pdf_filtered_search_response}\n"
-)
-
-
-print("Performing RAG...")
-# Perform a search on this file
-pdf_filtered_search_response = client.rag_completion(
-    "Are there any test documents?",
-    5,
-    filters={"document_id": generate_id_from_label("pdf 1")},
-)
-print(
-    f"Search response w/ uploaded pdf filter:\n{pdf_filtered_search_response}\n"
-)
-
-print("Performing RAG with streaming...")
-
-
-# Perform a RAG completion with streaming
-async def stream_rag_completion():
-    async for chunk in client.stream_rag_completion(
-        "Are there any test documents?",
-        5,
-        filters={"document_id": generate_id_from_label("pdf 1")},
-        generation_config={"stream": True},
-    ):
-        print(chunk, end="", flush=True)
-
-
-asyncio.run(stream_rag_completion())
-
-print("Fetching logs after all steps...")
-logs_response = client.get_logs()
-print(f"Logs response:\n{logs_response}\n")
-
-print("Fetching logs summary after all steps...")
-logs_summary_response = client.get_logs_summary()
-print(f"Logs summary response:\n{logs_summary_response}\n")
+# entry_response = client.add_entry(
+#     generate_id_from_label("doc 1"),
+#     {"txt": "This is a test entry"},
+#     {"tags": ["example", "test"]},
+#     do_upsert=False,
+# )
+# print(f"Copy same entry response:\n{entry_response}\n\n")
+
+
+# print("Upserting entries to remote db...")
+# # Upsert multiple entries
+# entries = [
+#     {
+#         "document_id": generate_id_from_label("doc 2"),
+#         "blobs": {"txt": "Second test entry"},
+#         "metadata": {"tags": "bulk"},
+#     },
+#     {
+#         "document_id": generate_id_from_label("doc 3"),
+#         "blobs": {"txt": "Third test entry"},
+#         "metadata": {"tags": "example"},
+#     },
+# ]
+# bulk_upsert_response = client.add_entries(entries, do_upsert=True)
+# print(f"Upsert entries response:\n{bulk_upsert_response}\n\n")
+
+# # Perform a search
+# print("Searching remote db...")
+# search_response = client.search("test", 5)
+# print(f"Search response:\n{search_response}\n\n")
+
+# print("Searching remote db with filter...")
+# # Perform a search w/ filter
+# filtered_search_response = client.search("test", 5, filters={"tags": "bulk"})
+# print(f"Search response w/ filter:\n{filtered_search_response}\n\n")
+
+# print("Deleting sample document in remote db...")
+# # Delete a document
+# response = client.filtered_deletion(
+#     "document_id", generate_id_from_label("doc 2")
+# )
+# print(f"Deletion response:\n{response}\n\n")
+
+# print("Searching remote db with filter after deletion...")
+# # Perform a search w/ filter after deletion
+# post_deletion_filtered_search_response = client.search(
+#     "test", 5, filters={"tags": "bulk"}
+# )
+# print(
+#     f"Search response w/ filter+deletion:\n{post_deletion_filtered_search_response}\n\n"
+# )
+
+# # Example file path for upload
+# # get file directory
+# current_file_directory = os.path.dirname(os.path.realpath(__file__))
+
+# file_path = os.path.join(current_file_directory, "..", "data", "test.pdf")
+
+# print(f"Uploading and processing file: {file_path}...")
+# # # Upload and process a file
+# metadata = {"tags": ["example", "test"]}
+# upload_pdf_response = client.upload_and_process_file(
+#     generate_id_from_label("pdf 1"), file_path, metadata, None
+# )
+# print(f"Upload test pdf response:\n{upload_pdf_response}\n\n")
+
+# print("Searching remote db after upload...")
+# # Perform a search on this file
+# pdf_filtered_search_response = client.search(
+#     "what is a cool physics equation?",
+#     5,
+#     filters={"document_id": generate_id_from_label("pdf 1")},
+# )
+# print(
+#     f"Search response w/ uploaded pdf filter:\n{pdf_filtered_search_response}\n"
+# )
+
+
+# print("Performing RAG...")
+# # Perform a search on this file
+# pdf_filtered_search_response = client.rag_completion(
+#     "Are there any test documents?",
+#     5,
+#     filters={"document_id": generate_id_from_label("pdf 1")},
+# )
+# print(
+#     f"Search response w/ uploaded pdf filter:\n{pdf_filtered_search_response}\n"
+# )
+
+# print("Performing RAG with streaming...")
+
+
+# # Perform a RAG completion with streaming
+# async def stream_rag_completion():
+#     async for chunk in client.stream_rag_completion(
+#         "Are there any test documents?",
+#         5,
+#         filters={"document_id": generate_id_from_label("pdf 1")},
+#         generation_config={"stream": True},
+#     ):
+#         print(chunk, end="", flush=True)
+
+
+# asyncio.run(stream_rag_completion())
+
+# print("Fetching logs after all steps...")
+# logs_response = client.get_logs()
+# print(f"Logs response:\n{logs_response}\n")
+
+# print("Fetching logs summary after all steps...")
+# logs_summary_response = client.get_logs_summary()
+# print(f"Logs summary response:\n{logs_summary_response}\n")
```

### Comparing `r2r-0.1.29/r2r/examples/clients/run_synthetic_query_client.py` & `r2r-0.1.31/r2r/examples/clients/run_synthetic_query_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/examples/data/meditations.pdf` & `r2r-0.1.31/r2r/examples/data/meditations.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/examples/data/test.pdf` & `r2r-0.1.31/r2r/examples/data/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/examples/data/the_republic.pdf` & `r2r-0.1.31/r2r/examples/data/the_republic.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/examples/servers/reducto_pipeline.py` & `r2r-0.1.31/r2r/examples/servers/reducto_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/examples/servers/synthetic_query_pipeline.py` & `r2r-0.1.31/r2r/examples/servers/synthetic_query_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/integrations/exa.py` & `r2r-0.1.31/r2r/integrations/exa.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/integrations/ionic.py` & `r2r-0.1.31/r2r/integrations/ionic.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/integrations/serper.py` & `r2r-0.1.31/r2r/integrations/serper.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/llms/litellm/base.py` & `r2r-0.1.31/r2r/llms/litellm/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/llms/llamacpp/base.py` & `r2r-0.1.31/r2r/llms/llama_cpp/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 @dataclass
 class LlamaCppConfig(LLMConfig):
     """Configuration for LlamaCpp models."""
 
     # Base
-    provider_name: str = "llamacpp"
+    provider_name: str = "llama-cpp"
     model_path: str = ""
     model_name: str = ""
 
     def __post_init__(self):
         if not self.model_path or self.model_path == "":
             self.model_path = os.path.join(
                 os.path.expanduser("~"), ".cache", "models"
@@ -96,14 +96,15 @@
 
         prompt = "\n".join([msg["content"] for msg in messages])
 
         response = self.client(prompt, **args)
 
         if not generation_config.stream:
             return ChatCompletion(
+                # TODO - Set an intelligent id
                 id="777",
                 object="chat.completion",
                 created=int(datetime.datetime.now().timestamp()),
                 model=generation_config.model,
                 choices=[
                     {
                         "message": {
```

### Comparing `r2r-0.1.29/r2r/llms/openai/base.py` & `r2r-0.1.31/r2r/llms/openai/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/main/app.py` & `r2r-0.1.31/r2r/main/app.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/main/factory.py` & `r2r-0.1.31/r2r/main/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,32 @@
 
     @staticmethod
     def get_embeddings_provider(embedding_config: dict[str, Any]):
         if embedding_config["provider"] == "openai":
             from r2r.embeddings import OpenAIEmbeddingProvider
 
             return OpenAIEmbeddingProvider()
-        elif embedding_config["provider"] == "sentence_transformers":
+        elif embedding_config["provider"] == "sentence-transformers":
             from r2r.embeddings import SentenceTransformerEmbeddingProvider
 
             return SentenceTransformerEmbeddingProvider(
                 embedding_config["model"]
             )
+        else:
+            raise ValueError(
+                f"Embedding provider {embedding_config['provider']} not supported"
+            )
 
     @staticmethod
     def get_llm(llm_config: dict[str, Any]):
         if llm_config["provider"] == "openai":
             return OpenAILLM(OpenAIConfig())
         elif llm_config["provider"] == "litellm":
             return LiteLLM(LiteLLMConfig())
-        elif llm_config["provider"] == "llamacpp":
+        elif llm_config["provider"] == "llama-cpp":
             return LlamaCPP(
                 LlamaCppConfig(
                     llm_config.get("model_path", ""),
                     llm_config.get("model_name", ""),
                 )
             )
```

### Comparing `r2r-0.1.29/r2r/main/models.py` & `r2r-0.1.31/r2r/main/models.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/main/utils.py` & `r2r-0.1.31/r2r/main/utils.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/pipelines/__init__.py` & `r2r-0.1.31/r2r/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/pipelines/basic/embedding.py` & `r2r-0.1.31/r2r/pipelines/basic/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/pipelines/basic/eval.py` & `r2r-0.1.31/r2r/pipelines/basic/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     EvalPipeline,
     LoggingDatabaseConnection,
     log_execution_to_db,
 )
 
 
 class BasicEvalPipeline(EvalPipeline):
-    eval_providers = ["deepeval", "parea"]
+    eval_providers = ["deepeval", "parea", "none"]
 
     def __init__(
         self,
         eval_config: dict,
         logging_connection: Optional[LoggingDatabaseConnection] = None,
         *args,
         **kwargs,
@@ -44,11 +44,13 @@
                 raise ImportError(
                     "Parea is not installed. Please install it using `pip install parea`."
                 )
             self.eval_provider = PareaEvalProvider(
                 provider,
                 eval_config.get("sampling_fraction", 1.0),
             )
+        else:
+            self.eval_provider = None
 
     @log_execution_to_db
     def evaluate(self, query: str, context: str, completion: str) -> Any:
         return self.eval_provider.evaluate(query, context, completion)
```

### Comparing `r2r-0.1.29/r2r/pipelines/basic/ingestion.py` & `r2r-0.1.31/r2r/pipelines/basic/ingestion.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/pipelines/basic/prompt_provider.py` & `r2r-0.1.31/r2r/pipelines/basic/prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/pipelines/basic/rag.py` & `r2r-0.1.31/r2r/pipelines/basic/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/pipelines/web_search/rag.py` & `r2r-0.1.31/r2r/pipelines/web_search/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/tests/end_to_end.py` & `r2r-0.1.31/r2r/tests/end_to_end.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/tests/test.pdf` & `r2r-0.1.31/r2r/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vecs/__init__.py` & `r2r-0.1.31/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vecs/adapter/base.py` & `r2r-0.1.31/r2r/vecs/adapter/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vecs/adapter/markdown.py` & `r2r-0.1.31/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vecs/adapter/noop.py` & `r2r-0.1.31/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vecs/adapter/text.py` & `r2r-0.1.31/r2r/vecs/adapter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vecs/client.py` & `r2r-0.1.31/r2r/vecs/client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vecs/collection.py` & `r2r-0.1.31/r2r/vecs/collection.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vecs/exc.py` & `r2r-0.1.31/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vector_dbs/local/base.py` & `r2r-0.1.31/r2r/vector_dbs/local/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vector_dbs/pg_vector/base.py` & `r2r-0.1.31/r2r/vector_dbs/pg_vector/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/r2r/vector_dbs/qdrant/base.py` & `r2r-0.1.31/r2r/vector_dbs/qdrant/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.29/PKG-INFO` & `r2r-0.1.31/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2r
-Version: 0.1.29
+Version: 0.1.31
 Summary: SciPhi R2R
 License: MIT
 Author: Owen Colegrove
 Author-email: owen@sciphi.ai
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -135,14 +135,17 @@
 
 [`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This **client script** should be executed subsequent to the server startup above. It facilitates the upload of text entries and PDFs to the server using the Python client and demonstrates the management of document and user-level vectors through its built-in features.
 
    ```bash
    # run the client
    python -m r2r.examples.clients.run_basic_client
    ```
+### Running Basic Local RAG
+
+[Refer here](https://r2r-docs.sciphi.ai/tutorials/local-rag) for a tutorial on how to modify the commands above to use local providers.
 
 ## Synthetic Queries Example
 
 [`synthetic_query_pipeline.py`](r2r/examples/servers/synthetic_query_pipeline.py): Execute this script to start a backend server equipped with an advanced pipeline. This pipeline is designed to create synthetic queries, enhancing the RAG system's learning and performance.
 
    ```bash
    # launch the server
@@ -152,15 +155,15 @@
 [`run_synthetic_query_client.py`](r2r/examples/clients/run_synthetic_query_client.py): Use this client script after the synthetic query pipeline is running. It's tailored for use with the synthetic query pipeline, demonstrating the improved features of the RAG system.
 
    ```bash
    # run the client
    python -m r2r.examples.clients.run_synthetic_query_client
    ```
 
-## Extras Examples
+## Extra Examples
 
 [`reducto_pipeline.py`](r2r/examples/servers/reducto_pipeline.py): Launch this script to activate a backend server that integrates a Reducto adapter for enhanced PDF ingestion.
 
    ```bash
    # launch the server
    python -m r2r.examples.servers.reducto_pipeline
    ```
@@ -172,17 +175,17 @@
    python -m r2r.examples.servers.web_search_pipeline
    ```
 
 ## Core Abstractions
 
 The framework primarily revolves around three core abstractions:
 
-- The **Ingestion Pipeline**: Facilitates the preparation of embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.). The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/ingestion).
+- The **Ingestion Pipeline**: Facilitates the preparation of embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.). The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/deep-dive/ingestion).
 
-- The **Embedding Pipeline**: Manages the transformation of text into stored vector embeddings, interacting with embedding and vector database providers through a series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks, etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/embedding.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/embedding).
+- The **Embedding Pipeline**: Manages the transformation of text into stored vector embeddings, interacting with embedding and vector database providers through a series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks, etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/embedding.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/deep-dive/embedding).
 
-- The **RAG Pipeline**: Works similarly to the embedding pipeline but incorporates an LLM provider to produce text completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/rag.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/rag).
+- The **RAG Pipeline**: Works similarly to the embedding pipeline but incorporates an LLM provider to produce text completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/rag.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/deep-dive/rag).
 
-- The **Eval Pipeline**: Samples some subset of rag_completion calls for evaluation. Currently [DeepEval](https://github.com/confident-ai/deepeval) is supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/eval).
+- The **Eval Pipeline**: Samples some subset of rag_completion calls for evaluation. Currently [DeepEval](https://github.com/confident-ai/deepeval) and [Parea](https://github.com/parea-ai/parea-sdk-py) are supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/deep-dive/eval).
 
 Each pipeline incorporates a logging database for operation tracking and observability.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: r2r Version: 0.1.29 Summary: SciPhi R2R License:
+Metadata-Version: 2.1 Name: r2r Version: 0.1.31 Summary: SciPhi R2R License:
 MIT Author: Owen Colegrove Author-email: owen@sciphi.ai Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: all Provides-Extra: deepeval Provides-Extra:
 embedding Provides-Extra: eval Provides-Extra: exa Provides-Extra: ionic
@@ -67,46 +67,50 @@
 encompasses ingestion, embedding, and RAG processes, all accessible via
 FastAPI. ```bash # launch the server python -
 m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
 clients/run_basic_client.py): This **client script** should be executed
 subsequent to the server startup above. It facilitates the upload of text
 entries and PDFs to the server using the Python client and demonstrates the
 management of document and user-level vectors through its built-in features.
-```bash # run the client python -m r2r.examples.clients.run_basic_client ``` ##
-Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/examples/servers/
-synthetic_query_pipeline.py): Execute this script to start a backend server
-equipped with an advanced pipeline. This pipeline is designed to create
-synthetic queries, enhancing the RAG system's learning and performance. ```bash
-# launch the server python -m r2r.examples.servers.synthetic_query_pipeline ```
+```bash # run the client python -m r2r.examples.clients.run_basic_client ```
+### Running Basic Local RAG [Refer here](https://r2r-docs.sciphi.ai/tutorials/
+local-rag) for a tutorial on how to modify the commands above to use local
+providers. ## Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/
+examples/servers/synthetic_query_pipeline.py): Execute this script to start a
+backend server equipped with an advanced pipeline. This pipeline is designed to
+create synthetic queries, enhancing the RAG system's learning and performance.
+```bash # launch the server python -
+m r2r.examples.servers.synthetic_query_pipeline ```
 [`run_synthetic_query_client.py`](r2r/examples/clients/
 run_synthetic_query_client.py): Use this client script after the synthetic
 query pipeline is running. It's tailored for use with the synthetic query
 pipeline, demonstrating the improved features of the RAG system. ```bash # run
 the client python -m r2r.examples.clients.run_synthetic_query_client ``` ##
-Extras Examples [`reducto_pipeline.py`](r2r/examples/servers/
+Extra Examples [`reducto_pipeline.py`](r2r/examples/servers/
 reducto_pipeline.py): Launch this script to activate a backend server that
 integrates a Reducto adapter for enhanced PDF ingestion. ```bash # launch the
 server python -m r2r.examples.servers.reducto_pipeline ```
 [`web_search_pipeline.py`](r2r/examples/servers/web_search_pipeline.py): This
 script sets up a backend server that includes a `WebSearchRAGPipeline`, adding
 web search functionality to your RAG setup. ```bash # launch the server python
 -m r2r.examples.servers.web_search_pipeline ``` ## Core Abstractions The
 framework primarily revolves around three core abstractions: - The **Ingestion
 Pipeline**: Facilitates the preparation of embeddable 'Documents' from various
 data formats (json, txt, pdf, html, etc.). The abstraction can be found in
 [`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is
-available [here](https://r2r-docs.sciphi.ai/core-features/ingestion). - The
+available [here](https://r2r-docs.sciphi.ai/deep-dive/ingestion). - The
 **Embedding Pipeline**: Manages the transformation of text into stored vector
 embeddings, interacting with embedding and vector database providers through a
 series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks,
 etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/
 embedding.py) and relevant documentation is available [here](https://r2r-
-docs.sciphi.ai/core-features/embedding). - The **RAG Pipeline**: Works
-similarly to the embedding pipeline but incorporates an LLM provider to produce
-text completions. The abstraction can be found in [`rag.py`](r2r/core/
-pipelines/rag.py) and relevant documentation is available [here](https://r2r-
-docs.sciphi.ai/core-features/rag). - The **Eval Pipeline**: Samples some subset
-of rag_completion calls for evaluation. Currently [DeepEval](https://
-github.com/confident-ai/deepeval) is supported. The abstraction can be found in
-[`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available
-[here](https://r2r-docs.sciphi.ai/core-features/eval). Each pipeline
-incorporates a logging database for operation tracking and observability.
+docs.sciphi.ai/deep-dive/embedding). - The **RAG Pipeline**: Works similarly to
+the embedding pipeline but incorporates an LLM provider to produce text
+completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/
+rag.py) and relevant documentation is available [here](https://r2r-
+docs.sciphi.ai/deep-dive/rag). - The **Eval Pipeline**: Samples some subset of
+rag_completion calls for evaluation. Currently [DeepEval](https://github.com/
+confident-ai/deepeval) and [Parea](https://github.com/parea-ai/parea-sdk-py)
+are supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/
+eval.py) and relevant documentation is available [here](https://r2r-
+docs.sciphi.ai/deep-dive/eval). Each pipeline incorporates a logging database
+for operation tracking and observability.
```

