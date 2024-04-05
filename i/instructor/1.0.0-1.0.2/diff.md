# Comparing `tmp/instructor-1.0.0.tar.gz` & `tmp/instructor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.0.0.tar", max compression
+gzip compressed data, was "instructor-1.0.2.tar", max compression
```

## Comparing `instructor-1.0.0.tar` & `instructor-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1066 2024-04-01 14:53:53.827751 instructor-1.0.0/LICENSE
--rw-r--r--   0        0        0     7175 2024-04-01 14:53:53.827751 instructor-1.0.0/README.md
--rw-r--r--   0        0        0      854 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/_types/_alias.py
--rw-r--r--   0        0        0     5738 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/anthropic_utils.py
--rw-r--r--   0        0        0        0 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6494 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/usage.py
--rw-r--r--   0        0        0    11304 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/client.py
--rw-r--r--   0        0        0     8968 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2642 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11922 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/partial.py
--rw-r--r--   0        0        0     6026 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/partialjson.py
--rw-r--r--   0        0        0     1733 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4381 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/exceptions.py
--rw-r--r--   0        0        0     7448 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/function_calls.py
--rw-r--r--   0        0        0      818 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/mode.py
--rw-r--r--   0        0        0     4820 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/patch.py
--rw-r--r--   0        0        0    12697 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/py.typed
--rw-r--r--   0        0        0     5640 2024-04-01 14:53:53.895753 instructor-1.0.0/instructor/retry.py
--rw-r--r--   0        0        0     3955 2024-04-01 14:53:53.895753 instructor-1.0.0/instructor/utils.py
--rw-r--r--   0        0        0     1497 2024-04-01 14:53:53.895753 instructor-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8199 1970-01-01 00:00:00.000000 instructor-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-05 03:42:44.643954 instructor-1.0.2/LICENSE
+-rw-r--r--   0        0        0     8979 2024-04-05 03:42:44.643954 instructor-1.0.2/README.md
+-rw-r--r--   0        0        0     1185 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3792 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/files.py
+-rw-r--r--   0        0        0     5348 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8255 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6494 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/usage.py
+-rw-r--r--   0        0        0     9586 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/client.py
+-rw-r--r--   0        0        0     1712 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     1335 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/client_groq.py
+-rw-r--r--   0        0        0     8968 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     7929 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2165 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2642 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11016 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1733 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4381 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/exceptions.py
+-rw-r--r--   0        0        0     7339 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/function_calls.py
+-rw-r--r--   0        0        0      818 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/mode.py
+-rw-r--r--   0        0        0     4820 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/patch.py
+-rw-r--r--   0        0        0    12534 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/py.typed
+-rw-r--r--   0        0        0     6171 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/retry.py
+-rw-r--r--   0        0        0      266 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/test.py
+-rw-r--r--   0        0        0     4373 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/utils.py
+-rw-r--r--   0        0        0     2151 2024-04-05 03:42:44.711954 instructor-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10659 1970-01-01 00:00:00.000000 instructor-1.0.2/PKG-INFO
```

### Comparing `instructor-1.0.0/LICENSE` & `instructor-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/_types/_alias.py` & `instructor-1.0.2/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/cli/cli.py` & `instructor-1.0.2/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/cli/files.py` & `instructor-1.0.2/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/cli/hub.py` & `instructor-1.0.2/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/cli/jobs.py` & `instructor-1.0.2/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/cli/usage.py` & `instructor-1.0.2/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/client.py` & `instructor-1.0.2/instructor/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import openai
 import inspect
 import instructor
-import anthropic
 from .utils import Provider, get_provider
 from openai.types.chat import ChatCompletion, ChatCompletionMessageParam
