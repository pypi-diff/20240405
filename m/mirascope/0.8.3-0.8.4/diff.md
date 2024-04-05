# Comparing `tmp/mirascope-0.8.3.tar.gz` & `tmp/mirascope-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirascope-0.8.3.tar", max compression
+gzip compressed data, was "mirascope-0.8.4.tar", max compression
```

## Comparing `mirascope-0.8.3.tar` & `mirascope-0.8.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1072 2024-04-04 01:09:48.611045 mirascope-0.8.3/LICENSE
--rw-r--r--   0        0        0    10093 2024-04-04 01:09:48.611045 mirascope-0.8.3/docs/README.md
--rw-r--r--   0        0        0      472 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/__init__.py
--rw-r--r--   0        0        0      270 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/__init__.py
--rw-r--r--   0        0        0     8732 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/calls.py
--rw-r--r--   0        0        0     4088 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/extractors.py
--rw-r--r--   0        0        0        0 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/py.typed
--rw-r--r--   0        0        0     9642 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/tools.py
--rw-r--r--   0        0        0     6705 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/types.py
--rw-r--r--   0        0        0      453 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/__init__.py
--rw-r--r--   0        0        0     3645 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/calls.py
--rw-r--r--   0        0        0     8304 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/extractors.py
--rw-r--r--   0        0        0     5696 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/prompts.py
--rw-r--r--   0        0        0        0 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/py.typed
--rw-r--r--   0        0        0     2890 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/tools.py
--rw-r--r--   0        0        0     5313 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/types.py
--rw-r--r--   0        0        0     5615 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/utils.py
--rw-r--r--   0        0        0       97 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/__init__.py
--rw-r--r--   0        0        0      199 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/__init__.py
--rw-r--r--   0        0        0     4213 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/add.py
--rw-r--r--   0        0        0     3002 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/init.py
--rw-r--r--   0        0        0        0 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/py.typed
--rw-r--r--   0        0        0     3101 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/remove.py
--rw-r--r--   0        0        0     2008 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/status.py
--rw-r--r--   0        0        0     2801 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/use.py
--rw-r--r--   0        0        0      118 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/constants.py
--rw-r--r--   0        0        0       86 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/generic/__init__.py
--rw-r--r--   0        0        0      494 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/generic/mirascope.ini.j2
--rw-r--r--   0        0        0     1554 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/generic/prompt_template.j2
--rw-r--r--   0        0        0     1067 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/py.typed
--rw-r--r--   0        0        0     1197 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/schemas.py
--rw-r--r--   0        0        0    24322 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/utils.py
--rw-r--r--   0        0        0     1552 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/enums.py
--rw-r--r--   0        0        0      241 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/__init__.py
--rw-r--r--   0        0        0     6333 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/calls.py
--rw-r--r--   0        0        0     3730 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/extractors.py
--rw-r--r--   0        0        0     4081 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/tools.py
--rw-r--r--   0        0        0     4950 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/types.py
--rw-r--r--   0        0        0      239 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/__init__.py
--rw-r--r--   0        0        0     5900 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/calls.py
--rw-r--r--   0        0        0     3940 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/extractors.py
--rw-r--r--   0        0        0        0 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/py.typed
--rw-r--r--   0        0        0     3896 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/tools.py
--rw-r--r--   0        0        0     6389 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/types.py
--rw-r--r--   0        0        0      232 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/__init__.py
--rw-r--r--   0        0        0     9068 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/calls.py
--rw-r--r--   0        0        0     3932 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/extractors.py
--rw-r--r--   0        0        0        0 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/py.typed
--rw-r--r--   0        0        0     3860 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/tools.py
--rw-r--r--   0        0        0     9087 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/types.py
--rw-r--r--   0        0        0        0 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/py.typed
--rw-r--r--   0        0        0      151 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/wandb/__init__.py
--rw-r--r--   0        0        0     9593 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/wandb/wandb.py
--rw-r--r--   0        0        0     1921 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/wandb/weave.py
--rw-r--r--   0        0        0     2763 2024-04-04 01:09:48.619045 mirascope-0.8.3/pyproject.toml
--rw-r--r--   0        0        0    11526 1970-01-01 00:00:00.000000 mirascope-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 05:54:10.645911 mirascope-0.8.4/LICENSE
+-rw-r--r--   0        0        0    10093 2024-04-05 05:54:10.645911 mirascope-0.8.4/docs/README.md
+-rw-r--r--   0        0        0      472 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/__init__.py
+-rw-r--r--   0        0        0      270 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/calls.py
+-rw-r--r--   0        0        0     4068 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/py.typed
+-rw-r--r--   0        0        0     3549 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/tools.py
+-rw-r--r--   0        0        0     6006 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/types.py
+-rw-r--r--   0        0        0      453 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/__init__.py
+-rw-r--r--   0        0        0     3645 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/calls.py
+-rw-r--r--   0        0        0     8304 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/extractors.py
+-rw-r--r--   0        0        0     5696 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/prompts.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/py.typed
+-rw-r--r--   0        0        0     2890 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/tools.py
+-rw-r--r--   0        0        0     5313 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/types.py
+-rw-r--r--   0        0        0     5615 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/utils.py
+-rw-r--r--   0        0        0       97 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4213 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/add.py
+-rw-r--r--   0        0        0     3002 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/init.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/py.typed
+-rw-r--r--   0        0        0     3101 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/remove.py
+-rw-r--r--   0        0        0     2008 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/status.py
+-rw-r--r--   0        0        0     2801 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/use.py
+-rw-r--r--   0        0        0      118 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/constants.py
+-rw-r--r--   0        0        0       86 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/generic/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/generic/mirascope.ini.j2
+-rw-r--r--   0        0        0     1554 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/generic/prompt_template.j2
+-rw-r--r--   0        0        0     1067 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/py.typed
+-rw-r--r--   0        0        0     1197 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/schemas.py
+-rw-r--r--   0        0        0    24322 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/utils.py
+-rw-r--r--   0        0        0     1552 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/enums.py
+-rw-r--r--   0        0        0      241 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/__init__.py
+-rw-r--r--   0        0        0     6333 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/calls.py
+-rw-r--r--   0        0        0     3730 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/extractors.py
+-rw-r--r--   0        0        0     4081 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/tools.py
+-rw-r--r--   0        0        0     4950 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/types.py
+-rw-r--r--   0        0        0      239 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/__init__.py
+-rw-r--r--   0        0        0     5900 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/calls.py
+-rw-r--r--   0        0        0     3940 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/py.typed
+-rw-r--r--   0        0        0     3896 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/tools.py
+-rw-r--r--   0        0        0     6389 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/types.py
+-rw-r--r--   0        0        0      232 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/__init__.py
+-rw-r--r--   0        0        0     9068 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/calls.py
+-rw-r--r--   0        0        0     3932 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/py.typed
+-rw-r--r--   0        0        0     3860 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/tools.py
+-rw-r--r--   0        0        0     9087 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/types.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/py.typed
+-rw-r--r--   0        0        0      151 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/wandb/__init__.py
+-rw-r--r--   0        0        0     9593 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/wandb/wandb.py
+-rw-r--r--   0        0        0     1921 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/wandb/weave.py
+-rw-r--r--   0        0        0     2763 2024-04-05 05:54:10.653911 mirascope-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0    11526 1970-01-01 00:00:00.000000 mirascope-0.8.4/PKG-INFO
```

### Comparing `mirascope-0.8.3/LICENSE` & `mirascope-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/docs/README.md` & `mirascope-0.8.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/anthropic/extractors.py` & `mirascope-0.8.4/mirascope/anthropic/extractors.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 logger = logging.getLogger("mirascope")
 
 T = TypeVar("T", bound=ExtractedType)
 
 
 EXTRACT_SYSTEM_MESSAGE = """
-OUTPUT ONLY FUNCTION CALLS WITHOUT ANY ADDITIONAL TEXT.
-You must wrap all invoke calls in the <function_calls> tag.
+OUTPUT ONLY TOOL CALLS.
 ONLY EXTRACT ANSWERS THAT YOU ARE ABSOLUTELY 100% CERTAIN ARE CORRECT.
+If asked to generate information, you may generate the tool call input.
 """.strip()
 
 
 class AnthropicExtractor(BaseExtractor[AnthropicCall, AnthropicTool, T], Generic[T]):
     '''A class for extracting structured information using Anthropic Claude models.
 
     Example:
```

### Comparing `mirascope-0.8.3/mirascope/anthropic/types.py` & `mirascope-0.8.4/mirascope/anthropic/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Type classes for interacting with Anthropics's Claude API."""
-
-import xml.etree.ElementTree as ET
-from typing import Any, Callable, Literal, Optional, Type, Union, cast
+from typing import Any, Callable, Literal, Optional, Type, Union
 
 from anthropic import Anthropic, AsyncAnthropic
 from anthropic._types import Body, Headers, Query
 from anthropic.types import (
     ContentBlockDeltaEvent,
     ContentBlockStartEvent,
     Message,
     MessageStreamEvent,
 )
+from anthropic.types.beta.tools import ToolsBetaMessage
 from anthropic.types.completion_create_params import Metadata
 from httpx import Timeout
 from pydantic import ConfigDict
 
 from ..base.types import BaseCallParams, BaseCallResponse, BaseCallResponseChunk
 from .tools import AnthropicTool
 
@@ -62,15 +61,17 @@
     ) -> dict[str, Any]:
         """Returns the keyword argument call parameters."""
         extra_exclude = {"wrapper", "wrapper_async"}
         exclude = extra_exclude if exclude is None else exclude.union(extra_exclude)
         return super().kwargs(tool_type, exclude)
 
 
-class AnthropicCallResponse(BaseCallResponse[Message, AnthropicTool]):
+class AnthropicCallResponse(
+    BaseCallResponse[Union[Message, ToolsBetaMessage], AnthropicTool]
+):
     """Convenience wrapper around the Anthropic Claude API.
 
     When using Mirascope's convenience wrappers to interact with Anthropic models via
     `AnthropicCall`, responses using `Anthropic.call()` will return an
     `AnthropicCallResponse`, whereby the implemented properties allow for simpler syntax
     and a convenient developer experience.
 
@@ -90,65 +91,48 @@
 
     @property
     def tools(self) -> Optional[list[AnthropicTool]]:
         """Returns the tools for the 0th choice message."""
         if not self.tool_types:
             return None
 
-        if (
-            self.response.stop_reason != "stop_sequence"
-            or self.response.stop_sequence != "</function_calls>"
-        ):
+        if self.response.stop_reason != "tool_use":
             raise RuntimeError(
-                "Generation stopped before `</function_calls>` stop sequence. "
+                "Generation stopped with stop reason that is not `tool_use`. "
                 "This is likely due to a limit on output tokens that is too low. "
                 "Note that this could also indicate no tool is beind called, so we "
                 "recommend that you check the output of the call to confirm. "
                 f"Stop Reason: {self.response.stop_reason} "
-                f"Stop Sequence: {self.response.stop_sequence}"
-            )
-
-        try:
-            root_node = ET.fromstring(
-                f"<wrapper>{self.response.content}</function_calls></wrapper>"
             )
-        except ET.ParseError as e:
-            raise ValueError("Unable to parse tools from response") from e
-
-        # There must be a <function_calls> tag since we successfully parsed the
-        # XML with the manually added </function_calls> tag.
-        tool_calls_node = cast(ET.Element, root_node.find("function_calls"))
 
         extracted_tools = []
-        for tool_call_node in tool_calls_node:
+        for tool_call in self.response.content:
+            if tool_call.type != "tool_use":
+                continue
             for tool_type in self.tool_types:
-                tool_name_node = tool_call_node.find("tool_name")
-                if (
-                    tool_name_node is not None
-                    and tool_name_node.text == tool_type.__name__
-                    and (parameters := tool_call_node.find("parameters"))
-                ):
-                    tool = tool_type.from_tool_call(parameters)
+                if tool_call.name == tool_type.__name__:
+                    tool = tool_type.from_tool_call(tool_call)
                     extracted_tools.append(tool)
                     break
 
         return extracted_tools
 
     @property
     def tool(self) -> Optional[AnthropicTool]:
-        """Returns the 0th tool for the 0th choice message."""
+        """Returns the 0th tool for the 0th choice text block."""
         tools = self.tools
         if tools:
             return tools[0]
         return None
 
     @property
     def content(self) -> str:
-        """Returns the string content of the 0th message."""
-        return self.response.content[0].text
+        """Returns the string text of the 0th text block."""
+        block = self.response.content[0]
+        return block.text if block.type == "text" else ""
 
     def dump(self) -> dict[str, Any]:
         """Dumps the response to a dictionary."""
         return {
             "start_time": self.start_time,
             "end_time": self.end_time,
             "output": self.response.model_dump(),
```

### Comparing `mirascope-0.8.3/mirascope/base/calls.py` & `mirascope-0.8.4/mirascope/base/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/base/extractors.py` & `mirascope-0.8.4/mirascope/base/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/base/prompts.py` & `mirascope-0.8.4/mirascope/base/prompts.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/base/tools.py` & `mirascope-0.8.4/mirascope/base/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/base/types.py` & `mirascope-0.8.4/mirascope/base/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/base/utils.py` & `mirascope-0.8.4/mirascope/base/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/commands/add.py` & `mirascope-0.8.4/mirascope/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/commands/init.py` & `mirascope-0.8.4/mirascope/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/commands/remove.py` & `mirascope-0.8.4/mirascope/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/commands/status.py` & `mirascope-0.8.4/mirascope/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/commands/use.py` & `mirascope-0.8.4/mirascope/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/generic/prompt_template.j2` & `mirascope-0.8.4/mirascope/cli/generic/prompt_template.j2`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/main.py` & `mirascope-0.8.4/mirascope/cli/main.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/schemas.py` & `mirascope-0.8.4/mirascope/cli/schemas.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/cli/utils.py` & `mirascope-0.8.4/mirascope/cli/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/enums.py` & `mirascope-0.8.4/mirascope/enums.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/gemini/calls.py` & `mirascope-0.8.4/mirascope/gemini/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/gemini/extractors.py` & `mirascope-0.8.4/mirascope/gemini/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/gemini/tools.py` & `mirascope-0.8.4/mirascope/gemini/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/gemini/types.py` & `mirascope-0.8.4/mirascope/gemini/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/mistral/calls.py` & `mirascope-0.8.4/mirascope/mistral/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/mistral/extractors.py` & `mirascope-0.8.4/mirascope/mistral/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/mistral/tools.py` & `mirascope-0.8.4/mirascope/mistral/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/mistral/types.py` & `mirascope-0.8.4/mirascope/mistral/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/openai/calls.py` & `mirascope-0.8.4/mirascope/openai/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/openai/extractors.py` & `mirascope-0.8.4/mirascope/openai/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/openai/tools.py` & `mirascope-0.8.4/mirascope/openai/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/openai/types.py` & `mirascope-0.8.4/mirascope/openai/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/wandb/wandb.py` & `mirascope-0.8.4/mirascope/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/mirascope/wandb/weave.py` & `mirascope-0.8.4/mirascope/wandb/weave.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.3/pyproject.toml` & `mirascope-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mirascope"
-version = "0.8.3"
+version = "0.8.4"
 description = "LLM toolkit for lightning-fast, high-quality development"
 license = "MIT"
 authors = [
     "William Bakst <william@mirascope.io>",
     "Brendan Kao <brendan@mirascope.io>",
 ]
 readme = "docs/README.md"
@@ -20,17 +20,17 @@
 typer = { version = "^0.9.0", extras = ["all"] }
 Jinja2 = "^3.1.3"
 openai = "^1.6.0"
 docstring-parser = "^0.15"
 
 # A list of optional dependencies that are required for certain features
 wandb = { version = "^0.16.4", optional = true }
-weave = { version = "^0.46.0", optional = true }
+weave = { version = "^0.50.0", optional = true }
 google-generativeai = { version = "^0.4.0", optional = true }
-anthropic = { version = "^0.21.3", optional = true }
+anthropic = { version = "^0.23.1", optional = true }
 mistralai = { version = "^0.1.6", optional = true }
 
 [tool.poetry.extras]
 wandb = ["wandb"]
 weave = ["weave"]
 gemini = ["google-generativeai"]
 anthropic = ["anthropic"]
```

### Comparing `mirascope-0.8.3/PKG-INFO` & `mirascope-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirascope
-Version: 0.8.3
+Version: 0.8.4
 Summary: LLM toolkit for lightning-fast, high-quality development
 Home-page: https://github.com/Mirascope/mirascope
 License: MIT
 Author: William Bakst
 Author-email: william@mirascope.io
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -16,23 +16,23 @@
 Provides-Extra: all
 Provides-Extra: anthropic
 Provides-Extra: gemini
 Provides-Extra: mistral
 Provides-Extra: wandb
 Provides-Extra: weave
 Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
-Requires-Dist: anthropic (>=0.21.3,<0.22.0) ; extra == "anthropic" or extra == "all"
+Requires-Dist: anthropic (>=0.23.1,<0.24.0) ; extra == "anthropic" or extra == "all"
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0) ; extra == "gemini" or extra == "all"
 Requires-Dist: mistralai (>=0.1.6,<0.2.0) ; extra == "mistral" or extra == "all"
 Requires-Dist: openai (>=1.6.0,<2.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: wandb (>=0.16.4,<0.17.0) ; extra == "wandb" or extra == "all"
-Requires-Dist: weave (>=0.46.0,<0.47.0) ; extra == "weave" or extra == "all"
+Requires-Dist: weave (>=0.50.0,<0.51.0) ; extra == "weave" or extra == "all"
 Project-URL: Repository, https://github.com/Mirascope/mirascope
 Description-Content-Type: text/markdown
 
 <div align="center" justiry="start">
     <a href="https://www.mirascope.io">
         <img align="bottom" src="https://github.com/Mirascope/mirascope/assets/99370834/e403d7ee-f8bc-4df1-b2d0-33763f021c89" alt="Frog Logo" width="84"/><br><img align="bottom" src="https://uploads-ssl.webflow.com/65a6fd6a1c3b2704d6217d3d/65b5674e9ceef563dc57eb11_Medium%20length%20hero%20headline%20goes%20here.svg" width="400" alt="Mirascope"/>
     </a>
```

