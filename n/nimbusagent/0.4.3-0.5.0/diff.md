# Comparing `tmp/nimbusagent-0.4.3.tar.gz` & `tmp/nimbusagent-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbusagent-0.4.3.tar", last modified: Fri Jan 26 21:48:27 2024, max compression
+gzip compressed data, was "nimbusagent-0.5.0.tar", last modified: Fri Apr  5 21:28:58 2024, max compression
```

## Comparing `nimbusagent-0.4.3.tar` & `nimbusagent-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.864926 nimbusagent-0.4.3/
--rw-r--r--   0 Lee        (501) staff       (20)     3101 2023-12-04 18:36:26.000000 nimbusagent-0.4.3/.gitignore
--rw-r--r--   0 Lee        (501) staff       (20)     1073 2023-12-06 18:57:23.000000 nimbusagent-0.4.3/LICENSE.txt
--rw-r--r--   0 Lee        (501) staff       (20)       48 2023-11-18 23:57:46.000000 nimbusagent-0.4.3/MANIFEST.in
--rw-r--r--   0 Lee        (501) staff       (20)    10298 2024-01-26 21:48:27.864175 nimbusagent-0.4.3/PKG-INFO
--rw-r--r--   0 Lee        (501) staff       (20)     7763 2024-01-26 20:49:40.000000 nimbusagent-0.4.3/README.md
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.782782 nimbusagent-0.4.3/bin/
--rwxr-xr-x   0 Lee        (501) staff       (20)      384 2023-12-26 20:55:01.000000 nimbusagent-0.4.3/bin/build.sh
--rwxr-xr-x   0 Lee        (501) staff       (20)      209 2023-12-22 17:10:13.000000 nimbusagent-0.4.3/bin/publish-pypi.sh
--rwxr-xr-x   0 Lee        (501) staff       (20)      240 2023-12-22 17:34:16.000000 nimbusagent-0.4.3/bin/run_tests.sh
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.800553 nimbusagent-0.4.3/examples/
--rw-r--r--   0 Lee        (501) staff       (20)      277 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/examples/completion_agent_basic_example.py
--rw-r--r--   0 Lee        (501) staff       (20)     1532 2023-12-26 21:17:23.000000 nimbusagent-0.4.3/examples/completion_agent_function_example.py
--rw-r--r--   0 Lee        (501) staff       (20)      427 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/examples/completion_agent_history_example.py
--rw-r--r--   0 Lee        (501) staff       (20)      362 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/examples/streaming_agent_basic_example.py
--rw-r--r--   0 Lee        (501) staff       (20)     1620 2023-12-26 21:17:23.000000 nimbusagent-0.4.3/examples/streaming_agent_function_example.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.809314 nimbusagent-0.4.3/examples/streaming_cli_chatbot/
--rw-r--r--   0 Lee        (501) staff       (20)     2376 2023-12-04 18:36:26.000000 nimbusagent-0.4.3/examples/streaming_cli_chatbot/simple_spinner.py
--rw-r--r--   0 Lee        (501) staff       (20)     2999 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/examples/streaming_cli_chatbot/streaming_cli_chatbot.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.809906 nimbusagent-0.4.3/nimbusagent/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/nimbusagent/__init__.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.827015 nimbusagent-0.4.3/nimbusagent/agent/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/nimbusagent/agent/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)    13097 2024-01-26 20:49:40.000000 nimbusagent-0.4.3/nimbusagent/agent/base.py
--rw-r--r--   0 Lee        (501) staff       (20)     5002 2023-12-26 21:17:23.000000 nimbusagent-0.4.3/nimbusagent/agent/completion.py
--rw-r--r--   0 Lee        (501) staff       (20)    12365 2024-01-05 21:11:54.000000 nimbusagent-0.4.3/nimbusagent/agent/streaming.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.835339 nimbusagent-0.4.3/nimbusagent/functions/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/nimbusagent/functions/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)    17923 2024-01-26 20:49:40.000000 nimbusagent-0.4.3/nimbusagent/functions/handler.py
--rw-r--r--   0 Lee        (501) staff       (20)     9997 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/nimbusagent/functions/parser.py
--rw-r--r--   0 Lee        (501) staff       (20)     2293 2023-12-26 21:17:23.000000 nimbusagent-0.4.3/nimbusagent/functions/responses.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.838915 nimbusagent-0.4.3/nimbusagent/memory/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/nimbusagent/memory/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     5417 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/nimbusagent/memory/base.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.840100 nimbusagent-0.4.3/nimbusagent/utils/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/nimbusagent/utils/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     4246 2024-01-26 21:46:54.000000 nimbusagent-0.4.3/nimbusagent/utils/helper.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.863581 nimbusagent-0.4.3/nimbusagent.egg-info/
--rw-r--r--   0 Lee        (501) staff       (20)    10298 2024-01-26 21:48:27.000000 nimbusagent-0.4.3/nimbusagent.egg-info/PKG-INFO
--rw-r--r--   0 Lee        (501) staff       (20)     1259 2024-01-26 21:48:27.000000 nimbusagent-0.4.3/nimbusagent.egg-info/SOURCES.txt
--rw-r--r--   0 Lee        (501) staff       (20)        1 2024-01-26 21:48:27.000000 nimbusagent-0.4.3/nimbusagent.egg-info/dependency_links.txt
--rw-r--r--   0 Lee        (501) staff       (20)       60 2024-01-26 21:48:27.000000 nimbusagent-0.4.3/nimbusagent.egg-info/requires.txt
--rw-r--r--   0 Lee        (501) staff       (20)       12 2024-01-26 21:48:27.000000 nimbusagent-0.4.3/nimbusagent.egg-info/top_level.txt
--rw-r--r--   0 Lee        (501) staff       (20)     1365 2024-01-26 20:49:40.000000 nimbusagent-0.4.3/pyproject.toml
--rw-r--r--   0 Lee        (501) staff       (20)       38 2024-01-26 21:48:27.865069 nimbusagent-0.4.3/setup.cfg
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-01-26 21:48:27.862976 nimbusagent-0.4.3/tests/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 18:36:26.000000 nimbusagent-0.4.3/tests/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     1961 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/tests/test_nimbusagent_agent_base.py
--rw-r--r--   0 Lee        (501) staff       (20)     1012 2023-12-26 21:17:23.000000 nimbusagent-0.4.3/tests/test_nimbusagent_functions_handler.py
--rw-r--r--   0 Lee        (501) staff       (20)     1874 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/tests/test_nimbusagent_functions_parser.py
--rw-r--r--   0 Lee        (501) staff       (20)      607 2023-12-26 21:17:23.000000 nimbusagent-0.4.3/tests/test_nimbusagent_functions_response.py
--rw-r--r--   0 Lee        (501) staff       (20)     4619 2023-12-04 21:15:51.000000 nimbusagent-0.4.3/tests/test_nimbusagent_memory_base.py
--rw-r--r--   0 Lee        (501) staff       (20)     6772 2024-01-05 19:48:38.000000 nimbusagent-0.4.3/tests/test_nimbusagent_utils.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.600841 nimbusagent-0.5.0/
+-rw-r--r--   0 Lee        (501) staff       (20)     3101 2023-12-04 18:36:26.000000 nimbusagent-0.5.0/.gitignore
+-rw-r--r--   0 Lee        (501) staff       (20)     1073 2023-12-06 18:57:23.000000 nimbusagent-0.5.0/LICENSE.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       48 2023-11-18 23:57:46.000000 nimbusagent-0.5.0/MANIFEST.in
+-rw-r--r--   0 Lee        (501) staff       (20)    10524 2024-04-05 21:28:58.600142 nimbusagent-0.5.0/PKG-INFO
+-rw-r--r--   0 Lee        (501) staff       (20)     7989 2024-04-05 21:23:21.000000 nimbusagent-0.5.0/README.md
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.518938 nimbusagent-0.5.0/bin/
+-rwxr-xr-x   0 Lee        (501) staff       (20)      384 2023-12-26 20:55:01.000000 nimbusagent-0.5.0/bin/build.sh
+-rwxr-xr-x   0 Lee        (501) staff       (20)      209 2023-12-22 17:10:13.000000 nimbusagent-0.5.0/bin/publish-pypi.sh
+-rwxr-xr-x   0 Lee        (501) staff       (20)      240 2023-12-22 17:34:16.000000 nimbusagent-0.5.0/bin/run_tests.sh
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.529665 nimbusagent-0.5.0/examples/
+-rw-r--r--   0 Lee        (501) staff       (20)      277 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/examples/completion_agent_basic_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1532 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/examples/completion_agent_function_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)      427 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/examples/completion_agent_history_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)      362 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/examples/streaming_agent_basic_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1620 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/examples/streaming_agent_function_example.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.535663 nimbusagent-0.5.0/examples/streaming_cli_chatbot/
+-rw-r--r--   0 Lee        (501) staff       (20)     2376 2023-12-04 18:36:26.000000 nimbusagent-0.5.0/examples/streaming_cli_chatbot/simple_spinner.py
+-rw-r--r--   0 Lee        (501) staff       (20)     2999 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/examples/streaming_cli_chatbot/streaming_cli_chatbot.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.536218 nimbusagent-0.5.0/nimbusagent/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/__init__.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.549908 nimbusagent-0.5.0/nimbusagent/agent/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/agent/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)    13678 2024-04-05 21:20:08.000000 nimbusagent-0.5.0/nimbusagent/agent/base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     5140 2024-04-05 21:23:21.000000 nimbusagent-0.5.0/nimbusagent/agent/completion.py
+-rw-r--r--   0 Lee        (501) staff       (20)    12843 2024-04-05 21:20:08.000000 nimbusagent-0.5.0/nimbusagent/agent/streaming.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.562969 nimbusagent-0.5.0/nimbusagent/functions/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/functions/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)    17923 2024-01-26 20:49:40.000000 nimbusagent-0.5.0/nimbusagent/functions/handler.py
+-rw-r--r--   0 Lee        (501) staff       (20)     9997 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/functions/parser.py
+-rw-r--r--   0 Lee        (501) staff       (20)     2293 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/nimbusagent/functions/responses.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.567805 nimbusagent-0.5.0/nimbusagent/memory/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/memory/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     5417 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/memory/base.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.573906 nimbusagent-0.5.0/nimbusagent/utils/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/utils/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     4246 2024-01-26 21:46:54.000000 nimbusagent-0.5.0/nimbusagent/utils/helper.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.599536 nimbusagent-0.5.0/nimbusagent.egg-info/
+-rw-r--r--   0 Lee        (501) staff       (20)    10524 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/PKG-INFO
+-rw-r--r--   0 Lee        (501) staff       (20)     1259 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/SOURCES.txt
+-rw-r--r--   0 Lee        (501) staff       (20)        1 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/dependency_links.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       60 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/requires.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       12 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/top_level.txt
+-rw-r--r--   0 Lee        (501) staff       (20)     1365 2024-04-05 21:23:21.000000 nimbusagent-0.5.0/pyproject.toml
+-rw-r--r--   0 Lee        (501) staff       (20)       38 2024-04-05 21:28:58.600921 nimbusagent-0.5.0/setup.cfg
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.598557 nimbusagent-0.5.0/tests/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 18:36:26.000000 nimbusagent-0.5.0/tests/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1961 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/tests/test_nimbusagent_agent_base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1012 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/tests/test_nimbusagent_functions_handler.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1874 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/tests/test_nimbusagent_functions_parser.py
+-rw-r--r--   0 Lee        (501) staff       (20)      607 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/tests/test_nimbusagent_functions_response.py
+-rw-r--r--   0 Lee        (501) staff       (20)     4619 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/tests/test_nimbusagent_memory_base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     6772 2024-01-05 19:48:38.000000 nimbusagent-0.5.0/tests/test_nimbusagent_utils.py
```

### Comparing `nimbusagent-0.4.3/.gitignore` & `nimbusagent-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/LICENSE.txt` & `nimbusagent-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/PKG-INFO` & `nimbusagent-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimbusagent
-Version: 0.4.3
+Version: 0.5.0
 Summary: An OpenAI agent with basic memory, functions, and moderation support
 Author: Lee Huffman
 License: MIT License
         
         Copyright (c) 2023 Vaisala Xweather
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -160,14 +160,15 @@
 #### `functions_embeddings`
 
 - **Description**: Embeddings for the functions to help the AI understand them better.
 - **Type**: `Optional[List[dict]]`
 - **Default**: `None`
 
 #### `functions_embeddings_model`
