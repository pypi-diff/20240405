# Comparing `tmp/jupyter_ai_magics-2.9.0.tar.gz` & `tmp/jupyter_ai_magics-2.9.1.tar.gz`

## Comparing `jupyter_ai_magics-2.9.0.tar` & `jupyter_ai_magics-2.9.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/setup.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/aliases.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/embedding_providers.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0    22623 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/parsers.py
--rw-r--r--   0        0        0    24003 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/jupyter_ai_magics/tests/test_utils.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/README.md
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/setup.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    22623 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/parsers.py
+-rw-r--r--   0        0        0    25345 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/tests/test_provider_metaclass.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/jupyter_ai_magics/tests/test_utils.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/README.md
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.9.1/PKG-INFO
```

### Comparing `jupyter_ai_magics-2.9.0/package.json` & `jupyter_ai_magics-2.9.1/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'2.9.1'"}*

```diff
@@ -17,9 +17,9 @@
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[dev,all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y",
         "install-from-src": "pip install ."
     },
-    "version": "2.9.0"
+    "version": "2.9.1"
 }
```

### Comparing `jupyter_ai_magics-2.9.0/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-2.9.1/jupyter_ai_magics/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.9.0/jupyter_ai_magics/embedding_providers.py` & `jupyter_ai_magics-2.9.1/jupyter_ai_magics/embedding_providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-import os
 from typing import ClassVar, List
 
 from jupyter_ai_magics.providers import (
     AuthStrategy,
     AwsAuthStrategy,
     EnvAuthStrategy,
     Field,
     MultiEnvAuthStrategy,
 )
