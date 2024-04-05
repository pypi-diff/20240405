# Comparing `tmp/langchain_cohere-0.1.0rc1.tar.gz` & `tmp/langchain_cohere-0.1.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cohere-0.1.0rc1.tar", max compression
+gzip compressed data, was "langchain_cohere-0.1.1rc0.tar", max compression
```

## Comparing `langchain_cohere-0.1.0rc1.tar` & `langchain_cohere-0.1.1rc0.tar`

### file list

```diff
@@ -1,13 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0       19 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/README.md
--rw-r--r--   0        0        0      450 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/__init__.py
--rw-r--r--   0        0        0    12664 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/chat_models.py
--rw-r--r--   0        0        0     7496 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/cohere_agent.py
--rw-r--r--   0        0        0     5193 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/embeddings.py
--rw-r--r--   0        0        0     7654 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/llms.py
--rw-r--r--   0        0        0        0 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/py.typed
--rw-r--r--   0        0        0     2974 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/rag_retrievers.py
--rw-r--r--   0        0        0     3995 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/rerank.py
--rw-r--r--   0        0        0      975 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/utils.py
--rw-r--r--   0        0        0     2471 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 langchain_cohere-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/LICENSE
+-rw-r--r--   0        0        0     3796 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/README.md
+-rw-r--r--   0        0        0      608 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/__init__.py
+-rw-r--r--   0        0        0    13374 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/chat_models.py
+-rw-r--r--   0        0        0     8089 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/cohere_agent.py
+-rw-r--r--   0        0        0     1215 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/common.py
+-rw-r--r--   0        0        0     5366 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/embeddings.py
+-rw-r--r--   0        0        0     8050 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/llms.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/py.typed
+-rw-r--r--   0        0        0     3349 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/rag_retrievers.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/__init__.py
+-rw-r--r--   0        0        0     4899 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/agent.py
+-rw-r--r--   0        0        0     4059 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py
+-rw-r--r--   0        0        0    10974 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/parsing.py
+-rw-r--r--   0        0        0     9635 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/prompt.py
+-rw-r--r--   0        0        0     3995 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/rerank.py
+-rw-r--r--   0        0        0     1655 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/utils.py
+-rw-r--r--   0        0        0     2331 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/pyproject.toml
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 langchain_cohere-0.1.1rc0/PKG-INFO
```

### Comparing `langchain_cohere-0.1.0rc1/LICENSE` & `langchain_cohere-0.1.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.0rc1/langchain_cohere/chat_models.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/chat_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from cohere.types import NonStreamedChatResponse, ToolCall
 from langchain_core._api import beta
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
+from langchain_core.documents import Document
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
     agenerate_from_stream,
     generate_from_stream,
 )
 from langchain_core.messages import (
@@ -69,16 +70,17 @@
     else:
         raise ValueError(f"Got unknown type {message}")
 
 
 def get_cohere_chat_request(
     messages: List[BaseMessage],
     *,
-    documents: Optional[List[Dict[str, str]]] = None,
+    documents: Optional[List[Document]] = None,
     connectors: Optional[List[Dict[str, str]]] = None,
+    stop_sequences: Optional[List[str]] = None,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     """Get the request for the Cohere chat API.
 
     Args:
         messages: The messages.
         connectors: The connectors.
@@ -91,25 +93,37 @@
 
     # cohere SDK will fail loudly if both connectors and documents are provided
     if additional_kwargs.get("documents", []) and documents and len(documents) > 0:
         raise ValueError(
             "Received documents both as a keyword argument and as an prompt additional keyword argument. Please choose only one option."  # noqa: E501
         )
 
+    parsed_docs: Optional[Union[List[Document], List[Dict]]] = None
+    if "documents" in additional_kwargs:
+        parsed_docs = (
+            additional_kwargs["documents"]
+            if len(additional_kwargs["documents"]) > 0
+            else None
+        )
+    elif documents is not None and len(documents) > 0:
+        parsed_docs = documents
+
     formatted_docs: Optional[List[Dict[str, Any]]] = None
-    if additional_kwargs.get("documents"):
-        formatted_docs = [
-            {
-                "text": doc.page_content,
-                "id": doc.metadata.get("id") or f"doc-{str(i)}",
-            }
-            for i, doc in enumerate(additional_kwargs.get("documents", []))
-        ]
-    elif documents:
-        formatted_docs = documents
+    if parsed_docs:
+        formatted_docs = []
+        for i, parsed_doc in enumerate(parsed_docs):
+            if isinstance(parsed_doc, Document):
+                formatted_docs.append(
+                    {
+                        "text": parsed_doc.page_content,
+                        "id": parsed_doc.metadata.get("id") or f"doc-{str(i)}",
+                    }
+                )
+            elif isinstance(parsed_doc, dict):
+                formatted_docs.append(parsed_doc)
 
     # by enabling automatic prompt truncation, the probability of request failure is
     # reduced with minimal impact on response quality
     prompt_truncation = (
         "AUTO" if formatted_docs is not None or connectors is not None else None
     )
 
@@ -117,14 +131,15 @@
         "message": messages[-1].content,
         "chat_history": [
             {"role": get_role(x), "message": x.content} for x in messages[:-1]
         ],
         "documents": formatted_docs,
         "connectors": connectors,
         "prompt_truncation": prompt_truncation,
+        "stop_sequences": stop_sequences,
         **kwargs,
     }
 
     return {k: v for k, v in req.items() if v is not None}
 
 
 class ChatCohere(BaseChatModel, BaseCohere):
@@ -187,18 +202,16 @@
                 then the model output will be an object of that class. If a dict then
                 the model output will be a dict.
 
         Returns:
             A Runnable that takes any ChatModel input and returns either a dict or
             Pydantic class as output.
         """
-        if kwargs:
-            raise ValueError(f"Received unsupported arguments {kwargs}")
         is_pydantic_schema = isinstance(schema, type) and issubclass(schema, BaseModel)
-        llm = self.bind_tools([schema])
+        llm = self.bind_tools([schema], **kwargs)
         if is_pydantic_schema:
             output_parser: OutputParserLike = PydanticToolsParser(
                 tools=[schema], first_tool_only=True
             )
         else:
             key_name = _convert_to_cohere_tool(schema)["name"]
             output_parser = JsonOutputKeyToolsParser(
@@ -215,15 +228,17 @@
     def _stream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
-        request = get_cohere_chat_request(messages, **self._default_params, **kwargs)
+        request = get_cohere_chat_request(
+            messages, stop_sequences=stop, **self._default_params, **kwargs
+        )
 
         if hasattr(self.client, "chat_stream"):  # detect and support sdk v5
             stream = self.client.chat_stream(**request)
         else:
             stream = self.client.chat(**request, stream=True)
 
         for data in stream:
@@ -245,15 +260,17 @@
     async def _astream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
-        request = get_cohere_chat_request(messages, **self._default_params, **kwargs)
+        request = get_cohere_chat_request(
+            messages, stop_sequences=stop, **self._default_params, **kwargs
+        )
 
         if hasattr(self.async_client, "chat_stream"):  # detect and support sdk v5
             stream = self.async_client.chat_stream(**request)
         else:
             stream = self.async_client.chat(**request, stream=True)
 
         async for data in stream:
@@ -301,15 +318,17 @@
     ) -> ChatResult:
         if self.streaming:
             stream_iter = self._stream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return generate_from_stream(stream_iter)
 
-        request = get_cohere_chat_request(messages, **self._default_params, **kwargs)
+        request = get_cohere_chat_request(
+            messages, stop_sequences=stop, **self._default_params, **kwargs
+        )
         response = self.client.chat(**request)
 
         generation_info = self._get_generation_info(response)
         message = AIMessage(content=response.text, additional_kwargs=generation_info)
         return ChatResult(
             generations=[
                 ChatGeneration(message=message, generation_info=generation_info)
@@ -325,15 +344,17 @@
     ) -> ChatResult:
         if self.streaming:
             stream_iter = self._astream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return await agenerate_from_stream(stream_iter)
 
-        request = get_cohere_chat_request(messages, **self._default_params, **kwargs)
+        request = get_cohere_chat_request(
+            messages, stop_sequences=stop, **self._default_params, **kwargs
+        )
         response = self.client.chat(**request)
 
         generation_info = self._get_generation_info(response)
         message = AIMessage(content=response.text, additional_kwargs=generation_info)
         return ChatResult(
             generations=[
                 ChatGeneration(message=message, generation_info=generation_info)
```

### Comparing `langchain_cohere-0.1.0rc1/langchain_cohere/cohere_agent.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/cohere_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,22 @@
 from langchain_core.outputs import Generation
 from langchain_core.outputs.chat_generation import ChatGeneration
 from langchain_core.prompts.chat import ChatPromptTemplate
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from langchain_core.runnables.base import RunnableLambda
 from langchain_core.tools import BaseTool
-from langchain_core.utils.function_calling import convert_to_openai_function
+from langchain_core.utils.function_calling import (
+    convert_to_openai_function,
+)
+
+from langchain_cohere.utils import (
+    JSON_TO_PYTHON_TYPES,
+    _remove_signature_from_tool_description,
+)
 
 
 def create_cohere_tools_agent(
     llm: BaseLanguageModel, tools: Sequence[BaseTool], prompt: ChatPromptTemplate
 ) -> Runnable:
     def llm_with_tools(input_: Dict) -> Runnable:
         tool_results = (
@@ -95,19 +102,25 @@
 ) -> Dict[str, Any]:
     """
     Convert a BaseTool instance, JSON schema dict, or BaseModel type to a Cohere tool.
     """
     if isinstance(tool, BaseTool):
         return Tool(
             name=tool.name,
-            description=tool.description,
+            description=_remove_signature_from_tool_description(
+                tool.name, tool.description
+            ),
             parameter_definitions={
                 param_name: ToolParameterDefinitionsValue(
-                    description=param_definition.get("description"),
-                    type=param_definition.get("type"),
+                    description=param_definition.get("description")
+                    if "description" in param_definition
+                    else "",
+                    type=JSON_TO_PYTHON_TYPES.get(
+                        param_definition.get("type"), param_definition.get("type")
+                    ),
                     required="default" not in param_definition,
                 )
                 for param_name, param_definition in tool.args.items()
             },
         ).dict()
     elif isinstance(tool, dict):
         if not all(k in tool for k in ("title", "description", "properties")):
@@ -116,15 +129,17 @@
             )
         return Tool(
             name=tool.get("title"),
             description=tool.get("description"),
             parameter_definitions={
                 param_name: ToolParameterDefinitionsValue(
                     description=param_definition.get("description"),
-                    type=param_definition.get("type"),
+                    type=JSON_TO_PYTHON_TYPES.get(
+                        param_definition.get("type"), param_definition.get("type")
+                    ),
                     required="default" not in param_definition,
                 )
                 for param_name, param_definition in tool.get("properties", {}).items()
             },
         ).dict()
     elif issubclass(tool, BaseModel):
         as_json_schema_function = convert_to_openai_function(tool)
@@ -136,15 +151,17 @@
                 # The Cohere API requires the description field.
                 "description",
                 as_json_schema_function.get("name"),
             ),
             parameter_definitions={
                 param_name: ToolParameterDefinitionsValue(
                     description=param_definition.get("description"),
-                    type=param_definition.get("type"),
+                    type=JSON_TO_PYTHON_TYPES.get(
+                        param_definition.get("type"), param_definition.get("type")
+                    ),
                     required=param_name in parameters.get("required", []),
                 )
                 for param_name, param_definition in properties.items()
             },
         ).dict()
     else:
         raise ValueError(
```

### Comparing `langchain_cohere-0.1.0rc1/langchain_cohere/embeddings.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,20 @@
 
     cohere_api_key: Optional[str] = None
 
     max_retries: int = 3
     """Maximum number of retries to make when generating."""
     request_timeout: Optional[float] = None
     """Timeout in seconds for the Cohere API request."""
-    user_agent: str = "langchain"
+    user_agent: str = "langchain:partner"
     """Identifier for the application making the request."""
 
+    base_url: Optional[str] = None
+    """Override the default Cohere API URL."""
+
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
         extra = Extra.forbid
 
     @root_validator()
@@ -60,19 +63,21 @@
         request_timeout = values.get("request_timeout")
 
         client_name = values["user_agent"]
         values["client"] = cohere.Client(
             cohere_api_key,
             timeout=request_timeout,
             client_name=client_name,
+            base_url=values["base_url"],
         )
         values["async_client"] = cohere.AsyncClient(
             cohere_api_key,
             timeout=request_timeout,
             client_name=client_name,
+            base_url=values["base_url"],
         )
 
         return values
 
     def embed_with_retry(self, **kwargs: Any) -> Any:
         """Use tenacity to retry the embed call."""
         retry_decorator = _create_retry_decorator(self.max_retries)
```

### Comparing `langchain_cohere-0.1.0rc1/langchain_cohere/llms.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/llms.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,28 +65,39 @@
 
     streaming: bool = Field(default=False)
     """Whether to stream the results."""
 
     user_agent: str = "langchain"
     """Identifier for the application making the request."""
 
+    timeout_seconds: Optional[float] = 300
+    """Timeout in seconds for the Cohere API request."""
+
+    base_url: Optional[str] = None
+    """Override the default Cohere API URL."""
+
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         values["cohere_api_key"] = convert_to_secret_str(
             get_from_dict_or_env(values, "cohere_api_key", "COHERE_API_KEY")
         )
         client_name = values["user_agent"]
+        timeout_seconds = values.get("timeout_seconds")
         values["client"] = cohere.Client(
             api_key=values["cohere_api_key"].get_secret_value(),
+            timeout=timeout_seconds,
             client_name=client_name,
+            base_url=values["base_url"],
         )
         values["async_client"] = cohere.AsyncClient(
             api_key=values["cohere_api_key"].get_secret_value(),
             client_name=client_name,
+            timeout=timeout_seconds,
+            base_url=values["base_url"],
         )
         return values
 
 
 class Cohere(LLM, BaseCohere):
     """Cohere large language models.
```

### Comparing `langchain_cohere-0.1.0rc1/langchain_cohere/rag_retrievers.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/rag_retrievers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForRetrieverRun,
     CallbackManagerForRetrieverRun,
 )
 from langchain_core.documents import Document
 from langchain_core.language_models.chat_models import BaseChatModel
@@ -13,23 +13,24 @@
 from langchain_core.retrievers import BaseRetriever
 
 if TYPE_CHECKING:
     from langchain_core.messages import BaseMessage
 
 
 def _get_docs(response: Any) -> List[Document]:
-    docs = (
-        []
-        if "documents" not in response.generation_info
-        or len(response.generation_info["documents"]) == 0
-        else [
-            Document(page_content=doc["snippet"], metadata=doc)
-            for doc in response.generation_info["documents"]
-        ]
-    )
+    docs = []
+    if (
+        "documents" in response.generation_info
+        and len(response.generation_info["documents"]) > 0
+    ):
+        for doc in response.generation_info["documents"]:
+            content = doc.get("snippet", None) or doc.get("text", None)
+            if content is not None:
+                docs.append(Document(page_content=content, metadata=doc))
+
     docs.append(
         Document(
             page_content=response.message.content,
             metadata={
                 "type": "model_response",
                 "citations": response.generation_info["citations"],
                 "search_results": response.generation_info["search_results"],
@@ -59,35 +60,43 @@
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
         """Allow arbitrary types."""
 
     def _get_relevant_documents(
-        self, query: str, *, run_manager: CallbackManagerForRetrieverRun, **kwargs: Any
+        self,
+        query: str,
+        *,
+        run_manager: CallbackManagerForRetrieverRun,
+        documents: Optional[List[Dict[str, str]]] = None,
+        **kwargs: Any,
     ) -> List[Document]:
         messages: List[List[BaseMessage]] = [[HumanMessage(content=query)]]
         res = self.llm.generate(
             messages,
-            connectors=self.connectors,
+            connectors=self.connectors if documents is None else None,
+            documents=documents,
             callbacks=run_manager.get_child(),
             **kwargs,
         ).generations[0][0]
         return _get_docs(res)
 
     async def _aget_relevant_documents(
         self,
         query: str,
         *,
         run_manager: AsyncCallbackManagerForRetrieverRun,
+        documents: Optional[List[Dict[str, str]]] = None,
         **kwargs: Any,
     ) -> List[Document]:
         messages: List[List[BaseMessage]] = [[HumanMessage(content=query)]]
         res = (
             await self.llm.agenerate(
                 messages,
-                connectors=self.connectors,
+                connectors=self.connectors if documents is None else None,
+                documents=documents,
                 callbacks=run_manager.get_child(),
                 **kwargs,
             )
         ).generations[0][0]
         return _get_docs(res)
```

### Comparing `langchain_cohere-0.1.0rc1/langchain_cohere/rerank.py` & `langchain_cohere-0.1.1rc0/langchain_cohere/rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.0rc1/pyproject.toml` & `langchain_cohere-0.1.1rc0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 [tool.poetry]
 name = "langchain-cohere"
-version = "0.1.0rc1"
+version = "0.1.1rc0"
 description = "An integration package connecting Cohere and LangChain"
 authors = []
 readme = "README.md"
-repository = "https://github.com/langchain-ai/langchain"
+repository = "https://github.com/langchain-ai/langchain-cohere"
 license = "MIT"
 
 [tool.poetry.urls]
-"Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/cohere"
+"Source Code" = "https://github.com/langchain-ai/langchain-cohere/tree/main/libs/cohere"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = "^0.1.32"
-cohere = "^5.1.4"
+cohere = ">=5.1.8,<5.2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
+langchain = "^0.1.14"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
-langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = { path = "../../core", develop = true }
 
 [tool.ruff]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
```

