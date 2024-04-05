# Comparing `tmp/comfy_script-0.4.2.tar.gz` & `tmp/comfy_script-0.4.3.tar.gz`

## Comparing `comfy_script-0.4.2.tar` & `comfy_script-0.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.4.2/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.4.2/requirements.txt
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.4.2/.vscode/launch.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/README.md
--rw-r--r--   0        0        0    18276 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/Runtime.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/Transpiler.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/Image/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/Latent/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/Models/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/Nodes/README.md
--rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/README/auto-queue.png
--rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/README/diff.png
--rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/README/plot.png
--rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/README/select.png
--rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/README/type-stubs.png
--rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/README/type-stubs2.png
--rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/README/workflow.png
--rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/README/workflow2.png
--rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.4.2/docs/images/Runtime/load-api-format.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/__init__.py
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/astutil.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/client/__init__.py
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/nodes/__init__.py
--rw-r--r--   0        0        0    42093 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/runtime/__init__.py
--rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/runtime/factory.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/runtime/nodes.py
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/runtime/data/Images.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/runtime/data/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/runtime/real/__init__.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/runtime/real/nodes.py
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/transpile/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/transpile/__main__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/transpile/prompt.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/transpile/passes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/ui/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/ui/solara/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.4.2/src/comfy_script/ui/solara/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.4.2/tests/test_astutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.2/tests/transpile/__init__.py
--rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.4.2/tests/transpile/bypass.json
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.4.2/tests/transpile/default.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.4.2/tests/transpile/test_transpiler.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.4.2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 comfy_script-0.4.2/README.md
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 comfy_script-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    16129 2020-02-02 00:00:00.000000 comfy_script-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.4.3/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.4.3/requirements.txt
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.4.3/.vscode/launch.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/README.md
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Runtime.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Transpiler.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Image/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Latent/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Models/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Nodes/README.md
+-rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/auto-queue.png
+-rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/diff.png
+-rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/plot.png
+-rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/select.png
+-rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/type-stubs.png
+-rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/type-stubs2.png
+-rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/workflow.png
+-rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/workflow2.png
+-rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/Runtime/load-api-format.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/__init__.py
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/astutil.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/client/__init__.py
+-rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/nodes/__init__.py
+-rw-r--r--   0        0        0    42190 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/__init__.py
+-rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/factory.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/nodes.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/data/Images.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/data/__init__.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/real/__init__.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/real/nodes.py
+-rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/transpile/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/transpile/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/transpile/prompt.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/transpile/passes/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/ui/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/ui/solara/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/ui/solara/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/test_astutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/transpile/__init__.py
+-rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/transpile/bypass.json
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/transpile/default.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/transpile/test_transpiler.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.4.3/LICENSE.txt
+-rw-r--r--   0        0        0    14265 2020-02-02 00:00:00.000000 comfy_script-0.4.3/README.md
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 comfy_script-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    15825 2020-02-02 00:00:00.000000 comfy_script-0.4.3/PKG-INFO
```

### Comparing `comfy_script-0.4.2/__init__.py` & `comfy_script-0.4.3/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/Runtime.md` & `comfy_script-0.4.3/docs/Runtime.md`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 - Scripts cannot be executed through the API of a ComfyUI server.
 
   However, it is still possible to run scripts on a remote machine without the API. For example, you can launching a [Jupyter Server](https://jupyter-server.readthedocs.io/en/latest/) and [connect to it remotely](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_connect-to-a-remote-jupyter-server).
 
 - As mentioned above, nodes will not cache the output themselves. It is the user's responsibility to avoid re-executing nodes with the same inputs.
 
 - Nodes with unused output 
+- No validation
 
 - The outputs of output nodes (e.g. `SaveImage`) is not converted to result classes (e.g. `ImageBatchResult`).
 
   This may be changed in future versions.
 
 A complete example:
 ```python
