# Comparing `tmp/llm_toolkit-0.1.1.tar.gz` & `tmp/llm_toolkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_toolkit-0.1.1.tar", max compression
+gzip compressed data, was "llm_toolkit-0.1.2.tar", max compression
```

## Comparing `llm_toolkit-0.1.1.tar` & `llm_toolkit-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0    10763 2024-03-28 14:24:09.965723 llm_toolkit-0.1.1/LICENSE
--rw-r--r--   0        0        0     7978 2024-04-02 21:32:50.444173 llm_toolkit-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-02 20:21:52.488574 llm_toolkit-0.1.1/llmtune/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 20:21:52.489039 llm_toolkit-0.1.1/llmtune/data/__init__.py
--rw-r--r--   0        0        0     2961 2024-04-02 20:21:52.489451 llm_toolkit-0.1.1/llmtune/data/dataset_generator.py
--rw-r--r--   0        0        0     1529 2024-04-02 20:21:52.489846 llm_toolkit-0.1.1/llmtune/data/ingestor.py
--rw-r--r--   0        0        0        0 2024-04-02 20:21:52.489987 llm_toolkit-0.1.1/llmtune/finetune/__init__.py
--rw-r--r--   0        0        0      176 2024-04-02 20:21:52.490502 llm_toolkit-0.1.1/llmtune/finetune/generics.py
--rw-r--r--   0        0        0     4608 2024-04-02 20:21:52.490938 llm_toolkit-0.1.1/llmtune/finetune/lora.py
--rw-r--r--   0        0        0        0 2024-04-02 20:21:52.491064 llm_toolkit-0.1.1/llmtune/inference/__init__.py
--rw-r--r--   0        0        0      190 2024-04-02 20:21:52.491330 llm_toolkit-0.1.1/llmtune/inference/generics.py
--rw-r--r--   0        0        0     4048 2024-04-02 20:21:52.491714 llm_toolkit-0.1.1/llmtune/inference/lora.py
--rw-r--r--   0        0        0        0 2024-04-02 20:21:52.491867 llm_toolkit-0.1.1/llmtune/pydantic_models/__init__.py
--rw-r--r--   0        0        0     8849 2024-04-02 20:21:52.492338 llm_toolkit-0.1.1/llmtune/pydantic_models/config_model.py
--rw-r--r--   0        0        0        0 2024-04-02 20:21:52.492454 llm_toolkit-0.1.1/llmtune/qa/__init__.py
--rw-r--r--   0        0        0     2720 2024-04-02 20:21:52.492710 llm_toolkit-0.1.1/llmtune/qa/generics.py
--rw-r--r--   0        0        0     5700 2024-04-02 20:21:52.493062 llm_toolkit-0.1.1/llmtune/qa/qa_tests.py
--rw-r--r--   0        0        0        0 2024-04-02 20:21:52.493176 llm_toolkit-0.1.1/llmtune/ui/__init__.py
--rw-r--r--   0        0        0     2151 2024-04-02 20:21:52.493473 llm_toolkit-0.1.1/llmtune/ui/generics.py
--rw-r--r--   0        0        0     6018 2024-04-02 20:21:52.493830 llm_toolkit-0.1.1/llmtune/ui/rich_ui.py
--rw-r--r--   0        0        0        0 2024-04-02 20:21:52.493946 llm_toolkit-0.1.1/llmtune/utils/__init__.py
--rw-r--r--   0        0        0     3474 2024-04-02 20:21:52.494078 llm_toolkit-0.1.1/llmtune/utils/ablation_utils.py
--rw-r--r--   0        0        0     1335 2024-04-02 20:21:52.494184 llm_toolkit-0.1.1/llmtune/utils/rich_print_utils.py
--rw-r--r--   0        0        0     2443 2024-04-02 20:21:52.494403 llm_toolkit-0.1.1/llmtune/utils/save_utils.py
--rw-r--r--   0        0        0     1053 2024-04-03 02:10:35.285883 llm_toolkit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9793 1970-01-01 00:00:00.000000 llm_toolkit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10763 2024-04-05 17:59:18.095929 llm_toolkit-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8680 2024-04-05 17:59:18.095929 llm_toolkit-0.1.2/README.md
+-rw-r--r--   0        0        0      601 2024-04-05 18:00:58.484840 llm_toolkit-0.1.2/llmtune/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/cli/__init__.py
+-rw-r--r--   0        0        0     3722 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/cli/toolkit.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/data/__init__.py
+-rw-r--r--   0        0        0     2917 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/data/dataset_generator.py
+-rw-r--r--   0        0        0     1477 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/data/ingestor.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/finetune/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/finetune/generics.py
+-rw-r--r--   0        0        0     4475 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/finetune/lora.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/inference/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/inference/generics.py
+-rw-r--r--   0        0        0     3823 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/inference/lora.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/pydantic_models/__init__.py
+-rw-r--r--   0        0        0     8549 2024-04-05 17:59:18.127929 llm_toolkit-0.1.2/llmtune/pydantic_models/config_model.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/qa/__init__.py
+-rw-r--r--   0        0        0     2550 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/qa/generics.py
+-rw-r--r--   0        0        0     5503 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/qa/qa_tests.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/ui/__init__.py
+-rw-r--r--   0        0        0     2149 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/ui/generics.py
+-rw-r--r--   0        0        0     5933 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/ui/rich_ui.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/utils/ablation_utils.py
+-rw-r--r--   0        0        0     1335 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/utils/rich_print_utils.py
+-rw-r--r--   0        0        0     2429 2024-04-05 17:59:18.131929 llm_toolkit-0.1.2/llmtune/utils/save_utils.py
+-rw-r--r--   0        0        0     1680 2024-04-05 18:00:58.484840 llm_toolkit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10442 1970-01-01 00:00:00.000000 llm_toolkit-0.1.2/PKG-INFO
```

### Comparing `llm_toolkit-0.1.1/LICENSE` & `llm_toolkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.1/README.md` & `llm_toolkit-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,74 +9,42 @@
 LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM finetuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
 
 <p align="center">
 <img src="assets/overview_diagram.png" width="900" />
 </p>
 
 ## Installation
-
-### Clone Repository
-
+### pipx (recommended)
+pipx installs the package and depdencies in a seperate virtual environment
 ```shell
-   git clone https://github.com/georgian-io/LLM-Finetuning-Hub.git
-   cd LLM-Finetuning-Hub/
+pipx install llm-toolkit
 ```
 
-### [Option 1] Docker (recommended)
-
+### pip
 ```shell
-   docker build -t llm-toolkit
+pip install llm-toolkit
 ```
 
