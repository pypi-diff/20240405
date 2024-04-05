# Comparing `tmp/schema-agents-0.1.7.tar.gz` & `tmp/schema-agents-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-agents-0.1.7.tar", last modified: Mon Oct 30 12:35:44 2023, max compression
+gzip compressed data, was "schema-agents-0.1.8.tar", last modified: Mon Oct 30 12:44:06 2023, max compression
```

## Comparing `schema-agents-0.1.7.tar` & `schema-agents-0.1.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.606497 schema-agents-0.1.7/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      859 2023-10-30 12:35:44.606104 schema-agents-0.1.7/PKG-INFO
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      345 2023-10-21 21:48:30.000000 schema-agents-0.1.7/README.md
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      611 2023-10-30 12:17:20.000000 schema-agents-0.1.7/pyproject.toml
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.596844 schema-agents-0.1.7/schema_agents/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)        0 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/__init__.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     4192 2023-10-30 12:27:35.000000 schema-agents-0.1.7/schema_agents/config.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      284 2023-10-22 00:58:55.000000 schema-agents-0.1.7/schema_agents/const.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      189 2023-10-30 12:28:26.000000 schema-agents-0.1.7/schema_agents/llm.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      498 2023-10-30 12:27:10.000000 schema-agents-0.1.7/schema_agents/logs.py
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.598744 schema-agents-0.1.7/schema_agents/memory/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      297 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/memory/__init__.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1368 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/memory/base_store.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2694 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/memory/faiss_store.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     4739 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/memory/long_term_memory.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3644 2023-10-28 23:32:37.000000 schema-agents-0.1.7/schema_agents/memory/memory.py
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.599858 schema-agents-0.1.7/schema_agents/provider/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      186 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/provider/__init__.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      659 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/provider/base_chatbot.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     6777 2023-10-28 19:06:51.000000 schema-agents-0.1.7/schema_agents/provider/base_gpt_api.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    12670 2023-10-28 19:31:01.000000 schema-agents-0.1.7/schema_agents/provider/openai_api.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    13383 2023-10-30 12:26:49.000000 schema-agents-0.1.7/schema_agents/role.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2100 2023-10-30 12:17:20.000000 schema-agents-0.1.7/schema_agents/schema.py
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.600185 schema-agents-0.1.7/schema_agents/teams/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3184 2023-10-30 12:20:17.000000 schema-agents-0.1.7/schema_agents/teams/__init__.py
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.600756 schema-agents-0.1.7/schema_agents/teams/databse_explore_hub/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     4935 2023-10-30 12:20:47.000000 schema-agents-0.1.7/schema_agents/teams/databse_explore_hub/__init__.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2746 2023-10-30 12:17:20.000000 schema-agents-0.1.7/schema_agents/teams/databse_explore_hub/database_explorer.py
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.602263 schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3591 2023-10-30 12:17:20.000000 schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/__init__.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    11378 2023-10-30 12:17:20.000000 schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/data_engineer.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     4934 2023-10-30 12:17:20.000000 schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/microscopist.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    10359 2023-10-28 22:22:33.000000 schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/schemas.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     6906 2023-10-30 12:17:20.000000 schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/web_developer.py
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.603267 schema-agents-0.1.7/schema_agents/tools/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)        0 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/tools/__init__.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     5860 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/tools/binder.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    15983 2023-10-21 21:11:58.000000 schema-agents-0.1.7/schema_agents/tools/code_interpreter.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    12600 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/tools/msgspec_v5.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2545 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/tools/ray_utils.py
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.604620 schema-agents-0.1.7/schema_agents/utils/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     4348 2023-10-30 12:17:20.000000 schema-agents-0.1.7/schema_agents/utils/__init__.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    10293 2023-10-30 12:33:20.000000 schema-agents-0.1.7/schema_agents/utils/common.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3043 2023-10-22 00:46:41.000000 schema-agents-0.1.7/schema_agents/utils/mermaid.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     4334 2023-10-28 23:33:02.000000 schema-agents-0.1.7/schema_agents/utils/serialize.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      532 2023-10-20 12:11:45.000000 schema-agents-0.1.7/schema_agents/utils/singleton.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3397 2023-10-21 21:48:30.000000 schema-agents-0.1.7/schema_agents/utils/token_counter.py
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.597596 schema-agents-0.1.7/schema_agents.egg-info/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      859 2023-10-30 12:35:44.000000 schema-agents-0.1.7/schema_agents.egg-info/PKG-INFO
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1595 2023-10-30 12:35:44.000000 schema-agents-0.1.7/schema_agents.egg-info/SOURCES.txt
--rw-r--r--   0 wei.ouyang   (501) staff       (20)        1 2023-10-30 12:35:44.000000 schema-agents-0.1.7/schema_agents.egg-info/dependency_links.txt
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      150 2023-10-30 12:35:44.000000 schema-agents-0.1.7/schema_agents.egg-info/requires.txt
--rw-r--r--   0 wei.ouyang   (501) staff       (20)       14 2023-10-30 12:35:44.000000 schema-agents-0.1.7/schema_agents.egg-info/top_level.txt
--rw-r--r--   0 wei.ouyang   (501) staff       (20)       38 2023-10-30 12:35:44.606549 schema-agents-0.1.7/setup.cfg
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:35:44.605761 schema-agents-0.1.7/tests/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2744 2023-10-20 12:18:19.000000 schema-agents-0.1.7/tests/test_code_interpreter.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3380 2023-10-28 23:33:24.000000 schema-agents-0.1.7/tests/test_hypha_ai_chat.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)       19 2023-10-20 12:11:45.000000 schema-agents-0.1.7/tests/test_hypha_bot.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     7068 2023-10-30 12:17:20.000000 schema-agents-0.1.7/tests/test_role.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2055 2023-10-30 12:17:20.000000 schema-agents-0.1.7/tests/test_team.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.047764 schema-agents-0.1.8/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      859 2023-10-30 12:44:06.047529 schema-agents-0.1.8/PKG-INFO
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      345 2023-10-21 21:48:30.000000 schema-agents-0.1.8/README.md
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      611 2023-10-30 12:42:09.000000 schema-agents-0.1.8/pyproject.toml
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.036030 schema-agents-0.1.8/schema_agents/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        0 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     4192 2023-10-30 12:27:35.000000 schema-agents-0.1.8/schema_agents/config.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      284 2023-10-22 00:58:55.000000 schema-agents-0.1.8/schema_agents/const.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      189 2023-10-30 12:28:26.000000 schema-agents-0.1.8/schema_agents/llm.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      498 2023-10-30 12:27:10.000000 schema-agents-0.1.8/schema_agents/logs.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.038030 schema-agents-0.1.8/schema_agents/memory/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      297 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/memory/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1368 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/memory/base_store.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2694 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/memory/faiss_store.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     4739 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/memory/long_term_memory.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3608 2023-10-30 12:41:50.000000 schema-agents-0.1.8/schema_agents/memory/memory.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.040875 schema-agents-0.1.8/schema_agents/provider/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      186 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/provider/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      659 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/provider/base_chatbot.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     6777 2023-10-28 19:06:51.000000 schema-agents-0.1.8/schema_agents/provider/base_gpt_api.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    12670 2023-10-28 19:31:01.000000 schema-agents-0.1.8/schema_agents/provider/openai_api.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    13239 2023-10-30 12:41:50.000000 schema-agents-0.1.8/schema_agents/role.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2088 2023-10-30 12:41:50.000000 schema-agents-0.1.8/schema_agents/schema.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.041170 schema-agents-0.1.8/schema_agents/teams/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3184 2023-10-30 12:20:17.000000 schema-agents-0.1.8/schema_agents/teams/__init__.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.041700 schema-agents-0.1.8/schema_agents/teams/databse_explore_hub/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     4935 2023-10-30 12:20:47.000000 schema-agents-0.1.8/schema_agents/teams/databse_explore_hub/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2746 2023-10-30 12:17:20.000000 schema-agents-0.1.8/schema_agents/teams/databse_explore_hub/database_explorer.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.043218 schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3591 2023-10-30 12:17:20.000000 schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    11366 2023-10-30 12:41:50.000000 schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/data_engineer.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     4862 2023-10-30 12:41:50.000000 schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/microscopist.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    10359 2023-10-28 22:22:33.000000 schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/schemas.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     6882 2023-10-30 12:41:50.000000 schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/web_developer.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.044330 schema-agents-0.1.8/schema_agents/tools/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        0 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/tools/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     5860 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/tools/binder.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    15983 2023-10-21 21:11:58.000000 schema-agents-0.1.8/schema_agents/tools/code_interpreter.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    12600 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/tools/msgspec_v5.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2545 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/tools/ray_utils.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.045734 schema-agents-0.1.8/schema_agents/utils/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     4348 2023-10-30 12:17:20.000000 schema-agents-0.1.8/schema_agents/utils/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    10293 2023-10-30 12:33:20.000000 schema-agents-0.1.8/schema_agents/utils/common.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3043 2023-10-22 00:46:41.000000 schema-agents-0.1.8/schema_agents/utils/mermaid.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     4202 2023-10-30 12:41:50.000000 schema-agents-0.1.8/schema_agents/utils/serialize.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      532 2023-10-20 12:11:45.000000 schema-agents-0.1.8/schema_agents/utils/singleton.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3397 2023-10-21 21:48:30.000000 schema-agents-0.1.8/schema_agents/utils/token_counter.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.036855 schema-agents-0.1.8/schema_agents.egg-info/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      859 2023-10-30 12:44:06.000000 schema-agents-0.1.8/schema_agents.egg-info/PKG-INFO
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1595 2023-10-30 12:44:06.000000 schema-agents-0.1.8/schema_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        1 2023-10-30 12:44:06.000000 schema-agents-0.1.8/schema_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      150 2023-10-30 12:44:06.000000 schema-agents-0.1.8/schema_agents.egg-info/requires.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       14 2023-10-30 12:44:06.000000 schema-agents-0.1.8/schema_agents.egg-info/top_level.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       38 2023-10-30 12:44:06.047814 schema-agents-0.1.8/setup.cfg
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-30 12:44:06.047009 schema-agents-0.1.8/tests/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2744 2023-10-20 12:18:19.000000 schema-agents-0.1.8/tests/test_code_interpreter.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3380 2023-10-28 23:33:24.000000 schema-agents-0.1.8/tests/test_hypha_ai_chat.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       19 2023-10-20 12:11:45.000000 schema-agents-0.1.8/tests/test_hypha_bot.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     6972 2023-10-30 12:41:50.000000 schema-agents-0.1.8/tests/test_role.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2031 2023-10-30 12:41:50.000000 schema-agents-0.1.8/tests/test_team.py
```

### Comparing `schema-agents-0.1.7/PKG-INFO` & `schema-agents-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-agents
-Version: 0.1.7
+Version: 0.1.8
 Summary: A schema-based LLM framework for building multi-agent collaborative systems.
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.21.2
 Requires-Dist: jsonschema>=4.0.1
 Requires-Dist: shortuuid>=1.0.1
 Requires-Dist: pydantic<2,>=1.8.2
 Requires-Dist: openai>=0.27.0
