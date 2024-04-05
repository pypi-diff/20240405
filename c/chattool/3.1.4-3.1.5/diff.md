# Comparing `tmp/chattool-3.1.4.tar.gz` & `tmp/chattool-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattool-3.1.4.tar", last modified: Thu Apr  4 13:18:50 2024, max compression
+gzip compressed data, was "chattool-3.1.5.tar", last modified: Fri Apr  5 16:35:38 2024, max compression
```

## Comparing `chattool-3.1.4.tar` & `chattool-3.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:18:50.091374 chattool-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 13:18:37.000000 chattool-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-04 13:18:50.091374 chattool-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-04 13:18:37.000000 chattool-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:18:50.091374 chattool-3.1.4/chattool/
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/asynctool.py
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/chattype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/functioncall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/tokencalc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:18:50.091374 chattool-3.1.4/chattool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-04 13:18:50.000000 chattool-3.1.4/chattool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:18:50.091374 chattool-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 13:18:37.000000 chattool-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:35:38.230668 chattool-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 16:35:27.000000 chattool-3.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-05 16:35:38.230668 chattool-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-05 16:35:27.000000 chattool-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:35:38.230668 chattool-3.1.5/chattool/
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/asynctool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20497 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/chattype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/functioncall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-05 16:35:27.000000 chattool-3.1.5/chattool/tokencalc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:35:38.230668 chattool-3.1.5/chattool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 16:35:38.000000 chattool-3.1.5/chattool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:35:38.230668 chattool-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-05 16:35:27.000000 chattool-3.1.5/setup.py
```

### Comparing `chattool-3.1.4/LICENSE` & `chattool-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/PKG-INFO` & `chattool-3.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattool
-Version: 3.1.4
+Version: 3.1.5
 Summary: Toolkit for Chat API
 Home-page: https://github.com/cubenlp/chattool
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: <div align="center">
             <a href="https://pypi.python.org/pypi/chattool">
@@ -75,28 +75,26 @@
         chat.print_log()
         ```
         
         示例2，批量处理数据（串行），并使用缓存文件 `checkpoint`：
         
         ```python
         # 编写处理函数
-        def msg2chat(msg):
+        def data2chat(msg):
             chat = Chat()
             chat.system("你是一个熟练的数字翻译家。")
             chat.user(f"请将该数字翻译为罗马数字：{msg}")
             # 注意，在函数内获取返回
             chat.getresponse()
             return chat
         
         checkpoint = "chat.jsonl" # 缓存文件的名称
         msgs = ["1", "2", "3", "4", "5", "6", "7", "8", "9"]
-        # 处理部分数据
-        chats = process_chats(msgs[:5], msg2chat, checkpoint)
-        # 处理所有数据，从上一次处理的位置继续
-        continue_chats = process_chats(msgs, msg2chat, checkpoint)
+        # 处理数据，如果 checkpoint 存在，则从上次中断处继续
+        continue_chats = process_chats(msgs, data2chat, checkpoint)
         ```
         
         示例3，批量处理数据（异步并行），用不同语言打印 hello，并使用两个协程：
         
         ```python
         from chattool import async_chat_completion, load_chats, Chat
         
@@ -107,14 +105,20 @@
             # 注意，这里不需要 getresponse 而交给异步处理
             return chat
         
         async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat)
         chats = load_chats("async_chat.jsonl")
         ```
         
+        在 Jupyter Notebook 中运行，需要使用 `await` 关键字和 `wait=True` 参数：
+        
+        ```python
+        await async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat, wait=True)
+        ```
+        
         示例4，使用工具（自定义函数）：
         
         ```python
         # 定义函数
         def add(a: int, b: int) -> int:
             """
             This function adds two numbers.
```

### Comparing `chattool-3.1.4/README.md` & `chattool-3.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -67,28 +67,26 @@
 chat.print_log()
 ```
 
 示例2，批量处理数据（串行），并使用缓存文件 `checkpoint`：
 
 ```python
 # 编写处理函数
-def msg2chat(msg):
+def data2chat(msg):
     chat = Chat()
     chat.system("你是一个熟练的数字翻译家。")
     chat.user(f"请将该数字翻译为罗马数字：{msg}")
     # 注意，在函数内获取返回
     chat.getresponse()
     return chat
 
 checkpoint = "chat.jsonl" # 缓存文件的名称
 msgs = ["1", "2", "3", "4", "5", "6", "7", "8", "9"]
-# 处理部分数据
-chats = process_chats(msgs[:5], msg2chat, checkpoint)
-# 处理所有数据，从上一次处理的位置继续
-continue_chats = process_chats(msgs, msg2chat, checkpoint)
+# 处理数据，如果 checkpoint 存在，则从上次中断处继续
+continue_chats = process_chats(msgs, data2chat, checkpoint)
 ```
 
 示例3，批量处理数据（异步并行），用不同语言打印 hello，并使用两个协程：
 
 ```python
 from chattool import async_chat_completion, load_chats, Chat
 
@@ -99,14 +97,20 @@
     # 注意，这里不需要 getresponse 而交给异步处理
     return chat
 
 async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat)
 chats = load_chats("async_chat.jsonl")
 ```
 
+在 Jupyter Notebook 中运行，需要使用 `await` 关键字和 `wait=True` 参数：
+
+```python
+await async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat, wait=True)
+```
+
 示例4，使用工具（自定义函数）：
 
 ```python
 # 定义函数
 def add(a: int, b: int) -> int:
     """
     This function adds two numbers.
