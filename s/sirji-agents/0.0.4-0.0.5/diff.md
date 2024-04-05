# Comparing `tmp/sirji-agents-0.0.4.tar.gz` & `tmp/sirji-agents-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-agents-0.0.4.tar", last modified: Thu Apr  4 13:12:11 2024, max compression
+gzip compressed data, was "sirji-agents-0.0.5.tar", last modified: Fri Apr  5 08:26:36 2024, max compression
```

## Comparing `sirji-agents-0.0.4.tar` & `sirji-agents-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.476536 sirji-agents-0.0.4/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-04 13:12:11.475705 sirji-agents-0.0.4/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3060 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 13:12:11.476765 sirji-agents-0.0.4/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      684 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.464194 sirji-agents-0.0.4/sirji_agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.468335 sirji-agents-0.0.4/sirji_agents/llm/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/llm/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2447 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/llm/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/llm/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/llm/planner.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.469345 sirji-agents-0.0.4/sirji_agents/researcher/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.471513 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5581 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/openai_assistant.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.473950 sirji-agents-0.0.4/sirji_agents/researcher/inferer/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/inferer/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/inferer/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/inferer/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/inferer/openai_assistant.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4442 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/researcher.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.474868 sirji-agents-0.0.4/sirji_agents.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:36.265935 sirji-agents-0.0.5/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-05 08:26:36.265426 sirji-agents-0.0.5/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3060 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 08:26:36.266054 sirji-agents-0.0.5/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      684 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:36.253035 sirji-agents-0.0.5/sirji_agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:36.257550 sirji-agents-0.0.5/sirji_agents/llm/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/llm/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2447 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/llm/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/llm/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/llm/planner.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:36.258492 sirji-agents-0.0.5/sirji_agents/researcher/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:36.261038 sirji-agents-0.0.5/sirji_agents/researcher/embeddings/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/embeddings/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/embeddings/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/embeddings/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5844 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/embeddings/openai_assistant.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:36.263961 sirji-agents-0.0.5/sirji_agents/researcher/inferer/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/inferer/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/inferer/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/inferer/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/inferer/openai_assistant.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4705 2024-04-05 08:26:17.000000 sirji-agents-0.0.5/sirji_agents/researcher/researcher.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 08:26:36.264808 sirji-agents-0.0.5/sirji_agents.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-05 08:26:36.000000 sirji-agents-0.0.5/sirji_agents.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-05 08:26:36.000000 sirji-agents-0.0.5/sirji_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 08:26:36.000000 sirji-agents-0.0.5/sirji_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-05 08:26:36.000000 sirji-agents-0.0.5/sirji_agents.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-05 08:26:36.000000 sirji-agents-0.0.5/sirji_agents.egg-info/top_level.txt
```

### Comparing `sirji-agents-0.0.4/LICENSE` & `sirji-agents-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.4/PKG-INFO` & `sirji-agents-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.4
+Version: 0.0.5
 Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sirji-messages==0.0.4
-Requires-Dist: sirji-tools==0.0.4
+Requires-Dist: sirji-tools==0.0.5
 Requires-Dist: openai==1.14.1
 
 # sirji-agents
 
 `sirji-agents` is a PyPI package that implements three key agents for Sirji:
 
 - Coding Agent
```

### Comparing `sirji-agents-0.0.4/README.md` & `sirji-agents-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.4/setup.py` & `sirji-agents-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-agents',
-    version='0.0.4',
+    version='0.0.5',
     author='Sirji',
     description='Research, Coding and Planning agents used by Sirji.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-agents-0.0.4/sirji_agents/llm/base.py` & `sirji-agents-0.0.5/sirji_agents/llm/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.4/sirji_agents/researcher/embeddings/openai_assistant.py` & `sirji-agents-0.0.5/sirji_agents/researcher/embeddings/openai_assistant.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             self.assistant_id = self._create_assistant()
             # Update payload
             self.init_payload['assistant_id'] = self.assistant_id
 
             # Provide a way to output this updated init_payload
             logger.info(f"New assistant created with ID: {self.assistant_id}")
 