+
 - **Description**: The name of the OpenAI model to use for generating embeddings for the functions.
 - **Type**: `str`
 - **Default**: `'text-embedding-ada-002'`
 
 #### `functions_always_use`
 
 - **Description**: Functions that should always be used by the agent.
@@ -263,14 +264,20 @@
 #### `max_event_size`
 
 - **Description**: The maximum size of an event in bytes. Allows limiting sending large data streams from a function
   response
 - **Type**: `int`
 - **Default**: `2000`
 
+#### `on_complete`
+- **Description**: Callback function triggered when the agent completes a response. The response is passed as an argument (string)
+  to the callback.
+- **Type**: `Optional[callable]`
+- **Default**: `None`
+
 ### Example of Initialization
 
 Here's an example of how you might initialize a `CompletionAgent` with some of these parameters:
 
 ```python
 agent = CompletionAgent(
     openai_api_key="your_api_key_here",
```

### Comparing `nimbusagent-0.4.3/README.md` & `nimbusagent-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 #### `functions_embeddings`
 
 - **Description**: Embeddings for the functions to help the AI understand them better.
 - **Type**: `Optional[List[dict]]`
 - **Default**: `None`
 
 #### `functions_embeddings_model`
+
 - **Description**: The name of the OpenAI model to use for generating embeddings for the functions.
 - **Type**: `str`
 - **Default**: `'text-embedding-ada-002'`
 
 #### `functions_always_use`
 
 - **Description**: Functions that should always be used by the agent.
