# Comparing `tmp/llama_index_llms_anthropic-0.1.8.tar.gz` & `tmp/llama_index_llms_anthropic-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_anthropic-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_llms_anthropic-0.1.9.tar", max compression
```

## Comparing `llama_index_llms_anthropic-0.1.8.tar` & `llama_index_llms_anthropic-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       41 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/README.md
--rw-r--r--   0        0        0       79 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/__init__.py
--rw-r--r--   0        0        0     9812 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/base.py
--rw-r--r--   0        0        0     3394 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/utils.py
--rw-r--r--   0        0        0     1455 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 llama_index_llms_anthropic-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-05 00:39:12.552541 llama_index_llms_anthropic-0.1.9/README.md
+-rw-r--r--   0        0        0       79 2024-04-05 00:39:12.552541 llama_index_llms_anthropic-0.1.9/llama_index/llms/anthropic/__init__.py
+-rw-r--r--   0        0        0    14609 2024-04-05 00:39:12.552541 llama_index_llms_anthropic-0.1.9/llama_index/llms/anthropic/base.py
+-rw-r--r--   0        0        0     4941 2024-04-05 00:39:12.552541 llama_index_llms_anthropic-0.1.9/llama_index/llms/anthropic/utils.py
+-rw-r--r--   0        0        0     1455 2024-04-05 00:39:12.552541 llama_index_llms_anthropic-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 llama_index_llms_anthropic-0.1.9/PKG-INFO
```

### Comparing `llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/base.py` & `llama_index_llms_anthropic-0.1.9/llama_index/llms/anthropic/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,23 @@
-from typing import Any, Callable, Dict, Optional, Sequence
-from anthropic.types import ContentBlockDeltaEvent
+import anthropic
+import json
+from anthropic.types import ContentBlockDeltaEvent, TextBlock
+from anthropic.types.beta.tools import ToolUseBlock
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+    TYPE_CHECKING,
+)
+
 from llama_index.core.base.llms.types import (
     ChatMessage,
     ChatResponse,
     ChatResponseAsyncGen,
     ChatResponseGen,
     CompletionResponse,
     CompletionResponseAsyncGen,
@@ -20,29 +34,34 @@
 )
 from llama_index.core.base.llms.generic_utils import (
     achat_to_completion_decorator,
     astream_chat_to_completion_decorator,
     chat_to_completion_decorator,
     stream_chat_to_completion_decorator,
 )
-from llama_index.core.llms.llm import LLM
+from llama_index.core.llms.function_calling import FunctionCallingLLM, ToolSelection
 from llama_index.core.types import BaseOutputParser, PydanticProgramMode
 from llama_index.llms.anthropic.utils import (
     anthropic_modelname_to_contextsize,
+    force_single_tool_call,
+    is_function_calling_model,
     messages_to_anthropic_messages,
 )
 from llama_index.core.utils import Tokenizer
 
-import anthropic
+if TYPE_CHECKING:
+    from llama_index.core.chat_engine.types import AgentChatResponse
+    from llama_index.core.tools.types import BaseTool
+
 
 DEFAULT_ANTHROPIC_MODEL = "claude-2.1"
 DEFAULT_ANTHROPIC_MAX_TOKENS = 512
 
 
