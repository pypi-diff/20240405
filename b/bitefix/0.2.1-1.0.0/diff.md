# Comparing `tmp/bitefix-0.2.1.tar.gz` & `tmp/bitefix-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitefix-0.2.1.tar", last modified: Thu Apr  4 05:47:35 2024, max compression
+gzip compressed data, was "bitefix-1.0.0.tar", last modified: Fri Apr  5 05:15:04 2024, max compression
```

## Comparing `bitefix-0.2.1.tar` & `bitefix-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:34.996323 bitefix-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 05:46:36.000000 bitefix-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-04 05:47:34.996323 bitefix-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-04 05:46:36.000000 bitefix-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:34.996323 bitefix-0.2.1/bitefix/
--rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-04-04 05:47:31.000000 bitefix-0.2.1/bitefix/BiteFixAIAgents.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-04 05:47:31.000000 bitefix-0.2.1/bitefix/BiteFixAICrew.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-04 05:47:31.000000 bitefix-0.2.1/bitefix/BiteFixAIRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-04 05:47:31.000000 bitefix-0.2.1/bitefix/BiteFixAITasks.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 05:46:36.000000 bitefix-0.2.1/bitefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-04 05:46:36.000000 bitefix-0.2.1/bitefix/bitefix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:34.996323 bitefix-0.2.1/bitefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 05:47:34.000000 bitefix-0.2.1/bitefix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 05:47:34.996323 bitefix-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-04 05:46:36.000000 bitefix-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:15:04.133184 bitefix-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 05:13:57.000000 bitefix-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-05 05:15:04.133184 bitefix-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-05 05:13:57.000000 bitefix-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:15:04.133184 bitefix-1.0.0/bitefix/
+-rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-04-05 05:15:00.000000 bitefix-1.0.0/bitefix/BiteFixAIAgents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 05:15:00.000000 bitefix-1.0.0/bitefix/BiteFixAICrew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-05 05:15:00.000000 bitefix-1.0.0/bitefix/BiteFixAIRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-05 05:15:00.000000 bitefix-1.0.0/bitefix/BiteFixAITasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 05:13:57.000000 bitefix-1.0.0/bitefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-05 05:13:57.000000 bitefix-1.0.0/bitefix/bitefix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:15:04.133184 bitefix-1.0.0/bitefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-05 05:15:04.000000 bitefix-1.0.0/bitefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-05 05:15:04.000000 bitefix-1.0.0/bitefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 05:15:04.000000 bitefix-1.0.0/bitefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 05:15:04.000000 bitefix-1.0.0/bitefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 05:15:04.000000 bitefix-1.0.0/bitefix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-05 05:15:04.133184 bitefix-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-05 05:13:57.000000 bitefix-1.0.0/setup.py
```

### Comparing `bitefix-0.2.1/LICENSE` & `bitefix-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.1/PKG-INFO` & `bitefix-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bitefix
-Version: 0.2.1
+Version: 1.0.0
 Summary: Bitefix is an efficient library designed to streamline Python Runtime error debugging with AI-powered decorators. 
 Home-page: https://github.com/Pallavi-Sinha-12/bitefix
 Author: Pallavi Sinha
 Author-email: dataaienthusiast128@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: crewai==0.14.4
 Requires-Dist: langchain==0.1.9
 Requires-Dist: crewai-tools==0.0.12
 
 # BiteFix 🛠️
@@ -143,15 +143,15 @@
 ```python
 
 from bitefix import resolve
 from langchain_community.llms import Ollama
 
 llm = Ollama("openhermes")
 
-@resolve_with_openai(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
+@resolve(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
 def max_profit(stock_prices):
 
     min_price = stock_prices[0]
     max_profit = 0 
 
     for price in stock_prices[1:]:
         min_price = min(min_price, price)
```

### Comparing `bitefix-0.2.1/README.md` & `bitefix-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 ```python
 
 from bitefix import resolve
 from langchain_community.llms import Ollama
 
 llm = Ollama("openhermes")
 
-@resolve_with_openai(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
+@resolve(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
 def max_profit(stock_prices):
 
     min_price = stock_prices[0]
     max_profit = 0 
 
     for price in stock_prices[1:]:
         min_price = min(min_price, price)
```

### Comparing `bitefix-0.2.1/bitefix/BiteFixAIAgents.py` & `bitefix-1.0.0/bitefix/BiteFixAIAgents.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.1/bitefix/BiteFixAICrew.py` & `bitefix-1.0.0/bitefix/BiteFixAICrew.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.1/bitefix/BiteFixAIRunner.py` & `bitefix-1.0.0/bitefix/BiteFixAIRunner.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.1/bitefix/BiteFixAITasks.py` & `bitefix-1.0.0/bitefix/BiteFixAITasks.py`

 * *Files identical despite different names*

### Comparing `bitefix-0.2.1/bitefix/bitefix_utils.py` & `bitefix-1.0.0/bitefix/bitefix_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 def resolve(
     llm: object,
     function_description: str = None,
     export_dir: str = None,
     verbose: bool = True,
 ) -> Callable:
     """
-    Bite Fix AI Decorator that provides error resolution on Runtime Errors using BiteFiix AI Agents and the provided Large Language Model.
+    Bite Fix AI Decorator that provides error resolution on Runtime Errors using BiteFiix AI Agents and the provided LLM.
 
     Args:
         llm (object): The language model object to use for error resolution.
         export_dir (str, optional): The directory to export Error Resoltion Report by BiteFix AI Agents and fixed code python file. Defaults to None.
         function_description (str, optional): Recommended to provide a description of the function to be resolved. Word limit: 20-50 words. Defaults to None.
         verbose (bool, optional): Whether to print the output of the BiteFix AI process. Defaults to True.
```

### Comparing `bitefix-0.2.1/bitefix.egg-info/PKG-INFO` & `bitefix-1.0.0/bitefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bitefix
-Version: 0.2.1
+Version: 1.0.0
 Summary: Bitefix is an efficient library designed to streamline Python Runtime error debugging with AI-powered decorators. 
 Home-page: https://github.com/Pallavi-Sinha-12/bitefix
 Author: Pallavi Sinha
 Author-email: dataaienthusiast128@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: crewai==0.14.4
 Requires-Dist: langchain==0.1.9
 Requires-Dist: crewai-tools==0.0.12
 
 # BiteFix 🛠️
@@ -143,15 +143,15 @@
 ```python
 
 from bitefix import resolve
 from langchain_community.llms import Ollama
 
 llm = Ollama("openhermes")
 
-@resolve_with_openai(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
+@resolve(llm = llm, function_description= function_description, export_dir="logs", verbose=True)
 def max_profit(stock_prices):
 
     min_price = stock_prices[0]
     max_profit = 0 
 
     for price in stock_prices[1:]:
         min_price = min(min_price, price)
```

### Comparing `bitefix-0.2.1/setup.py` & `bitefix-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="bitefix",
-    version="0.2.1",
+    version="1.0.0",
     description="""Bitefix is an efficient library designed to streamline Python Runtime error debugging with AI-powered decorators. 
     It initializes a crew of AI agents which work together to diagnose the error, generate ideas to fix the error, 
     evaluate the ideas to choose the best and develop the code to fix the error.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Pallavi Sinha",
     packages=find_packages(include=["bitefix"]),
@@ -20,9 +20,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=required,
     license="MIT",
     url="https://github.com/Pallavi-Sinha-12/bitefix",
-    python_requires=">=3.11",
+    python_requires=">=3.10",
 )
```

