# Comparing `tmp/patent_chart-0.2.5.tar.gz` & `tmp/patent_chart-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_chart-0.2.5.tar", max compression
+gzip compressed data, was "patent_chart-0.2.7.tar", max compression
```

## Comparing `patent_chart-0.2.5.tar` & `patent_chart-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0        0 2024-02-02 22:00:15.933827 patent_chart-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-02-02 22:00:15.824990 patent_chart-0.2.5/patent_chart/__init__.py
--rw-r--r--   0        0        0     3440 2024-02-02 22:00:15.821601 patent_chart-0.2.5/patent_chart/citation.py
--rw-r--r--   0        0        0     1555 2024-03-28 04:11:53.287226 patent_chart-0.2.5/patent_chart/data_structures.py
--rw-r--r--   0        0        0     1843 2024-02-02 22:00:15.871024 patent_chart-0.2.5/patent_chart/embeddings.py
--rw-r--r--   0        0        0     2811 2024-02-02 22:00:15.824681 patent_chart-0.2.5/patent_chart/evaluation.py
--rw-r--r--   0        0        0      498 2024-02-02 22:00:15.823970 patent_chart-0.2.5/patent_chart/filtering.py
--rw-r--r--   0        0        0    35761 2024-03-28 04:11:53.288326 patent_chart-0.2.5/patent_chart/generator.py
--rw-r--r--   0        0        0     3359 2024-03-28 04:11:53.289214 patent_chart-0.2.5/patent_chart/google_patents.py
--rw-r--r--   0        0        0     3838 2024-02-02 22:00:15.872576 patent_chart-0.2.5/patent_chart/integrationtests.py
--rw-r--r--   0        0        0     6662 2024-03-20 16:06:10.621710 patent_chart-0.2.5/patent_chart/opensearch.py
--rw-r--r--   0        0        0    64508 2024-03-28 04:11:53.290356 patent_chart-0.2.5/patent_chart/parser.py
--rw-r--r--   0        0        0     6528 2024-02-02 22:00:15.873335 patent_chart-0.2.5/patent_chart/ranking.py
--rw-r--r--   0        0        0      591 2024-02-02 22:00:15.820971 patent_chart-0.2.5/patent_chart/redis_utils.py
--rw-r--r--   0        0        0     5103 2024-02-02 22:00:15.870154 patent_chart-0.2.5/patent_chart/requests_utils.py
--rw-r--r--   0        0        0     5925 2024-03-20 16:06:10.624333 patent_chart-0.2.5/patent_chart/search_index.py
--rw-r--r--   0        0        0      567 2024-02-20 15:54:25.646442 patent_chart-0.2.5/patent_chart/settings.py
--rw-r--r--   0        0        0    31579 2024-03-28 04:11:53.291127 patent_chart-0.2.5/patent_chart/tests.py
--rw-r--r--   0        0        0     1825 2024-02-02 22:00:15.871782 patent_chart-0.2.5/patent_chart/utils.py
--rw-r--r--   0        0        0     1038 2024-03-28 16:13:16.863612 patent_chart-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 patent_chart-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-02 22:00:15.933827 patent_chart-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 22:16:17.760177 patent_chart-0.2.7/patent_chart/__init__.py
+-rw-r--r--   0        0        0     3440 2024-02-02 22:00:15.821601 patent_chart-0.2.7/patent_chart/citation.py
+-rw-r--r--   0        0        0     1759 2024-04-04 16:56:23.070248 patent_chart-0.2.7/patent_chart/data_structures.py
+-rw-r--r--   0        0        0     1843 2024-02-02 22:00:15.871024 patent_chart-0.2.7/patent_chart/embeddings.py
+-rw-r--r--   0        0        0     2811 2024-02-02 22:00:15.824681 patent_chart-0.2.7/patent_chart/evaluation.py
+-rw-r--r--   0        0        0      498 2024-02-02 22:00:15.823970 patent_chart-0.2.7/patent_chart/filtering.py
+-rw-r--r--   0        0        0    37060 2024-04-05 03:16:24.398048 patent_chart-0.2.7/patent_chart/generator.py
+-rw-r--r--   0        0        0     3249 2024-04-04 16:55:39.837226 patent_chart-0.2.7/patent_chart/google_patents.py
+-rw-r--r--   0        0        0     3838 2024-02-02 22:00:15.872576 patent_chart-0.2.7/patent_chart/integrationtests.py
+-rw-r--r--   0        0        0    64508 2024-04-02 04:43:42.390709 patent_chart-0.2.7/patent_chart/parser.py
+-rw-r--r--   0        0        0     4518 2024-04-05 02:43:11.615256 patent_chart-0.2.7/patent_chart/pinecone.py
+-rw-r--r--   0        0        0     5277 2024-04-04 03:03:09.786061 patent_chart-0.2.7/patent_chart/ranking.py
+-rw-r--r--   0        0        0      591 2024-02-02 22:00:15.820971 patent_chart-0.2.7/patent_chart/redis_utils.py
+-rw-r--r--   0        0        0     5103 2024-02-02 22:00:15.870154 patent_chart-0.2.7/patent_chart/requests_utils.py
+-rw-r--r--   0        0        0     5931 2024-04-04 03:03:09.787023 patent_chart-0.2.7/patent_chart/search_index.py
+-rw-r--r--   0        0        0      567 2024-02-20 15:54:25.646442 patent_chart-0.2.7/patent_chart/settings.py
+-rw-r--r--   0        0        0    31579 2024-04-02 04:43:42.392082 patent_chart-0.2.7/patent_chart/tests.py
+-rw-r--r--   0        0        0     6106 2024-04-04 03:49:22.349201 patent_chart-0.2.7/patent_chart/uspto_parse.py
+-rw-r--r--   0        0        0     1825 2024-02-02 22:00:15.871782 patent_chart-0.2.7/patent_chart/utils.py
+-rw-r--r--   0        0        0     1082 2024-04-05 03:18:45.504490 patent_chart-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 patent_chart-0.2.7/PKG-INFO
```

### Comparing `patent_chart-0.2.5/patent_chart/citation.py` & `patent_chart-0.2.7/patent_chart/citation.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/embeddings.py` & `patent_chart-0.2.7/patent_chart/embeddings.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/evaluation.py` & `patent_chart-0.2.7/patent_chart/evaluation.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/generator.py` & `patent_chart-0.2.7/patent_chart/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,89 +3,94 @@
 import time
 import asyncio
 import uuid
 import random
 from logging import getLogger
 from dataclasses import dataclass
 from typing import Callable, Optional, AsyncIterator, Coroutine, List
-from functools import partial
+from functools import partial, lru_cache
 
-import openai
+from openai import OpenAI, AsyncOpenAI, OpenAIError
 import tiktoken
-from dotenv import load_dotenv
+from anthropic import AsyncAnthropic
+from tenacity import (
+    retry,
+    stop_after_attempt,
+    wait_random_exponential,
+)
 
 from . import parser
 from . import ranking
 from . import search_index
 from .utils import num_tokens_from_messages
 from .data_structures import GeneratedPassage
 from .requests_utils import DistributedFixedWindowRateLimiter
 
 logger = getLogger(__name__)
 
-load_dotenv()
+oai = OpenAI()
+async_oai = AsyncOpenAI()
 
-# _openai_sync_client = None
-# _openai_async_client = None
-
-# def openai_sync_client():
-#     global _openai_sync_client
-#     if _openai_sync_client is None:
-#         _openai_sync_client = openai.OpenAI()
-#     return _openai_sync_client
-
-# def openai_async_client():
-#     global _openai_async_client
-#     if _openai_async_client is None:
-#         _openai_async_client = openai.AsyncOpenAI()
-#     return _openai_async_client
+ac = AsyncAnthropic()
 
 class GenerationError(Exception):
     pass
 
 RATE_LIMIT_INTERVAL = 60  # seconds
 
