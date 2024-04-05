# Comparing `tmp/spiceai-0.1.7.tar.gz` & `tmp/spiceai-0.1.8.tar.gz`

## Comparing `spiceai-0.1.7.tar` & `spiceai-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 spiceai-0.1.7/tags
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 spiceai-0.1.7/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spiceai-0.1.7/.ropeproject/globalnames
--rw-r--r--   0        0        0    33445 2020-02-02 00:00:00.000000 spiceai-0.1.7/.ropeproject/history
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 spiceai-0.1.7/scripts/run.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 spiceai-0.1.7/spice/__init__.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 spiceai-0.1.7/spice/client_manager.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 spiceai-0.1.7/spice/embeddings.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 spiceai-0.1.7/spice/errors.py
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 spiceai-0.1.7/spice/spice.py
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 spiceai-0.1.7/spice/utils.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spiceai-0.1.7/spice/whisper.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 spiceai-0.1.7/spice/wrapped_clients.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 spiceai-0.1.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.1.7/LICENSE
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 spiceai-0.1.7/README.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 spiceai-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 spiceai-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 spiceai-0.1.8/tags
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spiceai-0.1.8/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.1.8/.ropeproject/globalnames
+-rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.1.8/.ropeproject/history
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 spiceai-0.1.8/scripts/run.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/errors.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/models.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/providers.py
+-rw-r--r--   0        0        0    17415 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/spice.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/spice_message.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/utils.py
+-rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 spiceai-0.1.8/spice/wrapped_clients.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.1.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 spiceai-0.1.8/README.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 spiceai-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 spiceai-0.1.8/PKG-INFO
```

### Comparing `spiceai-0.1.7/.github/workflows/ruff.yml` & `spiceai-0.1.8/.github/workflows/ruff.yml`

 * *Files 3% similar despite different names*

```diff
@@ -12,12 +12,12 @@
           uv pip install .
           uv pip install .[dev]
       - name: activate venv
         run: |
           . .venv/bin/activate
           echo PATH=$PATH >> $GITHUB_ENV
       - name: ruff (linter)
-        run: ruff check .
+        run: ruff check --select I .
       - name: ruff (formatter)
         run: ruff format --check .
       - name: pyright
         run: pyright
```

### Comparing `spiceai-0.1.7/spice/client_manager.py` & `spiceai-0.1.8/spice/providers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,84 @@
+from __future__ import annotations
+
 import os
+from dataclasses import dataclass
+from typing import Callable, List
 
 from dotenv import load_dotenv
 
-from spice.errors import SpiceError
-from spice.wrapped_clients import WrappedAnthropicClient, WrappedAzureClient, WrappedOpenAIClient
+from spice.errors import InvalidProviderError, NoAPIKeyError, SpiceError
+from spice.wrapped_clients import WrappedAnthropicClient, WrappedAzureClient, WrappedClient, WrappedOpenAIClient
+
+# Used to fetch a provider by name
+providers: List[Provider] = []
+
+
+@dataclass
+class Provider:
+    name: str
+    get_client: Callable[[], WrappedClient]
+
+    def __post_init__(self):
+        providers.append(self)
 
-load_dotenv()
 
+def get_openai_client(cache=[]):
+    if cache:
+        return cache[0]
 