```

### Comparing `chattool-3.1.4/chattool/__init__.py` & `chattool-3.1.5/chattool/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,67 @@
 """Top-level package for Chattool."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '3.1.4'
+__version__ = '3.1.5'
 
 import os, sys, requests
 from .chattype import Chat, Resp
 from .checkpoint import load_chats, process_chats
 from .proxy import proxy_on, proxy_off, proxy_status
 from . import request
 from .tokencalc import model_cost_perktoken, findcost
 from .asynctool import async_chat_completion
 from .functioncall import generate_json_schema, exec_python_code
 from typing import Union
-import dotenv
+import dotenv 
+
+raw_env_text = f"""# Description: Env file for ChatTool.
+# Current version: {__version__}
+
+# The base url of the API (with suffix /v1)
+# This will override OPENAI_API_BASE_URL if both are set.
+OPENAI_API_BASE=''
+
+# The base url of the API (without suffix /v1)
+OPENAI_API_BASE_URL=''
+
+# Your API key
+OPENAI_API_KEY=''
+
+# The default model name
+OPENAI_API_MODEL=''
+"""
 
 def load_envs(env:Union[None, str, dict]=None):
     """Read the environment variables for the API call"""
     global api_key, base_url, api_base, model
     # update the environment variables
     if isinstance(env, str):
         dotenv.load_dotenv(env, override=True)
     elif isinstance(env, dict):
         for key, value in env.items():
             os.environ[key] = value
     # else: load from environment variables
     api_key = os.getenv('OPENAI_API_KEY')
-    base_url = os.getenv('OPENAI_API_BASE_URL') or "https://api.openai.com"
-    api_base = os.getenv('OPENAI_API_BASE') or os.path.join(base_url, 'v1')
-    base_url = request.normalize_url(base_url)
-    api_base = request.normalize_url(api_base)
-    model = os.getenv('OPENAI_API_MODEL') or "gpt-3.5-turbo"
+    base_url = os.getenv('OPENAI_API_BASE_URL') # or "https://api.openai.com"
+    api_base = os.getenv('OPENAI_API_BASE') # or os.path.join(base_url, 'v1')
+    model = os.getenv('OPENAI_API_MODEL') # or "gpt-3.5-turbo"
     return True
 
 def save_envs(env_file:str):
     """Save the environment variables for the API call"""
-    global api_key, base_url, model
+    global api_key, base_url, model, api_base
+    set_key = lambda key, value: dotenv.set_key(env_file, key, value) if value else None
     with open(env_file, "w") as f:
-        f.write(f"OPENAI_API_KEY={api_key}\n")
-        f.write(f"OPENAI_API_BASE_URL={base_url}\n")
-        f.write(f"OPENAI_API_BASE={api_base}\n")
-        f.write(f"OPENAI_API_MODEL={model}\n")
+        f.write(raw_env_text)
+    set_key('OPENAI_API_KEY', api_key)
+    set_key('OPENAI_API_BASE_URL', base_url)
+    set_key('OPENAI_API_BASE', api_base)
+    set_key('OPENAI_API_MODEL', model)
     return True
 
 # load the environment variables
 load_envs()
 
 # get the platform
 platform = sys.platform
@@ -96,22 +113,22 @@
     try:
         requests.get(net_url, timeout=timeout)
     except:
         print("Warning: Network is not available.")
         return False
     
     ## Check the proxy status
-    print("\nCheck your proxy:" +\
+    print("\nCheck your proxy: " +\
           "This is not necessary if the base url is already a proxy link.")
     proxy_status()
 
     ## Base url
     print("\nCheck the value OPENAI_API_BASE_URL:")
     print(base_url)
-    print("\nCheck the value OPENAI_API_BASE:" +\
+    print("\nCheck the value OPENAI_API_BASE: " +\
           "This will override OPENAI_API_BASE_URL if both are set.")
     print(api_base)
 
     ## Model
     print("\nYour default OPENAI_API_MODEL:")
     print(model)
```

### Comparing `chattool-3.1.4/chattool/asynctool.py` & `chattool-3.1.5/chattool/asynctool.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/chattool/chattype.py` & `chattool-3.1.5/chattool/chattype.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import os
 from .functioncall import generate_json_schema, delete_dialogue_assist
 
 class Chat():
     def __init__( self
                 , msg:Union[List[Dict], None, str]=None
                 , api_key:Union[None, str]=None
-                , chat_url:Union[None, str]=None
-                , base_url:Union[None, str]=None
                 , api_base:Union[None, str]=None
+                , base_url:Union[None, str]=None
+                , chat_url:Union[None, str]=None
                 , model:Union[None, str]=None
                 , functions:Union[None, List[Dict]]=None
                 , function_call:Union[None, str]=None
                 , name2func:Union[None, Dict]=None):
         """Initialize the chat log
 
         Args:
             msg (Union[List[Dict], None, str], optional): chat log. Defaults to None.
             api_key (Union[None, str], optional): API key. Defaults to None.
