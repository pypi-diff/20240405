# Comparing `tmp/exxa-0.6.3.tar.gz` & `tmp/exxa-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exxa-0.6.3.tar", max compression
+gzip compressed data, was "exxa-0.6.4.tar", max compression
```

## Comparing `exxa-0.6.3.tar` & `exxa-0.6.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-09-05 13:16:45.129344 exxa-0.6.3/LICENSE
--rw-r--r--   0        0        0     1795 2024-03-21 04:44:42.578987 exxa-0.6.3/README.md
--rw-r--r--   0        0        0      153 2024-03-24 01:16:41.366825 exxa-0.6.3/exa/__init__.py
--rw-r--r--   0        0        0     1480 2024-03-21 05:07:34.122499 exxa-0.6.3/exa/cluster_init.py
--rw-r--r--   0        0        0      425 2024-03-29 01:57:40.237644 exxa-0.6.3/exa/structs/__init__.py
--rw-r--r--   0        0        0     2844 2024-03-22 00:41:41.130842 exxa-0.6.3/exa/structs/hive_model.py
--rw-r--r--   0        0        0     4857 2024-03-29 01:57:40.301118 exxa-0.6.3/exa/structs/model_thread_router.py
--rw-r--r--   0        0        0     2864 2024-03-29 02:14:43.881478 exxa-0.6.3/exa/structs/parallelize_models_gpus.py
--rw-r--r--   0        0        0     1042 2024-03-29 01:57:40.252866 exxa-0.6.3/exa/utils/__init__.py
--rw-r--r--   0        0        0     2362 2024-03-21 16:57:43.336672 exxa-0.6.3/exa/utils/all_reduce.py
--rw-r--r--   0        0        0      282 2024-03-21 20:40:43.468852 exxa-0.6.3/exa/utils/count_cores_for_workers.py
--rw-r--r--   0        0        0     1638 2024-03-21 16:57:43.336615 exxa-0.6.3/exa/utils/dist_process_init.py
--rw-r--r--   0        0        0     3393 2024-03-22 00:41:41.141207 exxa-0.6.3/exa/utils/fused_all_gather.py
--rw-r--r--   0        0        0     3964 2024-03-29 01:57:40.291762 exxa-0.6.3/exa/utils/gpu_ops.py
--rw-r--r--   0        0        0     1389 2024-03-29 02:14:51.933671 exxa-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 exxa-0.6.3/setup.py
--rw-r--r--   0        0        0     2710 1970-01-01 00:00:00.000000 exxa-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-09-05 13:16:45.129344 exxa-0.6.4/LICENSE
+-rw-r--r--   0        0        0     1789 2024-04-05 04:36:13.518437 exxa-0.6.4/README.md
+-rw-r--r--   0        0        0      153 2024-03-24 01:16:41.366825 exxa-0.6.4/exa/__init__.py
+-rw-r--r--   0        0        0     1480 2024-03-21 05:07:34.122499 exxa-0.6.4/exa/cluster_init.py
+-rw-r--r--   0        0        0      425 2024-03-29 01:57:40.237644 exxa-0.6.4/exa/structs/__init__.py
+-rw-r--r--   0        0        0     2844 2024-03-22 00:41:41.130842 exxa-0.6.4/exa/structs/hive_model.py
+-rw-r--r--   0        0        0     4857 2024-03-29 01:57:40.301118 exxa-0.6.4/exa/structs/model_thread_router.py
+-rw-r--r--   0        0        0     2864 2024-03-29 02:14:43.881478 exxa-0.6.4/exa/structs/parallelize_models_gpus.py
+-rw-r--r--   0        0        0     1042 2024-03-29 01:57:40.252866 exxa-0.6.4/exa/utils/__init__.py
+-rw-r--r--   0        0        0     2343 2024-04-05 04:35:32.553984 exxa-0.6.4/exa/utils/all_reduce.py
+-rw-r--r--   0        0        0      282 2024-03-21 20:40:43.468852 exxa-0.6.4/exa/utils/count_cores_for_workers.py
+-rw-r--r--   0        0        0     1638 2024-03-21 16:57:43.336615 exxa-0.6.4/exa/utils/dist_process_init.py
+-rw-r--r--   0        0        0     3393 2024-03-22 00:41:41.141207 exxa-0.6.4/exa/utils/fused_all_gather.py
+-rw-r--r--   0        0        0     3964 2024-03-29 01:57:40.291762 exxa-0.6.4/exa/utils/gpu_ops.py
+-rw-r--r--   0        0        0     1389 2024-04-05 04:36:30.109729 exxa-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     2609 1970-01-01 00:00:00.000000 exxa-0.6.4/setup.py
+-rw-r--r--   0        0        0     2704 1970-01-01 00:00:00.000000 exxa-0.6.4/PKG-INFO
```

### Comparing `exxa-0.6.3/LICENSE` & `exxa-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/README.md` & `exxa-0.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 ## Principles
 - Radical Simplicity (Utilizing super-powerful LLMs with as minimal lines of code as possible)
 - Ultra-Optimizated Peformance (High Performance code that extract all the power from these LLMs)
 - Fludity & Shapelessness (Plug in and play and re-architecture as you please)
 
 ---
 