@@ -210,14 +211,20 @@
 #### `max_event_size`
 
 - **Description**: The maximum size of an event in bytes. Allows limiting sending large data streams from a function
   response
 - **Type**: `int`
 - **Default**: `2000`
 
+#### `on_complete`
+- **Description**: Callback function triggered when the agent completes a response. The response is passed as an argument (string)
+  to the callback.
+- **Type**: `Optional[callable]`
+- **Default**: `None`
+
 ### Example of Initialization
 
 Here's an example of how you might initialize a `CompletionAgent` with some of these parameters:
 
 ```python
 agent = CompletionAgent(
     openai_api_key="your_api_key_here",
```

### Comparing `nimbusagent-0.4.3/examples/completion_agent_function_example.py` & `nimbusagent-0.5.0/examples/completion_agent_function_example.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/examples/streaming_agent_function_example.py` & `nimbusagent-0.5.0/examples/streaming_agent_function_example.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/examples/streaming_cli_chatbot/simple_spinner.py` & `nimbusagent-0.5.0/examples/streaming_cli_chatbot/simple_spinner.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/examples/streaming_cli_chatbot/streaming_cli_chatbot.py` & `nimbusagent-0.5.0/examples/streaming_cli_chatbot/streaming_cli_chatbot.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/nimbusagent/agent/base.py` & `nimbusagent-0.5.0/nimbusagent/agent/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,16 @@
             memory_max_tokens: int = 2000,
 
             internal_thoughts_max_entries: int = 8,
             loops_max: int = 10,
 
             send_events: bool = False,
             max_event_size: int = 2000,
