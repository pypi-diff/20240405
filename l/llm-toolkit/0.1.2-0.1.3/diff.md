# Comparing `tmp/llm_toolkit-0.1.2.tar.gz` & `tmp/llm_toolkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_toolkit-0.1.2.tar", max compression
+gzip compressed data, was "llm_toolkit-0.1.3.tar", max compression
```

## Comparing `llm_toolkit-0.1.2.tar` & `llm_toolkit-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10763 2024-04-05 17:59:18.095929 llm_toolkit-0.1.2/LICENSE
--rw-r--r--   0        0        0     8680 2024-04-05 17:59:18.095929 llm_toolkit-0.1.2/README.md
--rw-r--r--   0        0        0      601 2024-04-05 18:00:58.484840 llm_toolkit-0.1.2/llmtune/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/cli/__init__.py
--rw-r--r--   0        0        0     3722 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/cli/toolkit.py
--rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/data/__init__.py
--rw-r--r--   0        0        0     2917 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/data/dataset_generator.py
--rw-r--r--   0        0        0     1477 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/data/ingestor.py
--rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/finetune/__init__.py
--rw-r--r--   0        0        0      176 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/finetune/generics.py
--rw-r--r--   0        0        0     4475 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/finetune/lora.py
--rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/inference/__init__.py
--rw-r--r--   0        0        0      190 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/inference/generics.py
--rw-r--r--   0        0        0     3823 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/inference/lora.py
--rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/pydantic_models/__init__.py
--rw-r--r--   0        0        0     8549 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/pydantic_models/config_model.py
--rw-r--r--   0        0        0        0 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/qa/__init__.py
--rw-r--r--   0        0        0     2550 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/qa/generics.py
--rw-r--r--   0        0        0     5503 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/qa/qa_tests.py
--rw-r--r--   0        0        0        0 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/ui/__init__.py
--rw-r--r--   0        0        0     2149 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/ui/generics.py
--rw-r--r--   0        0        0     5933 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/ui/rich_ui.py
--rw-r--r--   0        0        0        0 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/utils/__init__.py
--rw-r--r--   0        0        0     3338 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/utils/ablation_utils.py
--rw-r--r--   0        0        0     1335 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/utils/rich_print_utils.py
--rw-r--r--   0        0        0     2429 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/utils/save_utils.py
--rw-r--r--   0        0        0     1680 2024-04-05 18:00:58.484840 llm_toolkit-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10442 1970-01-01 00:00:00.000000 llm_toolkit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10763 2024-04-05 19:29:19.945310 llm_toolkit-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8733 2024-04-05 19:29:19.945310 llm_toolkit-0.1.3/README.md
+-rw-r--r--   0        0        0      601 2024-04-05 19:31:01.877064 llm_toolkit-0.1.3/llmtune/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/cli/__init__.py
+-rw-r--r--   0        0        0     3722 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/cli/toolkit.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/data/__init__.py
+-rw-r--r--   0        0        0     2917 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/data/dataset_generator.py
+-rw-r--r--   0        0        0     1477 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/data/ingestor.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/finetune/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/finetune/generics.py
+-rw-r--r--   0        0        0     4475 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/finetune/lora.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/inference/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/inference/generics.py
+-rw-r--r--   0        0        0     3823 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/inference/lora.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/pydantic_models/__init__.py
+-rw-r--r--   0        0        0     8549 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/pydantic_models/config_model.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/qa/__init__.py
+-rw-r--r--   0        0        0     2550 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/qa/generics.py
+-rw-r--r--   0        0        0     5503 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/qa/qa_tests.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/ui/__init__.py
+-rw-r--r--   0        0        0     2149 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/ui/generics.py
+-rw-r--r--   0        0        0     5933 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/ui/rich_ui.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/utils/ablation_utils.py
+-rw-r--r--   0        0        0     1335 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/utils/rich_print_utils.py
+-rw-r--r--   0        0        0     2429 2024-04-05 19:29:19.977310 llm_toolkit-0.1.3/llmtune/utils/save_utils.py
+-rw-r--r--   0        0        0     2044 2024-04-05 19:31:01.873064 llm_toolkit-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10876 1970-01-01 00:00:00.000000 llm_toolkit-0.1.3/PKG-INFO
```

### Comparing `llm_toolkit-0.1.2/LICENSE` & `llm_toolkit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/README.md` & `llm_toolkit-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # LLM Finetuning Toolkit
 
 <p align="center">
-  <img src="assets/toolkit-animation.gif" width="900" />
+  <img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/toolkit-animation.gif" width="900" />
 </p>
 
 ## Overview
 
 LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM finetuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
 
 <p align="center">
-<img src="assets/overview_diagram.png" width="900" />
+<img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/overview_diagram.png" width="900" />
 </p>
 
 ## Installation
 ### pipx (recommended)
 pipx installs the package and depdencies in a seperate virtual environment
 ```shell
 pipx install llm-toolkit
 ```
 
 ### pip
 ```shell
 pip install llm-toolkit
 ```
 
