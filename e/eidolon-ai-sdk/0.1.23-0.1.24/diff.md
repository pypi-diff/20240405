# Comparing `tmp/eidolon_ai_sdk-0.1.23.tar.gz` & `tmp/eidolon_ai_sdk-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.23.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.24.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.23.tar` & `eidolon_ai_sdk-0.1.24.tar`

### file list

```diff
@@ -1,124 +1,136 @@
--rw-r--r--   0        0        0     2569 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/README.md
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2415 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     4645 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2787 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4510 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     5516 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0     1970 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/openai_whisper_agent.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1444 2024-03-27 05:44:53.934342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2339 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     5770 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0     5638 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1825 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4446 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     7578 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     7842 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     5468 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      181 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4153 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2956 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     7916 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0      292 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0     8231 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/conversational_agent_cpu.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0    12773 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3104 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     1679 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     1910 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4199 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1157 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2620 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0     2517 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4220 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3912 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5627 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4837 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     4067 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     5453 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0      869 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2091 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1231 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1076 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2462 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     1780 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1052 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1377 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    20818 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    13339 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     3272 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4201 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6890 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1646 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-03-27 05:44:53.938342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     3748 2024-03-27 05:44:53.942342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6206 2024-03-27 05:44:53.942342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      370 2024-03-27 05:44:53.942342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-03-27 05:44:53.942342 eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-03-27 05:44:53.942342 eidolon_ai_sdk-0.1.23/logging.conf
--rw-r--r--   0        0        0     1845 2024-03-27 05:44:53.942342 eidolon_ai_sdk-0.1.23/pyproject.toml
--rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.23/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2415 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     4645 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4510 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     5516 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0     1998 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/openai_whisper_agent.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1444 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2339 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2939 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3640 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    11421 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1825 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4446 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     7578 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     8297 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      239 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      236 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      242 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      231 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      257 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      231 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      235 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      234 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4293 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2956 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     7916 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0      292 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0     8231 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/conversational_agent_cpu.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0    10036 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    12148 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0    12773 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3119 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     1679 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     1910 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4199 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1157 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2620 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0     2517 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4220 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3912 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5780 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4837 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     4067 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1976 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0     5453 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0      869 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2091 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1231 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1076 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2462 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     1780 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1052 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    20899 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    13397 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     3911 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     3812 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6483 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      900 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/logging.conf
+-rw-r--r--   0        0        0     2003 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/pyproject.toml
+-rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.24/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.23/README.md` & `eidolon_ai_sdk-0.1.24/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         elif blob.mimetype == "text/x-cobol":
             from eidolon_ai_sdk.agent.doc_manager.parsers.code_ast_parsers.programing_language_parser import (
                 LanguageParser,
             )
 
             yield from LanguageParser(LanguageParserSpec(language="cobol")).parse(blob)
         elif (
-            blob.mimetype.startswith("text/")
+            blob.mimetype and blob.mimetype.startswith("text/")
             or blob.mimetype == "application/json"
             or blob.mimetype == "application/xml"
             or blob.mimetype == "application/yaml"
             or blob.mimetype == "application/x-yaml"
             or blob.mimetype == "application/x-yml"
         ):
             from eidolon_ai_sdk.agent.doc_manager.parsers.text_parsers import TextParser
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/openai_whisper_agent.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/openai_whisper_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,26 +19,30 @@
 
     def __init__(self, spec: AutonomousSpeechAgentSpec):
         super().__init__(spec=spec)
         self.speech_llm = self.spec.speech_llm.instantiate()
         self.cpu = self.spec.cpu.instantiate()
 
     @register_program()
-    async def speech_to_text(self, process_id, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]):
+    async def speech_to_text(
+        self, process_id, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]
+    ):
         await ProcessDoc.set_delete_on_terminate(process_id, True)
         file, metadata = await AgentOS.process_file_system.read_file(process_id, audio.file_id)
         mimetype = "audio/wav"
         if metadata and "mimetype" in metadata:
             mimetype = metadata["mimetype"]
         # audio = AudioSegment.from_file(file)
         # # Convert to mp3
         # audio_mp3 = audio.export("audio.mp3", format="mp3")
 
         text = await self.speech_llm.speech_to_text(file, mimetype)
         return {"response": text}
 
     @register_program()
-    async def text_to_speech(self, process_id: str, text: Annotated[str, Body(description="The text to speak", embed=True)]) -> FileHandle:
+    async def text_to_speech(
+        self, process_id: str, text: Annotated[str, Body(description="The text to speak", embed=True)]
+    ) -> FileHandle:
         audio_result = await self.speech_llm.text_to_speech(text)
         file_id = await AgentOS.process_file_system.write_file(process_id, audio_result, {"mimetype": "audio/mpeg"})
 
         return FileHandle(machineURL=AgentOS.current_machine_url(), process_id=process_id, file_id=file_id)
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,42 +4,47 @@
 from openai.lib.azure import AsyncAzureOpenAI
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.trace import SpanProcessor
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SpanExporter
 from opentelemetry.sdk.trace.sampling import Sampler
 
 from eidolon_ai_client.util.logger import logger
+from eidolon_ai_sdk.agent.doc_manager.document_manager import DocumentManager
 from eidolon_ai_sdk.agent.doc_manager.loaders.base_loader import DocumentLoader
 from eidolon_ai_sdk.agent.doc_manager.loaders.filesystem_loader import FilesystemLoader
 from eidolon_ai_sdk.agent.doc_manager.loaders.github_loader import GitHubLoader
 from eidolon_ai_sdk.agent.doc_manager.parsers.auto_parser import AutoParser
 from eidolon_ai_sdk.agent.doc_manager.parsers.base_parser import DocumentParser
 from eidolon_ai_sdk.agent.doc_manager.transformer.auto_transformer import AutoTransformer
 from eidolon_ai_sdk.agent.doc_manager.transformer.document_transformer import DocumentTransformer
 from eidolon_ai_sdk.agent.generic_agent import GenericAgent
 from eidolon_ai_sdk.agent.openai_whisper_agent import AutonomousSpeechAgent
 from eidolon_ai_sdk.agent.retriever_agent.document_reranker import RAGFusionReranker, DocumentReranker
 from eidolon_ai_sdk.agent.retriever_agent.multi_question_transformer import MultiQuestionTransformer
 from eidolon_ai_sdk.agent.retriever_agent.question_transformer import QuestionTransformer
+from eidolon_ai_sdk.agent.retriever_agent.retriever import Retriever
 from eidolon_ai_sdk.agent.retriever_agent.retriever_agent import RetrieverAgent
 from eidolon_ai_sdk.agent.simple_agent import SimpleAgent
 from eidolon_ai_sdk.agent.tot_agent.checker import ToTChecker
 from eidolon_ai_sdk.agent.tot_agent.thought_generators import ThoughtGenerationStrategy, ProposePromptStrategy
 from eidolon_ai_sdk.agent.tot_agent.tot_agent import TreeOfThoughtsAgent
 from eidolon_ai_sdk.builtins.components.opentelemetry import OpenTelemetryManager, CustomSampler, NoopSpanExporter
 from eidolon_ai_sdk.builtins.components.usage import UsageMiddleware
 from eidolon_ai_sdk.builtins.logic_units.web_search import WebSearch, Browser, Search
 from eidolon_ai_sdk.cpu.agent_cpu import AgentCPU
 from eidolon_ai_sdk.cpu.agent_io import IOUnit
 from eidolon_ai_sdk.cpu.conversation_memory_unit import RawMemoryUnit
 from eidolon_ai_sdk.cpu.conversational_agent_cpu import ConversationalAgentCPU
+from eidolon_ai_sdk.cpu.llm.anthropic_llm_unit import AnthropicLLMUnit
+from eidolon_ai_sdk.cpu.llm.mistral_llm_unit import MistralGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_llm_unit import OpenAIGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_speech import OpenAiSpeech
 from eidolon_ai_sdk.cpu.llm_unit import LLMUnit
 from eidolon_ai_sdk.cpu.memory_unit import MemoryUnit
+from eidolon_ai_sdk.memory.s3_file_memory import S3FileMemory
 from eidolon_ai_sdk.security.azure_authorizer import AzureJWTProcessor
 from eidolon_ai_sdk.security.google_auth import GoogleJWTProcessor
 from eidolon_ai_sdk.system.dynamic_middleware import Middleware, MultiMiddleware
 from eidolon_ai_sdk.system.process_file_system import ProcessFileSystem
 from eidolon_ai_usage_client.client import UsageClient
 
 try:
@@ -121,25 +126,29 @@
         # cpu
         (AgentCPU, ConversationalAgentCPU),
         ConversationalAgentCPU,
         # cpu components
         IOUnit,
         (LLMUnit, OpenAIGPT),
         OpenAIGPT,
+        MistralGPT,
+        AnthropicLLMUnit,
         (MemoryUnit, RawMemoryUnit),
         RawMemoryUnit,
         WebSearch,
         Search,
         Browser,
+        Retriever,
         # machine components
         (SymbolicMemory, MongoSymbolicMemory),
         MongoSymbolicMemory,
         LocalSymbolicMemory,
         (FileMemory, LocalFileMemory),
         LocalFileMemory,
+        S3FileMemory,
         SimilarityMemory,
         (Embedding, OpenAIEmbedding),
         NoopEmbedding,
         OpenAIEmbedding,
         (VectorStore, ChromaVectorStore),
         NoopVectorStore,
         ChromaVectorStore,
@@ -165,14 +174,15 @@
         (ThoughtGenerationStrategy, ProposePromptStrategy),
         ProposePromptStrategy,
         (QuestionTransformer, MultiQuestionTransformer),
         MultiQuestionTransformer,
         (DocumentReranker, RAGFusionReranker),
         RAGFusionReranker,
         (DocumentLoader, FilesystemLoader),
+        DocumentManager,
         FilesystemLoader,
         GitHubLoader,
         ToTChecker,
         OpenAiSpeech,
         AsyncOpenAI,
         AsyncAzureOpenAI,
         UsageClient,
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class SearchResult(BaseModel):
     url: str
     title: str
     description: Optional[str]
 
 
 class BrowseSpec(BaseModel):
-    summarizer: Literal["BeautifulSoup"] = "BeautifulSoup"
+    summarizer: Literal["BeautifulSoup", "noop"] = "BeautifulSoup"
 
 
 class Browser(LogicUnit, Specable[BrowseSpec]):
     def __init__(self, **kwargs):
         LogicUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
 
@@ -39,15 +39,19 @@
         async with _get(url=url) as resp:
             text = resp.text
             if not resp.is_success:
                 logger.warning(f"Request to url '{url}' return {resp.status_code}")
                 return text
             if self.spec.summarizer == "BeautifulSoup":
                 soup = BeautifulSoup(text, "lxml")
+                for a in soup.findAll("a"):
+                    a.replace_with(a.text + f" {a.get('href')}")
                 return soup.get_text(separator="\n", strip=True)
+            elif self.spec.summarizer == "noop":
+                return text
             else:
                 raise ValueError(f"Summarizer {self.spec.summarizer} not supported")
 
 
 # Requires custom search engine + token setup in google project. See more at https://developers.google.com/custom-search/v1/reference/rest/v1/cse/list
 class SearchSpec(BaseModel):
     cse_id: str = Field(
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,20 @@
     max_num_function_calls: int = Field(
         10,
         description="The maximum number of function calls to make in a single request.",
     )
 
 
 class AgentCPU(Specable[AgentCPUSpec], ABC):
+    title: str
+
+    def __init__(self, spec: T, **kwargs: object):
+        super().__init__(spec, **kwargs)
+        self.title = "default"
+
     @abstractmethod
     async def set_boot_messages(self, call_context: CallContext, boot_messages: List[CPUMessageTypes]):
         pass
 
     @abstractmethod
     async def schedule_request(
         self,
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/conversational_agent_cpu.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/conversational_agent_cpu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     model: str
     temperature: float
     llm: AsyncOpenAI = None
 
     def __init__(self, spec: OpenAiSpeechSpec, **kwargs):
         super().__init__(spec, **kwargs)
 
-    async def text_to_speech(self, text: str, response_format: str ="mp3") -> bytes:
+    async def text_to_speech(self, text: str, response_format: str = "mp3") -> bytes:
         """
         Converts text to speech.
 
         Args:
             text (str): The text to convert to speech.
 
         Returns:
@@ -49,15 +49,17 @@
             voice=self.spec.text_to_speech_voice,
             response_format="mp3",
             input=text,
         )
 
         return response.content
 
-    async def speech_to_text(self, audio: bytes, mime_type: str, prompt: Optional[str] = None, language: Optional[str] = None) -> str:
+    async def speech_to_text(
+        self, audio: bytes, mime_type: str, prompt: Optional[str] = None, language: Optional[str] = None
+    ) -> str:
         """
         Converts speech to text.
 
         Args:
             audio (bytes): The audio data.
             prompt (Optional[str], optional): An optional text to guide the model's style or continue a previous audio segment. Defaults to None.
             language (Optional[str], optional): The language of the input audio. Supplying the input language in ISO-639-1 format will improve accuracy and latency.
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     root_dir: str = Field("/tmp/eidolon/file_memory", description="The root directory to store files in.")
 
     @field_validator("root_dir", mode="before")
     def validate_root_dir(cls, inValue: str):
         """
         Validates that the provided root directory is an absolute path and exists.
         """
+        inValue = str(inValue)
         value = replace_env_var_in_string(inValue)
         # Convert the string to a Path object
         path = Path(value).resolve()
 
         # Check if the path is absolute
         if not path.is_absolute():
             raise ValueError(f"The root_dir must be an absolute path. Received: {inValue}->{value}")
@@ -144,15 +145,18 @@
         safe_file_path = self.resolve(file_name)
 
         # Check if the file exists
         return safe_file_path.exists()
 
     async def glob(self, pattern):
         safe_file_path = self.resolve(pattern)
-        return glob.glob(str(safe_file_path))
+        return [
+            s.removeprefix(str(self.root_dir)).removeprefix("/")
+            for s in glob.glob(str(safe_file_path), root_dir=self.root_dir)
+        ]
 
     async def start(self):
         """
         Starts the memory implementation. Noop for this implementation.
         """
         if not self.root_dir.exists():
             self.root_dir.mkdir(parents=True)
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,16 +131,17 @@
                 f"Action {handler.name} cannot process state {process.state}. Allowed states: {handler.extra['allowed_states']}"
             )
             raise HTTPException(
                 status_code=409,
                 detail=f'Action "{handler.name}" cannot process state "{process.state}"',
             )
         last_state = process.state
+        RequestContext.set("__last_state__", last_state)
         process = await process.update(
-            agent=self.name, record_id=process_id, state="processing", data=dict(action=handler.name)
+            check_update_time=True, agent=self.name, record_id=process_id, state="processing", data=dict(action=handler.name)
         )
         parameters = inspect.signature(handler.fn).parameters
         if "process_id" in parameters:
             kwargs["process_id"] = process_id
         if "request" in parameters and parameters["request"].annotation == Request:
             kwargs["request"] = request
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
 
 class MachineSpec(BaseModel):
     symbolic_memory: AnnotatedReference[SymbolicMemory] = Field(description="The Symbolic Memory implementation.")
     file_memory: AnnotatedReference[FileMemory] = Field(desciption="The File Memory implementation.")
     similarity_memory: AnnotatedReference[SimilarityMemory] = Field(description="The Vector Memory implementation.")
     security_manager: AnnotatedReference[SecurityManager] = Field(description="The Security Manager implementation.")
-    process_file_system: AnnotatedReference[ProcessFileSystem] = Field(description="The Process File System implementation. Used to store files related to processes.")
+    process_file_system: AnnotatedReference[ProcessFileSystem] = Field(
+        description="The Process File System implementation. Used to store files related to processes."
+    )
 
     def get_agent_memory(self):
         file_memory = self.file_memory.instantiate()
         symbolic_memory = self.symbolic_memory.instantiate()
         vector_memory = self.similarity_memory.instantiate()
         return AgentMemory(
             file_memory=file_memory,
@@ -147,27 +149,35 @@
 
     def _get_agent_controller(self, agent_name: str) -> Optional[AgentController]:
         for controller in self.agent_controllers:
             if controller.name == agent_name:
                 return controller
         return None
 
-    async def upload_file(self, process_id: str,
-                          mime_type: Annotated[str | None, Header()] = None,
-                          file_bytes=Body(description="A byte stream that represents the file to be uploaded", media_type="application/octet-stream")):
+    async def upload_file(
+        self,
+        process_id: str,
+        mime_type: Annotated[str | None, Header()] = None,
+        file_bytes=Body(
+            description="A byte stream that represents the file to be uploaded", media_type="application/octet-stream"
+        ),
+    ):
         """
         Upload a file for this process
         :param process_id:
         :param file_bytes:
         :return: The file id that was written
         """
         file_md = None
         if mime_type:
             file_md = {"mime_type": mime_type}
-        return JSONResponse(content={"file_id": await self.process_file_system.write_file(process_id, file_bytes, file_md)}, status_code=200)
+        return JSONResponse(
+            content={"file_id": await self.process_file_system.write_file(process_id, file_bytes, file_md)},
+            status_code=200,
+        )
 
     async def download_file(self, process_id: str, file_id: str):
         """
         Download a file for this process
         :param process_id:
         :param file_id:
         :return: The file bytes
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/process_file_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import asyncio
+import json
 from pathlib import Path
 from typing import cast, Optional, Dict, Tuple
 from uuid import uuid4
-import asyncio
-import json
 
 from pydantic import BaseModel
 
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.memory.file_memory import FileMemory
 from eidolon_ai_sdk.system.reference_model import Specable
 
@@ -66,16 +66,22 @@
         :param process_id:
         :param file_contents:
         :return:
         """
         file_id = uuid4().hex
         await self.file_memory().mkdir(str(Path(self.root, process_id)), exist_ok=True)
         await self.file_memory().write_file(str(Path(self.root, process_id, file_id)), file_contents)
+        md_to_write = {
+            "process_id": process_id,
+            "file_id": file_id
+        }
         if file_md:
-            await self.file_memory().write_file(str(Path(self.root, process_id, file_id + ".md")), json.dumps(file_md).encode())
+            md_to_write.update(file_md)
+        path = str(Path(self.root, process_id, file_id + ".md"))
+        await self.file_memory().write_file(path, json.dumps(md_to_write).encode())
         return file_id
 
     async def delete_file(self, process_id: str, file_id: str):
         """
         Deletes the file specified by `file_id` within the context of the process_id.
         :param process_id:
         :param file_id:
@@ -84,18 +90,28 @@
         path = str(Path(self.root, process_id, file_id))
         exists = await self.file_memory().exists(path)
         if not exists:
             return None
         await self.file_memory().delete_file(path)
         return "deleted"
 
+    async def list_files(self, process_id: str, include_only_index: bool):
+        path = Path(self.root, process_id)
+        files = await AgentOS.file_memory.glob(f"{path}/*.md")
+        for file in files:
+            contents = await AgentOS.file_memory.read_file(file)
+            file_md = json.loads(contents)
+            if not include_only_index or ("indexed" in file_md and file_md["indexed"]):
+                yield file_md
+
     @classmethod
     async def delete_process(cls, process_id: str):
         """
         Deletes the entire process directory
         :param process_id:
         :return:
         """
         memory: FileMemory = AgentOS.file_memory
         pfs: ProcessFileSystem = AgentOS.process_file_system
-        found = await memory.glob(f"{Path(pfs.root, process_id)}/**/*")
+        process_path = str(Path(pfs.root, process_id))
+        found = await memory.glob(f"{process_path}/**/*")
         await asyncio.gather(*[memory.delete_file(file) for file in found])
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/processes.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,17 +41,19 @@
             data["updated"] = t
         if "_id" not in data:
             data["_id"] = str(bson.ObjectId())
         doc = cls(**data)
         await AgentOS.symbolic_memory.insert_one(cls.collection, doc.model_dump())
         return doc
 
-    async def update(self, **data):
+    async def update(self, check_update_time=False, **data):
         data = dict(**data, updated=datetime.now().isoformat())
-        query = {"_id": self.record_id, "updated": self.updated}
+        query = {"_id": self.record_id}
+        if check_update_time:
+            query["updated"] = self.updated
         try:
             await AgentOS.symbolic_memory.upsert_one(self.collection, query=query, document=data)
         except DuplicateKeyError:
             raise ValueError(f"{self.__class__.__name__} record {self.record_id} has been updated since last read")
         dump = self.model_dump()
         dump.update(**data)
         return self.__class__.model_validate(dump)
@@ -68,17 +70,17 @@
     state: str
     delete_on_terminate: bool = False
     error_info: Optional[Any] = None
     title: Optional[str] = None
 
     @classmethod
     async def set_delete_on_terminate(cls, process_id: str, delete_on_terminate: bool = True):
-        await AgentOS.symbolic_memory.upsert_one(cls.collection, document={
-            "delete_on_terminate": delete_on_terminate
-        }, query={"_id": process_id})
+        await AgentOS.symbolic_memory.upsert_one(
+            cls.collection, document={"delete_on_terminate": delete_on_terminate}, query={"_id": process_id}
+        )
 
 
 async def store_events(agent: str, process_id: str, events: list[StreamEvent]):
     try:
         stored_events = []
         for event_num, event in enumerate(events):
             event_obj: Dict[str, Any] = {
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/reference_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     model_config = ConfigDict(
         extra="allow",
     )
 
     def __class_getitem__(cls, params):
         if not isinstance(params, tuple):
-            params = (params, params)
+            params = (params, fqn(params))
 
         class _Reference(cls):
             _bound = params[0]
             _default = params[1]
 
             @model_validator(mode="before")
             def _dump_ref(cls, value):
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import os
-from typing import List, Literal, Optional, TypeVar, Type
+from typing import List, Literal, Optional, TypeVar, Type, Dict
 
 import yaml
 from pydantic import BaseModel
 
 from eidolon_ai_client.util.logger import logger
 
 
 class Metadata(BaseModel):
     name: str = "DEFAULT"
-    annotations: List[str] = []
+    annotations: List[Dict[str, str]] = []
     labels: List[str] = []
 
 
 T = TypeVar("T", bound=BaseModel)
 
 
 class Resource(BaseModel, extra="allow"):
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/replay.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from typing import Optional
 
 import dill
 from pydantic import BaseModel
 from srsly.ruamel_yaml import YAML
 from srsly.ruamel_yaml.scalarstring import walk_tree
 
-from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_client.util.logger import logger
+from eidolon_ai_sdk.agent_os import AgentOS
+from eidolon_ai_sdk.util.str_utils import log_stack_trace
 
 
 class ReplayConfig(BaseModel):
     save_loc: Optional[str] = None  # If None, resume points are disabled
     digit_length: int = 3
 
 
@@ -39,15 +40,15 @@
 
 
 async def default_parser(resp):
     yield await resp
 
 
 def replayable(
-    fn, serializer=default_serializer, deserializer=default_deserializer, parser=default_parser, name_override=None
+        fn, serializer=default_serializer, deserializer=default_deserializer, parser=default_parser, name_override=None
 ):
     config = AgentOS.get_instance(ReplayConfig)
 
     async def maybe_save_args(*args, **kwargs):
         if config.save_loc:
             try:
                 existing_dirs = [os.path.split(d)[-1] for d in await AgentOS.file_memory.glob(config.save_loc + "/*")]
@@ -65,15 +66,16 @@
 
                 data, file_type = serializer(*args, **kwargs)
                 await AgentOS.file_memory.write_file(loc + "/fn.dill", dill.dumps(fn))
                 await AgentOS.file_memory.write_file(loc + f"/data.{file_type}", data.encode())
                 await AgentOS.file_memory.write_file(loc + "/deserializer.dill", dill.dumps(deserializer))
                 await AgentOS.file_memory.write_file(loc + "/parser.dill", dill.dumps(parser))
             except Exception as e:
-                logger.exception(f"Error saving resume point: {e}")
+                log_stack_trace()
+                logger.exception(e)
 
     @wraps(fn)
     async def wrapper_async_gen(*args, **kwargs):
         await maybe_save_args(*args, **kwargs)
         async for e in fn(*args, **kwargs):
             yield e
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from datetime import date, datetime, time
-from typing import Dict, Any, Type
+from typing import Dict, Any, Type, Literal
 from typing import List
 from uuid import UUID
 
 from fastapi import UploadFile
 from pydantic import BaseModel, HttpUrl, EmailStr, Field, model_validator
 from pydantic import create_model, ValidationError
 from pydantic.fields import FieldInfo
@@ -116,18 +116,18 @@
                 if isinstance(items_schema, dict) and items_schema.get("type") == "object":
                     nested_item_model = schema_to_model(
                         items_schema,
                         f"{model_name}_{property_name.capitalize()}ItemModel",
                     )
                     fields[property_name] = wrap_optional(List[nested_item_model], makeFieldOrDefaultValue())
                 else:
-                    python_type = get_python_type(items_schema, str)
+                    python_type = get_python_type(property_name, items_schema, str)
                     fields[property_name] = wrap_optional(List[python_type], makeFieldOrDefaultValue())
             else:
-                fields[property_name] = wrap_optional(get_python_type(property_schema), makeFieldOrDefaultValue())
+                fields[property_name] = wrap_optional(get_python_type(property_name, property_schema), makeFieldOrDefaultValue())
         except Exception as e:
             raise ValueError(f"Error creating field '{property_name}': {e}")
 
     try:
         return create_model(model_name, **fields, __base__=JsonProofModel)
     except ValidationError as e:
         raise ValueError(f"Error creating model '{model_name}': {e}")
@@ -138,16 +138,20 @@
     @classmethod
     def validate_to_json(cls, value):
         if isinstance(value, str):
             return cls(**json.loads(value))
         return value
 
 
-def get_python_type(property_schema, default=None):
+def get_python_type(property_name, property_schema, default=None):
     field_type = property_schema.get("type")
     if field_type == "string" and "format" in property_schema and property_schema["format"] == "binary":
         return UploadFile
     else:
+        if field_type == "string" and "enum" in property_schema and property_schema["enum"]:
+            # noinspection PyTypeHints
+            literal_ = Literal[tuple(property_schema["enum"])]
+            return literal_
         python_type = type_mapping.get(field_type, default)
         if python_type is None:
             raise ValueError(f"Unsupported type '{field_type}'")
         return python_type
```