-            chat_url (Union[None, str], optional): base url. Defaults to None. Example: "https://api.openai.com/v1/chat/completions"
-            base_url (Union[None, str], optional): base url. Defaults to None. Example: "https://api.openai.com"
+            api_base (Union[None, str], optional): base url with suffix "/v1". Defaults to None. Example: "https://api.openai.com/v1"
+            base_url (Union[None, str], optional): base url without suffix "/v1". Defaults to None. Example: "https://api.openai.com"
+            chat_url (Union[None, str], optional): chat completion url. Defaults to None. Example: "https://api.openai.com/v1/chat/completions"
             model (Union[None, str], optional): model to use. Defaults to None.
             functions (Union[None, List[Dict]], optional): functions to use, each function is a JSON Schema. Defaults to None.
             function_call (str, optional): method to call the function. Defaults to None. Choices: ['auto', '$NameOfTheFunction', 'none']
             name2func (Union[None, Dict], optional): name to function mapping. Defaults to None.
         
         Raises:
             ValueError: msg should be a list of dict, a string or None
@@ -41,23 +42,31 @@
         elif isinstance(msg, str):
             self._chat_log = chattool.default_prompt(msg)
         elif isinstance(msg, list):
             assert all(isinstance(m, dict) for m in msg), "msg should be a list of dict"
             self._chat_log = msg.copy() # avoid changing the original list
         else:
             raise ValueError("msg should be a list of dict, a string or None")
-        self._api_key = api_key or chattool.api_key
-        # try: api_base => base_url => chattool.api_base => chattool.base_url
-        if api_base is None:
-            api_base = os.path.join(base_url, 'v1') if base_url is not None else chattool.api_base
-        base_url = base_url or chattool.base_url
-        self._base_url = base_url
-        self._api_base = api_base or os.path.join(base_url, "v1")
-        self._chat_url = chat_url or self._api_base.rstrip('/') + '/chat/completions'
-        self._model = model or chattool.model
+        self.api_key = api_key or chattool.api_key
+        # chat_url > api_base > base_url > chattool.api_base > chattool.base_url
+        self.api_base = api_base or chattool.api_base
+        self.base_url = base_url or chattool.base_url
+        self.model = model or chattool.model or "gpt-3.5-turbo"
+        if chat_url:
+            self.chat_url = chat_url
+        elif api_base:
+            self.chat_url = os.path.join(self.api_base, "chat/completions")
+        elif base_url:
+            self.chat_url = os.path.join(self.base_url, "v1/chat/completions")
+        elif chattool.api_base:
+            self.chat_url = os.path.join(chattool.api_base, "chat/completions")
+        elif chattool.base_url:
+            self.chat_url = os.path.join(chattool.base_url, "v1/chat/completions")
+        else:
+            self.chat_url = "https://api.openai.com/v1/chat/completions"
         if functions is not None:
             assert isinstance(functions, list), "functions should be a list of dict"
         self._functions, self._function_call = functions, function_call
         self._name2func, self._resp = name2func, None
     
     # Part1: basic operation of the chat object
     def add(self, role:str, **kwargs):
@@ -100,14 +109,15 @@
         return Chat( self._chat_log
                    , api_key=self.api_key
                    , chat_url=self.chat_url
                    , model=self.model
                    , functions=self.functions
                    , function_call=self.function_call
                    , name2func=self.name2func
+                   , api_base=self.api_base
                    , base_url=self.base_url)
 
     def save(self, path:str, mode:str='a', index:int=0):
         """
         Save the chat log to a file. Each line is a json string.
 
         Args:
@@ -329,15 +339,19 @@
 
         Args:
             gpt_only (bool, optional): whether to only show the GPT models. Defaults to True.
 
         Returns:
             List[str]: valid models
         """