-from langchain.embeddings import (
+from langchain.pydantic_v1 import BaseModel, Extra
+from langchain_community.embeddings import (
     BedrockEmbeddings,
     CohereEmbeddings,
     GPT4AllEmbeddings,
     HuggingFaceHubEmbeddings,
     OpenAIEmbeddings,
     QianfanEmbeddingsEndpoint,
 )
-from langchain.pydantic_v1 import BaseModel, Extra
 
 
 class BaseEmbeddingsProvider(BaseModel):
     """Base class for embedding providers"""
 
     class Config:
         extra = Extra.allow
```

### Comparing `jupyter_ai_magics-2.9.0/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-2.9.1/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.9.0/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-2.9.1/jupyter_ai_magics/magics.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.9.0/jupyter_ai_magics/parsers.py` & `jupyter_ai_magics-2.9.1/jupyter_ai_magics/parsers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.9.0/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-2.9.1/jupyter_ai_magics/providers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 import asyncio
 import base64
 import copy
 import functools
 import io
 import json
 from concurrent.futures import ThreadPoolExecutor
-from typing import (
-    Any,
-    ClassVar,
-    Coroutine,
-    Dict,
-    List,
-    Literal,
-    Mapping,
-    Optional,
-    Union,
-)
+from typing import Any, ClassVar, Coroutine, Dict, List, Literal, Optional, Union
 
 from jsonpath_ng import parse
-from langchain.chat_models import (
+from langchain.chat_models.base import BaseChatModel
+from langchain.llms.sagemaker_endpoint import LLMContentHandler
+from langchain.llms.utils import enforce_stop_tokens
+from langchain.prompts import PromptTemplate
+from langchain.pydantic_v1 import BaseModel, Extra, root_validator
+from langchain.schema import LLMResult
+from langchain.utils import get_from_dict_or_env
+from langchain_community.chat_models import (
     AzureChatOpenAI,
     BedrockChat,
     ChatAnthropic,
+    ChatOpenAI,
     QianfanChatEndpoint,
 )
-from langchain.chat_models.base import BaseChatModel
-from langchain.llms import (
+from langchain_community.llms import (
     AI21,
     Anthropic,
     Bedrock,
     Cohere,
     GPT4All,
     HuggingFaceHub,
     OpenAI,
-    OpenAIChat,
-    QianfanLLMEndpoint,
     SagemakerEndpoint,
 )
-from langchain.llms.sagemaker_endpoint import LLMContentHandler
-from langchain.llms.utils import enforce_stop_tokens
-from langchain.prompts import PromptTemplate
-from langchain.pydantic_v1 import BaseModel, Extra, root_validator
-from langchain.schema import LLMResult
-from langchain.utils import get_from_dict_or_env
-from langchain_community.chat_models import ChatOpenAI
+
+# this is necessary because `langchain.pydantic_v1.main` does not include
+# `ModelMetaclass`, as it is not listed in `__all__` by the `pydantic.main`
+# subpackage.
+try:
+    from pydantic.v1.main import ModelMetaclass
+except:
+    from pydantic.main import ModelMetaclass
 
 
 class EnvAuthStrategy(BaseModel):
     """Require one auth token via an environment variable."""
 
     type: Literal["env"] = "env"
     name: str
@@ -95,15 +91,42 @@
     key: str
     label: str
 
 
 Field = Union[TextField, MultilineTextField, IntegerField]
 
 
-class BaseProvider(BaseModel):
+class ProviderMetaclass(ModelMetaclass):
+    """
+    A metaclass that ensures all class attributes defined inline within the
+    class definition are accessible and included in `Class.__dict__`.
+
+    This is necessary because Pydantic drops any ClassVars that are defined as
+    an instance field by a parent class, even if they are defined inline within
+    the class definition. We encountered this case when `langchain` added a
+    `name` attribute to a parent class shared by all `Provider`s, which caused
+    `Provider.name` to be inaccessible. See #558 for more info.
+    """
+
+    def __new__(mcs, name, bases, namespace, **kwargs):
+        cls = super().__new__(mcs, name, bases, namespace, **kwargs)
+        for key in namespace:
+            # skip private class attributes
+            if key.startswith("_"):
+                continue
+            # skip class attributes already listed in `cls.__dict__`
+            if key in cls.__dict__:
+                continue
+
+            setattr(cls, key, namespace[key])
+
+        return cls
+
+
+class BaseProvider(BaseModel, metaclass=ProviderMetaclass):
     #
     # pydantic config
     #
     class Config:
         extra = Extra.allow
 
     #
@@ -336,15 +359,16 @@
     def allows_concurrency(self):
         return False
 
 
 class CohereProvider(BaseProvider, Cohere):
     id = "cohere"
     name = "Cohere"
-    models = ["medium", "xlarge"]
+    # Source: https://docs.cohere.com/reference/generate
+    models = ["command", "command-nightly", "command-light", "command-light-nightly"]
     model_id_key = "model"
     pypi_package_deps = ["cohere"]
     auth_strategy = EnvAuthStrategy(name="COHERE_API_KEY")
 
     async def _acall(self, *args, **kwargs) -> Coroutine[Any, Any, str]:
         return await self._call_in_executor(*args, **kwargs)
```

### Comparing `jupyter_ai_magics-2.9.0/jupyter_ai_magics/utils.py` & `jupyter_ai_magics-2.9.1/jupyter_ai_magics/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.9.0/jupyter_ai_magics/tests/test_utils.py` & `jupyter_ai_magics-2.9.1/jupyter_ai_magics/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.9.0/.gitignore` & `jupyter_ai_magics-2.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.9.0/LICENSE` & `jupyter_ai_magics-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.9.0/pyproject.toml` & `jupyter_ai_magics-2.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,44 +19,36 @@
 ]
 
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 dependencies = [
     "ipython",
     "importlib_metadata>=5.2.0",
-    "langchain==0.0.350",
-    "langchain-core>=0.1.0,<0.1.4",
+    "langchain>=0.1.0,<0.2.0",
     "typing_extensions>=4.5.0",
     "click~=8.0",
     "jsonpath-ng>=1.5.3,<2",
 ]
 
 [project.optional-dependencies]
-dev = [
-    "pre-commit>=3.3.3,<4"
-]
+dev = ["pre-commit>=3.3.3,<4"]
 
-test = [
-    "coverage",
-    "pytest",
-    "pytest-asyncio",
-    "pytest-cov"
-]
+test = ["coverage", "pytest", "pytest-asyncio", "pytest-cov"]
 
 all = [
     "ai21",
     "anthropic~=0.3.0",
     "cohere",
     "gpt4all",
     "huggingface_hub",
     "ipywidgets",
     "pillow",
     "openai~=1.6.1",
     "boto3",
-    "qianfan"
+    "qianfan",
 ]
 
 [project.entry-points."jupyter_ai.model_providers"]
 ai21 = "jupyter_ai_magics:AI21Provider"
 anthropic = "jupyter_ai_magics:AnthropicProvider"
 cohere = "jupyter_ai_magics:CohereProvider"
 gpt4all = "jupyter_ai_magics:GPT4AllProvider"
```

### Comparing `jupyter_ai_magics-2.9.0/PKG-INFO` & `jupyter_ai_magics-2.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 2.9.0
+Version: 2.9.1
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -45,16 +45,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: click~=8.0
 Requires-Dist: importlib-metadata>=5.2.0
 Requires-Dist: ipython
 Requires-Dist: jsonpath-ng<2,>=1.5.3
-Requires-Dist: langchain-core<0.1.4,>=0.1.0
-Requires-Dist: langchain==0.0.350
+Requires-Dist: langchain<0.2.0,>=0.1.0
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
 Requires-Dist: anthropic~=0.3.0; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
 Requires-Dist: cohere; extra == 'all'
 Requires-Dist: gpt4all; extra == 'all'
```

