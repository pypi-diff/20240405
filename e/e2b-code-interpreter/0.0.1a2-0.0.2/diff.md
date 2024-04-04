# Comparing `tmp/e2b_code_interpreter-0.0.1a2.tar.gz` & `tmp/e2b_code_interpreter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b_code_interpreter-0.0.1a2.tar", max compression
+gzip compressed data, was "e2b_code_interpreter-0.0.2.tar", max compression
```

## Comparing `e2b_code_interpreter-0.0.1a2.tar` & `e2b_code_interpreter-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3175 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/README.md
--rw-r--r--   0        0        0      114 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0    11096 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/main.py
--rw-r--r--   0        0        0     9100 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/messaging.py
--rw-r--r--   0        0        0     6192 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/models.py
--rw-r--r--   0        0        0      770 2024-04-03 21:44:56.742223 e2b_code_interpreter-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     3173 2024-04-04 22:21:46.230885 e2b_code_interpreter-0.0.2/README.md
+-rw-r--r--   0        0        0      114 2024-04-04 22:21:46.230885 e2b_code_interpreter-0.0.2/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    11060 2024-04-04 22:21:46.230885 e2b_code_interpreter-0.0.2/e2b_code_interpreter/main.py
+-rw-r--r--   0        0        0     9056 2024-04-04 22:21:46.230885 e2b_code_interpreter-0.0.2/e2b_code_interpreter/messaging.py
+-rw-r--r--   0        0        0     6858 2024-04-04 22:21:46.234885 e2b_code_interpreter-0.0.2/e2b_code_interpreter/models.py
+-rw-r--r--   0        0        0      768 2024-04-04 22:22:14.114828 e2b_code_interpreter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.2/PKG-INFO
```

### Comparing `e2b_code_interpreter-0.0.1a2/README.md` & `e2b_code_interpreter-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 data = pd.DataFrame(data=[[1, 2], [3, 4]], columns=["A", "B"])
 display(data.head(10))
 time.sleep(3)
 print("world")
 """
 
 with CodeInterpreter() as sandbox:
-    sandbox.notebook.exec_cell(code, on_stdout=print, on_stderr=print, on_display_data=(lambda data: print(data.text)))
+    sandbox.notebook.exec_cell(code, on_stdout=print, on_stderr=print, on_result=(lambda result: print(result.text)))
 ```
 
 ### Pre-installed Python packages inside the sandbox
 
 The full and always up-to-date list can be found in the [`requirements.txt`](https://github.com/e2b-dev/E2B/blob/stateful-code-interpreter/sandboxes/code-interpreter-stateful/requirements.txt) file.
 
 ```text
```

### Comparing `e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/main.py` & `e2b_code_interpreter-0.0.2/e2b_code_interpreter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from typing import Any, Callable, List, Optional, Dict
 
 import requests
 from e2b import EnvVars, ProcessMessage, Sandbox
 from e2b.constants import TIMEOUT
 
 from e2b_code_interpreter.messaging import JupyterKernelWebSocket
-from e2b_code_interpreter.models import KernelException, Execution
-
+from e2b_code_interpreter.models import KernelException, Execution, Result
 
 logger = logging.getLogger(__name__)
 
 
 class CodeInterpreter(Sandbox):
     """
     E2B code interpreter sandbox extension.
@@ -62,25 +61,25 @@
 
     def exec_cell(
         self,
         code: str,
         kernel_id: Optional[str] = None,
         on_stdout: Optional[Callable[[ProcessMessage], Any]] = None,
         on_stderr: Optional[Callable[[ProcessMessage], Any]] = None,
-        on_display_data: Optional[Callable[[Dict[str, Any]], Any]] = None,
+        on_result: Optional[Callable[[Result], Any]] = None,
         timeout: Optional[float] = TIMEOUT,
     ) -> Execution:
         """
         Execute code in a notebook cell.
 
         :param code: Code to execute
         :param kernel_id: The ID of the kernel to execute the code on. If not provided, the default kernel is used.
         :param on_stdout: A callback function to handle standard output messages from the code execution.
         :param on_stderr: A callback function to handle standard error messages from the code execution.
-        :param on_display_data: A callback function to handle display data messages from the code execution.
+        :param on_result: A callback function to handle the result and display calls of the code execution.
         :param timeout: Timeout for the call
 
         :return: Result of the execution
         """
         kernel_id = kernel_id or self.default_kernel_id
         ws_future = self._connected_kernels.get(kernel_id)
 