-def _get_client(provider):
-    if provider == "anthropic":
-        key = os.getenv("ANTHROPIC_API_KEY")
-        if key is None:
-            raise SpiceError("ANTHROPIC_API_KEY not set")
-        return WrappedAnthropicClient(key)
-    elif provider == "openai":
-        base_url = os.getenv("OPENAI_API_BASE")
-        key = os.getenv("OPENAI_API_KEY")
-        if key is None:
-            if base_url:
-                # Using a dummy key for LiteLLM proxy setup where OPENAI_API_BASE is set but OPENAI_API_KEY is not required.
-                key = "dummy_key_base_url"
-            else:
-                raise SpiceError("OPENAI_API_KEY not set")
-        return WrappedOpenAIClient(key, base_url)
-    elif provider == "azure":
-        key = os.getenv("AZURE_OPENAI_KEY")
-        endpoint = os.getenv("AZURE_OPENAI_ENDPOINT")
-        if key is None:
-            raise SpiceError("AZURE_OPENAI_KEY not set")
-        if endpoint is None:
-            raise SpiceError("AZURE_OPENAI_ENDPOINT not set")
-        return WrappedAzureClient(key, endpoint)
-    else:
-        raise SpiceError(f"Unknown provider: {provider}")
-
-
-def _get_clients_from_env():
-    known_providers = {"openai", "anthropic", "azure"}
-    clients = {}
-    for provider in known_providers:
-        try:
-            clients[provider] = _get_client(provider)
-        except SpiceError:
-            pass
-    if not clients:
-        raise SpiceError("No known providers found in environment")
-    return clients
-
-
-_model_info = {
-    "gpt-4-0125-preview": {"provider": "openai"},
-    "gpt-4-vision-preview": {"provider": "openai"},
-    "gpt-3.5-turbo-0125": {"provider": "openai"},
-    "claude-3-opus-20240229": {"provider": "anthropic"},
-    "claude-3-haiku-20240307": {"provider": "anthropic"},
-}
-
-
-def _get_provider_from_model_name(model):
-    if model not in _model_info:
-        raise SpiceError(f"Unknown provider for model: {model}")
-    return _model_info[model]["provider"]
-
-
-def _validate_model_aliases(model_aliases, clients):
-    for alias, model_dict in model_aliases.items():
-        model_name = model_dict["model"]
-        if "provider" in model_dict:
-            provider = model_dict["provider"]
+    base_url = os.getenv("OPENAI_API_BASE")
+    key = os.getenv("OPENAI_API_KEY")
+    if key is None:
+        if base_url:
+            # Using a dummy key for LiteLLM proxy setup where OPENAI_API_BASE is set but OPENAI_API_KEY is not required.
+            key = "dummy_key"
         else:
-            provider = _get_provider_from_model_name(model_name)
-        if provider not in clients:
-            raise SpiceError(f"Provider {provider} is not set up for model {model_name} ({alias})")
+            raise NoAPIKeyError("OPENAI_API_KEY not set")
+
+    client = WrappedOpenAIClient(key, base_url)
+    cache.append(client)
+    return client
+
+
+def get_azure_client(cache=[]):
+    if cache:
+        return cache[0]
+
+    key = os.getenv("AZURE_OPENAI_KEY")
+    endpoint = os.getenv("AZURE_OPENAI_ENDPOINT")
+    if key is None:
+        raise NoAPIKeyError("AZURE_OPENAI_KEY not set")
+    if endpoint is None:
+        raise SpiceError("AZURE_OPENAI_ENDPOINT not set")
+
+    client = WrappedAzureClient(key, endpoint)
+    cache.append(client)
+    return client
+
+
+def get_anthropic_client(cache=[]):
+    if cache:
+        return cache[0]
+
+    key = os.getenv("ANTHROPIC_API_KEY")
+    if key is None:
+        raise NoAPIKeyError("ANTHROPIC_API_KEY not set")
+
+    client = WrappedAnthropicClient(key)
+    cache.append(client)
+    return client
+
+
+load_dotenv()
+
+OPEN_AI = Provider("open_ai", get_openai_client)
+AZURE = Provider("azure", get_azure_client)
+ANTHROPIC = Provider("anthropic", get_anthropic_client)
+
+
+def get_provider_from_name(provider_name: str) -> Provider:
+    for provider in providers:
+        if provider.name == provider_name:
+            return provider
+
+    raise InvalidProviderError(f"Unknown provider {provider_name}")
```

### Comparing `spiceai-0.1.7/spice/utils.py` & `spiceai-0.1.8/spice/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import base64
 import io
 
 import tiktoken
 from PIL import Image
 