-        self.index_file_path = os.path.join(self._get_workspace_folder(), '.sirji', 'researcher', 'file_index.json')
+        self.index_file_path = os.path.join(self._get_workspace_folder(), '.sirji', self._get_run_id_folder(), 'researcher', 'file_index.json')
 
         # Load or initialize the index file
         self.index_data = self._load_or_initialize_index_file()
 
         logger.info("Completed initializing OpenAI Assistant Embeddings")
 
     def index(self, folder_path):
@@ -85,14 +85,21 @@
     def _get_workspace_folder(self):
         workspace = os.environ.get("SIRJI_WORKSPACE")
         if workspace is None:
             raise ValueError(
                 "SIRJI_WORKSPACE is not set as an environment variable")
         return workspace
 
+    def _get_run_id_folder(self):
+        run_id = os.environ.get("SIRJI_RUN_ID")
+        if run_id is None:
+            raise ValueError(
+                "SIRJI_RUN_ID is not set as an environment variable")
+        return run_id
+    
     def _create_assistant(self):
         logger.info("Creating a new assistant instance")
         """
         Create a new assistant
         """
         assistant = self.client.beta.assistants.create(
             name="Research Assistant",
```

### Comparing `sirji-agents-0.0.4/sirji_agents/researcher/inferer/base.py` & `sirji-agents-0.0.5/sirji_agents/researcher/inferer/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.4/sirji_agents/researcher/inferer/openai_assistant.py` & `sirji-agents-0.0.5/sirji_agents/researcher/inferer/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.4/sirji_agents/researcher/researcher.py` & `sirji-agents-0.0.5/sirji_agents/researcher/researcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             embeddings_type, init_payload)
 
         self.init_payload = self._embeddings_manager.init_payload
 
         self._inferer = InfererFactory.get_instance(
             inferer_type, self.init_payload)
 
-        self._research_folder = os.path.join(self._get_workspace_folder(), '.sirji', "researcher")
+        self._research_folder = os.path.join(self._get_workspace_folder(), '.sirji', self._get_run_id_folder(), "researcher")
 
         logger.info("Completed initializing researcher")
 
     def message(self, input_message):
         """Public method to process input messages and dispatch actions."""
         parsed_message = message_parse(input_message)
         action = parsed_message.get("ACTION")
@@ -41,14 +41,21 @@
         
     def _get_workspace_folder(self):
         workspace = os.environ.get("SIRJI_WORKSPACE")
         if workspace is None:
             raise ValueError(
                 "SIRJI_WORKSPACE is not set as an environment variable")
         return workspace
+    
+    def _get_run_id_folder(self):
+        run_id = os.environ.get("SIRJI_RUN_ID")
+        if run_id is None:
+            raise ValueError(
+                "SIRJI_RUN_ID is not set as an environment variable")
+        return run_id
 
     def _handle_train_using_search_term(self, parsed_message):
         """Private method to handle training using a search term."""
         logger.info(
             f"Training using search term: {parsed_message.get('TERM')}")
         self._search_and_index(parsed_message.get('TERM'))
```

### Comparing `sirji-agents-0.0.4/sirji_agents.egg-info/PKG-INFO` & `sirji-agents-0.0.5/sirji_agents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.4
+Version: 0.0.5
 Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sirji-messages==0.0.4
-Requires-Dist: sirji-tools==0.0.4
+Requires-Dist: sirji-tools==0.0.5
 Requires-Dist: openai==1.14.1
 
 # sirji-agents
 
 `sirji-agents` is a PyPI package that implements three key agents for Sirji:
 
 - Coding Agent
```

### Comparing `sirji-agents-0.0.4/sirji_agents.egg-info/SOURCES.txt` & `sirji-agents-0.0.5/sirji_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