-from anthropic.types import Message
 from typing import (
     Type,
     TypeVar,
     Generator,
     Iterable,
     Tuple,
     Callable,
@@ -24,23 +22,23 @@
 from instructor.dsl.partial import Partial
 
 
 T = TypeVar("T", bound=(BaseModel | Iterable | Partial))
 
 
 class Instructor:
-    client: openai.OpenAI | anthropic.Anthropic | None
+    client: Any | None
     create_fn: Any
     mode: instructor.Mode
     default_model: str | None = None
     provider: Provider
 
     def __init__(
         self,
-        client: openai.OpenAI | anthropic.Anthropic | None,
+        client: Any | None,
         create: Callable,
         mode: instructor.Mode = instructor.Mode.TOOLS,
         provider: Provider = Provider.OPENAI,
         **kwargs,
     ):
         self.client = client
         self.create_fn = create
@@ -127,15 +125,15 @@
     def create_with_completion(
         self,
         messages: List[ChatCompletionMessageParam],
         response_model: Type[T],
         max_retries: int = 3,
         validation_context: dict | None = None,
         **kwargs,
-    ) -> Tuple[T, ChatCompletion | Message]:
+    ) -> Tuple[T, ChatCompletion | Any]:
         kwargs = self.handle_kwargs(kwargs)
         model = self.create_fn(
             messages=messages,
             response_model=response_model,
             max_retries=max_retries,
             validation_context=validation_context,
             **kwargs,
@@ -146,23 +144,23 @@
         for key, value in self.kwargs.items():
             if key not in kwargs:
                 kwargs[key] = value
         return kwargs
 
 
 class AsyncInstructor(Instructor):
-    client: openai.AsyncOpenAI | anthropic.AsyncAnthropic | None
+    client: Any | None
     create_fn: Any
     mode: instructor.Mode
     default_model: str | None = None
     provider: Provider
 
     def __init__(
         self,
-        client: openai.AsyncOpenAI | anthropic.AsyncAnthropic | None,
+        client: Any | None,
         create: Callable,
         mode: instructor.Mode = instructor.Mode.TOOLS,
         provider: Provider = Provider.OPENAI,
         **kwargs,
     ):
         self.client = client
         self.create_fn = create
@@ -277,18 +275,15 @@
 
     if provider in {Provider.ANYSCALE, Provider.TOGETHER}:
         assert mode in {
             instructor.Mode.TOOLS,
             instructor.Mode.JSON,
             instructor.Mode.JSON_SCHEMA,
         }
-    if provider in {Provider.GROQ}:
-        assert mode in {
-            instructor.Mode.MD_JSON,
-        }
+
     if provider in {Provider.OPENAI}:
         assert mode in {
             instructor.Mode.TOOLS,
             instructor.Mode.JSON,
             instructor.Mode.FUNCTIONS,
             instructor.Mode.PARALLEL_TOOLS,
             instructor.Mode.MD_JSON,
@@ -347,56 +342,7 @@
     else:
         return AsyncInstructor(
             client=None,
             create=instructor.patch(create=completion, mode=mode),
             mode=mode,
             **kwargs,
         )
-
-
-@overload
-def from_anthropic(
-    client: anthropic.Anthropic,
-    mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
-    **kwargs,
-) -> Instructor: ...
-
-
-@overload
-def from_anthropic(
-    client: anthropic.AsyncAnthropic,
-    mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
-    **kwargs,
-) -> Instructor: ...
-
-
-def from_anthropic(
-    client: anthropic.Anthropic | anthropic.AsyncAnthropic,
-    mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
-    **kwargs,
-) -> Instructor | AsyncInstructor:
-    assert mode in {
-        instructor.Mode.ANTHROPIC_JSON,
-        instructor.Mode.ANTHROPIC_TOOLS,
-    }, "Mode be one of {instructor.Mode.ANTHROPIC_JSON, instructor.Mode.ANTHROPIC_TOOLS}"
-
-    assert isinstance(
-        client, (anthropic.Anthropic, anthropic.AsyncAnthropic)
-    ), "Client must be an instance of anthropic.Anthropic or anthropic.AsyncAnthropic"
-
-    if isinstance(client, anthropic.Anthropic):
-        return Instructor(
-            client=client,
-            create=instructor.patch(create=client.messages.create, mode=mode),
-            provider=Provider.ANTHROPIC,
-            mode=mode,
-            **kwargs,
-        )
-
-    else:
-        return AsyncInstructor(
-            client=client,
-            create=instructor.patch(create=client.messages.create, mode=mode),
-            provider=Provider.ANTHROPIC,
-            mode=mode,
-            **kwargs,
-        )
```

### Comparing `instructor-1.0.0/instructor/distil.py` & `instructor-1.0.2/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/dsl/citation.py` & `instructor-1.0.2/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/dsl/iterable.py` & `instructor-1.0.2/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/dsl/maybe.py` & `instructor-1.0.2/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/dsl/parallel.py` & `instructor-1.0.2/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/dsl/partial.py` & `instructor-1.0.2/instructor/dsl/partial.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # The following code is adapted from a comment on GitHub in the pydantic/pydantic repository by silviumarcu.
 # Source: https://github.com/pydantic/pydantic/issues/6381#issuecomment-1831607091
 #
 # This code is used in accordance with the repository's license, and this reference
 # serves as an acknowledgment of the original author's contribution to this project.
 # --------------------------------------------------------------------------------
 
+import pydantic_core
 from pydantic import BaseModel, create_model
 from pydantic.fields import FieldInfo
 from typing import (
     Any,
     AsyncGenerator,
     Generator,
     Generic,
@@ -20,18 +21,16 @@
     Optional,
     TypeVar,
 )
 from copy import deepcopy
 from functools import lru_cache
 
 from instructor.mode import Mode
-from instructor.dsl.partialjson import JSONParser
 from instructor.utils import extract_json_from_stream, extract_json_from_stream_async
 
-parser = JSONParser()
 T_Model = TypeVar("T_Model", bound=BaseModel)
 
 
 class MakeFieldsOptional:
     pass
 
 
@@ -125,49 +124,30 @@
     ) -> Generator[T_Model, None, None]:
         prev_obj = None
         potential_object = ""
         partial_model = cls.get_partial_model()
         for chunk in json_chunks:
             potential_object += chunk
 
-            # Avoid parsing incomplete json when its just whitespace otherwise parser throws an exception
-            task_json = (
-                parser.parse(potential_object) if potential_object.strip() else None
-            )
-            if task_json:
-                obj = partial_model.model_validate(task_json, strict=None, **kwargs)  # type: ignore[attr-defined]
-                if obj != prev_obj:
-                    obj.__dict__["chunk"] = (
-                        chunk  # Provide the raw chunk for debugging and benchmarking
-                    )
-                    prev_obj = obj
-                    yield obj
+            obj = pydantic_core.from_json(potential_object or "{}", allow_partial=True)
+            obj = partial_model.model_validate(obj, strict=None, **kwargs)  # type: ignore[attr-defined]
+            yield obj
 
     @classmethod
     async def model_from_chunks_async(
         cls, json_chunks: AsyncGenerator[str, None], **kwargs: Any
     ) -> AsyncGenerator[T_Model, None]:
         potential_object = ""
         prev_obj = None
         partial_model = cls.get_partial_model()
         async for chunk in json_chunks:
             potential_object += chunk
-
-            # Avoid parsing incomplete json when its just whitespace otherwise parser throws an exception
-            task_json = (
-                parser.parse(potential_object) if potential_object.strip() else None
-            )
-            if task_json:
-                obj = partial_model.model_validate(task_json, strict=None, **kwargs)  # type: ignore[attr-defined]
-                if obj != prev_obj:
-                    obj.__dict__["chunk"] = (
-                        chunk  # Provide the raw chunk for debugging and benchmarking
-                    )
-                    prev_obj = obj
-                    yield obj
+            obj = pydantic_core.from_json(potential_object or "{}", allow_partial=True)
+            obj = partial_model.model_validate(obj, strict=None, **kwargs)
+            yield obj
 
     @staticmethod
     def extract_json(
         completion: Iterable[Any], mode: Mode
     ) -> Generator[str, None, None]:
         for chunk in completion:
             try:
```

### Comparing `instructor-1.0.0/instructor/dsl/simple_type.py` & `instructor-1.0.2/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/dsl/validators.py` & `instructor-1.0.2/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/function_calls.py` & `instructor-1.0.2/instructor/function_calls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Any, Dict, Optional, Type, TypeVar
-from xml.dom.minidom import parseString
 from docstring_parser import parse
 from functools import wraps
 from pydantic import BaseModel, create_model
 from openai.types.chat import ChatCompletion
 from typing import Any, Dict, Optional, Type
 from instructor.mode import Mode
 from instructor.utils import extract_json_from_codeblock
@@ -59,21 +58,20 @@
             "name": schema["title"],
             "description": schema["description"],
             "parameters": parameters,
         }
 
     @classmethod
     @property
