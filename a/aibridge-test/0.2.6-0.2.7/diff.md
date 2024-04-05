# Comparing `tmp/aibridge_test-0.2.6.tar.gz` & `tmp/aibridge_test-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.2.6.tar", last modified: Thu Apr  4 11:50:25 2024, max compression
+gzip compressed data, was "aibridge_test-0.2.7.tar", last modified: Fri Apr  5 09:42:12 2024, max compression
```

## Comparing `aibridge_test-0.2.6.tar` & `aibridge_test-0.2.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.413412 aibridge_test-0.2.6/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.050423 aibridge_test-0.2.6/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.6/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.152414 aibridge_test-0.2.6/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.6/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    12813 2024-04-04 11:48:13.000000 aibridge_test-0.2.6/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0     8851 2024-04-02 05:11:27.000000 aibridge_test-0.2.6/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14053 2024-04-04 11:46:45.000000 aibridge_test-0.2.6/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.6/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11525 2024-04-04 09:42:06.000000 aibridge_test-0.2.6/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.6/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.6/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.6/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.181416 aibridge_test-0.2.6/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     6650 2024-04-04 09:20:56.000000 aibridge_test-0.2.6/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      729 2024-04-04 03:51:54.000000 aibridge_test-0.2.6/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.237414 aibridge_test-0.2.6/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.256416 aibridge_test-0.2.6/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.6/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.279428 aibridge_test-0.2.6/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.6/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.6/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.301416 aibridge_test-0.2.6/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.331417 aibridge_test-0.2.6/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.6/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    21533 2024-04-04 11:50:25.410415 aibridge_test-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 11:50:25.404415 aibridge_test-0.2.6/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21533 2024-04-04 11:50:24.000000 aibridge_test-0.2.6/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-04-04 11:50:24.000000 aibridge_test-0.2.6/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:50:24.000000 aibridge_test-0.2.6/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      227 2024-04-04 11:50:24.000000 aibridge_test-0.2.6/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-04 11:50:24.000000 aibridge_test-0.2.6/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 11:50:25.415413 aibridge_test-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2862 2024-04-04 11:49:03.000000 aibridge_test-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.274545 aibridge_test-0.2.7/
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:11.957546 aibridge_test-0.2.7/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.7/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.042545 aibridge_test-0.2.7/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.7/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    12813 2024-04-04 11:48:13.000000 aibridge_test-0.2.7/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    11900 2024-04-05 09:25:51.000000 aibridge_test-0.2.7/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14053 2024-04-04 11:46:45.000000 aibridge_test-0.2.7/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.7/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11525 2024-04-04 09:42:06.000000 aibridge_test-0.2.7/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.7/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.7/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.7/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.057546 aibridge_test-0.2.7/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7564 2024-04-05 09:34:27.000000 aibridge_test-0.2.7/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.2.7/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.091546 aibridge_test-0.2.7/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.109542 aibridge_test-0.2.7/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.7/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.133544 aibridge_test-0.2.7/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.7/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.7/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.151561 aibridge_test-0.2.7/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.174552 aibridge_test-0.2.7/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.7/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-04-05 09:42:12.270546 aibridge_test-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.258543 aibridge_test-0.2.7/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 09:42:12.275545 aibridge_test-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-04-05 08:20:15.000000 aibridge_test-0.2.7/setup.py
```

### Comparing `aibridge_test-0.2.6/AIBridge/__init__.py` & `aibridge_test-0.2.7/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.2.7/AIBridge/ai_services/ai21labs_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.2.7/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.2.7/AIBridge/ai_services/anthropic_ai.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.2.7/AIBridge/ai_services/palm_text.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import cohere
 import time
 import uuid
-from AIBridge.exceptions import CohereException, AIBridgeException
+from AIBridge.exceptions import PalmTextException, AIBridgeException
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import parse_fromat, parse_api_key
+import google.generativeai as palm
 from AIBridge.output_validation.convertors import FromJson, IntoJson
 
 
