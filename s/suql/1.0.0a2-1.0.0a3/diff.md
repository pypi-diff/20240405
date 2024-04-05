# Comparing `tmp/suql-1.0.0a2.tar.gz` & `tmp/suql-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.0.0a2.tar", last modified: Thu Apr  4 04:30:18 2024, max compression
+gzip compressed data, was "suql-1.0.0a3.tar", last modified: Fri Apr  5 18:03:19 2024, max compression
```

## Comparing `suql-1.0.0a2.tar` & `suql-1.0.0a3.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.642725 suql-1.0.0a2/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.0.0a2/LICENSE
--rw-------   0 oval      (1000) users      (100)     4619 2024-04-04 04:30:18.642725 suql-1.0.0a2/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4165 2024-04-03 06:02:31.000000 suql-1.0.0a2/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-04 04:30:18.642725 suql-1.0.0a2/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1395 2024-04-04 04:29:28.000000 suql-1.0.0a2/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17330 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16991 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     7885 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)    11962 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.0.0a2/src/suql/prompts/__init__.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.0.0a2/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    59411 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/suql.egg-info/
--rw-------   0 oval      (1000) users      (100)     4619 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      498 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      232 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-05 18:03:19.358048 suql-1.0.0a3/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.0.0a3/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4619 2024-04-05 18:03:19.358048 suql-1.0.0a3/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4165 2024-04-03 06:02:31.000000 suql-1.0.0a3/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-05 18:03:19.358048 suql-1.0.0a3/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1423 2024-04-05 18:02:40.000000 suql-1.0.0a3/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-05 18:03:19.354048 suql-1.0.0a3/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-05 18:03:19.354048 suql-1.0.0a3/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17330 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    16991 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     7895 2024-04-05 17:58:35.000000 suql-1.0.0a3/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)    12070 2024-04-05 18:02:21.000000 suql-1.0.0a3/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-05 18:03:19.354048 suql-1.0.0a3/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.0.0a3/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-05 18:03:19.354048 suql-1.0.0a3/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.0.0a3/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    59411 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.0.0a3/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-05 18:03:19.354048 suql-1.0.0a3/src/suql.egg-info/
+-rw-------   0 oval      (1000) users      (100)     4619 2024-04-05 18:03:19.000000 suql-1.0.0a3/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-05 18:03:19.000000 suql-1.0.0a3/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-05 18:03:19.000000 suql-1.0.0a3/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      217 2024-04-05 18:03:19.000000 suql-1.0.0a3/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-05 18:03:19.000000 suql-1.0.0a3/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.0.0a2/LICENSE` & `suql-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a2/PKG-INFO` & `suql-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.0.0a2 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.0.0a3 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
            ************ SSUUQQLL ((SSttrruuccttuurreedd aanndd UUnnssttrruuccttuurreedd QQuueerryy LLaanngguuaaggee))
                          _[[_aa_rr_XX_ii_vv_]]_[[_GG_ii_tt_hh_uu_bb_ _SS_tt_aa_rr_ss_]] ************
```

### Comparing `suql-1.0.0a2/README.md` & `suql-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a2/setup.py` & `suql-1.0.0a3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.0.0a2"
+version = "1.0.0a3"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
@@ -14,15 +14,14 @@
 # Define your dependencies
 install_requires = [
     'openai==1.3.2',
     'Jinja2==3.1.2',
     'Flask==2.3.2',
     'Flask-Cors==4.0.0',
     'Flask-RESTful==0.3.10',
-    'pymongo==4.3.3',
     'transformers==4.38.2',
     'torch==2.0.1',
     'requests==2.31.0',
     'spacy==3.7.4',
     'tiktoken==0.4.0',
     'psycopg2-binary==2.9.7',
     'pglast==5.3',
@@ -46,8 +45,11 @@
     author=author,
     author_email=author_email,
     packages=packages,
     package_dir={"": "src"},
     install_requires=install_requires,
     url=url,
     classifiers=classifiers,
+    package_data={
+        "": ["*.prompt"]
+    }
 )
```

### Comparing `suql-1.0.0a2/src/suql/agent.py` & `suql-1.0.0a3/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a2/src/suql/faiss_embedding.py` & `suql-1.0.0a3/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a2/src/suql/free_text_fcns_server.py` & `suql-1.0.0a3/src/suql/free_text_fcns_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         in the same order (Default set to 3800).
 
         Returns:
         {
             "result" (str): answer function result
         }
         """
-        from prompt_continuation import llm_generate
+        from suql.prompt_continuation import llm_generate
 
         data = request.get_json()
 
         if "text" not in data or "question" not in data:
             return None
 
         if not data["text"]:
@@ -119,15 +119,15 @@
 
         Returns:
         {
             "result" (str): summary function result
         }
         """
         print(k)
-        from prompt_continuation import llm_generate
+        from suql.prompt_continuation import llm_generate
 
         data = request.get_json()
 
         if "text" not in data:
             return None
 
         if not data["text"]:
```

### Comparing `suql-1.0.0a2/src/suql/postgresql_connection.py` & `suql-1.0.0a3/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a2/src/suql/prompt_continuation.py` & `suql-1.0.0a3/src/suql/prompt_continuation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 client = OpenAI()
 import os
 import time
 import traceback
 from functools import partial
 from threading import Thread
 