-class Anthropic(LLM):
+class Anthropic(FunctionCallingLLM):
     """Anthropic LLM.
 
     Examples:
         `pip install llama-index-llms-anthropic`
 
         ```python
         from llama_index.llms.anthropic import Anthropic
@@ -142,14 +161,15 @@
     @property
     def metadata(self) -> LLMMetadata:
         return LLMMetadata(
             context_window=anthropic_modelname_to_contextsize(self.model),
             num_output=self.max_tokens,
             is_chat_model=True,
             model_name=self.model,
+            is_function_calling_model=is_function_calling_model(self.model),
         )
 
     @property
     def tokenizer(self) -> Tokenizer:
         return self._client.get_tokenizer()
 
     @property
@@ -166,28 +186,46 @@
 
     def _get_all_kwargs(self, **kwargs: Any) -> Dict[str, Any]:
         return {
             **self._model_kwargs,
             **kwargs,
         }
 
+    def _get_content_and_tool_calls(
+        self, response: Any
+    ) -> Tuple[str, List[ToolUseBlock]]:
+        tool_calls = []
+        content = ""
+        for content_block in response.content:
+            if isinstance(content_block, TextBlock):
+                content += content_block.text
+            elif isinstance(content_block, ToolUseBlock):
+                tool_calls.append(content_block.dict())
+
+        return content, tool_calls
+
     @llm_chat_callback()
     def chat(self, messages: Sequence[ChatMessage], **kwargs: Any) -> ChatResponse:
         anthropic_messages, system_prompt = messages_to_anthropic_messages(messages)
         all_kwargs = self._get_all_kwargs(**kwargs)
 
-        response = self._client.messages.create(
+        response = self._client.beta.tools.messages.create(
             messages=anthropic_messages,
             stream=False,
             system=system_prompt,
             **all_kwargs,
         )
+
+        content, tool_calls = self._get_content_and_tool_calls(response)
+
         return ChatResponse(
             message=ChatMessage(
-                role=MessageRole.ASSISTANT, content=response.content[0].text
+                role=MessageRole.ASSISTANT,
+                content=content,
+                additional_kwargs={"tool_calls": tool_calls},
             ),
             raw=dict(response),
         )
 
     @llm_completion_callback()
     def complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
@@ -231,23 +269,28 @@
     @llm_chat_callback()
     async def achat(
         self, messages: Sequence[ChatMessage], **kwargs: Any
     ) -> ChatResponse:
         anthropic_messages, system_prompt = messages_to_anthropic_messages(messages)
         all_kwargs = self._get_all_kwargs(**kwargs)
 
-        response = await self._aclient.messages.create(
+        response = await self._aclient.beta.tools.messages.create(
             messages=anthropic_messages,
             system=system_prompt,
             stream=False,
             **all_kwargs,
         )
+
+        content, tool_calls = self._get_content_and_tool_calls(response)
+
         return ChatResponse(
             message=ChatMessage(
-                role=MessageRole.ASSISTANT, content=response.content[0].text
+                role=MessageRole.ASSISTANT,
+                content=content,
+                additional_kwargs={"tool_calls": tool_calls},
             ),
             raw=dict(response),
         )
 
     @llm_completion_callback()
     async def acomplete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
@@ -283,7 +326,116 @@
 
     @llm_completion_callback()
     async def astream_complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> CompletionResponseAsyncGen:
         astream_complete_fn = astream_chat_to_completion_decorator(self.astream_chat)
         return await astream_complete_fn(prompt, **kwargs)
+
+    def chat_with_tools(
+        self,
+        tools: List["BaseTool"],
+        user_msg: Optional[Union[str, ChatMessage]] = None,
+        chat_history: Optional[List[ChatMessage]] = None,
+        verbose: bool = False,
+        allow_parallel_tool_calls: bool = False,
+        **kwargs: Any,
+    ) -> ChatResponse:
+        """Predict and call the tool."""
+        chat_history = chat_history or []
+
+        if isinstance(user_msg, str):
+            user_msg = ChatMessage(role=MessageRole.USER, content=user_msg)
+            chat_history.append(user_msg)
+
+        tool_dicts = []
+        for tool in tools:
+            tool_dicts.append(
+                {
+                    "name": tool.metadata.name,
+                    "description": tool.metadata.description,
+                    "input_schema": tool.metadata.get_parameters_dict(),
+                }
+            )
+
+        response = self.chat(chat_history, tools=tool_dicts, **kwargs)
+
+        if not allow_parallel_tool_calls:
+            force_single_tool_call(response)
+
+        return response
+
+    async def achat_with_tools(
+        self,
+        tools: List["BaseTool"],
+        user_msg: Optional[Union[str, ChatMessage]] = None,
+        chat_history: Optional[List[ChatMessage]] = None,
+        verbose: bool = False,
+        allow_parallel_tool_calls: bool = False,
+        **kwargs: Any,
+    ) -> ChatResponse:
+        """Predict and call the tool."""
+        chat_history = chat_history or []
+
+        if isinstance(user_msg, str):
+            user_msg = ChatMessage(role=MessageRole.USER, content=user_msg)
+            chat_history.append(user_msg)
+
+        tool_dicts = []
+        for tool in tools:
+            tool_dicts.append(
+                {
+                    "name": tool.metadata.name,
+                    "description": tool.metadata.description,
+                    "input_schema": tool.metadata.get_parameters_dict(),
+                }
+            )
+
+        response = await self.achat(chat_history, tools=tool_dicts, **kwargs)
+
+        if not allow_parallel_tool_calls:
+            force_single_tool_call(response)
+
+        return response
+
+    def get_tool_calls_from_response(
+        self,
+        response: "AgentChatResponse",
+        error_on_no_tool_call: bool = True,
+        **kwargs: Any,
+    ) -> List[ToolSelection]:
+        """Predict and call the tool."""
+        tool_calls = response.message.additional_kwargs.get("tool_calls", [])
+
+        if len(tool_calls) < 1:
+            if error_on_no_tool_call:
+                raise ValueError(
+                    f"Expected at least one tool call, but got {len(tool_calls)} tool calls."
+                )
+            else:
+                return []
+
+        tool_selections = []
+        for tool_call in tool_calls:
+            if (
+                "input" not in tool_call
+                or "id" not in tool_call
+                or "name" not in tool_call
+            ):
+                raise ValueError("Invalid tool call.")
+            if tool_call["type"] != "tool_use":
+                raise ValueError("Invalid tool type. Unsupported by Anthropic")
+            argument_dict = (
+                json.loads(tool_call["input"])
+                if isinstance(tool_call["input"], str)
+                else tool_call["input"]
+            )
+
+            tool_selections.append(
+                ToolSelection(
+                    tool_id=tool_call["id"],
+                    tool_name=tool_call["name"],
+                    tool_kwargs=argument_dict,
+                )
+            )
+
+        return tool_selections
```

### Comparing `llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/utils.py` & `llama_index_llms_anthropic-0.1.9/llama_index/llms/anthropic/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Sequence, Tuple
 
-from llama_index.core.base.llms.types import ChatMessage, MessageRole
+from llama_index.core.base.llms.types import ChatMessage, ChatResponse, MessageRole
 
 from anthropic.types import MessageParam, TextBlockParam
+from anthropic.types.beta.tools import ToolResultBlockParam, ToolUseBlockParam
 
 HUMAN_PREFIX = "\n\nHuman:"
 ASSISTANT_PREFIX = "\n\nAssistant:"
 
 CLAUDE_MODELS: Dict[str, int] = {
     "claude-instant-1": 100000,
     "claude-instant-1.2": 100000,
@@ -15,14 +16,18 @@
     "claude-2.1": 200000,
     "claude-3-opus-20240229": 180000,
     "claude-3-sonnet-20240229": 180000,
     "claude-3-haiku-20240307": 180000,
 }
 
 
+def is_function_calling_model(modelname: str) -> bool:
+    return "claude-3" in modelname
+
+
 def anthropic_modelname_to_contextsize(modelname: str) -> int:
     if modelname not in CLAUDE_MODELS:
         raise ValueError(
             f"Unknown model: {modelname}. Please provide a valid Anthropic model name."
             "Known models are: " + ", ".join(CLAUDE_MODELS.keys())
         )
 
@@ -59,22 +64,51 @@
         - System prompt
     """
     anthropic_messages = []
     system_prompt = ""
     for message in messages:
         if message.role == MessageRole.SYSTEM:
             system_prompt = message.content