-class CohereApi(AIInterface):
+class PalmText(AIInterface):
     """
-    Base class for OpenAI Services
+    Base class for PalmText's Services
     """
 
     @classmethod
     def generate(
         self,
         prompts: list[str] = [],
         prompt_ids: list[str] = [],
         prompt_data: list[dict] = [],
         variables: list[dict] = [],
         output_format: list[str] = [],
         format_strcture: list[str] = [],
-        model="command-nightly",
+        model="models/text-bison-001",
         variation_count: int = 1,
-        max_tokens: int = 3500,  # max 4096
+        max_tokens: int = 10000,
         temperature: float = 0.5,
         message_queue=False,
         api_key=None,
         output_format_parse=True,
         context=[],
     ):
         try:
             if prompts and prompt_ids:
-                raise CohereException(
-                    "please provide either prompts or prompts ids at time"
+                raise PalmTextException(
+                    "please provide either prompts or prompts ids at atime"
                 )
             if not prompts and not prompt_ids:
-                raise CohereException(
+                raise PalmTextException(
                     "Either provide prompts or prompts ids to genrate the data"
                 )
             if prompt_ids:
                 prompts_list = Completion.create_prompt_from_id(
                     prompt_ids=prompt_ids,
                     prompt_data_list=prompt_data,
                     variables_list=variables,
@@ -87,15 +87,15 @@
                 message_data = {
                     "id": str(id),
                     "prompts": json.dumps(updated_prompts),
                     "model": model,
                     "variation_count": variation_count,
                     "max_tokens": max_tokens,
                     "temperature": temperature,
-                    "ai_service": "cohere_api",
+                    "ai_service": "palm_api",
                     "output_format": json.dumps(output_format),
                     "format_structure": json.dumps(format_strcture),
                     "api_key": api_key,
                     "context": context,
                 }
                 message = {"data": json.dumps(message_data)}
                 from AIBridge.queue_integration.message_queue import MessageQ
@@ -110,76 +110,83 @@
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
         except AIBridgeException as e:
-            raise CohereException(f"Error in generating AI data {e}")
+            raise PalmTextException(f"Error in generating AI data {e}")
+
+    @classmethod
+    def get_tokens(Self, model, text):
+        tokens = palm.count_text_tokens(model=model, prompt=text)
+        return tokens["token_count"]
 
     @classmethod
     def get_prompt_context(self, context):
         context_string = ""
         for _context in context:
             if _context["role"] not in ["user", "system", "assistant"]:
-                raise CohereException(
+                raise PalmTextException(
                     "Invalid role provided. Please provide either user or system, assistant"
                 )
             context_string = (
                 context_string + f"{_context['role']}:{_context['context']}" + "\n"
             )
         return context_string
 
     @classmethod
     def get_response(
         self,
         prompts,
-        model="command-nightly",
+        model="models/text-bison-001",
         variation_count=1,
-        max_tokens=3500,  # max 4096
+        max_tokens=10000,
         temperature=0.5,
         output_format=[],
         format_structure=[],
         api_key=None,
         context=[],
     ):
         try:
             if output_format:
                 if isinstance(output_format, str):
                     output_format = json.loads(output_format)
             if format_structure:
                 if isinstance(format_structure, str):
                     format_structure = json.loads(format_structure)
             if not prompts:
-                raise CohereException("No prompts provided")
-            API_KEY = api_key if api_key else parse_api_key("cohere_api")
-            co = cohere.Client(API_KEY)
+                raise PalmTextException("No prompts provided")
+            api_key = api_key if api_key else parse_api_key("palm_api")
+            palm.configure(api_key=api_key)
             model_output = []
+            token_used = 0
             context_string = self.get_prompt_context(context)
-            token_used = max_tokens
-            for ind, prompt in enumerate(prompts):
+            for index, prompt in enumerate(prompts):
                 prompt = context_string + "\n" + prompt
-                response = co.generate(
+                response = palm.generate_text(
                     model=model,
                     prompt=prompt,
-                    max_tokens=max_tokens,
                     temperature=temperature,
-                    num_generations=variation_count,
+                    max_output_tokens=max_tokens,
+                    candidate_count=variation_count,
                 )
-                for index, res in enumerate(response.generations):
-                    content = res.text
+                token_used = token_used + self.get_tokens(model, prompt)
+                for res in response.candidates:
+                    content = res["output"]
+                    token_used = token_used + self.get_tokens(model, content)
                     if output_format:
-                        _formatter = output_format[ind]
+                        _formatter = output_format[index]
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(json.loads(content))
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(json.loads(content))
                         except AIBridgeException as e:
-                            raise CohereException(
+                            raise PalmTextException(
                                 f"Ai response is not in valid {_formatter}"
                             )
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
@@ -202,13 +209,13 @@
                     else:
                         model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
                     "token_used": token_used,
                     "created_at": time.time(),
-                    "ai_service": "open_ai",
+                    "ai_service": "palm_api",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise CohereException(f"{e}")
+            raise PalmTextException(f"{e}")
```

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.2.7/AIBridge/ai_services/geminin_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.2.7/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.2.7/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.2.7/AIBridge/ai_services/openai_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.2.7/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.2.7/AIBridge/ai_services/cohere_llm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,50 @@
+import cohere
 import time
 import uuid
-from AIBridge.exceptions import PalmTextException, AIBridgeException
+from AIBridge.exceptions import CohereException, AIBridgeException
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import parse_fromat, parse_api_key
-import google.generativeai as palm
 from AIBridge.output_validation.convertors import FromJson, IntoJson
+from AIBridge.constant.common import get_function_from_json
 
 
-class PalmText(AIInterface):
+class CohereApi(AIInterface):
     """
-    Base class for PalmText's Services
+    Base class for OpenAI Services
     """
 
     @classmethod
     def generate(
         self,
         prompts: list[str] = [],
         prompt_ids: list[str] = [],
         prompt_data: list[dict] = [],
         variables: list[dict] = [],
         output_format: list[str] = [],
         format_strcture: list[str] = [],
-        model="models/text-bison-001",
+        model="command-nightly",
         variation_count: int = 1,
-        max_tokens: int = 10000,
+        max_tokens: int = 3500,  # max 4096
         temperature: float = 0.5,
         message_queue=False,
         api_key=None,
         output_format_parse=True,
         context=[],
     ):
         try:
             if prompts and prompt_ids:
-                raise PalmTextException(
-                    "please provide either prompts or prompts ids at atime"
+                raise CohereException(
+                    "please provide either prompts or prompts ids at time"
                 )
             if not prompts and not prompt_ids:
-                raise PalmTextException(
+                raise CohereException(
                     "Either provide prompts or prompts ids to genrate the data"
                 )
             if prompt_ids:
                 prompts_list = Completion.create_prompt_from_id(
                     prompt_ids=prompt_ids,
                     prompt_data_list=prompt_data,
                     variables_list=variables,
@@ -87,15 +88,15 @@
                 message_data = {
                     "id": str(id),
                     "prompts": json.dumps(updated_prompts),
                     "model": model,
                     "variation_count": variation_count,
                     "max_tokens": max_tokens,
                     "temperature": temperature,
-                    "ai_service": "palm_api",
+                    "ai_service": "cohere_api",
                     "output_format": json.dumps(output_format),
                     "format_structure": json.dumps(format_strcture),
                     "api_key": api_key,
                     "context": context,
                 }
                 message = {"data": json.dumps(message_data)}
                 from AIBridge.queue_integration.message_queue import MessageQ
@@ -110,112 +111,186 @@
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 context=context,
             )
         except AIBridgeException as e:
-            raise PalmTextException(f"Error in generating AI data {e}")
-
-    @classmethod
-    def get_tokens(Self, model, text):
-        tokens = palm.count_text_tokens(model=model, prompt=text)
-        return tokens["token_count"]
+            raise CohereException(f"Error in generating AI data {e}")
 
     @classmethod
     def get_prompt_context(self, context):
-        context_string = ""
+        context_list = []
+        prev_role = ""
         for _context in context:
             if _context["role"] not in ["user", "system", "assistant"]:
-                raise PalmTextException(
+                raise CohereException(
                     "Invalid role provided. Please provide either user or system, assistant"
                 )
-            context_string = (
-                context_string + f"{_context['role']}:{_context['context']}" + "\n"
-            )
-        return context_string
+            key = "USER"
+            if _context["role"] in ["assistant", "system"]:
+                key = "CHATBOT"
+            if prev_role == key:
+                if key == "USER":
+                    context_list.append({"role": "CHATBOT", "text": "understood"})
+                elif key == "CHATBOT":
+                    context_list.append({"role": "USER", "text": "generated"})
+            else:
+                context_list.append({"role": key, "text": _context["context"]})
+            prev_role = key
+        if context_list:
+            data_test = context_list[-1]
+            if data_test["role"] == "USER":
+                context_list.append({"role": "CHATBOT", "text": "understood"})
+        return context_list
+
+    @classmethod
+    def execute_text_prompt(
+        self, api_key, model, messages, n, max_tokens=3500, temperature=0.5, context=[]
+    ):
+        co = cohere.Client(api_key)
+        return co.chat(
+            model=model,
+            chat_history=context,
+            message=messages,
+            max_tokens=max_tokens,
+            temperature=temperature,
+        )
+
+    @classmethod
+    def execute_prompt_function_calling(
+        self,
+        api_key,
+        model,
+        messages,
+        n,
+        functions_call,
+        max_tokens=3500,
+        temperature=0.5,
+        context=[],
+    ):
+        co = cohere.Client(api_key)
+        return co.chat(
+            model=model,
+            chat_history=context,
+            message=messages,
+            tools=functions_call,
+            max_tokens=max_tokens,
+            temperature=temperature,
+        )
 
     @classmethod
     def get_response(
         self,
         prompts,
-        model="models/text-bison-001",
+        model="command-nightly",
         variation_count=1,
-        max_tokens=10000,
+        max_tokens=3500,  # max 4096
         temperature=0.5,
         output_format=[],
         format_structure=[],
         api_key=None,
         context=[],
     ):
         try:
             if output_format:
                 if isinstance(output_format, str):
                     output_format = json.loads(output_format)
             if format_structure:
                 if isinstance(format_structure, str):
                     format_structure = json.loads(format_structure)
             if not prompts:
-                raise PalmTextException("No prompts provided")
-            api_key = api_key if api_key else parse_api_key("palm_api")
-            palm.configure(api_key=api_key)
+                raise CohereException("No prompts provided")
+            api_key = api_key if api_key else parse_api_key("cohere_api")
             model_output = []
-            token_used = 0
-            context_string = self.get_prompt_context(context)
+            message_data = []
+            context = self.get_prompt_context(context)
+            token_used = max_tokens
+            _formatter = "string"
             for index, prompt in enumerate(prompts):
-                prompt = context_string + "\n" + prompt
-                response = palm.generate_text(
-                    model=model,
-                    prompt=prompt,
-                    temperature=temperature,
-                    max_output_tokens=max_tokens,
-                    candidate_count=variation_count,
+                if output_format:
+                    _formatter = output_format[index]
+                if _formatter not in ["json", "csv", "xml"]:
+                    response = self.execute_text_prompt(
+                        api_key,
+                        model=model,
+                        messages=prompt,
+                        n=variation_count,
+                        max_tokens=max_tokens,
+                        temperature=temperature,
+                        context=message_data,
+                    )
+                    message_data.append(
+                        {
+                            "role": "CHATBOT",
+                            "content": response.text,
+                        }
+                    )
+                    content = response.text
+                else:
+                    if _formatter == "csv":
+                        schema = IntoJson.csv_to_json(format_structure[index])
+                    elif _formatter == "xml":
+                        schema = IntoJson.xml_to_json(format_structure[index])
+                    elif _formatter == "json":
+                        schema = json.loads(format_structure[index])
+                    functions = [get_function_from_json(schema, call_from="cohere")]
+                    response = self.execute_prompt_function_calling(
+                        api_key=api_key,
+                        model=model,
+                        messages=prompt,
+                        n=variation_count,
+                        functions_call=functions,
+                        max_tokens=max_tokens,
+                        temperature=temperature,
+                        context=message_data,
+                    )
+                    content = response.tool_calls[0].parameters
+                tokens = (
+                    response.meta["billed_units"]["input_tokens"]
+                    + response.meta["billed_units"]["output_tokens"]
                 )
-                token_used = token_used + self.get_tokens(model, prompt)
-                for res in response.candidates:
-                    content = res["output"]
-                    token_used = token_used + self.get_tokens(model, content)
-                    if output_format:
-                        _formatter = output_format[index]
+                token_used = token_used + tokens
+                if output_format:
+                    if isinstance(content, dict):
+                        content = json.dumps(content)
+                    try:
+                        if _formatter == "csv":
+                            content = FromJson.json_to_csv(json.loads(content))
+                        elif _formatter == "xml":
+                            content = FromJson.json_to_xml(json.loads(content))
+                    except AIBridgeException as e:
+                        raise CohereException(
+                            f"Ai response is not in valid {_formatter}"
+                        )
+                    if _formatter == "json":
+                        _validate_obj = ActiveValidator.get_active_validator(_formatter)
                         try:
-                            if _formatter == "csv":
-                                content = FromJson.json_to_csv(json.loads(content))
-                            elif _formatter == "xml":
-                                content = FromJson.json_to_xml(json.loads(content))
-                        except AIBridgeException as e:
-                            raise PalmTextException(
-                                f"Ai response is not in valid {_formatter}"
-                            )
-                        if _formatter == "json":
-                            _validate_obj = ActiveValidator.get_active_validator(
-                                _formatter
+                            content = _validate_obj.validate(
+                                content,
+                                schema=(
+                                    format_structure[index]
+                                    if format_structure
+                                    else None
+                                ),
                             )
-                            try:
-                                content = _validate_obj.validate(
-                                    content,
-                                    schema=(
-                                        format_structure[index]
-                                        if format_structure
-                                        else None
-                                    ),
-                                )
-                            except AIBridgeException as e:
-                                content_error = {
-                                    "error": f"{e}",
-                                    "ai_response": content,
-                                }
-                                content = json.dumps(content_error)
-                    if index >= len(model_output):
-                        model_output.append({"data": [content]})
-                    else:
-                        model_output[index]["data"].append(content)
+                        except AIBridgeException as e:
+                            content_error = {
+                                "error": f"{e}",
+                                "ai_response": content,
+                            }
+                            content = json.dumps(content_error)
+                if index >= len(model_output):
+                    model_output.append({"data": [content]})
+                else:
+                    model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
                     "token_used": token_used,
                     "created_at": time.time(),
-                    "ai_service": "palm_api",
+                    "ai_service": "cohere",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise PalmTextException(f"{e}")
+            raise CohereException(f"{e}")
```

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.2.7/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.2.7/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/constant/common.py` & `aibridge_test-0.2.7/AIBridge/constant/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from AIBridge.constant.constant import FUNCTION_CALL_FORMAT, PRIORITY
+from AIBridge.constant.constant import (
+    COHERE_FUNCTION_CALL_FORMAT,
+    FUNCTION_CALL_FORMAT,
+    PRIORITY,
+)
 from AIBridge.setconfig import SetConfig
 from AIBridge.exceptions import ConfigException
 from AIBridge.database.sql_service import SQL
 from AIBridge.database.no_sql_service import Mongodb
 from AIBridge.exceptions import AIBridgeException
 from urllib.parse import urlparse
 from AIBridge.output_validation.convertors import FromJson, IntoJson
@@ -56,47 +60,69 @@
     array = "array"
     string = "string"
     if call_from == "gemini_ai":
         type_ = "type_"
         object = "OBJECT"
         array = "ARRAY"
         string = "STRING"
+    elif call_from == "cohere":
+        type_ = "type"
+        object = "object"
+        array = "array"
+        string = "str"
 
     def create_function_call(output_schema: dict):
-        key_dict = {type_: object, "properties": {}}
+        if call_from == "cohere":
+            # properties = "parameter_definitions"
+            properties = "properties"
+        else:
+            properties = "properties"
+        key_dict = {type_: object, properties: {}}
         for key, value in output_schema.items():
             if isinstance(value, dict):
-                key_dict["properties"][key] = create_function_call(value)
+                key_dict[properties][key] = create_function_call(value)
             elif isinstance(value, list):
                 key_d = {
                     type_: array,
                     "description": "Generate the information",
                 }
+                if call_from == "cohere":
+                    key_d["required"] = True
                 if value:
                     if isinstance(value[0], str):
                         key_d["items"] = {type_: string, "description": value[0]}
                     elif isinstance(value[0], dict):
                         key_d["items"] = create_function_call(value[0])
                 else:
                     key_d["items"] = {
                         type_: string,
                         "description": "provide the given information",
                     }
-                key_dict["properties"][key] = key_d
+                    if call_from == "cohere":
+                        key_d["required"] = True
+                key_dict[properties][key] = key_d
             else:
-                key_dict["properties"][key] = {type_: string, "description": value}
+                val_x = {type_: string, "description": value}
+                if call_from == "cohere":
+                    val_x["required"] = True
+                key_dict[properties][key] = val_x
         return key_dict
 
     required = []
     for key in output_schema.keys():
         required.append(key)
-    data = FUNCTION_CALL_FORMAT
     key_dict = create_function_call(output_schema)
-    data["parameters"] = key_dict
-    data["parameters"]["required"] = required
+    if call_from == "open_ai" or call_from == "gemini_ai":
+        data = FUNCTION_CALL_FORMAT
+        data["parameters"] = key_dict
+        if call_from == "open_ai":
+            data["parameters"]["required"] = required
+    elif call_from == "cohere":
+        data = COHERE_FUNCTION_CALL_FORMAT
+        data["parameter_definitions"] = key_dict["properties"]
     return data
 
 
 def check_url(url_list: list):
     for url in url_list:
         result = urlparse(url)
         if not all([result.scheme, result.netloc]):
```

### Comparing `aibridge_test-0.2.6/AIBridge/constant/constant.py` & `aibridge_test-0.2.7/AIBridge/constant/constant.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,11 +21,17 @@
 OPENAI_IMAGE_SIZES = ["256x256", "512x512", "1024x1024"]
 STABLE_DIFFUSION_TYPES = [
     "text2img",
     "img2img",
     "inpaint",
 ]
 FUNCTION_CALL_FORMAT = {
-    "name": "create_date",
+    "name": "Give_Information",
     "description": "Generate output in given key and valid json formate",
     "parameters": {},
 }
+
+COHERE_FUNCTION_CALL_FORMAT = {
+    "name": "Give_Information",
+    "description": "Generate output in given key and valid json formate",
+    "parameter_definitions": {},
+}
```

### Comparing `aibridge_test-0.2.6/AIBridge/database/db_layer.py` & `aibridge_test-0.2.7/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/database/no_sql_service.py` & `aibridge_test-0.2.7/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/database/session.py` & `aibridge_test-0.2.7/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/database/sql_service.py` & `aibridge_test-0.2.7/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/exceptions.py` & `aibridge_test-0.2.7/AIBridge/exceptions.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/output_validation/convertors.py` & `aibridge_test-0.2.7/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/output_validation/validations.py` & `aibridge_test-0.2.7/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.2.7/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.2.7/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.2.7/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.2.7/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.2.7/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.2.7/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/AIBridge/setconfig.py` & `aibridge_test-0.2.7/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/LICENSE` & `aibridge_test-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/PKG-INFO` & `aibridge_test-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.6
+Version: 0.2.7
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: pymongo>=4.4.1
 Requires-Dist: sqlparse>=0.4.4
 Requires-Dist: jsonschema>=4.18.4
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: google-generativeai>=0.4.1
-Requires-Dist: cohere>=4.24
+Requires-Dist: cohere>=5.2.2
 Requires-Dist: ai21>=1.2.8
 Requires-Dist: xmltodict>=0.13.0
 Requires-Dist: anthropic>=0.21.3
 
 
 ## AIBridge 0.0.1
```

### Comparing `aibridge_test-0.2.6/README.md` & `aibridge_test-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.2.7/aibridge_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.6
+Version: 0.2.7
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: pymongo>=4.4.1
 Requires-Dist: sqlparse>=0.4.4
 Requires-Dist: jsonschema>=4.18.4
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: google-generativeai>=0.4.1
-Requires-Dist: cohere>=4.24
+Requires-Dist: cohere>=5.2.2
 Requires-Dist: ai21>=1.2.8
 Requires-Dist: xmltodict>=0.13.0
 Requires-Dist: anthropic>=0.21.3
 
 
 ## AIBridge 0.0.1
```

### Comparing `aibridge_test-0.2.6/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.2.7/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.6/setup.py` & `aibridge_test-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.2.6"
+VERSION = "0.2.7"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
     "sqlparse>=0.4.4",
     "jsonschema>=4.18.4",
     "Pillow>=10.0.0",
     "google-generativeai>=0.4.1",
-    "cohere>=4.24",
+    "cohere>=5.2.2",
     "ai21>=1.2.8",
     "xmltodict>=0.13.0",
     "anthropic>=0.21.3",
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 try:
```