+
+            on_complete: callable = None,
     ):
         """
         Base Agent Class for Nimbus Agent
 
         Args:
             openai_api_key: the OpenAI API key to use
             model_name: The name of the model to use (default: 'gpt-4-0613')
@@ -85,14 +87,16 @@
                                     (default: "I'm sorry, I can't help you with that as it is not appropriate.")
             memory_max_entries: The maximum number of entries to store in the memory (default: 20)
             memory_max_tokens: The maximum number of tokens to store in the memory (default: 2000)
             internal_thoughts_max_entries: The maximum number of entries to store in the internal thoughts (default: 3)
             loops_max: The maximum number of loops to allow (default: 5)
             send_events: True if events should be sent (default: False)
             max_event_size: The maximum size of an event (default: 2000)
+            on_complete: The callback to call when the agent completes a response.
+                The response is passed to the callable. This can be useful with streaming. (default: None)
         """
 
         self.client = OpenAI(api_key=openai_api_key if openai_api_key is not None else os.getenv("OPENAI_API_KEY"))
 
         # self.internal_thoughts: A list that captures the agent's intermediate
         # processing and thoughts during a single 'ask' session. It gets cleared
         # at the beginning of every new 'ask' to ensure no residual information
@@ -109,14 +113,15 @@
         self.perform_moderation = perform_moderation
         self.moderation_fail_message = moderation_fail_message
         self.loops_max = loops_max
         self.send_events = send_events
         self.max_event_size = max_event_size
         self.calling_function_start_callback = calling_function_start_callback
         self.calling_function_stop_callback = calling_function_stop_callback