+from spice.spice_message import SpiceMessage
+
 
 def fuzzy_model_lookup(model_hint):
     model_hint = str(model_hint).lower()
 
     models_list = [
         "gpt-4-0125-preview",
         "gpt-3.5-turbo-0125",
@@ -38,15 +40,15 @@
     If full_message is true, will include the extra 4 tokens used in a chat completion by this message
     if this message is part of a prompt. You do NOT want full_message to be true for a response.
     """
     encoding = get_encoding_for_model(model)
     return len(encoding.encode(message, disallowed_special=())) + (4 if full_message else 0)
 
 
-def count_messages_tokens(messages: list[dict], model: str):
+def count_messages_tokens(messages: list[SpiceMessage], model: str):
     """
     Returns the number of tokens used by a prompt if it was sent to OpenAI for a chat completion.
     Adapted from https://platform.openai.com/docs/guides/text-generation/managing-tokens
     """
     encoding = get_encoding_for_model(model)
 
     num_tokens = 0
```

### Comparing `spiceai-0.1.7/LICENSE` & `spiceai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.7/README.md` & `spiceai-0.1.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,76 +3,100 @@
 ## Usage Examples
 
 All examples can be found in [scripts/run.py](scripts/run.py)
 
 ```python
 from spice import Spice
 
-messages = [
+client = Spice()
+
+messages: List[SpiceMessage] = [
     {"role": "system", "content": "You are a helpful assistant."},
     {"role": "user", "content": "list 5 random words"},
 ]
+response = await client.get_response(messages=messages, model="gpt-4-0125-preview")
 
-client = Spice()
-response = await client.call_llm(messages=messages, model="gpt-4-0125-preview")
 print(response.text)
 ```
 
 ### Streaming
 
 ```python
-# you can set a default model for the client instead of passing it with each call
-client = Spice(model="claude-3-opus-20240229")
+# You can set a default model for the client instead of passing it with each call
+client = Spice(default_text_model="claude-3-opus-20240229")
 
-# the messages format is automatically converted for the Anthropic API
-response = await client.call_llm(messages=messages, stream=True)
+messages: List[SpiceMessage] = [
+    {"role": "system", "content": "You are a helpful assistant."},
+    {"role": "user", "content": "list 5 random words"},
+]
+stream = await client.stream_response(messages=messages)
 
-# spice wraps the stream to extract just the text you care about
-async for text in response.stream():
+async for text in stream:
     print(text, end="", flush=True)
+# Retrieve the complete response from the stream
+response = await stream.complete_response()
 
-# response always includes the final text, no need build it from the stream yourself
+# Response always includes the final text, no need build it from the stream yourself
 print(response.text)
 
-# response also includes helpful stats
+# Response also includes helpful stats
 print(f"Took {response.total_time:.2f}s")
-print(f"Time to first token: {response.time_to_first_token:.2f}s")
 print(f"Input/Output tokens: {response.input_tokens}/{response.output_tokens}")
 ```
 
 ### Mixing Providers
 
 ```python
-# alias model names for easy configuration, even mixing providers
+# Commonly used models and providers have premade constants
+from spice.models import GPT_4_0125_PREVIEW
+
+# Alias models for easy configuration, even mixing providers
 model_aliases = {
-    "task1_model": {"model": "gpt-4-0125-preview"},
-    "task2_model": {"model": "claude-3-opus-20240229"},
-    "task3_model": {"model": "claude-3-haiku-20240307"},
+    "task1_model": GPT_4_0125_PREVIEW,
+    "task2_model": "claude-3-opus-20240229",
+    "task3_model": "claude-3-haiku-20240307",
 }
 
 client = Spice(model_aliases=model_aliases)
 
+messages: List[SpiceMessage] = [
+    {"role": "system", "content": "You are a helpful assistant."},
+    {"role": "user", "content": "list 5 random words"},
+]
 responses = await asyncio.gather(
-    client.call_llm(messages=messages, model="task1_model"),
-    client.call_llm(messages=messages, model="task2_model"),
-    client.call_llm(messages=messages, model="task3_model"),
+    client.get_response(messages=messages, model="task1_model"),
+    client.get_response(messages=messages, model="task2_model"),
+    client.get_response(messages=messages, model="task3_model"),
 )
 
 for i, response in enumerate(responses, 1):
     print(f"\nModel {i} response:")
     print(response.text)
     print(f"Characters per second: {response.characters_per_second:.2f}")
 ```
 
-### Logging Callbacks
+### Using unknown models
 
 ```python
-client = Spice(model="gpt-3.5-turbo-0125")
+client = Spice()
 
-# pass a logging function to get a callback after the stream completes
-response = await client.call_llm(
-    messages=messages, stream=True, logging_callback=lambda response: print(response.text)
-)
+messages: List[SpiceMessage] = [
+    {"role": "system", "content": "You are a helpful assistant."},
+    {"role": "user", "content": "list 5 random words"},
+]
 
-async for text in response.stream():
-    print(text, end="", flush=True)
+# To use Azure, specify the provider and the deployment model name
+response = await client.get_response(messages=messages, model="first-gpt35", provider="azure")
+print(response.text)
+
+# Alternatively, to make a model and it's provider known to Spice, create a custom Model object
+from spice.models import TextModel
+from spice.providers import AZURE
+
+AZURE_GPT = TextModel("first-gpt35", AZURE, context_length=16385)
+response = await client.get_response(messages=messages, model=AZURE_GPT)
+print(response.text)
+
+# Creating the model automatically registers it in Spice's model list, so listing the provider is no longer needed
+response = await client.get_response(messages=messages, model="first-gpt35")
+print(response.text)
 ```
```