### Comparing `eidolon_ai_sdk-0.1.23/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/logging.conf` & `eidolon_ai_sdk-0.1.24/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.23/pyproject.toml` & `eidolon_ai_sdk-0.1.24/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.23"
+version = "0.1.24"
 description = "An Open Source Agent Services Framework"
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 include = ["logging.conf"]
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
@@ -12,24 +12,26 @@
 
 [tool.poetry.scripts]
 eidolon-server = "eidolon_ai_sdk.bin.agent_http_server:main"
 replay = "eidolon_ai_sdk.bin.replay:app"
 #eidolon-create-agent = "eidolon_ai_sdk.bin.agent_creator:main"
 
 [tool.poetry.dependencies]
+setuptools = "^69.0.2"
 python = ">=3.11,<3.12"
 fastapi = "^0.109.0"
 pyyaml = "^6.0.1"
 jsonschema = "^4.21.1"
 httpx = "^0.27.0"
 uvicorn = "^0.27.0"
 numpy = "^1.26.3"
 motor = "^3.3.2"
 python-dotenv = "^1.0.1"
 openai = "^1.9.0"
+anthropic = "^0.21.3"
 jinja2 = "^3.1.3"
 pytest-json-report = "^1.5.0"
 tiktoken = "^0.5.1"
 jsonref = "^1.1.0"
 chromadb = "^0.4.18"
 spacy = "^3.7.2"
 lxml = "^5.1.0"