+# OpenAI text-embedding-3-large
+MAX_SEQ_LENGTH = 8191
+
 # rate limit
 token_rate_limit_by_model_name = {
     'gpt-4': 300_000,
     'gpt-3.5-turbo': 2_000_000,
     'gpt-3.5-turbo-16k': 2_000_000,
     'gpt-3.5-turbo-instruct': 250_000,
     'gpt-3.5-turbo-0125': 2_000_000,
     'gpt-4-turbo-preview': 600_000,
+    'claude-3-opus-20240229': 400_000,
 }
 
 # context window
 model_name_to_token_limit = {
     'gpt-4': 8192,
     'gpt-3.5-turbo-16k': 16384,
     'gpt-3.5-turbo': 4096,
     'gpt-3.5-turbo-16k-0613': 16384,
     'gpt-3.5-turbo-0125': 16385,
     'gpt-4-turbo-preview': 128_000,
+    'claude-3-opus-20240229': 200_000,
 }
 
+
 def prompt_claim_element_only(claim_element, prior_art_passage, n_passages_per_split=3):
     messages = [
         {"role": "system", "content": f"You work for a law firm. Your task is to interpret a single claim element that I select from the claims of a patent. Then I'm going to give you a passage from the prior art and you need to pick {n_passages_per_split} distinct sub-passages from the passage that you believe are the most similar to the claim element. Please output only those {n_passages_per_split} passages, copied verbatim from the prior art. Do not add any other text besides the verbatim passages."},
         {"role": "user", "content": f"Selected claim element: {claim_element}"},
         {"role": "user", "content": f"Prior art passage: {prior_art_passage}"},
     ]
     return messages
 
 def prompt_summary_full_set_of_claims(summary, claims, claim_element, prior_art_passage, n_passages_per_split=3):
     messages = [
         {"role": "system", "content": f"You work for a law firm. Your task is to read the summary of the written description of a patent and the full set of claims in the patent and interpret a single claim element that I select from the claims of the patent in light of the summary and the full set of claims. Then I'm going to give you a passage from the prior art and you need to pick{n_passages_per_split} distinct sub-passages from the passage that you believe are the most similar to the claim element. Please output only those {n_passages_per_split} passages, copied verbatim from the prior art, each separated by a single newline. Do not add any other text besides the verbatim passages. If you don't believe there are any sub-passages that are similar to the claim element, please output 'None'."},
-        {"role": "user", "content": f"Summary of the written description of the invention: {summary}"},
-        {"role": "user", "content": f"Full set of claims: {claims}"},
-        {"role": "user", "content": f"Selected claim element: {claim_element}"},
-        {"role": "user", "content": f"Prior art passage: {prior_art_passage}"},
+        {"role": "user", "content": f"Summary of the written description of the invention: {summary}\n\nFull set of claims: {claims}\n\nSelected claim element: {claim_element}Prior art passage: {prior_art_passage}"},
+    ]
+    return messages
+
+
+def prompt_full_spec_full_set_of_claims(full_spec, claims, claim_element, prior_art_passage, n_passages_per_split=3):
+    messages = [
+        {"role": "system", "content": f"You work for a law firm. Your task is to read the the written description of a patent and the full set of claims in the patent and interpret a single claim element selected from the claims of the patent in the context of the written description and the other claim elements. Then I'm going to give you a prior art document and you need to pick up to {n_passages_per_split} distinct passages from the prior art document that you believe are the most similar to the claim element. Please output only those {n_passages_per_split} passages, copied verbatim from the prior art document, each separated by a single '\n'. Do not add any other text besides the verbatim passages. If you don't believe there are any passages that are similar to the claim element, please output 'None'."},
+        {"role": "user", "content": f"Written description from the patent: {full_spec} \n\nFull set of claims from the patent: {claims} \n\nSelected claim element from the claims of the patent: {claim_element} \n\nPrior art document: {prior_art_passage}"},
     ]
     return messages
 
+
 def post_process_selected_passage_gpt4(passage: str) -> list[str]:
     split_strategies = [
         lambda passage: re.split(r'\d+\.', passage),
         lambda passage: passage.split('\n\n'),
         lambda passage: passage.split('\"\n'),
     ]
     for split_strategy in split_strategies:
@@ -97,47 +102,59 @@
     # filter whitespace only and empty string entries
     split_passages = [p for p in split_passages if p != '']
     # filter out passages that are just a newline
     split_passages = [p for p in split_passages if p != '\n']
         
     return split_passages
 
+
+def post_process_selected_passage_claude_opus(passage: str) -> list[str]:
+    passage = passage.split(':')[-1]
+    
+    split_strategies = [
+        lambda passage: passage.split('\n'),
+    ]
+    for split_strategy in split_strategies:
+        split_passages = split_strategy(passage)
+        if len(split_passages) > 1:
+            break
+    # strip newlines, quotes, and whitespace from beginning and end
+    split_passages = [p.strip().strip('"') for p in split_passages]
+    # filter whitespace only and empty string entries
+    split_passages = [p for p in split_passages if p != '']
+    # filter out passages that are just a newline
+    split_passages = [p for p in split_passages if p != '\n']
+    
+    return split_passages
+  
+
+def post_process_summary_claude_opus(summary: str) -> str:
+    summary = summary.split(':')[-1]
+    return summary.strip().strip('"')
+
+
 @dataclass
 class GeneratorConfig:
     model_name: str = 'gpt-4'
     target_n_passages: int = 10
     min_n_splits: int = 1
-    generate_passages_prompt_func: Callable[..., list[dict]] = prompt_summary_full_set_of_claims
-    post_process_generated_passages_func: Callable[[str], list[str]] = post_process_selected_passage_gpt4
 
 def load_generator_config_from_env():
     model_name = os.environ.get('LLM_MODEL_NAME', 'gpt-4')
     if model_name not in token_rate_limit_by_model_name:
         raise ValueError(f"Model name {model_name} not recognized.")
     target_n_passages = int(os.environ.get('LLM_TARGET_N_PASSAGES', 10))
     min_n_splits = int(os.environ.get('LLM_MIN_N_SPLITS', 1))
-    generate_passages_prompt_func = os.environ.get('LLM_GENERATE_PASSAGES_PROMPT_FUNC', 'prompt_summary_full_set_of_claims')
-    post_process_generated_passages_func = os.environ.get('LLM_POST_PROCESS_GENERATED_PASSAGES_FUNC', 'post_process_selected_passage_gpt4')
-    if generate_passages_prompt_func == 'prompt_summary_full_set_of_claims':
-        generate_passages_prompt_func = prompt_summary_full_set_of_claims
-    else:
-        raise NotImplementedError(f"Prompt func {generate_passages_prompt_func} not implemented.")
-    if post_process_generated_passages_func == 'post_process_selected_passage_gpt4':
-        post_process_generated_passages_func = post_process_selected_passage_gpt4
-    else:
-        raise NotImplementedError(f"Post process func {post_process_generated_passages_func} not implemented.")
     
     logger.info('Loaded generator config: \n %s \n', )
 
     config = GeneratorConfig(
         model_name=model_name,
         target_n_passages=target_n_passages,
         min_n_splits=min_n_splits,
-        generate_passages_prompt_func=generate_passages_prompt_func,
-        post_process_generated_passages_func=post_process_generated_passages_func
     )
 
     logger.info('Loaded generator config: \n %s \n', config)
 
     return config
 
 def num_tokens_in_text(text, model="gpt-3.5-turbo-0613"):