+        elif message.role == MessageRole.FUNCTION or message.role == MessageRole.TOOL:
+            content = ToolResultBlockParam(
+                tool_use_id=message.additional_kwargs["tool_call_id"],
+                type="tool_result",
+                content=[TextBlockParam(text=message.content, type="text")],
+            )
+            anth_message = MessageParam(
+                role=MessageRole.USER.value,
+                content=[content],
+            )
+            anthropic_messages.append(anth_message)
         else:
-            message = MessageParam(
+            content = []
+            if message.content:
+                content.append(TextBlockParam(text=message.content, type="text"))
+
+            tool_calls = message.additional_kwargs.get("tool_calls", [])
+            for tool_call in tool_calls:
+                assert "id" in tool_call
+                assert "input" in tool_call
+                assert "name" in tool_call
+
+                content.append(
+                    ToolUseBlockParam(
+                        id=tool_call["id"],
+                        input=tool_call["input"],
+                        name=tool_call["name"],
+                        type="tool_use",
+                    )
+                )
+
+            anth_message = MessageParam(
                 role=message.role.value,
-                content=[
-                    TextBlockParam(text=message.content, type="text")
-                ],  # TODO: type detect for multimodal
+                content=content,  # TODO: type detect for multimodal
             )
-            anthropic_messages.append(message)
+            anthropic_messages.append(anth_message)
+
     return __merge_common_role_msgs(anthropic_messages), system_prompt
 
 
 # Function used in bedrock
 def _message_to_anthropic_prompt(message: ChatMessage) -> str:
     if message.role == MessageRole.USER:
         prompt = f"{HUMAN_PREFIX} {message.content}"
@@ -99,7 +133,13 @@
         messages = [
             *list(messages),
             ChatMessage(role=MessageRole.ASSISTANT, content=""),
         ]
 
     str_list = [_message_to_anthropic_prompt(message) for message in messages]
     return "".join(str_list)
+
+
+def force_single_tool_call(response: ChatResponse) -> None:
+    tool_calls = response.message.additional_kwargs.get("tool_calls", [])
+    if len(tool_calls) > 1:
+        response.message.additional_kwargs["tool_calls"] = [tool_calls[0]]
```

### Comparing `llama_index_llms_anthropic-0.1.8/pyproject.toml` & `llama_index_llms_anthropic-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms anthropic integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-anthropic"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-anthropic = "^0.20.0"
+anthropic = "^0.23.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_llms_anthropic-0.1.8/PKG-INFO` & `llama_index_llms_anthropic-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-anthropic
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index llms anthropic integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anthropic (>=0.20.0,<0.21.0)
+Requires-Dist: anthropic (>=0.23.1,<0.24.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Anthropic
```

