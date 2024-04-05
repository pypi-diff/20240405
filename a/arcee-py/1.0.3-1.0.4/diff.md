# Comparing `tmp/arcee_py-1.0.3.tar.gz` & `tmp/arcee_py-1.0.4.tar.gz`

## Comparing `arcee_py-1.0.3.tar` & `arcee_py-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.3/.python-version
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.3/tasks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.3/.github/iced/test.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/__init__.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/api.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/api_handler.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/cli.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/cli_handler.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/config.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/dalm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/schemas/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/schemas/doc.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 arcee_py-1.0.3/arcee/schemas/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.3/tests/conftest.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.3/tests/test_api_handler.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.3/.gitignore
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 arcee_py-1.0.3/README.md
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 arcee_py-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 arcee_py-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.python-version
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.4/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.github/iced/test.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/__init__.py
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/api.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/api_handler.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/cli.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/cli_handler.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/config.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/dalm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/schemas/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/schemas/doc.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/schemas/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.4/tests/test_api_handler.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.gitignore
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 arcee_py-1.0.4/README.md
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 arcee_py-1.0.4/PKG-INFO
```

### Comparing `arcee_py-1.0.3/tasks.py` & `arcee_py-1.0.4/tasks.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/.github/iced/test.yml` & `arcee_py-1.0.4/.github/iced/test.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/.github/workflows/publish.yml` & `arcee_py-1.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/arcee/__init__.py` & `arcee_py-1.0.4/arcee/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 import os
 
 from arcee import config
-from arcee.api import upload_docs, upload_corpus_folder, upload_qa_pairs, start_alignment, start_pretraining, start_retriever_training, get_retriever_status, start_deployment, stop_deployment, generate, retrieve, delete_corpus
+from arcee.api import upload_docs, upload_corpus_folder, upload_qa_pairs, start_alignment, start_pretraining, start_retriever_training, get_retriever_status, start_deployment, stop_deployment, generate, retrieve, delete_corpus, upload_alignment
 from arcee.dalm import DALM, DALMFilter
 
 if not config.ARCEE_API_KEY:
     # We check this because it's impossible the user imported arcee, _then_ set the env, then imported again
     config.ARCEE_API_KEY = os.getenv("ARCEE_API_KEY", "")
     while not config.ARCEE_API_KEY:
         config.ARCEE_API_KEY = input("ARCEE_API_KEY not found in environment. Please input api key: ")
     os.environ["ARCEE_API_KEY"] = config.ARCEE_API_KEY
 
-__all__ = ["upload_docs", "DALM", "DALMFilter", "upload_corpus_folder", "upload_qa_pairs", "start_alignment", "start_pretraining", "start_retriever_training", "get_retriever_status", "start_deployment", "stop_deployment", "generate", "retrieve", "delete_corpus"]
+__all__ = ["upload_docs", "DALM", "DALMFilter", "upload_corpus_folder", "upload_qa_pairs", "start_alignment", "start_pretraining", "start_retriever_training", "get_retriever_status", "start_deployment", "stop_deployment", "generate", "retrieve", "delete_corpus", "upload_alignment"]
```

### Comparing `arcee_py-1.0.3/arcee/api.py` & `arcee_py-1.0.4/arcee/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,18 @@
         pretrained_model (str): The name of the pretrained model to use
     """
 
     data = {"alignment_name": alignment_name, "qa_set_name": qa_set, "pretrained_model": pretrained_model}
 
     return make_request("post", Route.alignment+"/startAlignment", data)
 
+def upload_alignment(alignment_name: str, alignment_id: str, qa_set_id: str, pretraining_id: str) -> None:
+    data = {"alignment_name": alignment_name, "alignment_id": alignment_id, "qa_set_id": qa_set_id, "pretraining_id": pretraining_id}
+    return make_request("post", Route.alignment+"/uploadAlignment", data)
+
 def start_retriever_training(name: str, context: str):
     data = {"name": name, "context": context}
     make_request("post", Route.train_model, data)
     org = get_current_org()
     status_url = f"{config.ARCEE_APP_URL}/{org}/models/{name}/training"
     print(
         f'Retriever model training started - view model status at {status_url} or with arcee.get_retriever_status("{name}")'
```

### Comparing `arcee_py-1.0.3/arcee/api_handler.py` & `arcee_py-1.0.4/arcee/api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/arcee/cli.py` & `arcee_py-1.0.4/arcee/cli.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/arcee/cli_handler.py` & `arcee_py-1.0.4/arcee/cli_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/arcee/config.py` & `arcee_py-1.0.4/arcee/config.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/arcee/dalm.py` & `arcee_py-1.0.4/arcee/dalm.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/tests/test_api_handler.py` & `arcee_py-1.0.4/tests/test_api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/.gitignore` & `arcee_py-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/README.md` & `arcee_py-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.3/pyproject.toml` & `arcee_py-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 [tool.hatch.build.targets.wheel]
 packages = ["arcee"]
 
 [tool.hatch.version]
 path = "arcee/__init__.py"
 
 
-
 [project.optional-dependencies]
 dev = [
     "black",
     "invoke",
     "mypy",
     "pytest",
     "pytest-cov",
```

### Comparing `arcee_py-1.0.3/PKG-INFO` & `arcee_py-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-py
-Version: 1.0.3
+Version: 1.0.4
 Project-URL: Home, https://arcee.ai
 Author-email: Jacob Solowetz <jacob@arcee.ai>, Ben Epstein <ben@arcee.ai>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: pydantic<3.0,>=2.4.2
 Requires-Dist: requests
 Requires-Dist: rich
```