@@ -45,16 +47,19 @@
 httpx-sse = "^0.4.0"
 sse-starlette = "^2.0.0"
 dill = "^0.3.8"
 typer = {extras = ["all"], version = "^0.9.0"}
 opentelemetry-instrumentation-fastapi = "^0.44b0"
 opentelemetry-instrumentation-logging = "^0.44b0"
 opentelemetry-sdk = "^1.23.0"
+eidolon-ai-mistralai = "^0.1.6a"
 eidolon-ai-client = "^0.1.5"
 eidolon-ai-usage-client =  "^0.1.0"
+boto3 = "^1.34.74"
+boto3-stubs = {extras = ["essential"], version = "^1.34.74"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pylint = "^3.0.3"
 ruff = "^0.1.7"
 pytest-recording = "^0.13.1"
 pytest-asyncio = "^0.23.4"
```

### Comparing `eidolon_ai_sdk-0.1.23/PKG-INFO` & `eidolon_ai_sdk-0.1.24/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.23
+Version: 0.1.24
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
+Requires-Dist: boto3 (>=1.34.74,<2.0.0)
+Requires-Dist: boto3-stubs[essential] (>=1.34.74,<2.0.0)
 Requires-Dist: chromadb (>=0.4.18,<0.5.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: eidolon-ai-client (>=0.1.5,<0.2.0)
+Requires-Dist: eidolon-ai-mistralai (>=0.1.6a,<0.2.0)
 Requires-Dist: eidolon-ai-usage-client (>=0.1.0,<0.2.0)
 Requires-Dist: esprima (>=4.0.1,<5.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
@@ -31,14 +35,15 @@
 Requires-Dist: pypdf (>=4.0.1,<5.0.0)
 Requires-Dist: pytest-json-report (>=1.5.0,<2.0.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.8)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: setuptools (>=69.0.2,<70.0.0)
 Requires-Dist: spacy (>=3.7.2,<4.0.0)
 Requires-Dist: sse-starlette (>=2.0.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.5.1,<0.6.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: unstructured (>=0.12.3,<0.13.0)
 Requires-Dist: uvicorn (>=0.27.0,<0.28.0)
 Project-URL: Github, https://github.com/eidolon-ai/eidolon
```