@@ -89,17 +88,15 @@
         if ws_future:
             logger.debug(f"Using existing websocket connection to kernel {kernel_id}")
             ws = ws_future.result(timeout=timeout)
         else:
             logger.debug(f"Creating new websocket connection to kernel {kernel_id}")
             ws = self._connect_to_kernel_ws(kernel_id, timeout=timeout)
 
-        session_id = ws.send_execution_message(
-            code, on_stdout, on_stderr, on_display_data
-        )
+        session_id = ws.send_execution_message(code, on_stdout, on_stderr, on_result)
         logger.debug(
             f"Sent execution message to kernel {kernel_id}, session_id: {session_id}"
         )
 
         result = ws.get_result(session_id, timeout=timeout)
         logger.debug(
             f"Received result from kernel {kernel_id}, session_id: {session_id}, result: {result}"
```

### Comparing `e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/messaging.py` & `e2b_code_interpreter-0.0.2/e2b_code_interpreter/messaging.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 from e2b import ProcessMessage
 from e2b.constants import TIMEOUT
 from e2b.sandbox import TimeoutException
 from e2b.sandbox.websocket_client import WebSocket
 from e2b.utils.future import DeferredFuture
 from pydantic import ConfigDict, PrivateAttr, BaseModel
 
-from e2b_code_interpreter.models import Execution, Result, Error, MIMEType
+from e2b_code_interpreter.models import Execution, Result, Error
 
 logger = logging.getLogger(__name__)
 
 
 class CellExecution:
     """
     Represents the execution of a cell in the Jupyter kernel.
     It's an internal class used by JupyterKernelWebSocket.
     """
 
     input_accepted: bool = False
-    on_stdout: Optional[Callable[[ProcessMessage], None]] = None
-    on_stderr: Optional[Callable[[ProcessMessage], None]] = None
-    on_display_data: Optional[Callable[[Dict[MIMEType, str]], None]] = None
+    on_stdout: Optional[Callable[[ProcessMessage], Any]] = None
+    on_stderr: Optional[Callable[[ProcessMessage], Any]] = None
+    on_result: Optional[Callable[[Result], Any]] = None
 
     def __init__(
         self,
-        on_stdout: Optional[Callable[[ProcessMessage], None]] = None,
-        on_stderr: Optional[Callable[[ProcessMessage], None]] = None,
-        on_display_data: Optional[Callable[[Dict[MIMEType, str]], None]] = None,
+        on_stdout: Optional[Callable[[ProcessMessage], Any]] = None,
+        on_stderr: Optional[Callable[[ProcessMessage], Any]] = None,
+        on_result: Optional[Callable[[Result], Any]] = None,
     ):
         self.partial_result = Execution()
         self.execution = Future()
         self.on_stdout = on_stdout
         self.on_stderr = on_stderr
-        self.on_display_data = on_display_data
+        self.on_result = on_result
 
 
 class JupyterKernelWebSocket(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     url: str
 
@@ -125,25 +125,25 @@
                 },
             }
         )
 
     def send_execution_message(
         self,
         code: str,
-        on_stdout: Optional[Callable[[ProcessMessage], None]] = None,
-        on_stderr: Optional[Callable[[ProcessMessage], None]] = None,
-        on_display_data: Optional[Callable[[Dict[MIMEType, str]], None]] = None,
+        on_stdout: Optional[Callable[[ProcessMessage], Any]] = None,
+        on_stderr: Optional[Callable[[ProcessMessage], Any]] = None,
+        on_result: Optional[Callable[[Result], Any]] = None,
     ) -> str:
         message_id = str(uuid.uuid4())
         logger.debug(f"Sending execution message: {message_id}")
 
         self._cells[message_id] = CellExecution(
             on_stdout=on_stdout,
             on_stderr=on_stderr,
-            on_display_data=on_display_data,
+            on_result=on_result,
         )
         request = self._get_execute_request(message_id, code)
         self._queue_in.put(request)
         return message_id
 
     def get_result(
         self, message_id: str, timeout: Optional[float] = TIMEOUT
@@ -200,20 +200,21 @@
                             timestamp=time.time_ns(),
                         )
                     )
 
         elif data["msg_type"] in "display_data":
             result = Result(is_main_result=False, data=data["content"]["data"])
             execution.results.append(result)