-    def anthropic_schema(cls) -> str:
-        from instructor.anthropic_utils import json_to_xml
-
-        return "\n".join(
-            line.lstrip()
-            for line in parseString(json_to_xml(cls)).toprettyxml().splitlines()[1:]
-        )
+    def anthropic_schema(cls) -> Dict[str, Any]:
+        return {
+            "name": cls.openai_schema["name"],
+            "description": cls.openai_schema["description"],
+            "input_schema": cls.model_json_schema(),
+        }
 
     @classmethod
     def from_response(
         cls,
         completion: ChatCompletion,
         validation_context: Optional[Dict[str, Any]] = None,
         strict: Optional[bool] = None,
@@ -88,15 +86,15 @@
             strict (bool): Whether to use strict json parsing
             mode (Mode): The openai completion mode
 
         Returns:
             cls (OpenAISchema): An instance of the class
         """
         if mode == Mode.ANTHROPIC_TOOLS:
-            return cls.parse_anthropic_tools(completion)
+            return cls.parse_anthropic_tools(completion, validation_context, strict)
 
         if mode == Mode.ANTHROPIC_JSON:
             return cls.parse_anthropic_json(completion, validation_context, strict)
 
         if completion.choices[0].finish_reason == "length":
             raise IncompleteOutputException()
 
@@ -111,33 +109,33 @@
 
         raise ValueError(f"Invalid patch mode: {mode}")
 
     @classmethod
     def parse_anthropic_tools(
         cls: Type[BaseModel],
         completion: ChatCompletion,
+        validation_context: Optional[Dict[str, Any]] = None,
+        strict: Optional[bool] = None,
     ) -> BaseModel:
-        try:
-            from instructor.anthropic_utils import extract_xml, xml_to_model
-        except ImportError as err:
-            raise ImportError(
-                "Please 'pip install anthropic xmltodict' package to proceed."
-            ) from err
-        assert hasattr(completion, "content")
-        return xml_to_model(cls, extract_xml(completion.content[0].text))  # type:ignore
+        tool_call = [c.input for c in completion.content if c.type == "tool_use"][0]
+
+        return cls.model_validate(tool_call, context=validation_context, strict=strict)  # type:ignore
 
     @classmethod
     def parse_anthropic_json(
         cls: Type[BaseModel],
-        completion: ChatCompletion,
+        completion,
         validation_context: Optional[Dict[str, Any]] = None,
         strict: Optional[bool] = None,
     ) -> BaseModel:
-        assert hasattr(completion, "content")
-        text = completion.content[0].text  # type: ignore
+        from anthropic.types import Message
+
+        assert isinstance(completion, Message)
+
+        text = completion.content[0].text
         extra_text = extract_json_from_codeblock(text)
         return cls.model_validate_json(
             extra_text, context=validation_context, strict=strict
         )
 
     @classmethod
     def parse_functions(
```

### Comparing `instructor-1.0.0/instructor/mode.py` & `instructor-1.0.2/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/patch.py` & `instructor-1.0.2/instructor/patch.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.0/instructor/process_response.py` & `instructor-1.0.2/instructor/process_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Iterable
 from textwrap import dedent
 from instructor.dsl.iterable import IterableBase, IterableModel
 from instructor.dsl.parallel import ParallelBase, ParallelModel, handle_parallel_model
 from instructor.dsl.partial import PartialBase
 from instructor.dsl.simple_type import AdapterBase, ModelAdapter, is_simple_type
 from instructor.function_calls import OpenAISchema, openai_schema
-
+from instructor.utils import merge_consecutive_messages
 from openai.types.chat import ChatCompletion
 from pydantic import BaseModel
 
 import json
 import inspect
 import logging
 from typing import (
@@ -278,37 +278,24 @@
                     },
                 )
             # if it is, system append the schema to the end
             else:
                 new_kwargs["messages"][0]["content"] += f"\n\n{message}"
         elif mode == Mode.ANTHROPIC_TOOLS:
             tool_descriptions = response_model.anthropic_schema
-            system_prompt = (
-                dedent(
-                    f"""In this environment you have access to a set of tools you can use to answer the user's question.
-                You may call them like this:
-                <function_calls>
-                <invoke>
-                <tool_name>$TOOL_NAME</tool_name>
-                <parameters>
-                <$PARAMETER_NAME>$PARAMETER_VALUE</$PARAMETER_NAME>
-                ...
-                </parameters>
-                </invoke>
-                </function_calls>
+            new_kwargs["tools"] = [tool_descriptions]
 
-                Here are the tools available:"""
-                )
-                + tool_descriptions
-            )
+            system_messages = [
+                m["content"] for m in new_kwargs["messages"] if m["role"] == "system"
+            ]
+            new_kwargs["system"] = "\n\n".join(system_messages)
+            new_kwargs["messages"] = [
+                m for m in new_kwargs["messages"] if m["role"] != "system"
+            ]
 
-            if "system" in new_kwargs:
-                new_kwargs["system"] = f"{system_prompt}\n{new_kwargs['system']}"
-            else:
-                new_kwargs["system"] = system_prompt
         elif mode == Mode.ANTHROPIC_JSON:
             # anthropic wants system message to be a string so we first extract out any system message
             openai_system_messages = [
                 message["content"]
                 for message in new_kwargs.get("messages", [])
                 if message["role"] == "system"
             ]
@@ -329,14 +316,19 @@
             new_kwargs["system"] = dedent(new_kwargs["system"])
 
             new_kwargs["messages"] = [
                 message
                 for message in new_kwargs.get("messages", [])
                 if message["role"] != "system"
             ]
+
+            # the messages array must be alternating roles of user and assistant, we must merge
+            # consecutive user messages into a single message
+            new_kwargs["messages"] = merge_consecutive_messages(new_kwargs["messages"])
+
         else:
             raise ValueError(f"Invalid patch mode: {mode}")
 
     logger.debug(
         f"Instructor Request: {mode.value=}, {response_model=}, {new_kwargs=}",
         extra={
             "mode": mode.value,
```

### Comparing `instructor-1.0.0/instructor/retry.py` & `instructor-1.0.2/instructor/retry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # type: ignore[all]
 import logging
 
 from openai.types.chat import ChatCompletion
 from instructor.mode import Mode
 from instructor.process_response import process_response, process_response_async
-from instructor.utils import dump_message, update_total_usage
+from instructor.utils import (
+    dump_message,
+    update_total_usage,
+    merge_consecutive_messages,
+)
 
 from openai.types.completion_usage import CompletionUsage
 from pydantic import ValidationError
 from tenacity import AsyncRetrying, RetryError, Retrying, stop_after_attempt
 
 
 from json import JSONDecodeError
@@ -24,15 +28,24 @@
 
 
 def reask_messages(response: ChatCompletion, mode: Mode, exception: Exception):
     if mode == Mode.ANTHROPIC_TOOLS:
         # TODO: we need to include the original response
         yield {
             "role": "user",
-            "content": f"Validation Error found:\n{exception}\nRecall the function correctly, fix the errors",
+            "content": f"Validation Errors found:\n{exception}\nReca ll the function correctly, fix the errors from\n{response.content}",
+        }
+        return
+    if mode == Mode.ANTHROPIC_JSON:
+        from anthropic.types import Message
+
+        assert isinstance(response, Message)
+        yield {
+            "role": "user",
+            "content": f"""Validation Errors found:\n{exception}\nRecall the function correctly, fix the errors found in the following attempt:\n{response.content[0].text}""",
         }
         return
 
     yield dump_message(response.choices[0].message)
     # TODO: Give users more control on configuration
     if mode == Mode.TOOLS:
         for tool_call in response.choices[0].message.tool_calls:  # type: ignore
@@ -90,14 +103,15 @@
                         validation_context=validation_context,
                         strict=strict,
                         mode=mode,
                     )
                 except (ValidationError, JSONDecodeError) as e:
                     logger.debug(f"Error response: {response}")
                     kwargs["messages"].extend(reask_messages(response, mode, e))
+                    kwargs["messages"] = merge_consecutive_messages(kwargs["messages"])
                     raise e
     except RetryError as e:
         logger.exception(f"Failed after retries: {e.last_attempt.exception}")
         raise e.last_attempt.exception from e
 
 
 async def retry_async(
```

### Comparing `instructor-1.0.0/instructor/utils.py` & `instructor-1.0.2/instructor/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -116,7 +116,19 @@
 def is_async(func: Callable) -> bool:
     """Returns true if the callable is async, accounting for wrapped callables"""
     is_coroutine = inspect.iscoroutinefunction(func)
     while hasattr(func, "__wrapped__"):
         func = func.__wrapped__
         is_coroutine = is_coroutine or inspect.iscoroutinefunction(func)
     return is_coroutine
+
+
+def merge_consecutive_messages(messages: list[dict]) -> list[dict]:
+    # merge all consecutive user messages into a single message
+    new_messages = []
+    for message in messages:
+        if len(new_messages) > 0 and message["role"] == new_messages[-1]["role"]:
+            new_messages[-1]["content"] += f"\n\n{message['content']}"
+        else:
+            new_messages.append(message)
+
+    return new_messages
```

### Comparing `instructor-1.0.0/PKG-INFO` & `instructor-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.0.0
+Version: 1.0.2
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic
+Provides-Extra: groq
+Provides-Extra: test-docs
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
-Requires-Dist: anthropic (>=0.18.1,<0.19.0) ; extra == "anthropic"
+Requires-Dist: anthropic (>=0.23.1,<0.24.0) ; extra == "anthropic" or extra == "test-docs"
+Requires-Dist: diskcache (>=5.6.3,<6.0.0) ; extra == "test-docs"
 Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: fastapi (>=0.109.2,<0.110.0) ; extra == "test-docs"
+Requires-Dist: groq (>=0.4.2,<0.5.0) ; extra == "groq" or extra == "test-docs"
+Requires-Dist: litellm (>=1.0.0,<2.0.0) ; extra == "test-docs"
 Requires-Dist: openai (>=1.1.0,<2.0.0)
+Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "test-docs"
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic-core (>=2.18.0,<3.0.0)
+Requires-Dist: pydantic_extra_types (>=2.6.0,<3.0.0) ; extra == "test-docs"
+Requires-Dist: redis (>=5.0.1,<6.0.0) ; extra == "test-docs"
 Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "test-docs"
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0) ; extra == "anthropic"
 Project-URL: Repository, https://github.com/jxnl/instructor
 Description-Content-Type: text/markdown
 
-# 🎓 Instructor: Your Friendly Guide to Structured LLM Outputs
+# Instructor: Structured LLM Outputs
 
 Instructor is a Python library that makes it a breeze to work with structured outputs from large language models (LLMs). Built on top of Pydantic, it provides a simple, transparent, and user-friendly API to manage validation, retries, and streaming responses. Get ready to supercharge your LLM workflows!
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/jxnlco?style=social)](https://twitter.com/jxnlco)
 [![Discord](https://img.shields.io/discord/1192334452110659664?label=discord)](https://discord.gg/CV8sPM5k5Y)
 [![Downloads](https://img.shields.io/pypi/dm/instructor.svg)](https://pypi.python.org/pypi/instructor)
 
 
-## 🌟 Key Features
+## Key Features
 
-- 🎭 **Response Models**: Specify Pydantic models to define the structure of your LLM outputs
-- 🔄 **Retry Management**: Easily configure the number of retry attempts for your requests
-- ✅ **Validation**: Ensure LLM responses conform to your expectations with Pydantic validation
-- 🌊 **Streaming Support**: Work with Lists and Partial responses effortlessly
-- 🔌 **Flexible Backends**: Seamlessly integrate with various LLM providers beyond OpenAI
+- **Response Models**: Specify Pydantic models to define the structure of your LLM outputs
+- **Retry Management**: Easily configure the number of retry attempts for your requests
+   **Validation**: Ensure LLM responses conform to your expectations with Pydantic validation
+- **Streaming Support**: Work with Lists and Partial responses effortlessly
+   **Flexible Backends**: Seamlessly integrate with various LLM providers beyond OpenAI
 
-## 🚀 Get Started in Minutes
+## Get Started in Minutes
 
 Install Instructor with a single command:
 
 ```bash
 pip install -U instructor
 ```
 
@@ -70,84 +81,21 @@
 # Extract structured data from natural language
 user_info = client.chat.completions.create(
     model="gpt-3.5-turbo",
     response_model=UserInfo,
     messages=[{"role": "user", "content": "John Doe is 30 years old."}],
 )
 
-print(user_info.name)  # "John Doe"
+print(user_info.name)
 #> John Doe
-print(user_info.age)  # 30
+print(user_info.age)
 #> 30
 ```
 
-## 🎯 Validation Made Easy
-
-Instructor leverages Pydantic to make validating LLM outputs a breeze. Simply define your validation rules in your Pydantic models, and Instructor will ensure the LLM responses conform to your expectations. No more manual checking or parsing!
-
-```python
-from pydantic import BaseModel, ValidationError, BeforeValidator
-from typing_extensions import Annotated
-from instructor import llm_validator
-
-import instructor
-import openai
-
-client = instructor.from_openai(openai.OpenAI())
-
-
-class QuestionAnswer(BaseModel):
-    question: str
-    answer: Annotated[
-        str,
-        BeforeValidator(llm_validator("Don't say objectionable things", client=client)),
-    ]
-
-
-try:
-    qa = QuestionAnswer(
-        question="What is the meaning of life?",
-        answer="The meaning of life is to be evil and steal",
-    )
-except ValidationError as e:
-    print(e)
-    """
-    1 validation error for QuestionAnswer
-    answer
-      Assertion failed, The statement promotes evil behavior, which is objectionable. [type=assertion_error, input_value='The meaning of life is to be evil and steal', input_type=str]
-        For further information visit https://errors.pydantic.dev/2.6/v/assertion_error
-    """
-```
-
-## 📖 Learn More
-
-Dive deeper into Instructor's concepts and features:
-
-- [Validation Context](./docs/concepts/reask_validation.md)
-- [Retrying](./docs/concepts/retrying.md) 
-- [Lists](./docs/concepts/lists.md)
-- [Partial Responses](./docs/concepts/partial.md)
-- [Patching](./docs/concepts/patching.md)
-
-## 🤝 Join the Community
-
-Have questions? Want to share your Instructor projects? Join our vibrant community on [Discord](https://discord.gg/CV8sPM5k5Y)! We're here to help you get the most out of Instructor and celebrate your successes.
-
-
-## 🎉 Start Building
-
-Instructor is your friendly companion on the exciting journey of working with LLMs. Install it now and unlock the full potential of structured outputs in your projects. Happy building! 🚀
-
----
-
-We can't wait to see the amazing things you create with Instructor. If you have any questions, ideas, or just want to say hello, don't hesitate to reach out on [Twitter](https://twitter.com/jxnlco) or [Discord](https://discord.gg/CV8sPM5k5Y). Let's build the future together! 🌟
-
----
-
-## Using Anthropic Models
+### Using Anthropic Models
 
 ```python
 import instructor
 from anthropic import Anthropic
 from pydantic import BaseModel
 
 
@@ -172,15 +120,15 @@
 )
 
 assert isinstance(resp, User)
 assert resp.name == "Jason"
 assert resp.age == 25
 ```
 
-## Using Litellm
+### Using Litellm
 
 ```python
 import instructor
 from litellm import completion
 from pydantic import BaseModel
 
 
@@ -204,17 +152,197 @@
 )
 
 assert isinstance(resp, User)
 assert resp.name == "Jason"
 assert resp.age == 25
 ```
 
-## [Evals](https://github.com/jxnl/instructor/tree/main/tests/openai/evals)
+## Type are infered correctly
+
+This was the dream of instructor but due to the patching of openai, it wasnt possible for me to get typing to work well. Now, with the new client, we can get typing to work well! We've also added a few `create_*` methods to make it easier to create iterables and partials, and to access the original completion.
+
+### Calling `create`
+
+```python
+import openai
+import instructor
+from pydantic import BaseModel
+
+
+class User(BaseModel):
+    name: str
+    age: int
+
+
+client = instructor.from_openai(openai.OpenAI())
+
+user = client.chat.completions.create(
+    model="gpt-4-turbo-preview",
+    messages=[
+        {"role": "user", "content": "Create a user"},
+    ],
+    response_model=User,
+)
+```
+
+Now if you use a IDE, you can see the type is correctly infered.
+
+![type](./docs/blog/posts/img/type.png)
+
+### Handling async: `await create`
+
+This will also work correctly with asynchronous clients. 
+
+```python
+import openai
+import instructor
+from pydantic import BaseModel
+
+
+client = instructor.from_openai(openai.AsyncOpenAI())
+
+
+class User(BaseModel):
+    name: str
+    age: int
+
+
+async def extract():
+    return await client.chat.completions.create(
+        model="gpt-4-turbo-preview",
+        messages=[
+            {"role": "user", "content": "Create a user"},
+        ],
+        response_model=User,
+    )
+```
+
+Notice that simply because we return the `create` method, the `extract()` function will return the correct user type.
+
+![async](./docs/blog/posts/img/async_type.png)
+
+### Returning the original completion: `create_with_completion`
+
+You can also return the original completion object
+
+```python
+import openai
+import instructor
+from pydantic import BaseModel
+
+
+client = instructor.from_openai(openai.OpenAI())
+
+
+class User(BaseModel):
+    name: str
+    age: int
+
+
+user, completion = client.chat.completions.create_with_completion(
+    model="gpt-4-turbo-preview",
+    messages=[
+        {"role": "user", "content": "Create a user"},
+    ],
+    response_model=User,
+)
+```
+
+![with_completion](./docs/blog/posts/img/with_completion.png)
+
+
+### Streaming Partial Objects: `create_partial`
+
+In order to handle streams, we still support `Iterable[T]` and `Partial[T]` but to simply the type inference, we've added `create_iterable` and `create_partial` methods as well!
+
+```python
+import openai
+import instructor
+from pydantic import BaseModel
+
+
+client = instructor.from_openai(openai.OpenAI())
+
+
+class User(BaseModel):
+    name: str
+    age: int
+
+
+user_stream = client.chat.completions.create_partial(
+    model="gpt-4-turbo-preview",
+    messages=[
+        {"role": "user", "content": "Create a user"},
+    ],
+    response_model=User,
+)
+
+for user in user_stream:
+    print(user)
+    #> name=None age=None
+    #> name=None age=None
+    #> name=None age=None
+    #> name=None age=None
+    #> name=None age=25
+    #> name=None age=25
+    #> name=None age=25
+    #> name=None age=25
+    #> name=None age=25
+    #> name=None age=25
+    #> name='John Doe' age=25
+    # name=None age=None
+    # name='' age=None
+    # name='John' age=None
+    # name='John Doe' age=None
+    # name='John Doe' age=30
+```
+
+Notice now that the type infered is `Generator[User, None]`
+
+![generator](./docs/blog/posts/img/generator.png)
+
+### Streaming Iterables: `create_iterable`
+
+We get an iterable of objects when we want to extract multiple objects.
+
+```python
+import openai
+import instructor
+from pydantic import BaseModel
+
+
+client = instructor.from_openai(openai.OpenAI())
+
+
+class User(BaseModel):
+    name: str
+    age: int
+
+
+users = client.chat.completions.create_iterable(
+    model="gpt-4-turbo-preview",
+    messages=[
+        {"role": "user", "content": "Create 2 users"},
+    ],
+    response_model=User,
+)
+
+for user in users:
+    print(user)
+    #> name='John' age=30
+    #> name='Jane' age=25
+    # User(name='John Doe', age=30)
+    # User(name='Jane Smith', age=25)
+```
+
+![iterable](./docs/blog/posts/img/iterable.png)
+
+## [Evals](https://github.com/jxnl/instructor/tree/main/tests/llm/test_openai/evals#how-to-contribute-writing-and-running-evaluation-tests)
 
-We invite you to contribute to evals in `pytest` as a way to monitor the quality of the OpenAI models and the `instructor` library. To get started check out the [jxnl/instructor/tests/evals](https://github.com/jxnl/instructor/tree/main/tests/openai/evals) and contribute your own evals in the form of pytest tests. These evals will be run once a week and the results will be posted.
+We invite you to contribute to evals in `pytest` as a way to monitor the quality of the OpenAI models and the `instructor` library. To get started check out the evals for [anthropic](https://github.com/jxnl/instructor/blob/main/tests/llm/test_anthropic/evals/test_simple.py) and [OpenAI](https://github.com/jxnl/instructor/tree/main/tests/llm/test_openai/evals#how-to-contribute-writing-and-running-evaluation-tests) and contribute your own evals in the form of pytest tests. These evals will be run once a week and the results will be posted.
 
 ## Contributing
 
 If you want to help, checkout some of the issues marked as `good-first-issue` or `help-wanted` found [here](https://github.com/jxnl/instructor/labels/good%20first%20issue). They could be anything from code improvements, a guest blog post, or a new cookbook.
 
 ## CLI
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