-## 📦 Installation 📦
+## 📦 Install 📦
 ```bash
 $ pip3 install exxa
 ```
 -----
 
 
-
 ## Usage
```

### Comparing `exxa-0.6.3/exa/cluster_init.py` & `exxa-0.6.4/exa/cluster_init.py`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/exa/structs/hive_model.py` & `exxa-0.6.4/exa/structs/hive_model.py`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/exa/structs/model_thread_router.py` & `exxa-0.6.4/exa/structs/model_thread_router.py`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/exa/structs/parallelize_models_gpus.py` & `exxa-0.6.4/exa/structs/parallelize_models_gpus.py`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/exa/utils/__init__.py` & `exxa-0.6.4/exa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/exa/utils/all_reduce.py` & `exxa-0.6.4/exa/utils/all_reduce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 from torch import Tensor
 import torch.distributed as dist
-from exa.utils.dist_process_init import initialize_distributed
+# from exa.utils.dist_process_init import initialize_distributed
 
 
-initialize_distributed()
+# initialize_distributed()
 
 
 def fused_all_reduce_v1(tensor: Tensor, op=dist.ReduceOp.SUM):
     """
     Hyper-optimized fused all_reduce operation with reduced communication overhead.
     This version uses a ring-reduce approach to minimize the amount of data sent across the network.
 
@@ -57,16 +57,15 @@
     Args:
         tensor (Tensor): The input tensor to be reduced.
         op (dist.ReduceOp, optional): The reduction operation to be applied. Defaults to dist.ReduceOp.SUM.
 
     Returns:
         Tensor: The tensor after the all-reduce operation has been applied.
     """
-    initialize_distributed()
 
     # Use pytorch's built-in all_reduce
     return dist.all_reduce(tensor, op)
 
 