+        self.on_complete = on_complete
 
         self.chat_history = AgentMemory(max_messages=memory_max_entries, max_tokens=memory_max_tokens)
         if message_history is not None:
             if self._history_needs_moderation(message_history):
                 raise ValueError('The message history contains inappropriate content.')
             self.chat_history.set_chat_history(message_history)
 
@@ -268,7 +273,16 @@
         :return: The functions
         """
         return self.function_handler.functions
 
     def clear_chat_history(self) -> None:
         """Clears the chat history."""
         self.chat_history.clear_chat_history()
+
+    def handle_on_complete(self) -> None:
+        """Handles the on_complete callback."""
+        if self.on_complete and self.last_response:
+            self.on_complete(self.last_response)
+
+    def _clear_last_response(self) -> None:
+        """Clears the last response."""
+        self.last_response = ""
```

### Comparing `nimbusagent-0.4.3/nimbusagent/agent/completion.py` & `nimbusagent-0.5.0/nimbusagent/agent/completion.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,27 +22,30 @@
         Ask the agent a question and return the response.
         :param query:  The query to ask the agent.
         :return:  The response.
         """
         if self._needs_moderation(query):
             return self.moderation_fail_message
 
+        self._clear_last_response()
         self._clear_internal_thoughts()
         self.function_handler.get_functions_from_query_and_history(query, self.get_chat_history())
         self._append_to_chat_history('user', query)
         res = self._generate_response()
         self.last_response = res
 
         if res is None:
             return None
         elif isinstance(res, str):
             self._append_to_chat_history('function', res)
             return res
         else:
             self._append_to_chat_history(res.choices[0].message.role, res.choices[0].message.content)
+            self.last_response = res.choices[0].message.content
+            self.handle_on_complete()
             return res.choices[0].message.content
 
     # noinspection PyUnresolvedReferences
     def _generate_response(self) -> Optional[Union[openai.types.chat.ChatCompletion, str]]:
         """
         Generate a response object based on the response from the AI
         :return:  The response object.
```

### Comparing `nimbusagent-0.4.3/nimbusagent/agent/streaming.py` & `nimbusagent-0.5.0/nimbusagent/agent/streaming.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         :return:  A generator that yields the response.
         """
         if self._needs_moderation(query):
             yield self.moderation_fail_message
             return
 
         self._clear_internal_thoughts()
+        self._clear_last_response()
         self.function_handler.get_functions_from_query_and_history(query, self.get_chat_history())
         self._append_to_chat_history('user', query)
 
         ai_response = self._generate_streaming_response(max_retries=max_retries)
         content_accumulated = []
         for content in ai_response:
             content_accumulated.append(content)