-import pymongo
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 from suql.utils import num_tokens_from_string
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 # create file handler which logs even debug messages
@@ -38,16 +37,20 @@
 )
 # # uncomment if using Azure OpenAI
 openai.api_type == "open_ai"
 # openai.api_type = "azure"
 # openai.api_base = "https://ovalopenairesource.openai.azure.com/"
 # openai.api_version = "2023-05-15"
 
-mongo_client = pymongo.MongoClient("localhost", 27017)
-prompt_cache_db = mongo_client["open_ai_prompts"]["caches"]
+ENABLE_CACHING = False
+
+if ENABLE_CACHING:
+    import pymongo
+    mongo_client = pymongo.MongoClient("localhost", 27017)
+    prompt_cache_db = mongo_client["open_ai_prompts"]["caches"]
 
 # inference_cost_per_1000_tokens = {'ada': 0.0004, 'babbage': 0.0005, 'curie': 0.002, 'davinci': 0.02, 'turbo': 0.003, 'gpt-4': 0.03} # for Azure
 inference_input_cost_per_1000_tokens = {
     "gpt-4": 0.03,
     "gpt-3.5-turbo-0613": 0.0010,
     "gpt-3.5-turbo-1106": 0.0010,
     "gpt-4-1106-preview": 0.01,
@@ -264,40 +267,40 @@
     filled_prompt gives direct access to the underlying model, without having to load a prompt template from a .prompt file. Used for testing.
     ban_line_break_start can potentially double the cost, though in practice (and especially with good prompts) this only happens for a fraction of inputs
     """
     start_time = time.time()
     if filled_prompt is None:
         filled_prompt = _fill_template(template_file, prompt_parameter_values)
 
-    cache_res = prompt_cache_db.find_one(
-        {
-            "model": engine,
-            "prompt": filled_prompt,
-            "max_tokens": max_tokens,
-            "temperature": temperature,
-            "stop_tokens": stop_tokens,
-            "top_p": top_p,
-            "frequency_penalty": frequency_penalty,
-            "presence_penalty": presence_penalty,
-        }
-    )
-    if cache_res:
-        return cache_res["res"], 0
+    if ENABLE_CACHING:
+        cache_res = prompt_cache_db.find_one(
+            {
+                "model": engine,
+                "prompt": filled_prompt,
+                "max_tokens": max_tokens,
+                "temperature": temperature,
+                "stop_tokens": stop_tokens,
+                "top_p": top_p,
+                "frequency_penalty": frequency_penalty,
+                "presence_penalty": presence_penalty,
+            }
+        )
+        if cache_res:
+            return cache_res["res"], 0
 
     # We have experiences very long latency from time to time from both Azure's and OpenAI's chatGPT response time
     # Here is a heuristics-based, dynamically-calculated max wait time, before we cancel the last request and re-issue a new one
     total_token = num_tokens_from_string(filled_prompt) + max_tokens
     if max_wait_time is None:
         max_wait_time = 0.05 * total_token + 1
 
     success = False
     final_result = None
 
     for attempt in range(attempts):
-        print(f"Attempt {attempt + 1} of {attempts}")
         success, result = call_with_timeout(
             _generate,
             max_wait_time,
             filled_prompt,
             engine,
             max_tokens,
             temperature,
@@ -308,16 +311,14 @@
             postprocess,
             max_tries,
             ban_line_break_start,
         )
         if success:
             final_result = result
             break
-        else:
-            print("Retrying...")
 
     if final_result is None:
         final_result = _generate(
             filled_prompt,
             engine,
             max_tokens,
             temperature,
@@ -329,27 +330,28 @@
             max_tries,
             ban_line_break_start,
         )
 
     end_time = time.time()
     elapsed_time = end_time - start_time
 
-    prompt_cache_db.insert_one(
-        {
-            "model": engine,
-            "prompt": filled_prompt,
-            "max_tokens": max_tokens,
-            "temperature": temperature,
-            "stop_tokens": stop_tokens,
-            "top_p": top_p,
-            "frequency_penalty": frequency_penalty,
-            "presence_penalty": presence_penalty,
-            "res": final_result,
-        }
-    )
+    if ENABLE_CACHING:
+        prompt_cache_db.insert_one(
+            {
+                "model": engine,
+                "prompt": filled_prompt,
+                "max_tokens": max_tokens,
+                "temperature": temperature,
+                "stop_tokens": stop_tokens,
+                "top_p": top_p,
+                "frequency_penalty": frequency_penalty,
+                "presence_penalty": presence_penalty,
+                "res": final_result,
+            }
+        )
 
     return final_result, elapsed_time
 
 
 def batch_llm_generate(
     template_file: str,
     prompt_parameter_values: List[dict],
```

### Comparing `suql-1.0.0a2/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.0.0a3/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a2/src/suql/utils.py` & `suql-1.0.0a3/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a2/src/suql.egg-info/PKG-INFO` & `suql-1.0.0a3/src/suql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.0.0a2 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.0.0a3 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
            ************ SSUUQQLL ((SSttrruuccttuurreedd aanndd UUnnssttrruuccttuurreedd QQuueerryy LLaanngguuaaggee))
                          _[[_aa_rr_XX_ii_vv_]]_[[_GG_ii_tt_hh_uu_bb_ _SS_tt_aa_rr_ss_]] ************
```

