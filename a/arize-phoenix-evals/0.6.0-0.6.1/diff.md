# Comparing `tmp/arize_phoenix_evals-0.6.0.tar.gz` & `tmp/arize_phoenix_evals-0.6.1.tar.gz`

## Comparing `arize_phoenix_evals-0.6.0.tar` & `arize_phoenix_evals-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/__init__.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/classify.py
--rw-r--r--   0        0        0    20700 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/default_templates.py
--rw-r--r--   0        0        0    15930 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/evaluators.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/exceptions.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/executors.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/generate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/py.typed
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/retrievals.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/templates.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/utils.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/anthropic.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/base.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/bedrock.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/litellm.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/mistralai.py
--rw-r--r--   0        0        0    15069 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/openai.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/rate_limiters.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/vertex.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/src/phoenix/evals/models/vertexai.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/.gitignore
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/IP_NOTICE
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/LICENSE
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/README.md
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/__init__.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/classify.py
+-rw-r--r--   0        0        0    20700 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/default_templates.py
+-rw-r--r--   0        0        0    15930 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/evaluators.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/exceptions.py
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/executors.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/generate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/py.typed
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/retrievals.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/templates.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/utils.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/anthropic.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/base.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/bedrock.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/litellm.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/mistralai.py
+-rw-r--r--   0        0        0    15069 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/openai.py
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/rate_limiters.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/vertex.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/src/phoenix/evals/models/vertexai.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/.gitignore
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/IP_NOTICE
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/README.md
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.6.1/PKG-INFO
```

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/__init__.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/classify.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/classify.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/default_templates.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/default_templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/evaluators.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/evaluators.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/executors.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/executors.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/generate.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/generate.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/retrievals.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/retrievals.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/templates.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/utils.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/anthropic.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/base.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/base.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/bedrock.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/litellm.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/litellm.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/mistralai.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/mistralai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/openai.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/openai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/rate_limiters.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/rate_limiters.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/vertex.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/vertex.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/src/phoenix/evals/models/vertexai.py` & `arize_phoenix_evals-0.6.1/src/phoenix/evals/models/vertexai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/LICENSE` & `arize_phoenix_evals-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/README.md` & `arize_phoenix_evals-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.6.0/pyproject.toml` & `arize_phoenix_evals-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "arize-phoenix-evals"
 description = "LLM Evaluations"
 readme = "README.md"
 requires-python = ">=3.8, <3.13"
-license = "Elastic-2.0"
+license = {text="Elastic-2.0"}
 license-files = { paths = ["LICENSE", "IP_NOTICE"] }
 keywords = [
   "Observability",
   "Monitoring",
   "Explainability",
 ]
 authors = [
@@ -17,15 +17,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
   "pandas",
   "tqdm",
   "typing-extensions>=4.5, <5",
 ]
 
 [project.optional-dependencies]
```

### Comparing `arize_phoenix_evals-0.6.0/PKG-INFO` & `arize_phoenix_evals-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: arize-phoenix-evals
-Version: 0.6.0
+Version: 0.6.1
 Summary: LLM Evaluations
 Project-URL: Documentation, https://docs.arize.com/phoenix/
 Project-URL: Issues, https://github.com/Arize-ai/phoenix/issues
 Project-URL: Source, https://github.com/Arize-ai/phoenix
 Author-email: Arize AI <phoenix-devs@arize.com>
-License-Expression: Elastic-2.0
+License: Elastic-2.0
 License-File: IP_NOTICE
 License-File: LICENSE
 Keywords: Explainability,Monitoring,Observability
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