@@ -52,15 +53,17 @@
             Generate a response from the AI and return a generator that yields the response.
             :return:  A generator that yields the response.
             """
             retries = max_retries
 
             def output_post_content(post_content: List[str]):
                 if post_content:
-                    return f"{' '.join(post_content)}\n"
+                    post_content_str = f"{' '.join(post_content)}\n"
+                    self.last_response += post_content_str
+                    return post_content_str
                 return ""
 
             def output_event(event_type: str, name: str, data: any):
 
                 if not data:
                     return f"[[[{event_type}:{name}]]]"
 
@@ -226,26 +229,35 @@
                                     use_secondary_model = True
                                 if func_results.force_no_functions:
                                     force_no_functions = True
 
                         content = delta.content
                         if content is not None:
                             has_content = True
+                            if self.last_response is None:
+                                self.last_response = content
+                            else:
+                                self.last_response += content
+
                             yield delta.content
 
                         if message.choices[0].finish_reason == 'stop':
                             yield output_post_content(post_content_items)
+
+                            self.handle_on_complete()
                             return
                         if len(self.internal_thoughts) > self.internal_thoughts_max_entries:
                             if post_content_items:
                                 yield output_post_content(post_content_items)
                             else:
                                 num_thoughts = len(self.internal_thoughts)
                                 logging.error(f"Too many internal thoughts: {num_thoughts}.")
                                 yield "Too many internal thoughts."
+
+                            self.handle_on_complete()
                             return
 
                 except Exception as e:
                     logging.error("Exception encountered: %s (%s)", str(e), type(e).__name__, exc_info=True)
 
                     if retries > 0 and not has_content:
                         retries -= 1
```

### Comparing `nimbusagent-0.4.3/nimbusagent/functions/handler.py` & `nimbusagent-0.5.0/nimbusagent/functions/handler.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/nimbusagent/functions/parser.py` & `nimbusagent-0.5.0/nimbusagent/functions/parser.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/nimbusagent/functions/responses.py` & `nimbusagent-0.5.0/nimbusagent/functions/responses.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/nimbusagent/memory/base.py` & `nimbusagent-0.5.0/nimbusagent/memory/base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/nimbusagent/utils/helper.py` & `nimbusagent-0.5.0/nimbusagent/utils/helper.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/nimbusagent.egg-info/PKG-INFO` & `nimbusagent-0.5.0/nimbusagent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimbusagent
-Version: 0.4.3
+Version: 0.5.0
 Summary: An OpenAI agent with basic memory, functions, and moderation support
 Author: Lee Huffman
 License: MIT License
         
         Copyright (c) 2023 Vaisala Xweather
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -160,14 +160,15 @@
 #### `functions_embeddings`
 
 - **Description**: Embeddings for the functions to help the AI understand them better.
 - **Type**: `Optional[List[dict]]`
 - **Default**: `None`
 
 #### `functions_embeddings_model`
+
 - **Description**: The name of the OpenAI model to use for generating embeddings for the functions.
 - **Type**: `str`
 - **Default**: `'text-embedding-ada-002'`
 
 #### `functions_always_use`
 
 - **Description**: Functions that should always be used by the agent.
@@ -263,14 +264,20 @@
 #### `max_event_size`
 
 - **Description**: The maximum size of an event in bytes. Allows limiting sending large data streams from a function
   response
 - **Type**: `int`
 - **Default**: `2000`
 
+#### `on_complete`
+- **Description**: Callback function triggered when the agent completes a response. The response is passed as an argument (string)
+  to the callback.
+- **Type**: `Optional[callable]`
+- **Default**: `None`
+
 ### Example of Initialization
 
 Here's an example of how you might initialize a `CompletionAgent` with some of these parameters:
 
 ```python
 agent = CompletionAgent(
     openai_api_key="your_api_key_here",
```

### Comparing `nimbusagent-0.4.3/nimbusagent.egg-info/SOURCES.txt` & `nimbusagent-0.5.0/nimbusagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/pyproject.toml` & `nimbusagent-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nimbusagent"
-version = "0.4.3"
+version = "0.5.0"
 description = "An OpenAI agent with basic memory, functions, and moderation support"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 keywords = [
     "openai",
     "gpt3",
     "gpt3.5",
```

### Comparing `nimbusagent-0.4.3/tests/test_nimbusagent_agent_base.py` & `nimbusagent-0.5.0/tests/test_nimbusagent_agent_base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/tests/test_nimbusagent_functions_handler.py` & `nimbusagent-0.5.0/tests/test_nimbusagent_functions_handler.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/tests/test_nimbusagent_functions_parser.py` & `nimbusagent-0.5.0/tests/test_nimbusagent_functions_parser.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/tests/test_nimbusagent_functions_response.py` & `nimbusagent-0.5.0/tests/test_nimbusagent_functions_response.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/tests/test_nimbusagent_memory_base.py` & `nimbusagent-0.5.0/tests/test_nimbusagent_memory_base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.4.3/tests/test_nimbusagent_utils.py` & `nimbusagent-0.5.0/tests/test_nimbusagent_utils.py`

 * *Files identical despite different names*