@@ -228,90 +245,76 @@
         {"role": "system", "content": f"Your task is to read the written description and of an invention disclosed in a patent and the full set of claims in the patent and interpret a single claim element that I select from the claims of the patent in light of the written description and the full set of claims. Then I'm going to give you {n_completions} sub-passages from the prior art passage i presented to you that you chose because they were the most semantically similar to the selected claim element interpreted in light of the written description and the full set of claims. Please rank these {n_completions} passages in descending order of similarity to the selected claim element interpreted in light of the written description and the full set of claims. I will give you passages numbered by roman numerals, for example: 'I. Passage One... II. Passage two... III. Passage three...'. Please output only the integer ranking following by the roman numeral and passage, for example: '1. II. Passage two ... 2. I. Passage one... 3. III Passage three...' if you believe the ranking should be passage two > passage one > passage three."},
         {"role": "user", "content": f"Written description of invention: {all_but_claims}"},
         {"role": "user", "content": f"Claim element: {claim_element}"},
         {"role": "user", "content": f"Prior art passages to rank: {chosen_prior_art_passage}"},
     ]
     return messages
 
-def openai_chat_completion_request_with_retry(model_name, messages, backoff_factor=2, backoff_override=None):
+def openai_chat_completion_request_with_retry(model_name, messages, backoff_factor=2, backoff_override=None) -> str:
     for i in range(1, 3):
         try:
