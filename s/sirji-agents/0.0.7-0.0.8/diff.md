# Comparing `tmp/sirji-agents-0.0.7.tar.gz` & `tmp/sirji-agents-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-agents-0.0.7.tar", last modified: Fri Apr  5 12:37:24 2024, max compression
+gzip compressed data, was "sirji-agents-0.0.8.tar", last modified: Fri Apr  5 13:25:47 2024, max compression
```

## Comparing `sirji-agents-0.0.7.tar` & `sirji-agents-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:24.314843 sirji-agents-0.0.7/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-05 12:37:24.314363 sirji-agents-0.0.7/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3060 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 12:37:24.314955 sirji-agents-0.0.7/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      684 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:24.306300 sirji-agents-0.0.7/sirji_agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:24.309641 sirji-agents-0.0.7/sirji_agents/llm/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/llm/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2447 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/llm/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/llm/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/llm/planner.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:24.310371 sirji-agents-0.0.7/sirji_agents/researcher/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:24.311843 sirji-agents-0.0.7/sirji_agents/researcher/embeddings/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/embeddings/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/embeddings/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/embeddings/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5844 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/embeddings/openai_assistant.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:24.313327 sirji-agents-0.0.7/sirji_agents/researcher/inferer/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/inferer/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/inferer/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/inferer/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/inferer/openai_assistant.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4705 2024-04-05 12:37:19.000000 sirji-agents-0.0.7/sirji_agents/researcher/researcher.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:37:24.313836 sirji-agents-0.0.7/sirji_agents.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-05 12:37:24.000000 sirji-agents-0.0.7/sirji_agents.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-05 12:37:24.000000 sirji-agents-0.0.7/sirji_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 12:37:24.000000 sirji-agents-0.0.7/sirji_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-05 12:37:24.000000 sirji-agents-0.0.7/sirji_agents.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-05 12:37:24.000000 sirji-agents-0.0.7/sirji_agents.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.587227 sirji-agents-0.0.8/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-05 13:25:47.585115 sirji-agents-0.0.8/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3060 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 13:25:47.587534 sirji-agents-0.0.8/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      684 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.569756 sirji-agents-0.0.8/sirji_agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.574743 sirji-agents-0.0.8/sirji_agents/llm/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/llm/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2545 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/llm/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/llm/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/llm/planner.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.575730 sirji-agents-0.0.8/sirji_agents/researcher/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.578370 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5844 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/openai_assistant.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.581852 sirji-agents-0.0.8/sirji_agents/researcher/inferer/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/inferer/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/inferer/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/inferer/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/inferer/openai_assistant.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4705 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/researcher.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.583593 sirji-agents-0.0.8/sirji_agents.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/top_level.txt
```

### Comparing `sirji-agents-0.0.7/LICENSE` & `sirji-agents-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.7/PKG-INFO` & `sirji-agents-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.7
+Version: 0.0.8
 Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sirji-agents-0.0.7/README.md` & `sirji-agents-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.7/setup.py` & `sirji-agents-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-agents',
-    version='0.0.7',
+    version='0.0.8',
     author='Sirji',
     description='Research, Coding and Planning agents used by Sirji.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-agents-0.0.7/sirji_agents/llm/base.py` & `sirji-agents-0.0.8/sirji_agents/llm/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,11 +62,14 @@
             messages=history,
             model="gpt-4-turbo-preview",
             temperature=0,
             max_tokens=4095,
         )
 
         response_message = chat_completion.choices[0].message.content
+
+        self.logger.info(f"Raw response from Chat Completions API: \n{response_message}\n\n\n")
+
         parsed_response_message = message_parse(response_message)
         conversation.append({"role": "assistant", "content": response_message, "parsed_content": parsed_response_message})
 
         return response_message
```

### Comparing `sirji-agents-0.0.7/sirji_agents/researcher/embeddings/openai_assistant.py` & `sirji-agents-0.0.8/sirji_agents/researcher/embeddings/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.7/sirji_agents/researcher/inferer/base.py` & `sirji-agents-0.0.8/sirji_agents/researcher/inferer/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.7/sirji_agents/researcher/inferer/openai_assistant.py` & `sirji-agents-0.0.8/sirji_agents/researcher/inferer/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.7/sirji_agents/researcher/researcher.py` & `sirji-agents-0.0.8/sirji_agents/researcher/researcher.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.7/sirji_agents.egg-info/PKG-INFO` & `sirji-agents-0.0.8/sirji_agents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.7
+Version: 0.0.8
 Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sirji-agents-0.0.7/sirji_agents.egg-info/SOURCES.txt` & `sirji-agents-0.0.8/sirji_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