-x = torch.tensor([1, 2, 3, 4, 5], dtype=torch.float32)
-fused_all_reduce_v1(x)  # Output: tensor([ 1.,  2.,  3.,  4.,  5.])
-print(x)
+# x = torch.tensor([1, 2, 3, 4, 5], dtype=torch.float32)
+# fused_all_reduce_v1(x)  # Output: tensor([ 1.,  2.,  3.,  4.,  5.])
+# print(x)
```

### Comparing `exxa-0.6.3/exa/utils/dist_process_init.py` & `exxa-0.6.4/exa/utils/dist_process_init.py`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/exa/utils/fused_all_gather.py` & `exxa-0.6.4/exa/utils/fused_all_gather.py`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/exa/utils/gpu_ops.py` & `exxa-0.6.4/exa/utils/gpu_ops.py`

 * *Files identical despite different names*

### Comparing `exxa-0.6.3/pyproject.toml` & `exxa-0.6.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exxa"
-version = "0.6.3"
+version = "0.6.4"
 description = "Exa - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/Exa"
 documentation = "https://github.com/kyegomez/Exa"
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/Exa"
```

### Comparing `exxa-0.6.3/setup.py` & `exxa-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['loguru>=0.5.3,<0.6.0', 'torch>2.0.0']
 
 entry_points = \
 {'console_scripts': ['swarms = swarms.cli._cli:main']}
 
 setup_kwargs = {
     'name': 'exxa',
-    'version': '0.6.3',
+    'version': '0.6.4',
     'description': 'Exa - Pytorch',
-    'long_description': "[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Exa\nBoost your GPU's LLM performance by 300% on everyday GPU hardware, as validated by renowned developers, in just 5 minutes of setup and with no additional hardware costs.\n\n-----\n\n## Principles\n- Radical Simplicity (Utilizing super-powerful LLMs with as minimal lines of code as possible)\n- Ultra-Optimizated Peformance (High Performance code that extract all the power from these LLMs)\n- Fludity & Shapelessness (Plug in and play and re-architecture as you please)\n\n---\n\n## 📦 Installation 📦\n```bash\n$ pip3 install exxa\n```\n-----\n\n\n\n## Usage\n\n\n\n\n\n\n## 🎉 Features 🎉\n\n- **World-Class Quantization**: Get the most out of your models with top-tier performance and preserved accuracy! 🏋️\u200d♂️\n  \n- **Automated PEFT**: Simplify your workflow! Let our toolkit handle the optimizations. 🛠️\n\n- **LoRA Configuration**: Dive into the potential of flexible LoRA configurations, a game-changer for performance! 🌌\n\n- **Seamless Integration**: Designed to work seamlessly with popular models like LLAMA, Falcon, and more! 🤖\n\n----\n\n## 💌 Feedback & Contributions 💌\n\nWe're excited about the journey ahead and would love to have you with us! For feedback, suggestions, or contributions, feel free to open an issue or a pull request. Let's shape the future of fine-tuning together! 🌱\n\n[Check out our project board for our current backlog and features we're implementing](https://github.com/users/kyegomez/projects/8/views/2)\n\n\n# License\nMIT\n\n# Todo\n\n- Setup utils logger classes for metric logging with useful metadata such as token inference per second, latency, memory consumption\n- Add cuda c++ extensions for radically optimized classes for high performance quantization + inference on the edge\n\n\n\n",
+    'long_description': "[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Exa\nBoost your GPU's LLM performance by 300% on everyday GPU hardware, as validated by renowned developers, in just 5 minutes of setup and with no additional hardware costs.\n\n-----\n\n## Principles\n- Radical Simplicity (Utilizing super-powerful LLMs with as minimal lines of code as possible)\n- Ultra-Optimizated Peformance (High Performance code that extract all the power from these LLMs)\n- Fludity & Shapelessness (Plug in and play and re-architecture as you please)\n\n---\n\n## 📦 Install 📦\n```bash\n$ pip3 install exxa\n```\n-----\n\n\n## Usage\n\n\n\n\n\n\n## 🎉 Features 🎉\n\n- **World-Class Quantization**: Get the most out of your models with top-tier performance and preserved accuracy! 🏋️\u200d♂️\n  \n- **Automated PEFT**: Simplify your workflow! Let our toolkit handle the optimizations. 🛠️\n\n- **LoRA Configuration**: Dive into the potential of flexible LoRA configurations, a game-changer for performance! 🌌\n\n- **Seamless Integration**: Designed to work seamlessly with popular models like LLAMA, Falcon, and more! 🤖\n\n----\n\n## 💌 Feedback & Contributions 💌\n\nWe're excited about the journey ahead and would love to have you with us! For feedback, suggestions, or contributions, feel free to open an issue or a pull request. Let's shape the future of fine-tuning together! 🌱\n\n[Check out our project board for our current backlog and features we're implementing](https://github.com/users/kyegomez/projects/8/views/2)\n\n\n# License\nMIT\n\n# Todo\n\n- Setup utils logger classes for metric logging with useful metadata such as token inference per second, latency, memory consumption\n- Add cuda c++ extensions for radically optimized classes for high performance quantization + inference on the edge\n\n\n\n",
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/Exa',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `exxa-0.6.3/PKG-INFO` & `exxa-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exxa
-Version: 0.6.3
+Version: 0.6.4
 Summary: Exa - Pytorch
 Home-page: https://github.com/kyegomez/Exa
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
@@ -32,22 +32,21 @@
 ## Principles
 - Radical Simplicity (Utilizing super-powerful LLMs with as minimal lines of code as possible)
 - Ultra-Optimizated Peformance (High Performance code that extract all the power from these LLMs)
 - Fludity & Shapelessness (Plug in and play and re-architecture as you please)
 
 ---
 
-## 📦 Installation 📦
+## 📦 Install 📦
 ```bash
 $ pip3 install exxa
 ```
 -----
 
 
-
 ## Usage
```