```

### Comparing `comfy_script-0.4.2/docs/Image/README.md` & `comfy_script-0.4.3/docs/Image/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/Latent/README.md` & `comfy_script-0.4.3/docs/Latent/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/Nodes/README.md` & `comfy_script-0.4.3/docs/Nodes/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/README/auto-queue.png` & `comfy_script-0.4.3/docs/images/README/auto-queue.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/README/diff.png` & `comfy_script-0.4.3/docs/images/README/diff.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/README/plot.png` & `comfy_script-0.4.3/docs/images/README/plot.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/README/select.png` & `comfy_script-0.4.3/docs/images/README/select.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/README/type-stubs.png` & `comfy_script-0.4.3/docs/images/README/type-stubs.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/README/type-stubs2.png` & `comfy_script-0.4.3/docs/images/README/type-stubs2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/README/workflow.png` & `comfy_script-0.4.3/docs/images/README/workflow.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/README/workflow2.png` & `comfy_script-0.4.3/docs/images/README/workflow2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/docs/images/Runtime/load-api-format.png` & `comfy_script-0.4.3/docs/images/Runtime/load-api-format.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/astutil.py` & `comfy_script-0.4.3/src/comfy_script/astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/client/__init__.py` & `comfy_script-0.4.3/src/comfy_script/client/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/nodes/__init__.py` & `comfy_script-0.4.3/src/comfy_script/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/runtime/__init__.py` & `comfy_script-0.4.3/src/comfy_script/runtime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     - `comfyui`: A URL of the ComfyUI server API, or a path to the ComfyUI directory, or `'comfyui'` to use the [`comfyui` package](https://github.com/comfyanonymous/ComfyUI/pull/298).
 
       If not specified, the following ones will be tried in order:
       1. Local server API: http://127.0.0.1:8188/
       2. Parent ComfyUI directory: The default path is `ComfyScript/../..`, which only works if ComfyScript is installed at `ComfyUI/custom_nodes/ComfyScript`.
       3. `comfyui` package
     
-    - `comfyui_args`: CLI arguments to be passed to ComfyUI, if the value of `comfyui` is not an API. See `ComfyUIArgs` for details.
+    - `args`: CLI arguments to be passed to ComfyUI, if the value of `comfyui` is not an API. See `ComfyUIArgs` for details.
     '''
     asyncio.run(_load(comfyui, args, vars, watch, save_script_source))
 
 async def _load(comfyui: str | Path = None, args: ComfyUIArgs | None = None, vars: dict | None = None, watch: bool = True, save_script_source: bool = True):
     global _save_script_source, queue
 
     _save_script_source = save_script_source
@@ -718,14 +718,16 @@
                     display(clear=True)
                 if image_batches:
                     await Images(*image_batches)._display()
                 if others:
                     display(*others)
     
     async def _wait(self) -> list[data.Result]:
+        '''`Task` can be directly awaited like `await task`. This method is for internal use only.'''
+
         outputs: dict = await self._fut
         return [data.Result.from_output(output) for output in outputs.values()]
     
     def __await__(self) -> list[data.Result]:
         return self._wait().__await__()
 
     def wait(self) -> list[data.Result]:
```

### Comparing `comfy_script-0.4.2/src/comfy_script/runtime/factory.py` & `comfy_script-0.4.3/src/comfy_script/runtime/factory.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/runtime/nodes.py` & `comfy_script-0.4.3/src/comfy_script/runtime/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/runtime/data/Images.py` & `comfy_script-0.4.3/src/comfy_script/runtime/data/Images.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,17 @@
                     return
     
     def __await__(self) -> list[Image.Image | None]:
         async def f(self):
             return [await self._get_image(image) for image in self._output['images']]
         return f(self).__await__()
     
+    def wait(self) -> list[Image.Image | None]:
+        return asyncio.run(self)
+    
     async def get(self, i: int) -> Image.Image | None:
         return await self._get_image(self._output['images'][i])
     
     def __getitem__(self, i: int) -> Image.Image | None:
         return asyncio.run(self.get(i))
     
     def display(self, rows: int | None = 1, cols: int | None = None, height: int | None = None, width: int | None = None, **kwds):
```

### Comparing `comfy_script-0.4.2/src/comfy_script/runtime/data/__init__.py` & `comfy_script-0.4.3/src/comfy_script/runtime/data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,16 @@
         prompt[new_id] = {
             'inputs': prompt_inputs,
             'class_type': self.node_prompt['class_type'],
         }
         return new_id
 
     async def _wait(self, source = None) -> Result | None:
+        '''`NodeOutput` can be directly awaited like `await node_output`. This method should only be used if one need to specify `source`.'''
+
         if self.task is None:
             from ...runtime import queue
             self.task = await queue._put(self, source)
         return await self.task.result(self)
     
     def __await__(self) -> Result | None:
         outer = inspect.currentframe().f_back
@@ -131,14 +133,15 @@
     def __str__(self) -> str:
         return f'{self.__class__.__name__}({self._output.__str__()})'
 
     @classmethod
     def from_output(cls, output: dict) -> Result:
         if 'images' in output:
             return ImageBatchResult(output)
+        return Result(output)
 
 from .Images import ImageBatchResult, Images
 
 __all__ = [
     'NodeOutput',
     'Result',
     'ImageBatchResult',
```

### Comparing `comfy_script-0.4.2/src/comfy_script/runtime/real/__init__.py` & `comfy_script-0.4.3/src/comfy_script/runtime/real/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/runtime/real/nodes.py` & `comfy_script-0.4.3/src/comfy_script/runtime/real/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,16 +95,19 @@
                         kwds = { k: v for k, v in defaults.items() if k not in pos_kwds } | kwds
                 
                 # TODO: Bool enum, path
                 
                 if config.track_workflow:
                     virtual_kwds = {}
                     for k, v in kwds.items():
-                        virtual_v = getattr(v, '_self_virtual_output', None)
-                        virtual_kwds[k] = virtual_v if virtual_v is not None else v
+                        if isinstance(v, RealNodeOutputWrapper):
+                            virtual_kwds[k] = v._self_virtual_output
+                            kwds[k] = v.__wrapped__
+                        else:
+                            virtual_kwds[k] = v
                     
                     virtual_outputs = None
                     try:
                         virtual_outputs = virtual_node(**virtual_kwds)
                     except Exception as e:
                         print(f'ComfyScript: track_workflow: Failed to call {info["name"]}: {e}')
```

### Comparing `comfy_script-0.4.2/src/comfy_script/transpile/__init__.py` & `comfy_script-0.4.3/src/comfy_script/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/transpile/prompt.py` & `comfy_script-0.4.3/src/comfy_script/transpile/prompt.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/transpile/passes/__init__.py` & `comfy_script-0.4.3/src/comfy_script/transpile/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/src/comfy_script/ui/solara/metadata.py` & `comfy_script-0.4.3/src/comfy_script/ui/solara/metadata.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/tests/test_astutil.py` & `comfy_script-0.4.3/tests/test_astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/tests/transpile/bypass.json` & `comfy_script-0.4.3/tests/transpile/bypass.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/tests/transpile/default.json` & `comfy_script-0.4.3/tests/transpile/default.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/tests/transpile/test_transpiler.py` & `comfy_script-0.4.3/tests/transpile/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/.gitignore` & `comfy_script-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/LICENSE.txt` & `comfy_script-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.2/README.md` & `comfy_script-0.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,16 @@
 - Retrieving any wanted information by running the script with some stubs.
 
   See [workflow information retrieval](docs/README.md#workflow-information-retrieval) for details.
 
 - Converting workflows from ComfyUI's web UI format to API format without the web UI.
 
 ## Installation
-ComfyScript can be installed in different ways.
-
-### Package and nodes with ComfyUI
-Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI) first. And then:
+### With ComfyUI
+Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI#installing) first. And then run the following commands:
 ```sh
 cd ComfyUI/custom_nodes
 git clone https://github.com/Chaoses-Ib/ComfyScript.git
 cd ComfyScript
 python -m pip install -e ".[default]"
 ```
 (If you see `ERROR: File "setup.py" or "setup.cfg" not found`, run `python -m pip install -U pip` first.)
@@ -52,61 +50,37 @@
 Update:
 ```sh
 cd ComfyUI/custom_nodes/ComfyScript
 git pull
 python -m pip install -e ".[default]"
 ```
 
-### Package and nodes with ComfyUI package
-Install [ComfyUI package](https://github.com/comfyanonymous/ComfyUI/pull/298) first:
-```sh
-python -m pip install git+https://github.com/hiddenswitch/ComfyUI.git
-```
+### With ComfyUI package
+Install [ComfyUI package](https://github.com/hiddenswitch/ComfyUI) first:
+- If PyTorch is not installed:
+
+  ```sh
+  python -m pip install git+https://github.com/hiddenswitch/ComfyUI.git
+  ```
+- If PyTorch is already installed (e.g. Google Colab):
+
+  ```sh
+  python -m pip install wheel
+  python -m pip install --no-build-isolation git+https://github.com/hiddenswitch/ComfyUI.git
+  ```
 
 Install/update ComfyScript:
 ```sh
 python -m pip install -U "comfy-script[default]"
 ```
 
 (`[default]` is necessary to install common dependencies. See [`pyproject.toml`](pyproject.toml) for other options. If no option is specified, `comfy-script` will be installed without any dependencies.)
 
-### Only package
-Install/update:
-```sh
-python -m pip install -U "comfy-script[default]"
-```
-
-### Only nodes with ComfyUI
-<details>
-
-Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI) first. And then:
-```sh
-cd ComfyUI/custom_nodes
-git clone https://github.com/Chaoses-Ib/ComfyScript.git
-cd ComfyScript
-python -m pip install -r requirements.txt
-```
-
-Update:
-```sh
-cd ComfyUI/custom_nodes/ComfyScript
-git pull
-python -m pip install -r requirements.txt
-```
-
-If you want, you can still import the package with a hardcoded path:
-```python
-import sys
-# Or just '../src' if used in the examples directory
-sys.path.insert(0, r'D:\...\ComfyUI\custom_nodes\ComfyScript\src')
-
-import comfy_script
-```
-
-</details>
+### Other ways
+ComfyScript can also be used without installed ComfyUI. See [only ComfyScript package](docs/README.md#only-comfyscript-package) for details. And see [uninstallation](docs/README.md#uninstallation) for how to uninstall.
 
 ## Transpiler
 The transpiler can translate ComfyUI's workflows to ComfyScript.
 
 When ComfyScript is installed as custom nodes, `SaveImage` and similar nodes will be hooked to automatically save the script as images' metadata. And the script will also be output to the terminal.
 
 For example, here is a workflow in ComfyUI:
```

### Comparing `comfy_script-0.4.2/pyproject.toml` & `comfy_script-0.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comfy-script"
-version = "0.4.2"
+version = "0.4.3"
 description = "A Python front end and library for ComfyUI"
 readme = "README.md"
 # ComfyUI: >=3.8
 # comfyui: >=3.9
 # >=3.6 is required to preserve insertion order of input types
 requires-python = ">=3.9"
 authors = [
@@ -47,15 +47,15 @@
 
   # Used to save script to images
   "comfy-script[transpile]",
 ]
 
 # Addtional nodes
 nodes = [
-  "ComfyUI_Ib_CustomNodes >= 0.2.1",
+  "ComfyUI_Ib_CustomNodes >= 0.2.2",
   "comfyui-tooling-nodes",
 ]
 
 # Everything except UI (Jupyter and CLI)
 no-ui = [
   "comfy-script[client]",
   "comfy-script[transpile]",
```

### Comparing `comfy_script-0.4.2/PKG-INFO` & `comfy_script-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-script
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python front end and library for ComfyUI
 Project-URL: Homepage, https://github.com/Chaoses-Ib/ComfyScript
 Project-URL: Issues, https://github.com/Chaoses-Ib/ComfyScript/issues
 Author-email: Chaoses-Ib <Chaos-es@outlook.com>
 License-File: LICENSE.txt
 Keywords: comfyui
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: pillow; extra == 'jupyter'
 Provides-Extra: no-ui
 Requires-Dist: comfy-script[client]; extra == 'no-ui'
 Requires-Dist: comfy-script[nodes]; extra == 'no-ui'
 Requires-Dist: comfy-script[runtime]; extra == 'no-ui'
 Requires-Dist: comfy-script[transpile]; extra == 'no-ui'
 Provides-Extra: nodes
-Requires-Dist: comfyui-ib-customnodes>=0.2.1; extra == 'nodes'
+Requires-Dist: comfyui-ib-customnodes>=0.2.2; extra == 'nodes'
 Requires-Dist: comfyui-tooling-nodes; extra == 'nodes'
 Provides-Extra: runtime
 Requires-Dist: comfy-script[client]; extra == 'runtime'
 Requires-Dist: comfy-script[transpile]; extra == 'runtime'
 Requires-Dist: pillow; extra == 'runtime'
 Requires-Dist: wrapt~=1.0; extra == 'runtime'
 Provides-Extra: transpile
@@ -78,18 +78,16 @@
 - Retrieving any wanted information by running the script with some stubs.
 
   See [workflow information retrieval](docs/README.md#workflow-information-retrieval) for details.
 
 - Converting workflows from ComfyUI's web UI format to API format without the web UI.
 
 ## Installation
-ComfyScript can be installed in different ways.
-
-### Package and nodes with ComfyUI
-Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI) first. And then:
+### With ComfyUI
+Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI#installing) first. And then run the following commands:
 ```sh
 cd ComfyUI/custom_nodes
 git clone https://github.com/Chaoses-Ib/ComfyScript.git
 cd ComfyScript
 python -m pip install -e ".[default]"
 ```
 (If you see `ERROR: File "setup.py" or "setup.cfg" not found`, run `python -m pip install -U pip` first.)
@@ -97,61 +95,37 @@
 Update:
 ```sh
 cd ComfyUI/custom_nodes/ComfyScript
 git pull
 python -m pip install -e ".[default]"
 ```
 
-### Package and nodes with ComfyUI package
-Install [ComfyUI package](https://github.com/comfyanonymous/ComfyUI/pull/298) first:
-```sh
-python -m pip install git+https://github.com/hiddenswitch/ComfyUI.git
-```
+### With ComfyUI package
+Install [ComfyUI package](https://github.com/hiddenswitch/ComfyUI) first:
+- If PyTorch is not installed:
+
+  ```sh
+  python -m pip install git+https://github.com/hiddenswitch/ComfyUI.git
+  ```
+- If PyTorch is already installed (e.g. Google Colab):
+
+  ```sh
+  python -m pip install wheel
+  python -m pip install --no-build-isolation git+https://github.com/hiddenswitch/ComfyUI.git
+  ```
 
 Install/update ComfyScript:
 ```sh
 python -m pip install -U "comfy-script[default]"
 ```
 
 (`[default]` is necessary to install common dependencies. See [`pyproject.toml`](pyproject.toml) for other options. If no option is specified, `comfy-script` will be installed without any dependencies.)
 
-### Only package
-Install/update:
-```sh
-python -m pip install -U "comfy-script[default]"
-```
-
-### Only nodes with ComfyUI
-<details>
-
-Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI) first. And then:
-```sh
-cd ComfyUI/custom_nodes
-git clone https://github.com/Chaoses-Ib/ComfyScript.git
-cd ComfyScript
-python -m pip install -r requirements.txt
-```
-
-Update:
-```sh
-cd ComfyUI/custom_nodes/ComfyScript
-git pull
-python -m pip install -r requirements.txt
-```
-
-If you want, you can still import the package with a hardcoded path:
-```python
-import sys
-# Or just '../src' if used in the examples directory
-sys.path.insert(0, r'D:\...\ComfyUI\custom_nodes\ComfyScript\src')
-
-import comfy_script
-```
-
-</details>
+### Other ways
+ComfyScript can also be used without installed ComfyUI. See [only ComfyScript package](docs/README.md#only-comfyscript-package) for details. And see [uninstallation](docs/README.md#uninstallation) for how to uninstall.
 
 ## Transpiler
 The transpiler can translate ComfyUI's workflows to ComfyScript.
 
 When ComfyScript is installed as custom nodes, `SaveImage` and similar nodes will be hooked to automatically save the script as images' metadata. And the script will also be output to the terminal.
 
 For example, here is a workflow in ComfyUI:
```