-#### CPU Only
-
+### docker
 ```shell
-   docker run -it llm-toolkit
-```
-
-#### With GPU
-
-```shell
-   docker run -it --gpus all llm-toolkit
-```
-
-### [Option 2] Poetry (recommended)
-
-See poetry documentation page for poetry [installation instructions](https://python-poetry.org/docs/#installation)
-
-```shell
-   poetry install
-```
-
-### [Option 3] pip
-
-```shell
-   pip install -r requirements.txt
-```
-
-### [Option 4] Conda
-
-```shell
-   conda create --name llm-toolkit python=3.11
-   conda activate llm-toolkit
-   pip install -r requirements.txt
+docker pull ghcr.io/georgian-io/llm-toolkit:latest
 ```
 
 ## Quick Start
 
 This guide contains 3 stages that will enable you to get the most out of this toolkit!
 
 - **Basic**: Run your first LLM fine-tuning experiment
 - **Intermediate**: Run a custom experiment by changing the componenets of the YAML configuration file
 - **Advanced**: Launch series of fine-tuning experiments across different prompt templates, LLMs, optimization techniques -- all through **one** YAML configuration file
 
 ### Basic
 
 ```python
-   python toolkit.py --config ./config.yml
+   llmtune --config-path ./config.yml
 ```
 
 This command initiates the fine-tuning process using the settings specified in the default YAML configuration file `config.yaml`.
 
 ### Intermediate
 
 The configuration file is the central piece that defines the behavior of the toolkit. It is written in YAML format and consists of several sections that control different aspects of the process, such as data ingestion, model definition, training, inference, and quality assurance. We highlight some of the critical sections.
@@ -252,18 +220,76 @@
 2.  **Clone** the project to your own machine
 3.  **Commit** changes to your own branch
 4.  **Push** your work back up to your fork
 5.  Submit a **Pull request** so that we can review your changes
 
 NOTE: Be sure to merge the latest from "upstream" before making a pull request!
 
+### Set Up Dev Environment
+
+<details>
+<summary>1. Clone Repo</summary>
+  
+```shell
+   git clone https://github.com/georgian-io/LLM-Finetuning-Toolkit.git
+   cd LLM-Finetuning-Toolkit/
+```
 
-## Releasing
+</details>
+
+<details>
+<summary>2. Install Dependencies</summary>
+<details>
+<summary>Install with Docker [Recommended]</summary>
+
+```shell
+   docker build -t llm-toolkit
+```
+
+```shell
+   # CPU
+   docker run -it llm-toolkit
+   # GPU
+   docker run -it --gpus all llm-toolkit
+```
+</details>
+
+<details>
+<summary>Poetry (recommended)</summary>
+
+See poetry documentation page for poetry [installation instructions](https://python-poetry.org/docs/#installation)
+
+```shell
+   poetry install
+```
+</details>
+<details>
+<summary>pip</summary>
+We recommend using a virtual environment like `venv` or `conda` for installation
+
+```shell
+   pip install -e .
+```
+</details>
+</details>
+
+
+
+### Checklist Before Pull Request (Optional)
+
+1. Use `ruff check --fix` to check and fix lint errors
+2. Use `ruff format` to apply formatting
+
+NOTE: Ruff linting and formatting checks are done when PR is raised via Git Action. Before raising a PR, it is a good practice to check and fix lint errors, as well as apply formatting.
+
+
+### Releasing
 
 
 To manually release a PyPI package, please run: 
 
 ```shell
    make build-release
 ```
 
-Note: Make sure you have pypi token for this [pipy repo](https://pypi.org/project/llm-toolkit/).
+Note: Make sure you have pypi token for this [PyPI repo](https://pypi.org/project/llm-toolkit/).
+
```

### Comparing `llm_toolkit-0.1.1/llmtune/data/dataset_generator.py` & `llm_toolkit-0.1.2/llmtune/data/dataset_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
-from os.path import join, exists
+import pickle
+import re
 from functools import partial
+from os.path import exists, join
 from typing import Tuple, Union
-import pickle
 
-import re
 from datasets import Dataset
 
 from llmtune.data.ingestor import Ingestor, get_ingestor
 
 
 class DatasetGenerator:
     def __init__(
@@ -57,20 +57,16 @@
         if not is_test:
             test_mapping = {self.test_column: example[self.test_column]}
             example["formatted_prompt"] += self.prompt_stub.format(**test_mapping)
 
         return example
 
     def _format_prompts(self):
-        self.dataset["train"] = self.dataset["train"].map(
-            partial(self._format_one_prompt, is_test=False)
-        )
-        self.dataset["test"] = self.dataset["test"].map(
-            partial(self._format_one_prompt, is_test=True)
-        )
+        self.dataset["train"] = self.dataset["train"].map(partial(self._format_one_prompt, is_test=False))
+        self.dataset["test"] = self.dataset["test"].map(partial(self._format_one_prompt, is_test=True))
 
     def get_dataset(self) -> Tuple[Dataset, Dataset]:
         self._train_test_split()
         self._format_prompts()
 
         return self.dataset["train"], self.dataset["test"]
```

### Comparing `llm_toolkit-0.1.1/llmtune/data/ingestor.py` & `llm_toolkit-0.1.2/llmtune/data/ingestor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,23 @@
+import csv
 from abc import ABC, abstractmethod
-from functools import partial
 
 import ijson
-import csv
-from datasets import Dataset, load_dataset, concatenate_datasets
+from datasets import Dataset, concatenate_datasets, load_dataset
 
 
 def get_ingestor(data_type: str):
     if data_type == "json":
         return JsonIngestor
     elif data_type == "csv":
         return CsvIngestor
     elif data_type == "huggingface":
         return HuggingfaceIngestor
     else:
-        raise ValueError(
-            f"'type' must be one of 'json', 'csv', or 'huggingface', you have {data_type}"
-        )
+        raise ValueError(f"'type' must be one of 'json', 'csv', or 'huggingface', you have {data_type}")
 
 
 class Ingestor(ABC):
     @abstractmethod
     def to_dataset(self) -> Dataset:
         pass
```

### Comparing `llm_toolkit-0.1.1/llmtune/finetune/lora.py` & `llm_toolkit-0.1.2/llmtune/finetune/lora.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-from os.path import join, exists
-from typing import Tuple
-
-import torch
+from os.path import join
 
 import bitsandbytes as bnb
+import torch
 from datasets import Dataset
+from peft import (
+    LoraConfig,
+    get_peft_model,
+    prepare_model_for_kbit_training,
+)
 from transformers import (
-    AutoTokenizer,
     AutoModelForCausalLM,
-    BitsAndBytesConfig,
-    TrainingArguments,
     AutoTokenizer,
+    BitsAndBytesConfig,
     ProgressCallback,
-)
-from peft import (
-    prepare_model_for_kbit_training,
-    get_peft_model,
-    LoraConfig,
+    TrainingArguments,
 )
 from trl import SFTTrainer
-from rich.console import Console
 
-
-from llmtune.pydantic_models.config_model import Config
-from llmtune.utils.save_utils import DirectoryHelper
 from llmtune.finetune.generics import Finetune
+from llmtune.pydantic_models.config_model import Config
 from llmtune.ui.rich_ui import RichUI
+from llmtune.utils.save_utils import DirectoryHelper
 
 
 class LoRAFinetune(Finetune):
     def __init__(self, config: Config, directory_helper: DirectoryHelper):
         self.config = config
 
         self._model_config = config.model
@@ -95,17 +90,15 @@
     def _inject_lora(self):
         if not self.config.accelerate:
             self.model.gradient_checkpointing_enable()
             self.model = prepare_model_for_kbit_training(self.model)
         self.model = get_peft_model(self.model, self._lora_config)
 
         if not self.config.accelerate:
-            self.optimizer = bnb.optim.Adam8bit(
-                self.model.parameters(), lr=self._training_args.learning_rate
-            )
+            self.optimizer = bnb.optim.Adam8bit(self.model.parameters(), lr=self._training_args.learning_rate)
             self.lr_scheduler = torch.optim.lr_scheduler.ConstantLR(self.optimizer)
         if self.config.accelerate:
             self.model, self.optimizer, self.lr_scheduler = self.accelerator.prepare(
                 self.model, self.optimizer, self.lr_scheduler
             )
 
     def finetune(self, train_dataset: Dataset):
@@ -128,12 +121,12 @@
             args=training_args,
             dataset_text_field="formatted_prompt",  # TODO: maybe move consts to a dedicated folder
             callbacks=[progress_callback],
             # optimizers=[self.optimizer, self.lr_scheduler],
             **self._sft_args.model_dump(),
         )
 
-        trainer_stats = self._trainer.train()
+        self._trainer.train()
 
     def save_model(self) -> None:
         self._trainer.model.save_pretrained(self._weights_path)
         self.tokenizer.save_pretrained(self._weights_path)
```

### Comparing `llm_toolkit-0.1.1/llmtune/inference/lora.py` & `llm_toolkit-0.1.2/llmtune/inference/lora.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,22 @@
+import csv
 import os
 from os.path import join
 from threading import Thread
-import csv
 
-from transformers import TextIteratorStreamer
-from rich.text import Text
+import torch
 from datasets import Dataset
-from transformers import AutoTokenizer, BitsAndBytesConfig
 from peft import AutoPeftModelForCausalLM
-import torch
-
+from rich.text import Text
+from transformers import AutoTokenizer, BitsAndBytesConfig, TextIteratorStreamer
 
-from llmtune.pydantic_models.config_model import Config
-from llmtune.utils.save_utils import DirectoryHelper
 from llmtune.inference.generics import Inference
+from llmtune.pydantic_models.config_model import Config
 from llmtune.ui.rich_ui import RichUI
+from llmtune.utils.save_utils import DirectoryHelper
 
 
 # TODO: Add type hints please!
 class LoRAInference(Inference):
     def __init__(
         self,
         test_dataset: Dataset,
@@ -31,97 +29,81 @@
         self.config = config
 
         self.save_dir = dir_helper.save_paths.results
         self.save_path = join(self.save_dir, "results.csv")
         self.device_map = self.config.model.device_map
         self._weights_path = dir_helper.save_paths.weights
 
-        self.model, self.tokenizer = self._get_merged_model(
-            dir_helper.save_paths.weights
-        )
+        self.model, self.tokenizer = self._get_merged_model(dir_helper.save_paths.weights)
 
     def _get_merged_model(self, weights_path: str):
         # purge VRAM
         torch.cuda.empty_cache()
 
         # Load from path
         dtype = (
             torch.float16
             if self.config.training.training_args.fp16
-            else (
-                torch.bfloat16
-                if self.config.training.training_args.bf16
-                else torch.float32
-            )
+            else (torch.bfloat16 if self.config.training.training_args.bf16 else torch.float32)
         )
 
         self.model = AutoPeftModelForCausalLM.from_pretrained(
             weights_path,
             torch_dtype=dtype,
             device_map=self.device_map,
-            quantization_config=(
-                BitsAndBytesConfig(**self.config.model.bitsandbytes.model_dump())
-            ),
+            quantization_config=(BitsAndBytesConfig(**self.config.model.bitsandbytes.model_dump())),
         )
 
         """TODO: figure out multi-gpu
         if self.config.accelerate:
             self.model = self.accelerator.prepare(self.model)
         """
 
         model = self.model.merge_and_unload()
 
-        tokenizer = AutoTokenizer.from_pretrained(
-            self._weights_path, device_map=self.device_map
-        )
+        tokenizer = AutoTokenizer.from_pretrained(self._weights_path, device_map=self.device_map)
 
         return model, tokenizer
 
     def infer_all(self):
         results = []
         prompts = self.test_dataset["formatted_prompt"]
         labels = self.test_dataset[self.label_column]
 
         # inference loop
         for idx, (prompt, label) in enumerate(zip(prompts, labels)):
-            RichUI.inference_ground_truth_display(
-                f"Generating on test set: {idx+1}/{len(prompts)}", prompt, label
-            )
+            RichUI.inference_ground_truth_display(f"Generating on test set: {idx+1}/{len(prompts)}", prompt, label)
 
             try:
                 result = self.infer_one(prompt)
-            except:
+            except Exception:
                 continue
             results.append((prompt, label, result))
 
         # TODO: seperate this into another method
         header = ["Prompt", "Ground Truth", "Predicted"]
         os.makedirs(self.save_dir, exist_ok=True)
         with open(self.save_path, "w", newline="") as f:
             writer = csv.writer(f)
             writer.writerow(header)
             for row in results:
                 writer.writerow(row)
 
     def infer_one(self, prompt: str) -> str:
-        input_ids = self.tokenizer(
-            prompt, return_tensors="pt", truncation=True
-        ).input_ids.cuda()
+        input_ids = self.tokenizer(prompt, return_tensors="pt", truncation=True).input_ids.cuda()
 
         # stream processor
         streamer = TextIteratorStreamer(
             self.tokenizer,
             skip_prompt=True,
             decode_kwargs={"skip_special_tokens": True},
             timeout=60,  # 60 sec timeout for generation; to handle OOM errors
         )
 
-        generation_kwargs = dict(
-            input_ids=input_ids, streamer=streamer, **self.config.inference.model_dump()
-        )
+        generation_kwargs = dict(input_ids=input_ids, streamer=streamer, **self.config.inference.model_dump())
 
         thread = Thread(target=self.model.generate, kwargs=generation_kwargs)
         thread.start()
 
         result = Text()
         with RichUI.inference_stream_display(result) as live:
             for new_text in streamer:
```

### Comparing `llm_toolkit-0.1.1/llmtune/pydantic_models/config_model.py` & `llm_toolkit-0.1.2/llmtune/pydantic_models/config_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-from typing import Literal, Union, List, Dict, Optional
-from pydantic import BaseModel, FilePath, validator, Field
-
-from huggingface_hub.utils import validate_repo_id
+from typing import List, Literal, Optional, Union
 
 import torch
+from pydantic import BaseModel, Field, FilePath, validator
+
 
 # TODO: Refactor this into multiple files...
 HfModelPath = str
 
+
 class QaConfig(BaseModel):
-    llm_tests: Optional[List[str]] = Field([], description = "list of tests that needs to be connected")
-    
+    llm_tests: Optional[List[str]] = Field([], description="list of tests that needs to be connected")
+
 
 class DataConfig(BaseModel):
-    file_type: Literal["json", "csv", "huggingface"] = Field(
-        None, description="File type"
-    )
-    path: Union[FilePath, HfModelPath] = Field(
-        None, description="Path to the file or HuggingFace model"
-    )
-    prompt: str = Field(
-        None, description="Prompt for the model. Use {} brackets for column name"
-    )
+    file_type: Literal["json", "csv", "huggingface"] = Field(None, description="File type")
+    path: Union[FilePath, HfModelPath] = Field(None, description="Path to the file or HuggingFace model")
+    prompt: str = Field(None, description="Prompt for the model. Use {} brackets for column name")
     prompt_stub: str = Field(
         None,
         description="Stub for the prompt; this is injected during training. Use {} brackets for column name",
     )
     train_size: Optional[Union[float, int]] = Field(
         0.9,
         description="Size of the training set; float for proportion and int for # of examples",
@@ -44,30 +38,26 @@
     #     if "file_type" in values and values["file_type"] == "huggingface":
     #         if not validate_repo_id(v):
     #             raise ValueError("Invalid HuggingFace dataset path")
     #     return v
 
 
 class BitsAndBytesConfig(BaseModel):
-    load_in_8bit: Optional[bool] = Field(
-        False, description="Enable 8-bit quantization with LLM.int8()"
-    )
+    load_in_8bit: Optional[bool] = Field(False, description="Enable 8-bit quantization with LLM.int8()")
     llm_int8_threshold: Optional[float] = Field(
         6.0, description="Outlier threshold for outlier detection in 8-bit quantization"
     )
     llm_int8_skip_modules: Optional[List[str]] = Field(
         None, description="List of modules that we do not want to convert in 8-bit"
     )
     llm_int8_enable_fp32_cpu_offload: Optional[bool] = Field(
         False,
         description="Enable splitting model parts between int8 on GPU and fp32 on CPU",
     )
-    llm_int8_has_fp16_weight: Optional[bool] = Field(
-        False, description="Run LLM.int8() with 16-bit main weights"
-    )
+    llm_int8_has_fp16_weight: Optional[bool] = Field(False, description="Run LLM.int8() with 16-bit main weights")
 
     load_in_4bit: Optional[bool] = Field(
         True,
         description="Enable 4-bit quantization by replacing the Linear layers with FP4/NF4 layers from bitsandbytes",
     )
     bnb_4bit_compute_dtype: Optional[str] = Field(
         torch.bfloat16, description="Computational type for 4-bit quantization"
@@ -82,22 +72,18 @@
 
 
 class ModelConfig(BaseModel):
     hf_model_ckpt: Optional[str] = Field(
         "NousResearch/Llama-2-7b-hf",
         description="Path to the model (huggingface repo or local path)",
     )
-    device_map: Optional[str] = Field(
-        "auto", description="device onto which to load the model"
-    )
+    device_map: Optional[str] = Field("auto", description="device onto which to load the model")
 
     quantize: Optional[bool] = Field(False, description="Flag to enable quantization")
-    bitsandbytes: BitsAndBytesConfig = Field(
-        None, description="Bits and Bytes configuration"
-    )
+    bitsandbytes: BitsAndBytesConfig = Field(None, description="Bits and Bytes configuration")
 
     # @validator("hf_model_ckpt")
     # def validate_model(cls, v, **kwargs):
     #     if not validate_repo_id(v):
     #         raise ValueError("Invalid HuggingFace dataset path")
     #     return v
 
@@ -112,73 +98,53 @@
         if v.lower() == "none":
             return None
         return v
 
 
 class LoraConfig(BaseModel):
     r: Optional[int] = Field(8, description="Lora rank")
-    task_type: Optional[str] = Field(
-        "CAUSAL_LM", description="Base Model task type during training"
-    )
+    task_type: Optional[str] = Field("CAUSAL_LM", description="Base Model task type during training")
 
-    lora_alpha: Optional[int] = Field(
-        16, description="The alpha parameter for Lora scaling"
-    )
-    bias: Optional[str] = Field(
-        "none", description="Bias type for Lora. Can be 'none', 'all' or 'lora_only'"
-    )
-    lora_dropout: Optional[float] = Field(
-        0.1, description="The dropout probability for Lora layers"
-    )
-    target_modules: Optional[List[str]] = Field(
-        None, description="The names of the modules to apply Lora to"
-    )
+    lora_alpha: Optional[int] = Field(16, description="The alpha parameter for Lora scaling")
+    bias: Optional[str] = Field("none", description="Bias type for Lora. Can be 'none', 'all' or 'lora_only'")
+    lora_dropout: Optional[float] = Field(0.1, description="The dropout probability for Lora layers")
+    target_modules: Optional[List[str]] = Field(None, description="The names of the modules to apply Lora to")
     fan_in_fan_out: Optional[bool] = Field(
         False,
         description="Flag to indicate if the layer to replace stores weight like (fan_in, fan_out)",
     )
     modules_to_save: Optional[List[str]] = Field(
         None,
         description="List of modules apart from LoRA layers to be set as trainable and saved in the final checkpoint",
     )
-    layers_to_transform: Optional[Union[List[int], int]] = Field(
-        None, description="The layer indexes to transform"
-    )
+    layers_to_transform: Optional[Union[List[int], int]] = Field(None, description="The layer indexes to transform")
     layers_pattern: Optional[str] = Field(None, description="The layer pattern name")
     # rank_pattern: Optional[Dict[str, int]] = Field(
     #     {}, description="The mapping from layer names or regexp expression to ranks"
     # )
     # alpha_pattern: Optional[Dict[str, int]] = Field(
     #     {}, description="The mapping from layer names or regexp expression to alphas"
     # )
 
 
 # TODO: Get comprehensive Args!
 class TrainingArgs(BaseModel):
     num_train_epochs: Optional[int] = Field(1, description="Number of training epochs")
-    per_device_train_batch_size: Optional[int] = Field(
-        1, description="Batch size per training device"
-    )
-    gradient_accumulation_steps: Optional[int] = Field(
-        1, description="Number of steps for gradient accumulation"
-    )
-    gradient_checkpointing: Optional[bool] = Field(
-        True, description="Flag to enable gradient checkpointing"
-    )
+    per_device_train_batch_size: Optional[int] = Field(1, description="Batch size per training device")
+    gradient_accumulation_steps: Optional[int] = Field(1, description="Number of steps for gradient accumulation")
+    gradient_checkpointing: Optional[bool] = Field(True, description="Flag to enable gradient checkpointing")
     optim: Optional[str] = Field("paged_adamw_32bit", description="Optimizer")
     logging_steps: Optional[int] = Field(100, description="Number of logging steps")
     learning_rate: Optional[float] = Field(2.0e-4, description="Learning rate")
     bf16: Optional[bool] = Field(False, description="Flag to enable bf16")
     tf32: Optional[bool] = Field(False, description="Flag to enable tf32")
     fp16: Optional[bool] = Field(False, description="Flag to enable fp16")
     max_grad_norm: Optional[float] = Field(0.3, description="Maximum gradient norm")
     warmup_ratio: Optional[float] = Field(0.03, description="Warmup ratio")
-    lr_scheduler_type: Optional[str] = Field(
-        "constant", description="Learning rate scheduler type"
-    )
+    lr_scheduler_type: Optional[str] = Field("constant", description="Learning rate scheduler type")
 
 
 # TODO: Get comprehensive Args!
 class SftArgs(BaseModel):
     max_seq_length: Optional[int] = Field(None, description="Maximum sequence length")
     neftune_noise_alpha: Optional[float] = Field(
         None,
```

### Comparing `llm_toolkit-0.1.1/llmtune/qa/generics.py` & `llm_toolkit-0.1.2/llmtune/qa/generics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+import statistics
 from abc import ABC, abstractmethod
-from typing import Union, List, Tuple, Dict
+from typing import Dict, List, Union
+
 import pandas as pd
+
 from llmtune.ui.rich_ui import RichUI
-import statistics
-from llmtune.qa.qa_tests import *
 
 
 class LLMQaTest(ABC):
     @property
     @abstractmethod
     def test_name(self) -> str:
         pass
 
     @abstractmethod
-    def get_metric(
-        self, prompt: str, grount_truth: str, model_pred: str
-    ) -> Union[float, int, bool]:
+    def get_metric(self, prompt: str, grount_truth: str, model_pred: str) -> Union[float, int, bool]:
         pass
 
 
 class QaTestRegistry:
     registry = {}
 
     @classmethod
@@ -28,64 +27,54 @@
             for name in names:
                 cls.registry[name] = wrapped_class
             return wrapped_class
 
         return inner_wrapper
 
     @classmethod
-    def create_tests_from_list(cls, test_name: str) -> List[LLMQaTest]:
+    def create_tests_from_list(cls, test_names: List[str]) -> List[LLMQaTest]:
         return [cls.create_test(test) for test in test_names]
 
 
 class LLMTestSuite:
     def __init__(
         self,
         tests: List[LLMQaTest],
         prompts: List[str],
         ground_truths: List[str],
         model_preds: List[str],
     ) -> None:
-
         self.tests = tests
         self.prompts = prompts
         self.ground_truths = ground_truths
         self.model_preds = model_preds
 
         self.test_results = {}
 
     def run_tests(self) -> Dict[str, List[Union[float, int, bool]]]:
         test_results = {}
         for test in zip(self.tests):
             metrics = []
-            for prompt, ground_truth, model_pred in zip(
-                self.prompts, self.ground_truths, self.model_preds
-            ):
+            for prompt, ground_truth, model_pred in zip(self.prompts, self.ground_truths, self.model_preds):
                 metrics.append(test.get_metric(prompt, ground_truth, model_pred))
             test_results[test.test_name] = metrics
 
         self.test_results = test_results
         return test_results
 
     @property
     def test_results(self):
         return self.test_results if self.test_results else self.run_tests()
 
     def print_test_results(self):
         result_dictionary = self.test_results()
-        column_data = {
-            key: [value for value in result_dictionary[key]]
-            for key in result_dictionary
-        }
+        column_data = {key: list(result_dictionary[key]) for key in result_dictionary}
         mean_values = {key: statistics.mean(column_data[key]) for key in column_data}
-        median_values = {
-            key: statistics.median(column_data[key]) for key in column_data
-        }
+        median_values = {key: statistics.median(column_data[key]) for key in column_data}
         stdev_values = {key: statistics.stdev(column_data[key]) for key in column_data}
         # Use the RichUI class to display the table
-        RichUI.display_table(
-            result_dictionary, mean_values, median_values, stdev_values
-        )
+        RichUI.display_table(result_dictionary, mean_values, median_values, stdev_values)
 
     def save_test_results(self, path: str):
         # TODO: save these!
         resultant_dataframe = pd.DataFrame(self.test_results())
         resultant_dataframe.to_csv(path, index=False)
```

### Comparing `llm_toolkit-0.1.1/llmtune/qa/qa_tests.py` & `llm_toolkit-0.1.2/llmtune/qa/qa_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from llmtune.qa.generics import LLMQaTest
-from typing import Union, List, Tuple, Dict
-import torch
-from transformers import DistilBertModel, DistilBertTokenizer
+from typing import List, Union
+
 import nltk
 import numpy as np
-from rouge_score import rouge_scorer
+import torch
+from nltk import pos_tag
 from nltk.corpus import stopwords
 from nltk.tokenize import word_tokenize
-from nltk import pos_tag
-from llmtune.qa.generics import TestRegistry
+from rouge_score import rouge_scorer
+from transformers import DistilBertModel, DistilBertTokenizer
+
+from llmtune.qa.generics import LLMQaTest, TestRegistry
+
 
 model_name = "distilbert-base-uncased"
 tokenizer = DistilBertTokenizer.from_pretrained(model_name)
 model = DistilBertModel.from_pretrained(model_name)
 
 nltk.download("stopwords")
 nltk.download("punkt")
@@ -21,29 +23,25 @@
 
 @TestRegistry.register("summary_length")
 class LengthTest(LLMQaTest):
     @property
     def test_name(self) -> str:
         return "summary_length"
 
-    def get_metric(
-        self, prompt: str, ground_truth: str, model_prediction: str
-    ) -> Union[float, int, bool]:
+    def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         return abs(len(ground_truth) - len(model_prediction))
 
 
 @TestRegistry.register("jaccard_similarity")
 class JaccardSimilarityTest(LLMQaTest):
     @property
     def test_name(self) -> str:
         return "jaccard_similarity"
 
-    def get_metric(
-        self, prompt: str, ground_truth: str, model_prediction: str
-    ) -> Union[float, int, bool]:
+    def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         set_ground_truth = set(ground_truth.lower())
         set_model_prediction = set(model_prediction.lower())
 
         intersection_size = len(set_ground_truth.intersection(set_model_prediction))
         union_size = len(set_ground_truth.union(set_model_prediction))
 
         similarity = intersection_size / union_size if union_size != 0 else 0
@@ -58,34 +56,28 @@
 
     def _encode_sentence(self, sentence):
         tokens = tokenizer(sentence, return_tensors="pt")
         with torch.no_grad():
             outputs = model(**tokens)
         return outputs.last_hidden_state.mean(dim=1).squeeze().numpy()
 
-    def get_metric(
-        self, prompt: str, ground_truth: str, model_prediction: str
-    ) -> Union[float, int, bool]:
+    def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         embedding_ground_truth = self._encode_sentence(ground_truth)
         embedding_model_prediction = self._encode_sentence(model_prediction)
-        dot_product_similarity = np.dot(
-            embedding_ground_truth, embedding_model_prediction
-        )
+        dot_product_similarity = np.dot(embedding_ground_truth, embedding_model_prediction)
         return dot_product_similarity
 
 
 @TestRegistry.register("rouge_score")
 class RougeScoreTest(LLMQaTest):
     @property
     def test_name(self) -> str:
         return "rouge_score"
 
-    def get_metric(
-        self, prompt: str, ground_truth: str, model_prediction: str
-    ) -> Union[float, int, bool]:
+    def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         scorer = rouge_scorer.RougeScorer(["rouge1"], use_stemmer=True)
         scores = scorer.score(model_prediction, ground_truth)
         return float(scores["rouge1"].precision)
 
 
 @TestRegistry.register("word_overlap")
 class WordOverlapTest(LLMQaTest):
@@ -95,17 +87,15 @@
 
     def _remove_stopwords(self, text: str) -> str:
         stop_words = set(stopwords.words("english"))
         word_tokens = word_tokenize(text)
         filtered_text = [word for word in word_tokens if word.lower() not in stop_words]
         return " ".join(filtered_text)
 
-    def get_metric(
-        self, prompt: str, ground_truth: str, model_prediction: str
-    ) -> Union[float, int, bool]:
+    def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         cleaned_model_prediction = self._remove_stopwords(model_prediction)
         cleaned_ground_truth = self._remove_stopwords(ground_truth)
 
         words_model_prediction = set(cleaned_model_prediction.split())
         words_ground_truth = set(cleaned_ground_truth.split())
 
         common_words = words_model_prediction.intersection(words_ground_truth)
@@ -124,43 +114,35 @@
 
 @TestRegistry.register("verb_percent")
 class VerbPercent(PosCompositionTest):
     @property
     def test_name(self) -> str:
         return "verb_percent"
 
-    def get_metric(
-        self, prompt: str, ground_truth: str, model_prediction: str
-    ) -> float:
-        return self._get_pos_percent(
-            model_prediction, ["VB", "VBD", "VBG", "VBN", "VBP", "VBZ"]
-        )
+    def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> float:
+        return self._get_pos_percent(model_prediction, ["VB", "VBD", "VBG", "VBN", "VBP", "VBZ"])
 
 
 @TestRegistry.register("adjective_percent")
 class AdjectivePercent(PosCompositionTest):
     @property
     def test_name(self) -> str:
         return "adjective_percent"
 
-    def get_metric(
-        self, prompt: str, ground_truth: str, model_prediction: str
-    ) -> float:
+    def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> float:
         return self._get_pos_percent(model_prediction, ["JJ", "JJR", "JJS"])
 
 
 @TestRegistry.register("noun_percent")
 class NounPercent(PosCompositionTest):
     @property
     def test_name(self) -> str:
         return "noun_percent"
 
-    def get_metric(
-        self, prompt: str, ground_truth: str, model_prediction: str
-    ) -> float:
+    def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> float:
         return self._get_pos_percent(model_prediction, ["NN", "NNS", "NNP", "NNPS"])
 
 
 # Instantiate tests
 # length_test = LengthTest()
 # jaccard_similarity_test = JaccardSimilarityTest()
 # dot_product_similarity_test = DotProductSimilarityTest()
```

### Comparing `llm_toolkit-0.1.1/llmtune/ui/generics.py` & `llm_toolkit-0.1.2/llmtune/ui/generics.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         pass
 
     @abstractstaticmethod
     def finetune_found(weights_path: str):
         pass
 
     """
-    INFERENCE 
+    INFERENCE
     """
 
     # Lifecycle functions
     @abstractstaticmethod
     def before_inference():
         pass
 
@@ -87,15 +87,15 @@
         pass
 
     @abstractstaticmethod
     def inference_stream_display(text: Text):
         pass
 
     """
-    QA 
+    QA
     """
 
     # Lifecycle functions
     @abstractstaticmethod
     def before_qa(cls):
         pass
```

### Comparing `llm_toolkit-0.1.1/llmtune/ui/rich_ui.py` & `llm_toolkit-0.1.2/llmtune/ui/rich_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from datasets import Dataset
-
 from rich.console import Console
 from rich.layout import Layout
+from rich.live import Live
 from rich.panel import Panel
 from rich.table import Table
-from rich.live import Live
 from rich.text import Text
 
 from llmtune.ui.generics import UI
 from llmtune.utils.rich_print_utils import inject_example_to_rich_layout
 
+
 console = Console()
 
 
 class StatusContext:
     def __init__(self, console, message, spinner):
         self.console = console
         self.message = message
@@ -21,17 +21,15 @@
 
     def __enter__(self):
         self.task = self.console.status(self.message, spinner=self.spinner)
         self.task.__enter__()  # Manually enter the console status context
         return self  # This allows you to use variables from this context if needed
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.task.__exit__(
-            exc_type, exc_val, exc_tb
-        )  # Cleanly exit the console status context
+        self.task.__exit__(exc_type, exc_val, exc_tb)  # Cleanly exit the console status context
 
 
 class LiveContext:
     def __init__(self, text: Text, refresh_per_second=4, vertical_overflow="visible"):
         self.console = console
         self.text = text
         self.refresh_per_second = refresh_per_second
@@ -43,17 +41,15 @@
             refresh_per_second=self.refresh_per_second,
             vertical_overflow=self.vertical_overflow,
         )
         self.task.__enter__()  # Manually enter the console status context
         return self  # This allows you to use variables from this context if needed
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.task.__exit__(
-            exc_type, exc_val, exc_tb
-        )  # Cleanly exit the console status context
+        self.task.__exit__(exc_type, exc_val, exc_tb)  # Cleanly exit the console status context
 
     def update(self, new_text: Text):
         self.task.update(new_text)
 
 
 class RichUI(UI):
     """
@@ -68,15 +64,15 @@
     @staticmethod
     def during_dataset_creation(message: str, spinner: str):
         return StatusContext(console, message, spinner)
 
     @staticmethod
     def after_dataset_creation(save_dir: str, train: Dataset, test: Dataset):
         console.print(f"Dataset Saved at {save_dir}")
-        console.print(f"Post-Split data size:")
+        console.print("Post-Split data size:")
         console.print(f"Train: {len(train)}")
         console.print(f"Test: {len(test)}")
 
     @staticmethod
     def dataset_found(save_dir: str):
         console.print(f"Loading formatted dataset from directory {save_dir}")
 
@@ -89,17 +85,15 @@
             Layout(
                 Panel("Inference Sample"),
                 name="inference",
             ),
         )
 
         inject_example_to_rich_layout(layout["train"], "Train Example", train_row)
-        inject_example_to_rich_layout(
-            layout["inference"], "Inference Example", test_row
-        )
+        inject_example_to_rich_layout(layout["inference"], "Inference Example", test_row)
 
         console.print(layout)
 
     """
     FINETUNING
     """
 
@@ -118,22 +112,22 @@
 
     @staticmethod
     def during_finetune():
         return StatusContext(console, "Finetuning Model...", "runner")
 
     @staticmethod
     def after_finetune():
-        console.print(f"Finetuning complete!")
+        console.print("Finetuning complete!")
 
     @staticmethod
     def finetune_found(weights_path: str):
         console.print(f"Fine-Tuned Model Found at {weights_path}... skipping training")
 
     """
-    INFERENCE 
+    INFERENCE
     """
 
     # Lifecycle functions
     @staticmethod
     def before_inference():
         console.rule("[bold pink]:face_with_monocle: Testing")
 
@@ -163,15 +157,15 @@
 
     @staticmethod
     def inference_stream_display(text: Text):
         console.print("[bold red]Prediction >")
         return LiveContext(text)
 
     """
-    QA 
+    QA
     """
 
     # Lifecycle functions
     @staticmethod
     def before_qa():
         pass
 
@@ -184,18 +178,15 @@
         pass
 
     @staticmethod
     def qa_found():
         pass
 
     @staticmethod
-    def qa_display_table(
-        self, result_dictionary, mean_values, median_values, stdev_values
-    ):
-
+    def qa_display_table(self, result_dictionary, mean_values, median_values, stdev_values):
         # Create a table
         table = Table(show_header=True, header_style="bold", title="Test Results")
 
         # Add columns to the table
         table.add_column("Metric", style="cyan")
         table.add_column("Mean", style="magenta")
         table.add_column("Median", style="green")
```

### Comparing `llm_toolkit-0.1.1/llmtune/utils/ablation_utils.py` & `llm_toolkit-0.1.2/llmtune/utils/ablation_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 import copy
 import itertools
-from typing import List, Type, Any, Dict, Optional, Union, Tuple
-from typing import get_args, get_origin, get_type_hints
-
-import yaml
+from typing import Dict, Tuple, Union, get_args, get_origin
 
 
 # TODO: organize this a little bit. It's a bit of a mess rn.
 
 """
 Helper functions to create multiple valid configs based on ablation (i.e. list of values)
 fron a single config yaml
 """
 
 
-def get_types_from_dict(
-    source_dict: dict, root="", type_dict={}
-) -> Dict[str, Tuple[type, type]]:
+def get_types_from_dict(source_dict: dict, root="", type_dict={}) -> Dict[str, Tuple[type, type]]:
     for key, val in source_dict.items():
-        if type(val) is not dict:
+        if not isinstance(val, dict):
             attr = f"{root}.{key}" if root else key
-            tp = (
-                (type(val), None)
-                if type(val) is not list
-                else (type(val), type(val[0]))
-            )
+            tp = (type(val), None) if not isinstance(val, list) else (type(val), type(val[0]))
             type_dict[attr] = tp
         else:
             join_array = [root, key] if root else [key]
             new_root = ".".join(join_array)
             get_types_from_dict(val, new_root, type_dict)
 
     return type_dict
```

### Comparing `llm_toolkit-0.1.1/llmtune/utils/rich_print_utils.py` & `llm_toolkit-0.1.2/llmtune/utils/rich_print_utils.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from rich.panel import Panel
 from rich.layout import Layout
-from rich.text import Text
+from rich.panel import Panel
 from rich.table import Table
+from rich.text import Text
 
 
 def inject_example_to_rich_layout(layout: Layout, layout_name: str, example: dict):
     example = example.copy()
 
     # Crate Table
     table = Table(expand=True)
```

### Comparing `llm_toolkit-0.1.1/llmtune/utils/save_utils.py` & `llm_toolkit-0.1.2/llmtune/utils/save_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
 Helper functions to help managing saving and loading of experiments:
     1. Generate save directory name
     2. Check if files are present at various experiment stages
 """
 
-import shutil
+import hashlib
 import os
-from os.path import exists
-import yaml
-
 import re
-import hashlib
-from functools import cached_property
 from dataclasses import dataclass
+from functools import cached_property
+from os.path import exists
 
+import yaml
 from sqids import Sqids
 
 from llmtune.pydantic_models.config_model import Config
 
+
 NUM_MD5_DIGITS_FOR_SQIDS = 5  # TODO: maybe move consts to a dedicated folder
 
 
 @dataclass
 class DirectoryList:
     save_dir: str
     config_hash: str
```

### Comparing `llm_toolkit-0.1.1/pyproject.toml` & `llm_toolkit-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 [tool.poetry]
 name = "llm-toolkit"
-version = "0.1.1"
+version = "0.1.2"
 description = "LLM Finetuning resource hub + toolkit"
 authors = ["Benjamin Ye <benjamin.ye@georgian.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "llmtune"}]
 
+[tool.poetry.scripts]
+llmtune = "llmtune.cli.toolkit:cli"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+
+[tool.poetry-dynamic-versioning.substitution]
+folders = [
+  { path = "llmtune" }
+]
+
 [tool.poetry.dependencies]
-python = ">=3.9, <=3.12.1"
+python = ">=3.9, <=3.12"
 transformers = "~4.37.2"
 datasets = "^2.17.0"
 peft = "^0.8.2"
 pandas = "^2.2.0"
 numpy = "^1.26.4"
 ipdb = "^0.13.13"
 evaluate = "^0.4.1"
@@ -39,13 +52,34 @@
 sqids = "^0.4.1"
 pydantic = "^2.6.1"
 typer = "^0.10.0"
 shellingham = "^1.5.4"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "^24.3.0"
-twine = "^5.0.0"
+ruff = "~0.3.5"
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
+
+[tool.ruff]
+lint.ignore = ["C901", "E501", "E741", "F402", "F823" ]
+lint.select = ["C", "E", "F", "I", "W"]
+line-length = 119
+exclude = [
+    "llama2",
+    "mistral",
+]
+
+
+[tool.ruff.lint.isort]
+lines-after-imports = 2
+known-first-party = ["llmtune"]
+
+[tool.ruff.format]
+quote-style = "double"
+indent-style = "space"
+skip-magic-trailing-comma = false
+line-ending = "auto"
+
+
```

### Comparing `llm_toolkit-0.1.1/PKG-INFO` & `llm_toolkit-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llm-toolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: LLM Finetuning resource hub + toolkit
 License: Apache 2.0
 Author: Benjamin Ye
 Author-email: benjamin.ye@georgian.io
-Requires-Python: >=3.9,<=3.12.1
+Requires-Python: >=3.9,<=3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: absl-py (>=2.1.0,<3.0.0)
 Requires-Dist: accelerate (>=0.27.0,<0.28.0)
 Requires-Dist: ai21 (>=2.0.3,<3.0.0)
 Requires-Dist: bitsandbytes (>=0.42.0,<0.43.0)
 Requires-Dist: datasets (>=2.17.0,<3.0.0)
 Requires-Dist: einops (>=0.7.0,<0.8.0)
 Requires-Dist: evaluate (>=0.4.1,<0.5.0)
@@ -56,74 +55,42 @@
 LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM finetuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
 
 <p align="center">
 <img src="assets/overview_diagram.png" width="900" />
 </p>
 
 ## Installation
-
-### Clone Repository
-
+### pipx (recommended)
+pipx installs the package and depdencies in a seperate virtual environment
 ```shell
-   git clone https://github.com/georgian-io/LLM-Finetuning-Hub.git
-   cd LLM-Finetuning-Hub/
+pipx install llm-toolkit
 ```
 
-### [Option 1] Docker (recommended)
-
+### pip
 ```shell
-   docker build -t llm-toolkit
+pip install llm-toolkit
 ```
 
-#### CPU Only
-
+### docker
 ```shell
-   docker run -it llm-toolkit
-```
-
-#### With GPU
-
-```shell
-   docker run -it --gpus all llm-toolkit
-```
-
-### [Option 2] Poetry (recommended)
-
-See poetry documentation page for poetry [installation instructions](https://python-poetry.org/docs/#installation)
-
-```shell
-   poetry install
-```
-
-### [Option 3] pip
-
-```shell
-   pip install -r requirements.txt
-```
-
-### [Option 4] Conda
-
-```shell
-   conda create --name llm-toolkit python=3.11
-   conda activate llm-toolkit
-   pip install -r requirements.txt
+docker pull ghcr.io/georgian-io/llm-toolkit:latest
 ```
 
 ## Quick Start
 
 This guide contains 3 stages that will enable you to get the most out of this toolkit!
 
 - **Basic**: Run your first LLM fine-tuning experiment
 - **Intermediate**: Run a custom experiment by changing the componenets of the YAML configuration file
 - **Advanced**: Launch series of fine-tuning experiments across different prompt templates, LLMs, optimization techniques -- all through **one** YAML configuration file
 
 ### Basic
 
 ```python
-   python toolkit.py --config ./config.yml
+   llmtune --config-path ./config.yml
 ```
 
 This command initiates the fine-tuning process using the settings specified in the default YAML configuration file `config.yaml`.
 
 ### Intermediate
 
 The configuration file is the central piece that defines the behavior of the toolkit. It is written in YAML format and consists of several sections that control different aspects of the process, such as data ingestion, model definition, training, inference, and quality assurance. We highlight some of the critical sections.
@@ -299,19 +266,77 @@
 2.  **Clone** the project to your own machine
 3.  **Commit** changes to your own branch
 4.  **Push** your work back up to your fork
 5.  Submit a **Pull request** so that we can review your changes
 
 NOTE: Be sure to merge the latest from "upstream" before making a pull request!
 
+### Set Up Dev Environment
+
+<details>
+<summary>1. Clone Repo</summary>
+  
+```shell
+   git clone https://github.com/georgian-io/LLM-Finetuning-Toolkit.git
+   cd LLM-Finetuning-Toolkit/
+```
 
-## Releasing
+</details>
+
+<details>
+<summary>2. Install Dependencies</summary>
+<details>
+<summary>Install with Docker [Recommended]</summary>
+
+```shell
+   docker build -t llm-toolkit
+```
+
+```shell
+   # CPU
+   docker run -it llm-toolkit
+   # GPU
+   docker run -it --gpus all llm-toolkit
+```
+</details>
+
+<details>
+<summary>Poetry (recommended)</summary>
+
+See poetry documentation page for poetry [installation instructions](https://python-poetry.org/docs/#installation)
+
+```shell
+   poetry install
+```
+</details>
+<details>
+<summary>pip</summary>
+We recommend using a virtual environment like `venv` or `conda` for installation
+
+```shell
+   pip install -e .
+```
+</details>
+</details>
+
+
+
+### Checklist Before Pull Request (Optional)
+
+1. Use `ruff check --fix` to check and fix lint errors
+2. Use `ruff format` to apply formatting
+
+NOTE: Ruff linting and formatting checks are done when PR is raised via Git Action. Before raising a PR, it is a good practice to check and fix lint errors, as well as apply formatting.
+
+
+### Releasing
 
 
 To manually release a PyPI package, please run: 
 
 ```shell
    make build-release
 ```
 
-Note: Make sure you have pypi token for this [pipy repo](https://pypi.org/project/llm-toolkit/).
+Note: Make sure you have pypi token for this [PyPI repo](https://pypi.org/project/llm-toolkit/).
+
```