-            # completion = openai_sync_client().chat.completions.create(
-            #     model=model_name,
-            #     messages=messages
-            # )
-            completion = openai.ChatCompletion.create(
+            completion = oai.chat.completions.create(
                 model=model_name,
                 messages=messages
             )
-            return completion
-        except openai.OpenAIError as e:
+            return completion.choices[0].message.content
+        except OpenAIError as e:
             if backoff_override is not None:
                 time.sleep(backoff_override)
             else:
                 time.sleep(backoff_factor**i)
             continue
         except Exception as e:
             raise e
     raise Exception("Failed to send chat completion request to OpenAI after 4 retries.")
 
 
-
-async def aopenai_chat_completion_request_with_retry(model_name, messages, backoff_factor=2, backoff_override=None, n_retries=3, rate_limiter: Optional[DistributedFixedWindowRateLimiter] = None, **kwargs) -> dict:
+async def aopenai_chat_completion_request_with_retry(model_name, messages, backoff_factor=2, backoff_override=None, n_retries=3, rate_limiter: Optional[DistributedFixedWindowRateLimiter] = None, **kwargs) -> str:
     """Send a chat completion request to OpenAI with retries."""
     for i in range(1, 1 + n_retries):
         try:
             if rate_limiter is not None:
                 num_tokens_in_messages = num_tokens_from_messages(messages)
                 # NOTE: separating wait for tokens, the request, and removing tokens is prone to race conditions. We can tolerate occasionally making requests that receive rate limit errors so long as we retry them with backoff.
                 if await rate_limiter.wait_for_tokens(num_tokens_in_messages):
-                    # completion = await openai_async_client().chat.completions.create(
-                    #     model=model_name,
-                    #     messages=messages,
-                    #     **kwargs
-                    # )
-                    completion = await openai.ChatCompletion.acreate(
+                    completion = await async_oai.chat.completions.create(
                         model=model_name,
                         messages=messages,
                         **kwargs
                     )
-                    n_tokens_in_completion = completion['usage']['completion_tokens']
+                    n_tokens_in_completion = completion.usage.completion_tokens
                     await rate_limiter.remove_tokens(n_tokens_in_completion)
             else:
-                # completion = await openai_async_client().chat.completions.create(
-                #         model=model_name,
-                #         messages=messages,
-                #         **kwargs
-                #     )
-                completion = await openai.ChatCompletion.acreate(
+                completion = await async_oai.chat.completions.create(
                     model=model_name,
                     messages=messages,
                     **kwargs
                 )
-            return completion
-        # except openai.OpenAIError as e:
-        except openai.error.OpenAIError as e:
+            return completion.choices[0].message.content
+        except OpenAIError as e:
             logger.error(f"OpenAIError: {e}")
             if backoff_override is not None:
                 jitter = random.uniform(-0.10, 0.10)
                 await asyncio.sleep(backoff_override * (1 + jitter))
             else:
                 jitter = random.uniform(-0.10, 0.10) 
                 await asyncio.sleep(backoff_factor**i * (1 + jitter))
             continue
         except Exception as e:
             raise e
     raise Exception(f"Failed to send chat completion request to OpenAI after {n_retries} retries.")
 
+
 def split_passage_to_meet_model_token_limit(passage: str, prompt_func: Callable[[str], list[dict]], model_name: str, min_n_splits: int = 1) -> list[str]:
     """ 
     Given a passage string, a prompt func that takes only the passage string, and a model, find the smallest number of splits necessary to get messages under token limit and return splits of the passage.
     """
     token_limit = model_name_to_token_limit[model_name]
     min_split_size = 256
+    # We use cl100k_base as the tokenizer for estimating even for Claude which has a closed-source tokenizer.
     base_num_tokens = num_tokens_from_messages(
         prompt_func(' ' * min_split_size)
     )
     if base_num_tokens > token_limit:
         raise GenerationError("Prompt exceeds token limit by itself.")
     
     passage_splits = []
@@ -330,214 +333,236 @@
             passage_splits = candidate_splits
             break
         passage_split_count += 1
 
     return passage_splits
 
 
-def openai_model_id_from_completion(completion: dict) -> str:
-    try:
-        return f'{completion["model"]}-{completion["system_fingerprint"]}'
-    except KeyError:
-        return load_generator_config_from_env().model_name
+@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(6), reraise=True)
+async def aclaude_chat_completion_request(model_name, messages) -> str:
+    system_message = messages.pop(0)
+    completion = await ac.messages.create(
+        max_tokens=4096,
+        system=system_message['content'],
+        messages=messages,
+        model=model_name,
+    )
+    print(completion)
+    return completion.content[0].text
+
+
+def make_get_completion_coro(model_name, messages, rate_limiter=None):
+    if model_name == 'gpt-4':
+        return aopenai_chat_completion_request_with_retry(model_name, messages, rate_limiter=rate_limiter)
+    elif model_name == 'claude-3-opus-20240229':
+        return aclaude_chat_completion_request(model_name, messages)
 
 
 async def agenerate_passages_for_prior_art_splits(prior_art_splits: list[str], prompt_func: Callable[[str], list[dict]], model_name: str, claim_element_id: int, prior_art_id: int, rate_limiter: Optional[DistributedFixedWindowRateLimiter] = None) -> list[GeneratedPassage | Exception]:
     # make parallel requests to openai api for prior art splits
     passages: list[GeneratedPassage | Exception] = []
     coros = []
     for prior_art_split in prior_art_splits:
         messages = prompt_func(prior_art_split)
-        coros.append(aopenai_chat_completion_request_with_retry(model_name, messages, rate_limiter=rate_limiter))
+        coros.append(make_get_completion_coro(model_name, messages, rate_limiter=rate_limiter))
         
     completions = await asyncio.gather(*coros, return_exceptions=True)
     for i, completion in enumerate(completions):
         if isinstance(completion, Exception):
             print(f'Failed to get completion for prior art split {i} of prior art {prior_art_id} for claim element {claim_element_id}')
             print(completion)
             passages.append(completion)
         else:
-            selected_passages = completion['choices'][0]['message']['content']
-            post_process_generated_passages_func = load_generator_config_from_env().post_process_generated_passages_func
+            selected_passages = completion
+            if model_name == 'gpt-4':
+                post_process_generated_passages_func = post_process_selected_passage_gpt4
+            elif model_name == 'claude-3-opus-20240229':
+                post_process_generated_passages_func = post_process_selected_passage_claude_opus
+            else:
+                raise NotImplementedError(f"Post processing function for model {model_name} not implemented.")
+            
             post_processed_passages = post_process_generated_passages_func(selected_passages)
-            # if len(post_processed_passages) == 1:
-            #     logger.error(f'Possible error post processing selected passages for claim element {claim_element_id} and prior art {prior_art_id}: \nCompletion: {selected_passages} \nPost-processed: {post_processed_passages}')
 
             for processed_passage in post_processed_passages:
                 # We'll add the start line and end line later
                 passages.append(
                     GeneratedPassage(
                         prior_art_source_id=prior_art_id,
                         text=processed_passage,
                         claim_element_id=claim_element_id,
-                        model_id=openai_model_id_from_completion(completion)
+                        model_id=model_name
                     )
                 )
 
     passages = [p for p in passages if not isinstance(p, Exception)]
 
-
     return passages
 
+
 async def agenerate_passages(claim_elements: list[tuple[int, str]], prior_art: tuple[int, str], prompt_func: Callable[[str], list[dict]], model_name: str, target_n_passages: int = 10, min_n_splits:int = 1, rate_limiter: Optional[DistributedFixedWindowRateLimiter] = None) -> AsyncIterator[tuple[int, tuple[int, list[str]]]]:
     tasks = []
     for i, claim_element in claim_elements:
         prior_art_splits = split_passage_to_meet_model_token_limit(prior_art[1], partial(prompt_func, claim_element), model_name, min_n_splits=min_n_splits)
         n_passages_per_split = max(target_n_passages // len(prior_art_splits), 1)
         tasks.append(asyncio.create_task(
             agenerate_passages_for_prior_art_splits(prior_art_splits, partial(prompt_func, claim_element, n_passages_per_split=n_passages_per_split), model_name, claim_element_id=i, prior_art_id=prior_art[0], rate_limiter=rate_limiter)
         ))
     
     for coro in asyncio.as_completed(tasks):
         yield await coro
 
+
 def create_generate_passages_tasks(claim_elements: list[tuple[int, str]], prior_art: tuple[int, str], prompt_func: Callable[[str], list[dict]], model_name: str, target_n_passages: int = 10, min_n_splits:int = 1, rate_limiter: Optional[DistributedFixedWindowRateLimiter] = None) -> list[asyncio.Task]:
     tasks = []
     for i, claim_element in claim_elements:
         prior_art_splits = split_passage_to_meet_model_token_limit(prior_art[1], partial(prompt_func, claim_element), model_name, min_n_splits=min_n_splits)
         n_passages_per_split = max(target_n_passages // len(prior_art_splits), 1)
         tasks.append(asyncio.create_task(
             agenerate_passages_for_prior_art_splits(prior_art_splits, partial(prompt_func, claim_element, n_passages_per_split=n_passages_per_split), model_name, claim_element_id=i, prior_art_id=prior_art[0], rate_limiter=rate_limiter)
         ))
 
     return tasks
 
 
 def summarize_patent_prompt_func(serialized_patent_spec: str, instruction: str = None):
     if instruction is None:
-        instruction = "Summarize the following patent specification in approximately 250 words."
+        instruction = "Summarize the following patent specification in approximately 250 words. Your summary should not mention the 'patent', 'the specification', 'various embodiments', or any other language that suggests the summary is from a patent. You should not prefix the summary with 'Summary:' or any other prefatory language. The summary should be a standalone short paragraph."
     return [
         {"role": "system", "content": f"{instruction}"},
-        {"role": "user", "content": serialized_patent_spec},
+        {"role": "user", "content": f'Here is the specification to summarize: {serialized_patent_spec}'},
     ]
 
 
 def summarize_summaries_prompt_func(summaries: List[str], instruction: Optional[str] = None):
     if instruction is None:
-        instruction = "Summarize the following partial summaries of sequential portions of a patent specification in approximately 250 words:"
+        instruction = "Summarize the following partial summaries of sequential portions of a patent specification in approximately 250 words. Your summary should not mention the 'patent', 'the specification', 'various embodiments', or any other language that suggests the summary is from a patent. You should not prefix the summary with 'Summary:' or any other prefatory language. The summary should be a standalone short paragraph"
+    partial_summaries = '\n'.join(summaries)
     return [
         {"role": "system", "content": f"{instruction}"},
-        {"role": "user", "content": '\n'.join(summaries)},
+        {"role": "user", "content": f"Here are the sequential partial summaries I'd like you to summarize: {partial_summaries}"},
     ]
 
+
 def short_summary_prompt_func(summary: str):
     return [
-        {"role": "system", "content": "Condense the following summary to approximately 25 words."},
-        {"role": "system", "content": "As an example, here is a long summary: 'The patent specification describes a closed-loop/semi-closed loop therapy modification system for insulin delivery in diabetes patients, focusing on managing over/under-delivery of medication. The system, incorporating a glucose sensor and insulin pump, triggers alarms based on blood glucose levels or insulin delivery discrepancies, prompting calibration of the sensor system and adjustments to therapy delivery parameters. The system aims to achieve and maintain target blood glucose levels effectively.\n\nThe invention relies on monitoring glucose levels continuously or periodically, adjusting insulin delivery based on the difference between measured and target values. Patient intervention may be required to approve calibration or therapy adjustments. The algorithm limits adjustments within preset boundaries, considering patient's basal pattern. It logs adjustments for patient reference and recommends new basal rates if adjustments consistently reach boundaries.\n\nSafeguards are incorporated to prevent excessive insulin delivery, including safety reviews, real-time calibration adjustment procedures, and safeguards when transitioning from closed-loop to open-loop systems. Additionally, the system accounts for insulin on board delays, ensuring insulin action is adequate before increasing doses. A model supervisory system and tolerance intervals further enhance safety and accuracy in therapy management.\n\nThe specification emphasizes versatility, adaptability, and patient-centric customization, aiming to optimize insulin therapy for diabetes patients. Various embodiments are discussed to address different scenarios and challenges that may arise during insulin delivery, ensuring patient safety and treatment effectiveness throughout the process.'"},
-        {"role": "system", "content": "Here is an initial attempt at a condensed summary: 'Description of a closed-loop/semi-closed loop system for insulin delivery in diabetes patients, focusing on managing medication delivery with glucose sensor and insulin pump for optimized therapy results.'"},
-        {"role": "system", "content": "Here is a second attempt at a condensed summary: 'Closed-loop/semi-closed loop therapy modification system for insulin delivery in diabetes patients, focusing on managing medication delivery with glucose sensor and insulin pump for optimized therapy results.' This attempt is better because it omits the 'Description of' preamble and focuses exlusively on describing the invention. Your condensed summary should not mention the 'patent', 'the specification', 'various embodiments', or any other language that suggests the summary is from a patent. You should not prefix the summary with 'Summary:' or the like. The summary should be a standalone short paragraph or sentence."},
+        {"role": "system", "content": "Condense the following summary to approximately 25 words. As an example, here is a long summary: 'The patent specification describes a closed-loop/semi-closed loop therapy modification system for insulin delivery in diabetes patients, focusing on managing over/under-delivery of medication. The system, incorporating a glucose sensor and insulin pump, triggers alarms based on blood glucose levels or insulin delivery discrepancies, prompting calibration of the sensor system and adjustments to therapy delivery parameters. The system aims to achieve and maintain target blood glucose levels effectively.\n\nThe invention relies on monitoring glucose levels continuously or periodically, adjusting insulin delivery based on the difference between measured and target values. Patient intervention may be required to approve calibration or therapy adjustments. The algorithm limits adjustments within preset boundaries, considering patient's basal pattern. It logs adjustments for patient reference and recommends new basal rates if adjustments consistently reach boundaries.\n\nSafeguards are incorporated to prevent excessive insulin delivery, including safety reviews, real-time calibration adjustment procedures, and safeguards when transitioning from closed-loop to open-loop systems. Additionally, the system accounts for insulin on board delays, ensuring insulin action is adequate before increasing doses. A model supervisory system and tolerance intervals further enhance safety and accuracy in therapy management.\n\nThe specification emphasizes versatility, adaptability, and patient-centric customization, aiming to optimize insulin therapy for diabetes patients. Various embodiments are discussed to address different scenarios and challenges that may arise during insulin delivery, ensuring patient safety and treatment effectiveness throughout the process.' Here is an initial attempt at a condensed summary: 'Description of a closed-loop/semi-closed loop system for insulin delivery in diabetes patients, focusing on managing medication delivery with glucose sensor and insulin pump for optimized therapy results.' Here is a second attempt at a condensed summary: 'Closed-loop/semi-closed loop therapy modification system for insulin delivery in diabetes patients, focusing on managing medication delivery with glucose sensor and insulin pump for optimized therapy results.' This attempt is better because it omits the 'Description of' preamble and focuses exclusively on describing the invention. Your condensed summary should not mention the 'patent', 'the specification', 'various embodiments', or any other language that suggests the summary is from a patent. You should not prefix the summary with 'Summary:' or any other prefatory language. The summary should be a standalone short paragraph or sentence."},
         {"role": "user", "content": f'Here is the long summary for you to summarize: {summary}'},
     ]
 
+
 def topics_from_summary_prompt_func(summary: str):
     return [
-        {"role": "system", "content": "Identify the main topics in the following summary. You may state up to 5 topics in a comma separated list. If you believe there are fewer than 5 topics, you may state fewer. If you believe there are more than 5 topics, you may state the most important 5. Each topic should be one exactly one word. As an example, here is a long summary: 'The patent specification describes a closed-loop/semi-closed loop therapy modification system for insulin delivery in diabetes patients, focusing on managing over/under-delivery of medication. The system, incorporating a glucose sensor and insulin pump, triggers alarms based on blood glucose levels or insulin delivery discrepancies, prompting calibration of the sensor system and adjustments to therapy delivery parameters. The system aims to achieve and maintain target blood glucose levels effectively.\n\nThe invention relies on monitoring glucose levels continuously or periodically, adjusting insulin delivery based on the difference between measured and target values. Patient intervention may be required to approve calibration or therapy adjustments. The algorithm limits adjustments within preset boundaries, considering patient's basal pattern. It logs adjustments for patient reference and recommends new basal rates if adjustments consistently reach boundaries.\n\nSafeguards are incorporated to prevent excessive insulin delivery, including safety reviews, real-time calibration adjustment procedures, and safeguards when transitioning from closed-loop to open-loop systems. Additionally, the system accounts for insulin on board delays, ensuring insulin action is adequate before increasing doses. A model supervisory system and tolerance intervals further enhance safety and accuracy in therapy management.\n\nThe specification emphasizes versatility, adaptability, and patient-centric customization, aiming to optimize insulin therapy for diabetes patients. Various embodiments are discussed to address different scenarios and challenges that may arise during insulin delivery, ensuring patient safety and treatment effectiveness throughout the process.' And this would be an acceptable output: 'Insulin delivery, Diabetes, Therapy system, Monitoring, Glucose sensor'. Topics should reference the specifics of the invention, not the patent or the specification. For example, 'Patent specification' would be an unacceptable topic."},
+        {"role": "system", "content": "Identify the main topics in the following summary. You may state up to 5 topics in a comma separated list. If you believe there are fewer than 5 topics, you may state fewer. If you believe there are more than 5 topics, you may state the most important 5. Each topic should be one exactly one word. As an example, here is a long summary: 'The patent specification describes a closed-loop/semi-closed loop therapy modification system for insulin delivery in diabetes patients, focusing on managing over/under-delivery of medication. The system, incorporating a glucose sensor and insulin pump, triggers alarms based on blood glucose levels or insulin delivery discrepancies, prompting calibration of the sensor system and adjustments to therapy delivery parameters. The system aims to achieve and maintain target blood glucose levels effectively.\n\nThe invention relies on monitoring glucose levels continuously or periodically, adjusting insulin delivery based on the difference between measured and target values. Patient intervention may be required to approve calibration or therapy adjustments. The algorithm limits adjustments within preset boundaries, considering patient's basal pattern. It logs adjustments for patient reference and recommends new basal rates if adjustments consistently reach boundaries.\n\nSafeguards are incorporated to prevent excessive insulin delivery, including safety reviews, real-time calibration adjustment procedures, and safeguards when transitioning from closed-loop to open-loop systems. Additionally, the system accounts for insulin on board delays, ensuring insulin action is adequate before increasing doses. A model supervisory system and tolerance intervals further enhance safety and accuracy in therapy management.\n\nThe specification emphasizes versatility, adaptability, and patient-centric customization, aiming to optimize insulin therapy for diabetes patients. Various embodiments are discussed to address different scenarios and challenges that may arise during insulin delivery, ensuring patient safety and treatment effectiveness throughout the process.' And this would be an acceptable output: 'Insulin delivery, Diabetes, Therapy system, Monitoring, Glucose sensor'. Topics should reference the specifics of the invention, not the patent or the specification. For example, 'Patent specification' would be an unacceptable topic. Do not include prefatory language such as 'Based on the provided summary, here are the main topics:' or 'The main topics are:', just return the five topics each separated by a comma."},
         {"role": "user", "content": f'Here is the long summary for you to choose topics from: {summary}'},
     ]
 
-# def topics_from_summary_prompt_func(summary: str):
-#     return [
-#         {"role": "system", "content": "Identify the main topics in the following summary. You may state up to 5 topics in a comma separated list. If you believe there are fewer than 5 topics, you may state fewer. If you believe there are more than 5 topics, you may state the most important 5. Each topic should be one or two words. For a hypothetical patent on a glucose monitoring system for diabetics, this is an acceptable output: 'Insulin delivery, Diabetes, Therapy, Glucose monitoring, Sensor'. Do not add numbering or any other punctuation besides commas between each topic."},
-#         {"role": "user", "content": f'Here is the long summary for you to choose topics from: {summary}'},
-#     ]
 
 def parse_topics(topics: str) -> list[str]:
     topics_list = topics.split(',')
-    topics_list = [t.strip(' \'') for t in topics_list]
+    topics_list = [t.strip(' \'\n') for t in topics_list]
     return topics_list
 
+
 async def asummarize_patent(patent: parser.GoogleParsedPatent, rate_limiter: Optional[DistributedFixedWindowRateLimiter] = None, generator_config=None):
     if generator_config is None:
         generator_config = load_generator_config_from_env()
     serialized_patent_spec = patent.specification
 
     split_instruction = "Summarize the following portion of a patent specification in approximately 250 words:"
     spec_splits = split_passage_to_meet_model_token_limit(serialized_patent_spec, partial(summarize_patent_prompt_func, instruction=split_instruction), generator_config.model_name)
 
     if len(spec_splits) == 1:
-        summarization_completion = await aopenai_chat_completion_request_with_retry(
+        summarization = await make_get_completion_coro(
             generator_config.model_name, summarize_patent_prompt_func(serialized_patent_spec), rate_limiter=rate_limiter
         )
-        summarization = summarization_completion['choices'][0]['message']['content']
     else:
         tasks = []
         # TODO: hack
         for spec_split in spec_splits[:10]:
             tasks.append(
-                aopenai_chat_completion_request_with_retry(
+                make_get_completion_coro(
                     generator_config.model_name, summarize_patent_prompt_func(spec_split, instruction=split_instruction), rate_limiter=rate_limiter
                 )
             )
-        completions = await asyncio.gather(*tasks)
-        partial_summaries = []
-        for completion in completions:
-            partial_summaries.append(completion['choices'][0]['message']['content'])
-
+        partial_summaries = await asyncio.gather(*tasks)
+        if generator_config.model_name == 'claude-3-opus-20240229':
+            partial_summaries = [post_process_summary_claude_opus(partial_summary) for partial_summary in partial_summaries]
         try:
-            summarization_completion = await aopenai_chat_completion_request_with_retry(
+            summarization = await make_get_completion_coro(
                 generator_config.model_name, summarize_summaries_prompt_func(partial_summaries), rate_limiter=rate_limiter
             )
-            summarization = summarization_completion['choices'][0]['message']['content']
         except GenerationError as e:
             logger.error('Failed to summarize patent %s', patent.unique_id)
             summarization = ''
 
-    short_summary_completion = await aopenai_chat_completion_request_with_retry(
+    if generator_config.model_name == 'claude-3-opus-20240229':
+        summarization = post_process_summary_claude_opus(summarization)
+
+    short_summary = await make_get_completion_coro(
         generator_config.model_name, short_summary_prompt_func(summarization), rate_limiter=rate_limiter
     )
-    short_summary = short_summary_completion['choices'][0]['message']['content']
+    if generator_config.model_name == 'claude-3-opus-20240229':
+        short_summary = post_process_summary_claude_opus(short_summary)
 
-    topics_completion = await aopenai_chat_completion_request_with_retry(
+    topics = await make_get_completion_coro(
         generator_config.model_name, topics_from_summary_prompt_func(summarization), rate_limiter=rate_limiter
     )
-    topics = parse_topics(topics_completion['choices'][0]['message']['content'])
+    topics = parse_topics(topics)
 
     search_index.update_patent_by_id(patent, summary=summarization, short_summary=short_summary, topics=topics)
 
     return summarization
 
 
 async def asummarize_patents(patents: list[parser.GoogleParsedPatent]):
     generator_config = load_generator_config_from_env()
     async with DistributedFixedWindowRateLimiter(token_rate_limit_by_model_name[generator_config.model_name], RATE_LIMIT_INTERVAL) as rate_limiter:
         tasks = [asummarize_patent(patent, rate_limiter=rate_limiter) for patent in patents]
         return await asyncio.gather(*tasks)
 
+
 async def asummarize_patents_gpt4_turbo_preview(patents: list[parser.GoogleParsedPatent]):
     generator_config = load_generator_config_from_env()
     generator_config.model_name = 'gpt-4-turbo-preview'
     async with DistributedFixedWindowRateLimiter(token_rate_limit_by_model_name[generator_config.model_name], RATE_LIMIT_INTERVAL) as rate_limiter:
         tasks = [asummarize_patent(patent, rate_limiter=rate_limiter, generator_config=generator_config) for patent in patents]
         return await asyncio.gather(*tasks)
 
+
+async def hydrate_prompt_with_patent(patent: parser.GoogleParsedPatent, generator_config: GeneratorConfig) -> partial[Callable[[str], list[dict]]]:
+    claims = patent[1].claims
+    all_patent_claim_elements = []
+    for claim in claims:
+        all_patent_claim_elements.extend(claim.claim_elements)
+    serialized_claims = '\n'.join(all_patent_claim_elements)
+    
+    if generator_config.model_name == 'gpt-4':
+        patent_summary = search_index.get_patent_summary(patent[1])
+        if patent_summary is None:
+            patent_summary = await asummarize_patent(patent[1])
+        prompt_func = partial(prompt_summary_full_set_of_claims, patent_summary, serialized_claims)
+        return prompt_func
+    elif generator_config.model_name == 'claude-3-opus-20240229':
+        return partial(prompt_full_spec_full_set_of_claims, patent[1].specification, serialized_claims)
+    else:
+        raise NotImplementedError(f"Model {generator_config} not supported.")
+
+
 async def abulk_generate_passages(
         patent: tuple[int, parser.GoogleParsedPatent], 
         prior_art_sources: list[tuple[int, parser.GoogleParsedPatent]], claim_elements: list[tuple[int, str]],
         ranking_params: dict,
         ) -> AsyncIterator[GeneratedPassage]:
     # TODO: this function should be refactored to separate concerns
     generator_config = load_generator_config_from_env()
     async with DistributedFixedWindowRateLimiter(token_rate_limit_by_model_name[generator_config.model_name], RATE_LIMIT_INTERVAL) as rate_limiter:
-        patent_summary = search_index.get_patent_summary(patent[1])
-        if patent_summary is None:
-            patent_summary = await asummarize_patent(patent[1])
-        claims = patent[1].claims
-        all_patent_claim_elements = []
-        for claim in claims:
-            all_patent_claim_elements.extend(claim.claim_elements)
-        serialized_claims = '\n'.join(all_patent_claim_elements)
+        prompt_func = await hydrate_prompt_with_patent(patent, generator_config)
         tasks = []
         for prior_art_source_uid, prior_art_source in prior_art_sources:
             serialized_prior_art_source = prior_art_source.specification
-            prompt_func = generator_config.generate_passages_prompt_func
-            if prompt_func is prompt_summary_full_set_of_claims:
-                prompt_func = partial(prompt_func, patent_summary, serialized_claims)
-            else:
-                raise NotImplementedError(f"Prompt func {prompt_func} not implemented.")
-
             tasks.extend(
                 create_generate_passages_tasks(
                     claim_elements, (prior_art_source_uid, serialized_prior_art_source), 
                     prompt_func,
                     generator_config.model_name,
                     target_n_passages=generator_config.target_n_passages,
                     min_n_splits=generator_config.min_n_splits,
@@ -553,19 +578,41 @@
                 matching_claim_element = [c for c in claim_elements if c[0] == claim_element_id][0]
                 if not all([p.claim_element_id == claim_element_id for p in generated_passages]):
                     logger.error('Claim element ids do not match')
                 
                 logger.info(f'Ranking {len(generated_passages)} passages')
                 ranked_generated_passages = await ranking.arank_passages(generated_passages, matching_claim_element[1], **ranking_params)
                 for generated_passage in ranked_generated_passages:
-                    # TODO: this depends on parsing patent from pdf working properly
-                    # citation = None
-                    # try:
-                    #     citation = utils.cite_passage(generated_passage.text, patent[1])
-                    # except utils.CitationError as e:
-                    #     logger.error(e)
-                    # else:
-                    #     generated_passage.start_line = citation[0]
-                    #     generated_passage.end_line = citation[1]
-                    # TODO: this doesn't need to be a yield, should just return the whole passage set for each claim element
                     yield generated_passage
-                    
+
+
+@lru_cache
+def num_tokens_from_string(string: str, encoding_name: str = 'cl100k_base') -> int:
+    """Returns the number of tokens in a text string."""
+    encoding = tiktoken.get_encoding(encoding_name)
+    num_tokens = len(encoding.encode(string))
+    return num_tokens
+
+
+@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(6), reraise=True)
+def encode_openai(text_batch):
+    embeddings = oai.embeddings.create(
+        input=text_batch,
+        model='text-embedding-3-large',
+        dimensions=1024
+    )
+    return [e.embedding for e in embeddings.data]
+
+
+def batch_encode_openai(texts):
+    i = 0
+    embeddings = []
+    while i < len(texts):
+        batch_tok_count = 0
+        batch = []
+        while i < len(texts) and batch_tok_count + num_tokens_from_string(texts[i]) < MAX_SEQ_LENGTH:
+            batch_tok_count += num_tokens_from_string(texts[i])
+            batch.append(texts[i])
+            i += 1
+        embeddings.extend(encode_openai(batch))
+        
+    return embeddings
```

### Comparing `patent_chart-0.2.5/patent_chart/google_patents.py` & `patent_chart-0.2.7/patent_chart/google_patents.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,16 +49,15 @@
             )
         claim.claim_elements.append(line)
 
     return google_claims
 
 
 def parse_google_patent(patent_unique_id: PatentUniqueID) ->  GoogleParsedPatent | None:
-    google_id = f'{patent_unique_id.country_code}{patent_unique_id.patent_number}{patent_unique_id.kind_code or ""}'
-    url = f"https://patents.google.com/patent/{google_id}/en"
+    url = f"https://patents.google.com/patent/{patent_unique_id}/en"
 
     logger.info('Requesting %s', url)
 
     # Send an HTTP GET request to fetch the webpage
     response = google_request_with_retry(url)
 
     # Parse the HTML content of the page using BeautifulSoup
```

### Comparing `patent_chart-0.2.5/patent_chart/integrationtests.py` & `patent_chart-0.2.7/patent_chart/integrationtests.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/opensearch.py` & `patent_chart-0.2.7/patent_chart/search_index.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,72 @@
 import typing
 
-from elasticsearch import Elasticsearch, RequestsHttpConnection
-from requests_aws4auth import AWS4Auth
-import boto3
+from elasticsearch import Elasticsearch
 
+from . import settings
 from . import parser
 
-host = 'vpc-patents-fbqas7tj6njmlbjopex7thfxzm.us-east-2.es.amazonaws.com'
-region = 'us-east-2'
+client = Elasticsearch(settings.ELASTIC_HOST)
 
-session = boto3.Session()
-credentials = session.get_credentials()
-
-awsauth = AWS4Auth(
-    credentials.access_key,
-    credentials.secret_key,
-    region,
-    'es',
-    session_token=credentials.token
-)
-
-client = Elasticsearch(
-    hosts=[{'host': host, 'port': 443}],
-    http_auth=awsauth,
-    use_ssl=True,
-    verify_certs=True,
-    connection_class=RequestsHttpConnection
-)
+XML_USPTO_POST_2001 = 'xml_uspto_post_2001'
 
 
 class IndexedPatent(parser.GoogleParsedPatent):
     summary: typing.Optional[str] = None
     short_summary: typing.Optional[str] = None
     topics: typing.Optional[typing.List[str]] = None
     text: typing.Optional[str] = None
     text_format: typing.Optional[str] = None
 
-XML_USPTO_POST_2001 = 'xml_uspto_post_2001'
 
-CLAIM_EMBEDDING_MAPPINGS = {
+claim_embedding_scheme = {
     "properties": {
         "patent_doc_id": {
             "type": "keyword"
         },
         "claim_id": {
             "type": "keyword"
         },
         "embedding": {
-            "type": "knn_vector",
-            "dimension": 1024,
-            "method": {
-                "name": "hnsw",
-                "space_type": "cosinesimil",
-                "engine": "nmslib",
-                "parameters": {
-                    "ef_construction": 128,
-                    "m": 64
-                }
-            }
+            "type": "dense_vector",
+            "dims": 1024
+        },
+        'filing_date': {
+            'type': 'date'
+        },
+        'priority_date': {
+            'type': 'date'
         }
     }
 }
 
-SPECIFICATION_EMBEDDING_MAPPINGS = {
+
+specification_embedding_scheme = {
     "properties": {
         "patent_doc_id": {
             "type": "keyword"
         },
         "paragraph_id": {
             "type": "keyword"
         },
         "embedding": {
-            "type": "knn_vector",
-            "dimension": 1024,
-            "method": {
-                "name": "hnsw",
-                "space_type": "cosinesimil",
-                "engine": "nmslib",
-                "parameters": {
-                    "ef_construction": 128,
-                    "m": 64
-                }
-            }
+            "type": "dense_vector",
+            "dims": 1024
+        },
+        'filing_date': {
+            'type': 'date'
+        },
+        'priority_date': {
+            'type': 'date'
         }
     }
 }
 
-PATENTS_MAPPINGS = {
+
+patent_scheme = {
     "properties": {
         "unique_id": {
             "properties": {
                 "patent_number": {
                     "type": "keyword"
                 },
                 "country_code": {
@@ -150,71 +126,69 @@
         },
         'text': {
             'type': 'text'
         },
         'text_format': {
             'type': 'keyword'
         },
+        'filing_date': {
+            'type': 'date'
+        },
+        'priority_date': {
+            'type': 'date'
+        }
     }
 }
 
+
 def create_specification_embedding_index():
-    body = {
-        "settings": {
-            "index": {
-                "knn": True,
-                "knn.algo_param.ef_search": 100
-            }
-        },
-    }
     try:
-        client.indices.create(index='patents_specification_embedding', body=body)
+        client.indices.create(index='patents_specification_embedding')
     except Exception as e:
         pass
-    client.indices.put_mapping(index='patents_specification_embedding', body=SPECIFICATION_EMBEDDING_MAPPINGS)
+    client.indices.put_mapping(index='patents_specification_embedding', body=specification_embedding_scheme)
 
 
 def create_claim_embedding_index():
-    body = {
-        "settings": {
-            "index": {
-                "knn": True,
-                "knn.algo_param.ef_search": 100
-            }
-        },
-    }
     try:
-        client.indices.create(index='patents_claim_embedding', body=body)
+        client.indices.create(index='patents_claim_embedding')
     except Exception as e:
         pass
-    client.indices.put_mapping(index='patents_claim_embedding', body=CLAIM_EMBEDDING_MAPPINGS)
+    client.indices.put_mapping(index='patents_claim_embedding', body=claim_embedding_scheme)
 
 
 def create_patents_index():
     try:
         client.indices.create(index='patents')
     except Exception as e:
         pass
-    client.indices.put_mapping(index='patents', body=PATENTS_MAPPINGS)
+    client.indices.put_mapping(index='patents', body=patent_scheme)
 
-def index_patent(unique_id, text, title, text_format=None):
+
+def index_patent(unique_id, text, title, text_format=None, filing_date=None, priority_date=None):
     body = {
         "unique_id": {
             "patent_number": unique_id.patent_number,
             "kind_code": unique_id.kind_code,
             "country_code": unique_id.country_code
         },
         "text": text,
         "title": title
     }
 
     if text_format:
         body['text_format'] = text_format
     else:
         body['text_format'] = XML_USPTO_POST_2001
+
+    if filing_date:
+        body['filing_date'] = filing_date
+
+    if priority_date:
+        body['priority_date'] = priority_date
         
     client.index(index='patents', id=str(unique_id), body=body)
     return str(unique_id)
 
 
 def index_claim_embedding(patent_doc_id, embedding, claim_id=None):
     body = {
@@ -222,36 +196,42 @@
         "embedding": embedding
     }
     if claim_id:
         body['claim_id'] = claim_id
 
     client.index(index='patents_claim_embedding', body=body)
 
+
 def index_specification_embedding(patent_doc_id, embedding, paragraph_id=None):
     body = {
         "patent_doc_id": patent_doc_id,
         "embedding": embedding
     }
     if paragraph_id:
         body['paragraph_id'] = paragraph_id
     client.index(index='patents_specification_embedding', body=body)
 
+
 def get_patent_summary(patent: parser.GoogleParsedPatent) -> str:
     response = client.get(index='patents', id=str(patent.unique_id))
     return response['_source'].get('summary')
 
+
 def update_patent_by_id(patent: parser.GoogleParsedPatent, **kwargs):
     client.update(index='patents', id=str(patent.unique_id), body={'doc': kwargs})
 
-def patent_specification_knn_search(query_vector: list[float]):
-    body = {
-        'query': {
-            'knn': {
-                'embedding': {
-                    'vector': query_vector,
-                    'k': 10
-                }
-            }
-        }
-    }
-    response = client.search(index='patents_specification_embedding', body=body)
-    return [hit['_source'] for hit in response['hits']['hits']]
+
+def patent_exists(patent_unique_id: parser.PatentUniqueID | str) -> bool:
+    try:
+        client.get(index='patents', id=str(patent_unique_id))
+        return True
+    except Exception as e:
+        return False
+    
+
+def get_patent_content_by_id(patent_id: str) -> IndexedPatent | None:
+    try:
+        response = client.get(index='patents', id=patent_id)
+    except Exception as e:
+        logger.error('Patent id %s not found in the index', patent_id)
+        return None
+    return IndexedPatent(**response['_source'])
```

### Comparing `patent_chart-0.2.5/patent_chart/parser.py` & `patent_chart-0.2.7/patent_chart/parser.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/ranking.py` & `patent_chart-0.2.7/patent_chart/ranking.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,49 @@
 import random
 import asyncio
 import time
 from logging import getLogger
 from typing import Optional
 
 import numpy as np
-# from sentence_transformers import SentenceTransformer
-# See https://gitlab.com/bloomsday-labs/ulysses/-/issues/47
-import openai
+from openai import OpenAI, AsyncOpenAI, OpenAIError
 import tiktoken
 
 from .data_structures import GeneratedPassage
 from .requests_utils import DistributedFixedWindowRateLimiter
 from .utils import num_tokens_from_messages
 
 logger = getLogger(__name__)
 
-# _cached_sentence_transformer_model = None
+oai = OpenAI()
+async_oai = AsyncOpenAI()
+
 
-# sentence_transformer_models = [
-#     'all-MiniLM-L6-v2'
-# ]
 openai_models = [
     'text-embedding-3-large'
 ]
 
-def num_tokens_from_string(string: str, encoding_name: str) -> int:
+def num_tokens_from_string(string: str, encoding_name: str = 'cl100k_base') -> int:
     """Returns the number of tokens in a text string."""
     encoding = tiktoken.get_encoding(encoding_name)
     num_tokens = len(encoding.encode(string))
     return num_tokens
 
-# def get_cached_sentence_transformer_model(model_name):
-#     global _model
-#     if _cached_sentence_transformer_model is None:
-#         _cached_sentence_transformer_model = SentenceTransformer(model_name)
-#     return _cached_sentence_transformer_model
 
 def openai_embedding_request_with_retry(model_name, input, backoff_factor=2, backoff_override=None, n_retries=3, **kwargs) -> list[list[float]]:
     """Send a chat completion request to OpenAI with retries."""
     for i in range(1, 1 + n_retries):
         try:
-            embeddings = openai.Embedding.create(
+            embeddings = oai.embeddings.create(
                 input=input,
                 model=model_name,
                 **kwargs
             )
-            return [e['embedding'] for e in embeddings['data']]
-        # except openai.OpenAIError as e:
-        except openai.error.OpenAIError as e:
+            return [e.embedding for e in embeddings.data]
+        except OpenAIError as e:
             logger.error(f"OpenAIError: {e}")
             if backoff_override is not None:
                 jitter = random.uniform(-0.10, 0.10)
                 time.sleep(backoff_override * (1 + jitter))
             else:
                 jitter = random.uniform(-0.10, 0.10) 
                 time.sleep(backoff_factor**i * (1 + jitter))
@@ -61,22 +52,21 @@
             raise e
     raise Exception(f"Failed to send embedding request to OpenAI after {n_retries} retries.")
 
 async def aopenai_embedding_request_with_retry(model_name, input, backoff_factor=2, backoff_override=None, n_retries=3, **kwargs) -> list[list[float]]:
     """Send a chat completion request to OpenAI with retries."""
     for i in range(1, 1 + n_retries):
         try:
-            embeddings = await openai.Embedding.acreate(
+            embeddings = await async_oai.embeddings.create(
                 input=input,
                 model=model_name,
                 **kwargs
             )
-            return [e['embedding'] for e in embeddings['data']]
-        # except openai.OpenAIError as e:
-        except openai.error.OpenAIError as e:
+            return [e.embedding for e in embeddings.data]
+        except OpenAIError as e:
             logger.error(f"OpenAIError: {e}")
             if backoff_override is not None:
                 jitter = random.uniform(-0.10, 0.10)
                 await asyncio.sleep(backoff_override * (1 + jitter))
             else:
                 jitter = random.uniform(-0.10, 0.10) 
                 await asyncio.sleep(backoff_factor**i * (1 + jitter))
@@ -84,37 +74,21 @@
         except Exception as e:
             raise e
     raise Exception(f"Failed to send embedding request to OpenAI after {n_retries} retries.")
 
 class RankingModel:
     def __init__(self, model):
         self.model_name = model
-        # if self.model_name not in sentence_transformer_models and self.model_name not in openai_models:
-        #     raise ValueError(f'Invalid model name: {model}')
         if self.model_name not in openai_models:
             raise ValueError(f'Invalid model name: {model}')
 
-    # @property
-    # def openai_client(self):
-    #     if not hasattr(self, '_open_ai_client'):
-    #         self._openai_client = openai.OpenAI()
-    #     return self._openai_client
-
     def encode(self, chunks: list[str] | str):
-        # if self.model_name in sentence_transformer_models:
-        #     return get_cached_sentence_transformer_model(self.model_name).encode(chunks)
-        # elif self.model_name in openai_models:
         if self.model_name in openai_models:
             if isinstance(chunks, str):
                 chunks = [chunks]
-            # embeddings = self.openai_client.embeddings.create(
-            #     input=chunks,
-            #     model=self.model_name,
-            #     dimensions=256,
-            # )
             return openai_embedding_request_with_retry(self.model_name, chunks, dimensions=256)
         
     async def aencode(self, chunks: list[str] | str):
         if self.model_name in openai_models:
             if isinstance(chunks, str):
                 chunks = [chunks]
             return await aopenai_embedding_request_with_retry(self.model_name, chunks, dimensions=256)
```

### Comparing `patent_chart-0.2.5/patent_chart/redis_utils.py` & `patent_chart-0.2.7/patent_chart/redis_utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/requests_utils.py` & `patent_chart-0.2.7/patent_chart/requests_utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/settings.py` & `patent_chart-0.2.7/patent_chart/settings.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/tests.py` & `patent_chart-0.2.7/patent_chart/tests.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/patent_chart/utils.py` & `patent_chart-0.2.7/patent_chart/utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.5/pyproject.toml` & `patent_chart-0.2.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "patent-chart"
-version = "0.2.5"
+version = "0.2.7"
 description = "Automated invalidity contention charts"
 authors = ["Josh Hedtke"]
 license = "Proprietary"
 readme = "README.md"
 
 exclude = ["experiments.ipynb"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^1.0.0"
 tiktoken = "^0.5.1"
 pdfminer-six = "^20221105"
 pydantic = "^2.4.2"
 beautifulsoup4 = "^4.12.2"
-openai = "0.28.1"
+openai = "^1.13.1"
 redis = "^5.0.1"
 pandas = "2.1"
 huggingface-hub = "^0.21.3"
 requests-aws4auth = "^1.2.3"
-opensearch-py = "^2.4.2"
-anthropic = "^0.20.0"
+anthropic = "^0.21.0"
 elasticsearch = "^8.12.1"
+pinecone-client = {version = "^3.2.1", extras = ["grpc"]}
+tenacity = "^8.2.3"
+langchain = "^0.1.14"
 
 
 [tool.poetry.group.dev.dependencies]
 pdfplumber = "^0.10.2"
 jupyter = "^1.0.0"
 tiktoken = "^0.5.1"
 python-dotenv = "^1.0.0"
@@ -34,14 +36,14 @@
 pypdf2 = "^3.0.1"
 pdfminer-six = "^20221105"
 pypdf = "^3.16.4"
 matplotlib = "^3.8.0"
 tabula-py = "^2.8.2"
 sentence-transformers = "^2.3.1"
 boto3 = "^1.34.46"
-langchain = "^0.1.8"
 tqdm = "^4.66.2"
-apache-beam = {extras = ["aws"], version = "^2.54.0"}
+plotly = "^5.20.0"
+apache-beam = "^2.55.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `patent_chart-0.2.5/PKG-INFO` & `patent_chart-0.2.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: patent-chart
-Version: 0.2.5
+Version: 0.2.7
 Summary: Automated invalidity contention charts
 License: Proprietary
 Author: Josh Hedtke
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anthropic (>=0.20.0,<0.21.0)
+Requires-Dist: anthropic (>=0.21.0,<0.22.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: elasticsearch (>=8.12.1,<9.0.0)
 Requires-Dist: huggingface-hub (>=0.21.3,<0.22.0)
-Requires-Dist: openai (==0.28.1)
-Requires-Dist: opensearch-py (>=2.4.2,<3.0.0)
+Requires-Dist: langchain (>=0.1.14,<0.2.0)
+Requires-Dist: openai (>=1.13.1,<2.0.0)
 Requires-Dist: pandas (==2.1)
 Requires-Dist: pdfminer-six (>=20221105,<20221106)
+Requires-Dist: pinecone-client[grpc] (>=3.2.1,<4.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: redis (>=5.0.1,<6.0.0)
 Requires-Dist: requests-aws4auth (>=1.2.3,<2.0.0)
+Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tiktoken (>=0.5.1,<0.6.0)
 Description-Content-Type: text/markdown
```