-### docker
-```shell
-docker pull ghcr.io/georgian-io/llm-toolkit:latest
-```
 
 ## Quick Start
 
 This guide contains 3 stages that will enable you to get the most out of this toolkit!
 
 - **Basic**: Run your first LLM fine-tuning experiment
 - **Intermediate**: Run a custom experiment by changing the componenets of the YAML configuration file
```

### Comparing `llm_toolkit-0.1.2/llmtune/__init__.py` & `llm_toolkit-0.1.3/llmtune/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `llm_toolkit-0.1.2/llmtune/cli/toolkit.py` & `llm_toolkit-0.1.3/llmtune/cli/toolkit.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/data/dataset_generator.py` & `llm_toolkit-0.1.3/llmtune/data/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/data/ingestor.py` & `llm_toolkit-0.1.3/llmtune/data/ingestor.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/finetune/lora.py` & `llm_toolkit-0.1.3/llmtune/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/inference/lora.py` & `llm_toolkit-0.1.3/llmtune/inference/lora.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/pydantic_models/config_model.py` & `llm_toolkit-0.1.3/llmtune/pydantic_models/config_model.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/qa/generics.py` & `llm_toolkit-0.1.3/llmtune/qa/generics.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/qa/qa_tests.py` & `llm_toolkit-0.1.3/llmtune/qa/qa_tests.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/ui/generics.py` & `llm_toolkit-0.1.3/llmtune/ui/generics.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/ui/rich_ui.py` & `llm_toolkit-0.1.3/llmtune/ui/rich_ui.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/utils/ablation_utils.py` & `llm_toolkit-0.1.3/llmtune/utils/ablation_utils.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/utils/rich_print_utils.py` & `llm_toolkit-0.1.3/llmtune/utils/rich_print_utils.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/llmtune/utils/save_utils.py` & `llm_toolkit-0.1.3/llmtune/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.2/pyproject.toml` & `llm_toolkit-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 [tool.poetry]
 name = "llm-toolkit"
-version = "0.1.2"
+version = "0.1.3"
 description = "LLM Finetuning resource hub + toolkit"
 authors = ["Benjamin Ye <benjamin.ye@georgian.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "llmtune"}]
+repository = "https://github.com/georgian-io/LLM-Finetuning-Toolkit"
+# homepage = ""
+# documentation = ""
+keywords = ["llm", "finetuning", "language models", "machine learning", "deep learning"]
+classifiers = [
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
+
 
 [tool.poetry.scripts]
 llmtune = "llmtune.cli.toolkit:cli"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `llm_toolkit-0.1.2/PKG-INFO` & `llm_toolkit-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: llm-toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: LLM Finetuning resource hub + toolkit
+Home-page: https://github.com/georgian-io/LLM-Finetuning-Toolkit
 License: Apache 2.0
+Keywords: llm,finetuning,language models,machine learning,deep learning
 Author: Benjamin Ye
 Author-email: benjamin.ye@georgian.io
 Requires-Python: >=3.9,<=3.12
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: absl-py (>=2.1.0,<3.0.0)
 Requires-Dist: accelerate (>=0.27.0,<0.28.0)
 Requires-Dist: ai21 (>=2.0.3,<3.0.0)
 Requires-Dist: bitsandbytes (>=0.42.0,<0.43.0)
 Requires-Dist: datasets (>=2.17.0,<3.0.0)
 Requires-Dist: einops (>=0.7.0,<0.8.0)
 Requires-Dist: evaluate (>=0.4.1,<0.5.0)
@@ -38,46 +43,43 @@
 Requires-Dist: sqids (>=0.4.1,<0.5.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: transformers (>=4.37.2,<4.38.0)
 Requires-Dist: trl (>=0.7.10,<0.8.0)
 Requires-Dist: typer (>=0.10.0,<0.11.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Requires-Dist: wandb (>=0.16.3,<0.17.0)
+Project-URL: Repository, https://github.com/georgian-io/LLM-Finetuning-Toolkit
 Description-Content-Type: text/markdown
 
 # LLM Finetuning Toolkit
 
 <p align="center">
-  <img src="assets/toolkit-animation.gif" width="900" />
+  <img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/toolkit-animation.gif" width="900" />
 </p>
 
 ## Overview
 
 LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM finetuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
 
 <p align="center">
-<img src="assets/overview_diagram.png" width="900" />
+<img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/overview_diagram.png" width="900" />
 </p>
 
 ## Installation
 ### pipx (recommended)
 pipx installs the package and depdencies in a seperate virtual environment
 ```shell
 pipx install llm-toolkit
 ```
 
 ### pip
 ```shell
 pip install llm-toolkit
 ```
 
-### docker
-```shell
-docker pull ghcr.io/georgian-io/llm-toolkit:latest
-```
 
 ## Quick Start
 
 This guide contains 3 stages that will enable you to get the most out of this toolkit!
 
 - **Basic**: Run your first LLM fine-tuning experiment
 - **Intermediate**: Run a custom experiment by changing the componenets of the YAML configuration file
```