-            if cell.on_display_data:
-                cell.on_display_data(result)
+            if cell.on_result:
+                cell.on_result(result)
         elif data["msg_type"] == "execute_result":
-            execution.results.append(
-                Result(is_main_result=True, data=data["content"]["data"])
-            )
+            result = Result(is_main_result=True, data=data["content"]["data"])
+            execution.results.append(result)
+            if cell.on_result:
+                cell.on_result(result)
         elif data["msg_type"] == "status":
             if data["content"]["execution_state"] == "idle":
                 if cell.input_accepted:
                     logger.debug(f"Cell {parent_msg_ig} finished execution")
                     cell.execution.set_result(execution)
 
             elif data["content"]["execution_state"] == "error":
```

### Comparing `e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/models.py` & `e2b_code_interpreter-0.0.2/e2b_code_interpreter/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Represents a MIME type.
     """
 
 
 class Result:
     """
     Represents the data to be displayed as a result of executing a cell in a Jupyter notebook.
-    This is result returned by ipython kernel: https://ipython.readthedocs.io/en/stable/development/execution.html#execution-semantics
+    The result is similar to the structure returned by ipython kernel: https://ipython.readthedocs.io/en/stable/development/execution.html#execution-semantics
 
     The result can contain multiple types of data, such as text, images, plots, etc. Each type of data is represented
     as a string, and the result can contain multiple types of data. The text representation is always present, and
     the other representations are optional.
 
     The class also provides methods to display the data in a Jupyter notebook.
     """
@@ -76,21 +76,44 @@
         self.jpeg = data.pop("image/jpeg", None)
         self.pdf = data.pop("application/pdf", None)
         self.latex = data.pop("text/latex", None)
         self.json = data.pop("application/json", None)
         self.javascript = data.pop("application/javascript", None)
         self.extra = data
 
-    def keys(self) -> Iterable[str]:
+    def formats(self) -> Iterable[str]:
         """
-        Returns the MIME types of the data.
+        Returns all available formats of the result.
 
-        :return: The MIME types of the data.
+        :return: All available formats of the result in MIME types.
         """
-        return self.raw.keys()
+        formats = []
+        if self.html:
+            formats.append("html")
+        if self.markdown:
+            formats.append("markdown")
+        if self.svg:
+            formats.append("svg")
+        if self.png:
+            formats.append("png")
+        if self.jpeg:
+            formats.append("jpeg")
+        if self.pdf:
+            formats.append("pdf")
+        if self.latex:
+            formats.append("latex")
+        if self.json:
+            formats.append("json")
+        if self.javascript:
+            formats.append("javascript")
+
+        for key in self.extra:
+            formats.append(key)
+
+        return formats
 
     def __str__(self) -> str:
         """
         Returns the text representation of the data.
 
         :return: The text representation of the data.
         """
```

### Comparing `e2b_code_interpreter-0.0.1a2/pyproject.toml` & `e2b_code_interpreter-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "e2b-code-interpreter"
-version = "0.0.1a2"
+version = "0.0.2"
 description = "E2B Code Interpreter - Stateful code execution"
 authors = ["e2b <hello@e2b.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b-code-interpreter/tree/python"
 packages = [{ include = "e2b_code_interpreter" }]
```

### Comparing `e2b_code_interpreter-0.0.1a2/PKG-INFO` & `e2b_code_interpreter-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2b-code-interpreter
-Version: 0.0.1a2
+Version: 0.0.2
 Summary: E2B Code Interpreter - Stateful code execution
 Home-page: https://e2b.dev/
 License: Apache-2.0
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -105,15 +105,15 @@
 data = pd.DataFrame(data=[[1, 2], [3, 4]], columns=["A", "B"])
 display(data.head(10))
 time.sleep(3)
 print("world")
 """
 
 with CodeInterpreter() as sandbox:
-    sandbox.notebook.exec_cell(code, on_stdout=print, on_stderr=print, on_display_data=(lambda data: print(data.text)))
+    sandbox.notebook.exec_cell(code, on_stdout=print, on_stderr=print, on_result=(lambda result: print(result.text)))
 ```
 
 ### Pre-installed Python packages inside the sandbox
 
 The full and always up-to-date list can be found in the [`requirements.txt`](https://github.com/e2b-dev/E2B/blob/stateful-code-interpreter/sandboxes/code-interpreter-stateful/requirements.txt) file.
 
 ```text
```