```

### Comparing `schema-agents-0.1.7/pyproject.toml` & `schema-agents-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "schema-agents"
-version = "0.1.7"
+version = "0.1.8"
 readme = "README.md"
 description = "A schema-based LLM framework for building multi-agent collaborative systems."
 dependencies = [
     "numpy>=1.21.2",
     "jsonschema>=4.0.1",
     "shortuuid>=1.0.1",
     "pydantic<2,>=1.8.2",
```

### Comparing `schema-agents-0.1.7/schema_agents/config.py` & `schema-agents-0.1.8/schema_agents/config.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/memory/base_store.py` & `schema-agents-0.1.8/schema_agents/memory/base_store.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/memory/faiss_store.py` & `schema-agents-0.1.8/schema_agents/memory/faiss_store.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/memory/long_term_memory.py` & `schema-agents-0.1.8/schema_agents/memory/long_term_memory.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/memory/memory.py` & `schema-agents-0.1.8/schema_agents/memory/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,17 @@
         """Return all messages containing a specified content"""
         return [message for message in self.storage if content in message.content]
     
     def get_by_schemas(self, schemas: list[BaseModel]) -> list[Message]:
         ret = []
         for schema in schemas:
             if schema is str:
-                ret += [message for message in self.storage if not message.instruct_content and isinstance(message.content, str)]
+                ret += [message for message in self.storage if not message.data and isinstance(message.content, str)]
             else:
-                ret += [message for message in self.storage if message.instruct_content and isinstance(message.instruct_content, schema)]
+                ret += [message for message in self.storage if message.data and isinstance(message.data, schema)]
         return ret
 
     def delete(self, message: Message):
         """Delete the specified message from storage, while updating the index"""
         self.storage.remove(message)
         if message.cause_by and message in self.index[message.cause_by]:
             self.index[message.cause_by].remove(message)
```

### Comparing `schema-agents-0.1.7/schema_agents/provider/base_chatbot.py` & `schema-agents-0.1.8/schema_agents/provider/base_chatbot.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/provider/base_gpt_api.py` & `schema-agents-0.1.8/schema_agents/provider/base_gpt_api.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/provider/openai_api.py` & `schema-agents-0.1.8/schema_agents/provider/openai_api.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/role.py` & `schema-agents-0.1.8/schema_agents/role.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,17 @@
         self._watch_actions.update(actions)
     
     def set_event_bus(self, event_bus: EventBus):
         """Set event bus."""
         self._event_bus = event_bus
 
         async def handle_message(msg):
-            if msg.instruct_content and type(msg.instruct_content) in self._watch_actions:
+            if msg.data and type(msg.data) in self._watch_actions:
                 await self.handle(msg)
-            elif msg.instruct_content is None and str in self._watch_actions:
+            elif msg.data is None and str in self._watch_actions:
                 await self.handle(msg)
 
         self._event_bus.on("message", handle_message)
         logger.info(f"Mounting {self._setting} to event bus: {self._event_bus.name}.")
     
     def get_event_bus(self):
         """Get event bus."""
@@ -140,33 +140,33 @@
     
     async def _run_action(self, action, msg):
         sig = signature(action)
         keys = [p.name for p in sig.parameters.values() if p.kind == p.POSITIONAL_OR_KEYWORD and p.annotation == Role]
         kwargs = {k: self for k in keys}
         pos = [p for p in sig.parameters.values() if p.kind == p.POSITIONAL_OR_KEYWORD and p.annotation != Role]
         for p in pos:
-            if not msg.instruct_content and isinstance(msg.content, str):
+            if not msg.data and isinstance(msg.content, str):
                 kwargs[p.name] = msg.content
                 msg.processed_by.add(self)
                 break
-            elif msg.instruct_content and isinstance(msg.instruct_content, p.annotation.__args__ if isinstance(p.annotation, typing._UnionGenericAlias) else p.annotation):
-                kwargs[p.name] = msg.instruct_content
+            elif msg.data and isinstance(msg.data, p.annotation.__args__ if isinstance(p.annotation, typing._UnionGenericAlias) else p.annotation):
+                kwargs[p.name] = msg.data
                 msg.processed_by.add(self)
                 break
             if p.name not in kwargs:
                 kwargs[p.name] = None
         
         if inspect.iscoroutinefunction(action):
             return await action(**kwargs)
         else:
             return action(**kwargs)
 
     def can_handle(self, message: Message) -> bool:
         """Check if the role can handle the message."""
-        context_class = message.instruct_content.__class__ if message.instruct_content else type(message.content)
+        context_class = message.data.__class__ if message.data else type(message.content)
         if context_class in self._input_schemas:
             return True
         return False
     
     # @retry(stop=stop_after_attempt(2), wait=wait_fixed(1))
     async def handle(self, msg: Union[str, Message]) -> list[Message]:
         """Handle message"""
@@ -179,15 +179,15 @@
         messages = []
         def on_message(new_msg):
             if session_id in new_msg.session_ids:
                 messages.append(new_msg)
 
         self._event_bus.on("message", on_message)
         try:
-            context_class = msg.instruct_content.__class__ if msg.instruct_content else type(msg.content)
+            context_class = msg.data.__class__ if msg.data else type(msg.content)
             responses = []
             if context_class in self._input_schemas:
                 actions = self._action_index[context_class]
                 for action in actions:
                     responses.append(self._run_action(action, msg))
             responses = await asyncio.gather(*responses)
             outputs = []  
@@ -195,15 +195,15 @@
                 if not response:
                     continue
                 # logger.info(response)
                 if isinstance(response, str):
                     output = Message(content=response, role=self.profile, cause_by=action, session_ids=msg.session_ids.copy())
                 else:
                     assert isinstance(response, BaseModel), f"Action must return pydantic BaseModel, but got {response}"
-                    output = Message(content=response.json(), instruct_content=response, session_ids=msg.session_ids.copy(),
+                    output = Message(content=response.json(), data=response, session_ids=msg.session_ids.copy(),
                                 role=self.profile, cause_by=action)
                 # self._rc.memory.add(output)
                 # logger.debug(f"{response}")
                 outputs.append(output)
                 await self._event_bus.aemit("message", output)
         finally:
             self._event_bus.off("message", on_message)
```

### Comparing `schema-agents-0.1.7/schema_agents/schema.py` & `schema-agents-0.1.8/schema_agents/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     role: str
 
 
 @dataclass
 class Message:
     """list[<role>: <content>]"""
     content: str
-    instruct_content: BaseModel = field(default=None)
+    data: BaseModel = field(default=None)
     role: str = field(default='user')  # system / user / assistant
     cause_by: Callable = field(default=None)
     processed_by: set['Role'] = field(default_factory=set)
     session_ids: list[str] = field(default_factory=list)
 
     def __str__(self):
         return f"{self.role}: {self.content}"
```

### Comparing `schema-agents-0.1.7/schema_agents/teams/__init__.py` & `schema-agents-0.1.8/schema_agents/teams/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/teams/databse_explore_hub/__init__.py` & `schema-agents-0.1.8/schema_agents/teams/databse_explore_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/teams/databse_explore_hub/database_explorer.py` & `schema-agents-0.1.8/schema_agents/teams/databse_explore_hub/database_explorer.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/__init__.py` & `schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/data_engineer.py` & `schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/data_engineer.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
     DataEngineer = create_data_engineer(client=create_mock_client())
     ds = DataEngineer()
 
     pr = SoftwareRequirement.parse_obj(mock_software_requirements)
     req = Message(
         content=pr.json(),
-        instruct_content=pr,
+        data=pr,
         role="Project Manager",
     )
 
     event_bus = ds.get_event_bus()
     event_bus.register_default_events()
     messages = await ds.handle(req)
     print(messages)
```

### Comparing `schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/microscopist.py` & `schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/microscopist.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,24 +88,24 @@
         constraints=None,
         actions=[microscope.plan, microscope.multi_dimensional_acquisition],
         event_bus=event_bus
     )
 
     messages = await ms.handle(Message(content="acquire an image and save to /tmp/img.png", role="User"))
     assert len(messages) == 2
-    assert isinstance(messages[-1].instruct_content, ExecutionResult)
-    assert messages[-1].instruct_content.status == "ok"
+    assert isinstance(messages[-1].data, ExecutionResult)
+    assert messages[-1].data.status == "ok"
 
     messages = await ms.handle(Message(content="acquire image every 2nm along x, y in a 2x2um square, gradually increase exposure time from 0.1 to 2.0s", role="User"))
     assert len(messages) == 2
-    assert isinstance(messages[-1].instruct_content, ExecutionResult)
-    assert messages[-1].instruct_content.status == "ok"
+    assert isinstance(messages[-1].data, ExecutionResult)
+    assert messages[-1].data.status == "ok"
 
 
     messages = await ms.handle(Message(content="acquire an image every 1 second for 10 seconds", role="User"))
     assert len(messages) == 2
-    assert isinstance(messages[-1].instruct_content, ExecutionResult)
-    assert messages[-1].instruct_content.status == "ok"
+    assert isinstance(messages[-1].data, ExecutionResult)
+    assert messages[-1].data.status == "ok"
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/schemas.py` & `schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/schemas.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/teams/image_analysis_hub/web_developer.py` & `schema-agents-0.1.8/schema_agents/teams/image_analysis_hub/web_developer.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,18 +126,18 @@
             );
         """
     }
     # context['plugin'] = ReactUI.parse_obj(mock_plugin)
     WebDeveloper = create_web_developer(client=create_mock_client())
     wd = WebDeveloper()
     pr = SoftwareRequirement.parse_obj(mock_software_requirements)
-    req = Message(content=pr.json(), instruct_content=pr, role="Project Manager")
+    req = Message(content=pr.json(), data=pr, role="Project Manager")
     resp = await wd.handle(req)
     print(resp)
     if context is not None:
-        context['plugin'] = resp[0].instruct_content
+        context['plugin'] = resp[0].data
     
 
 if __name__ == "__main__":
     context = {}
     asyncio.run(main(context))
     serve_plugin(context['plugin'])
```

### Comparing `schema-agents-0.1.7/schema_agents/tools/binder.py` & `schema-agents-0.1.8/schema_agents/tools/binder.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/tools/code_interpreter.py` & `schema-agents-0.1.8/schema_agents/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/tools/msgspec_v5.py` & `schema-agents-0.1.8/schema_agents/tools/msgspec_v5.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/tools/ray_utils.py` & `schema-agents-0.1.8/schema_agents/tools/ray_utils.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/utils/__init__.py` & `schema-agents-0.1.8/schema_agents/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/utils/common.py` & `schema-agents-0.1.8/schema_agents/utils/common.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/utils/mermaid.py` & `schema-agents-0.1.8/schema_agents/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/utils/serialize.py` & `schema-agents-0.1.8/schema_agents/utils/serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,19 +39,19 @@
         elif property['type'] == 'array' and property['items']['type'] == 'array':
             # here only consider the `Tuple[str, str]` situation
             mapping[field] = (List[Tuple[str, str]], ...)
     return mapping
 
 class ActionOutput:
     content: str
-    instruct_content: BaseModel
+    data: BaseModel
 
-    def __init__(self, content: str, instruct_content: BaseModel):
+    def __init__(self, content: str, data: BaseModel):
         self.content = content
-        self.instruct_content = instruct_content
+        self.data = data
 
     @classmethod
     def create_model_class(cls, class_name: str, mapping: Dict[str, Type]):
         new_class = create_model(class_name, **mapping)
 
         @validator('*', allow_reuse=True)
         def check_name(v, field):
@@ -68,45 +68,45 @@
             return values
 
         new_class.__validator_check_name = classmethod(check_name)
         new_class.__root_validator_check_missing_fields = classmethod(check_missing_fields)
         return new_class
 
 def serialize_message(message: Message):
-    message_cp = copy.deepcopy(message)  # avoid `instruct_content` value update by reference
-    ic = message_cp.instruct_content
+    message_cp = copy.deepcopy(message)  # avoid `data` value update by reference
+    ic = message_cp.data
     if ic:
         # model create by pydantic create_model like `pydantic.main.prd`, can't pickle.dump directly
         schema = ic.schema()
         mapping = actionoutout_schema_to_mapping(schema)
 
-        message_cp.instruct_content = {
+        message_cp.data = {
             'class': schema['title'],
             'mapping': mapping,
             'value': ic.dict()
         }
     msg_ser = pickle.dumps(message_cp)
 
     return msg_ser
 
 
 def deserialize_message(message_ser: str) -> Message:
     message = pickle.loads(message_ser)
-    if message.instruct_content:
-        ic = message.instruct_content
+    if message.data:
+        ic = message.data
         ic_obj = ActionOutput.create_model_class(class_name=ic['class'],
                                                  mapping=ic['mapping'])
         ic_new = ic_obj(**ic['value'])
-        message.instruct_content = ic_new
+        message.data = ic_new
 
     return message
 
 
 def serialize_memory(memory: MemoryChunk):
-    memory_cp = copy.deepcopy(memory)  # avoid `instruct_content` value update by reference
+    memory_cp = copy.deepcopy(memory)  # avoid `data` value update by reference
     ic = memory_cp.content
     if ic:
         # model create by pydantic create_model like `pydantic.main.prd`, can't pickle.dump directly
         schema = ic.schema()
         mapping = actionoutout_schema_to_mapping(schema)
 
         memory_cp.content = {
```

### Comparing `schema-agents-0.1.7/schema_agents/utils/singleton.py` & `schema-agents-0.1.8/schema_agents/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents/utils/token_counter.py` & `schema-agents-0.1.8/schema_agents/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/schema_agents.egg-info/PKG-INFO` & `schema-agents-0.1.8/schema_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-agents
-Version: 0.1.7
+Version: 0.1.8
 Summary: A schema-based LLM framework for building multi-agent collaborative systems.
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.21.2
 Requires-Dist: jsonschema>=4.0.1
 Requires-Dist: shortuuid>=1.0.1
 Requires-Dist: pydantic<2,>=1.8.2
 Requires-Dist: openai>=0.27.0
```

### Comparing `schema-agents-0.1.7/schema_agents.egg-info/SOURCES.txt` & `schema-agents-0.1.8/schema_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/tests/test_code_interpreter.py` & `schema-agents-0.1.8/tests/test_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/tests/test_hypha_ai_chat.py` & `schema-agents-0.1.8/tests/test_hypha_ai_chat.py`

 * *Files identical despite different names*

### Comparing `schema-agents-0.1.7/tests/test_role.py` & `schema-agents-0.1.8/tests/test_role.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         goal="Provide the use case and requirements for the development, the aim is to create a cell counting software for U2OS cells under confocal microscope, I would like to use web interface in Imjoy.",
         constraints=None,
         actions=[get_user_response])
     user.get_event_bus().register_default_events()
     # create a form_schema for get user name
     form_schema = json.dumps({"title": "Get User Name", "type": "object", "properties": {"name": {"type": "string"}}})
     form_dialog = FormDialogInfo(form_schema=form_schema)
-    msg = Message(content=form_dialog.json(), instruct_content=form_dialog, role="Boss")
+    msg = Message(content=form_dialog.json(), data=form_dialog, role="Boss")
     responses = await user.handle(msg)
-    assert isinstance(responses[0].instruct_content, UserClarification)
+    assert isinstance(responses[0].data, UserClarification)
 
 @pytest.mark.asyncio
 async def test_schema_str_input():
     async def create_user_requirements(query: str, role: Role) -> SoftwareRequirementDocument:
         """Create user requirements."""
         response = await role.aask(query, Union[SoftwareRequirementDocument, GetExtraInformation])
         if isinstance(response, SoftwareRequirementDocument):
@@ -86,31 +86,31 @@
     bioimage_analyst = Role(name="Alice",
                 profile="BioImage Analyst",
                 goal="Efficiently communicate with the user and translate the user's needs into software requirements",
                 constraints=None,
                 actions=[create_user_requirements])
     bioimage_analyst.get_event_bus().register_default_events()
     responses = await bioimage_analyst.handle(Message(role="Bot", content="Create a segmentation software"))
-    assert isinstance(responses[0].instruct_content, SoftwareRequirementDocument)
+    assert isinstance(responses[0].data, SoftwareRequirementDocument)
 
 @pytest.mark.asyncio
 async def test_schemas():
     user = Role(name="Bob",
                 profile="User",
                 goal="Provide the use case and requirements for the development, the aim is to create a cell counting software for U2OS cells under confocal microscope, I would like to use web interface in Imjoy.",
                 constraints=None,
                 actions=[clarify, search_internet])
     user.get_event_bus().register_default_events()
     responses = await user.handle(Message(role="Bot", content="Find more information on the internet about cell counting software."))
-    assert responses[0].instruct_content is None
+    assert responses[0].data is None
     assert responses[0].content == "Nothing found"
 
     instruct = GetExtraInformation(content="Tell me the use case in 1 sentence.", summary="Requesting details about the use case")
-    responses = await user.handle(Message(role="Bot", content=instruct.json(), instruct_content=instruct))
-    assert isinstance(responses[0].instruct_content, UserClarification)
+    responses = await user.handle(Message(role="Bot", content=instruct.json(), data=instruct))
+    assert isinstance(responses[0].data, UserClarification)
 
 
 
 @pytest.mark.asyncio
 async def test_schema_str():
     async def process_user_input(query: GetExtraInformation, role: Role) -> str:
         """Process user input."""
@@ -120,9 +120,9 @@
     user = Role(name="Bob",
                 profile="User",
                 goal="Provide the use case and requirements for the development, the aim is to create a cell counting software for U2OS cells under confocal microscope, I would like to use web interface in Imjoy.",
                 constraints=None,
                 actions=[process_user_input])
     user.get_event_bus().register_default_events()
     instruct = GetExtraInformation(content="Tell me the use case in 1 sentence.", summary="Requesting details about the use case")
-    responses = await user.handle(Message(role="Bot", content=instruct.json(), instruct_content=instruct))
-    assert isinstance(responses[0].instruct_content, SearchInternetQuery)
+    responses = await user.handle(Message(role="Bot", content=instruct.json(), data=instruct))
+    assert isinstance(responses[0].data, SearchInternetQuery)
```

### Comparing `schema-agents-0.1.7/tests/test_team.py` & `schema-agents-0.1.8/tests/test_team.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,11 +40,11 @@
                 actions=[write_code])
     
     team = Team(name="Test Team")
     team.hire([bioimage_analyst, coder])
     event_bus = team.get_event_bus()
     event_bus.register_default_events()
     responses = await team.handle(Message(role="Bot", content="Create a segmentation software"))
-    assert isinstance(responses[1].instruct_content, SoftwareRequirementDocument)
-    assert isinstance(responses[2].instruct_content, AnalysisScript)
+    assert isinstance(responses[1].data, SoftwareRequirementDocument)
+    assert isinstance(responses[2].data, AnalysisScript)
```