-        model_url = os.path.join(self.api_base, 'models')
+        model_url = "https://api.openai.com/v1/models"
+        if self.api_base:
+            model_url = os.path.join(self.api_base, 'models')
+        elif self.base_url:
+            model_url = os.path.join(self.base_url, 'v1/models')
         return valid_models(self.api_key, model_url, gpt_only=gpt_only)
     
     # Part5: properties and setters
     @property
     def last_message(self):
         """Get the last message"""
         return self._chat_log[-1]['content']
@@ -403,21 +417,25 @@
     
     @chat_url.setter
     def chat_url(self, chat_url:str):
         """Set base url"""
         self._chat_url = chat_url
 
     @base_url.setter
-    def base_url(self, base_url:str):
+    def base_url(self, base_url:Union[None, str]):
         """Set base url"""
+        if base_url:
+            self.chat_url = base_url.rstrip('/') + '/v1/chat/completions'
         self._base_url = base_url
     
     @api_base.setter
-    def api_base(self, api_base:str):
+    def api_base(self, api_base:Union[None, str]):
         """Set base url"""
+        if api_base:
+            self.chat_url = api_base.rstrip('/') + '/chat/completions'
         self._api_base = api_base
 
     @functions.setter
     def functions(self, functions:List[Dict]):
         """Set functions"""
         assert isinstance(functions, list), "functions should be a list of dict"
         self._functions = functions
```

### Comparing `chattool-3.1.4/chattool/checkpoint.py` & `chattool-3.1.5/chattool/checkpoint.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/chattool/finetune.py` & `chattool-3.1.5/chattool/finetune.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/chattool/functioncall.py` & `chattool-3.1.5/chattool/functioncall.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/chattool/proxy.py` & `chattool-3.1.5/chattool/proxy.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/chattool/request.py` & `chattool-3.1.5/chattool/request.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/chattool/response.py` & `chattool-3.1.5/chattool/response.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/chattool/tokencalc.py` & `chattool-3.1.5/chattool/tokencalc.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.4/chattool.egg-info/PKG-INFO` & `chattool-3.1.5/chattool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattool
-Version: 3.1.4
+Version: 3.1.5
 Summary: Toolkit for Chat API
 Home-page: https://github.com/cubenlp/chattool
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: <div align="center">
             <a href="https://pypi.python.org/pypi/chattool">
@@ -75,28 +75,26 @@
         chat.print_log()
         ```
         
         示例2，批量处理数据（串行），并使用缓存文件 `checkpoint`：
         
         ```python
         # 编写处理函数
-        def msg2chat(msg):
+        def data2chat(msg):
             chat = Chat()
             chat.system("你是一个熟练的数字翻译家。")
             chat.user(f"请将该数字翻译为罗马数字：{msg}")
             # 注意，在函数内获取返回
             chat.getresponse()
             return chat
         
         checkpoint = "chat.jsonl" # 缓存文件的名称
         msgs = ["1", "2", "3", "4", "5", "6", "7", "8", "9"]
-        # 处理部分数据
-        chats = process_chats(msgs[:5], msg2chat, checkpoint)
-        # 处理所有数据，从上一次处理的位置继续
-        continue_chats = process_chats(msgs, msg2chat, checkpoint)
+        # 处理数据，如果 checkpoint 存在，则从上次中断处继续
+        continue_chats = process_chats(msgs, data2chat, checkpoint)
         ```
         
         示例3，批量处理数据（异步并行），用不同语言打印 hello，并使用两个协程：
         
         ```python
         from chattool import async_chat_completion, load_chats, Chat
         
@@ -107,14 +105,20 @@
             # 注意，这里不需要 getresponse 而交给异步处理
             return chat
         
         async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat)
         chats = load_chats("async_chat.jsonl")
         ```
         
+        在 Jupyter Notebook 中运行，需要使用 `await` 关键字和 `wait=True` 参数：
+        
+        ```python
+        await async_chat_completion(langs, chkpoint="async_chat.jsonl", nproc=2, data2chat=data2chat, wait=True)
+        ```
+        
         示例4，使用工具（自定义函数）：
         
         ```python
         # 定义函数
         def add(a: int, b: int) -> int:
             """
             This function adds two numbers.
```

### Comparing `chattool-3.1.4/setup.py` & `chattool-3.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '3.1.4'
+VERSION = '3.1.5'
 
 requirements = [
     'Click>=7.0', 'requests>=2.20', "responses>=0.23", 'aiohttp>=3.8',
     'tqdm>=4.60', 'docstring_parser>=0.10', "python-dotenv>=0.17.0"]
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
```

