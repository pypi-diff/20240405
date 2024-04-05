# Comparing `tmp/falcon_challenge-0.2.5.tar.gz` & `tmp/falcon_challenge-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.2.5.tar", last modified: Wed Apr  3 15:08:22 2024, max compression
+gzip compressed data, was "falcon_challenge-0.2.7.tar", last modified: Fri Apr  5 20:40:38 2024, max compression
```

## Comparing `falcon_challenge-0.2.5.tar` & `falcon_challenge-0.2.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.240143 falcon_challenge-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 15:08:22.240143 falcon_challenge-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.232143 falcon_challenge-0.2.5/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/ndt2_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.236143 falcon_challenge-0.2.5/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    20507 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.236143 falcon_challenge-0.2.5/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.236143 falcon_challenge-0.2.5/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:08:22.240143 falcon_challenge-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.753359 falcon_challenge-0.2.7/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/ndt2_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/setup.py
```

### Comparing `falcon_challenge-0.2.5/LICENSE` & `falcon_challenge-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/PKG-INFO` & `falcon_challenge-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.5
+Version: 0.2.7
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.2.5/README.md` & `falcon_challenge-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/decoder_demos/decoding_utils.py` & `falcon_challenge-0.2.7/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/decoder_demos/filtering.py` & `falcon_challenge-0.2.7/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/decoder_demos/ndt2_decoder.py` & `falcon_challenge-0.2.7/decoder_demos/ndt2_decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 from falcon_challenge.interface import BCIDecoder
 
 from context_general_bci.utils import suppress_default_registry
 suppress_default_registry()
 from context_general_bci.config import RootConfig, propagate_config, DataKey, MetaKey
 from context_general_bci.dataset import DataAttrs, ContextAttrs
 from context_general_bci.subjects import SubjectName
-from context_general_bci.contexts.context_registry import context_registry
-from context_general_bci.contexts.context_info import FalconContextInfo, ExperimentalTask
+from context_general_bci.contexts.context_info import ExperimentalTask
 from context_general_bci.model import load_from_checkpoint
 from context_general_bci.model_slim import transfer_model
 
 def format_array_name(subject: str):
     return f'FALCON{subject}-M1'
 
 class NDT2Decoder(BCIDecoder):
@@ -34,32 +33,22 @@
 
     def __init__(
             self,
             task_config: FalconConfig,
             model_ckpt_path: str,
             model_cfg_stem: str,
             zscore_path: str,
+            dataset_handles: List[str] = []
         ):
         r"""
             Loading NDT2 requires both weights and model config. Weight loading through a checkpoint is standard.
             Model config is typically stored on wandb, but this is not portable enough. Instead, directly reference the model config file.
         """
         self._task_config = task_config
         self.exp_task = getattr(ExperimentalTask, f'falcon_{task_config.task.name}')
-
-        context_registry.register([
-            *FalconContextInfo.build_from_dir(
-                f'./data/{task_config.task.name}/eval',
-                task=self.exp_task,
-                suffix='eval'),
-            *FalconContextInfo.build_from_dir(
-                f'./data/{task_config.task.name}/minival',
-                task=self.exp_task,
-                suffix='minival')])
-
         try:
             initialize_config_module(
                 config_module="context_general_bci.config",
                 job_name="falcon",
                 version_base="1.3",
             )
         except:
@@ -72,17 +61,15 @@
         propagate_config(cfg)
         pl.seed_everything(seed=cfg.seed)
 
         self.subject = getattr(SubjectName, f'falcon_{task_config.task.name}')
         context_idx = {
             MetaKey.array.name: [format_array_name(self.subject)],
             MetaKey.subject.name: [self.subject],
-            MetaKey.session.name: sorted([
-                self._task_config.hash_dataset(handle) for handle in task_config.dataset_handles
-            ]),
+            MetaKey.session.name: sorted([self._task_config.hash_dataset(handle) for handle in dataset_handles]),
             MetaKey.task.name: [self.exp_task],
         }
         data_attrs = DataAttrs.from_config(cfg.dataset, context=ContextAttrs(**context_idx))
         cfg.model.task.decode_normalizer = zscore_path
         model = load_from_checkpoint(model_ckpt_path, cfg=cfg.model, data_attrs=data_attrs)
         model = transfer_model(model, cfg.model, data_attrs)
         self.model = model.to('cuda:0')
```

### Comparing `falcon_challenge-0.2.5/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.2.7/decoder_demos/ndt2_sample.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,24 +37,22 @@
     args = parser.parse_args()
 
     evaluator = FalconEvaluator(
         eval_remote=args.evaluation == "remote",
         split=args.split)
 
     task = getattr(FalconTask, args.split)
-    config = FalconConfig(
-        task=task,
-        dataset_handles=[x.stem for x in evaluator.get_eval_files(phase=args.phase)]
-    )
+    config = FalconConfig(task=task)
 
     decoder = NDT2Decoder(
         task_config=config,
         model_ckpt_path=args.model_path,
         model_cfg_stem=args.config_stem,
-        zscore_path=args.zscore_path
+        zscore_path=args.zscore_path,
+        dataset_handles=[x.stem for x in evaluator.get_eval_files(phase=args.phase)]
     )
 
 
     evaluator.evaluate(decoder, phase=args.phase)
 
 
 if __name__ == "__main__":
```

### Comparing `falcon_challenge-0.2.5/decoder_demos/random_decoder.py` & `falcon_challenge-0.2.7/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.2.7/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.2.7/decoder_demos/sklearn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.2.7/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/falcon_challenge/config.py` & `falcon_challenge-0.2.7/falcon_challenge/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+from typing import Union
 from pathlib import Path
 from dataclasses import dataclass, field
 
 from hydra.core.config_store import ConfigStore
 from hydra.core.config_search_path import ConfigSearchPath
 from hydra.plugins.search_path_plugin import SearchPathPlugin
 
@@ -48,15 +49,15 @@
             return 28
         elif self.task == FalconTask.m1:
             return 16
         elif self.task == FalconTask.m2:
             return 2
         raise NotImplementedError(f"Task {self.task} not implemented.")
         
-    def hash_dataset(self, handle: str | Path):
+    def hash_dataset(self, handle: Union[str, Path]):
         r"""
             handle - path.stem of a datafile.
             Convenience function to help identify what "session" a datafile belongs to.. If multiple files per session in real-world time, this may _not_ uniquely identify runfile.
         """
         if isinstance(handle, Path):
             handle = handle.stem
         if self.task == FalconTask.h1:
```

### Comparing `falcon_challenge-0.2.5/falcon_challenge/dataloaders.py` & `falcon_challenge-0.2.7/falcon_challenge/dataloaders.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/falcon_challenge/evaluator.py` & `falcon_challenge-0.2.7/falcon_challenge/evaluator.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,16 +41,16 @@
             'S8_set_2', 
             'S9_set_1', 
             'S9_set_2', 
             'S10_set_1', 
             'S10_set_2', 
             'S11_set_1', 
             'S11_set_2', 
-            'S12_set_1'
-            'S12_set_2'
+            'S12_set_1',
+            'S12_set_2',
         ],
     },
     'm1': {
         'held_in': ['20120924', '20120926', '20120927', '20120928'],
         'held_out': ['20121004', '20121017', '20121022', '20121024'],
     },
     'h2': {
@@ -76,59 +76,14 @@
 USE_PKLS = True
 
 HELDIN_OR_OUT_MAP = {
     'held_in': "Held In",
     'held_out': "Held Out",
 }
 
-# def evaluate(
-#     test_annotation_file: str, # The annotation file for the phase - but our labels are pulled from eval data.
-#     user_submission_file: str, # * JY: This appears to always be /submission/submission.csv on EvalAI. No matter - load it as a pickle.
-#     phase_codename: str, # e.g. minival or test
-#     **kwargs
-# ):
-#     r"""
-#         Evaluate payloads with potentially multiple splits worth of data
-#         - Low pri: can I provide all results or just one split's worth entry? Currently providing 1, examples just provide 1, but in general would be nice to provide all. User shouldn't be able to submit more than 1, though.
-#     """
-#     # ! Want: Locally, test_annotation should be somewhere safe (tmp)
-#     # ! Remotely, it shoudl be /submission/submission.csv exactly.
-#     # Ignore explicit annotations provided and directly search for concatenated answers
-#     logger.info(f"Evaluation: Docker side")
-#     logger.info(f"Loading GT from {test_annotation_file}")
-#     logger.info(f"Loading submission from {user_submission_file}")
-#     logger.info(f"Phase: {phase_codename}")
-
-#     result = []
-#     # Load pickles
-#     with open(test_annotation_file, 'rb') as test_annotation_file, open(user_submission_file, 'rb') as user_submission_file:
-#         test_annotations = pickle.load(test_annotation_file)
-#         user_submission = pickle.load(user_submission_file)
-#     for datasplit in user_submission: # datasplit e.g. h1, m1
-#         if datasplit not in test_annotations:
-#             raise ValueError(f"Missing {datasplit} in GT labels.")
-#         split_annotations = test_annotations[datasplit]
-#         split_result = {}
-#         split_result["Normalized Latency"] = user_submission[datasplit]["normalized_latency"]
-#         for in_or_out in split_annotations.keys():
-#             if f'{in_or_out}_pred' in user_submission[datasplit]:
-#                 pred = user_submission[datasplit][f'{in_or_out}_pred']
-#                 mask = user_submission[datasplit][f'{in_or_out}_eval_mask']
-#                 # User submission should be in an expected format because we force predictions through our codepack interface... right? They could hypothetically spoof. But we see dockerfile.
-#                 eval_fn = FalconEvaluator.compute_metrics_classification if 'h2' in datasplit else FalconEvaluator.compute_metrics_regression
-#                 metrics_held_in = eval_fn(pred, split_annotations[in_or_out], mask)
-#                 for k in metrics_held_in:
-#                     split_result[f'{HELDIN_OR_OUT_MAP[in_or_out]} {k}'] = metrics_held_in[k]
-#         result.append({datasplit: split_result})
-            
-#     print(f"Returning result from phase: {phase_codename}: {result}")
-#     # Out struct according to https://evalai.readthedocs.io/en/latest/evaluation_scripts.html
-#     return {"result": result, 'submission_result': result[0]}
-
-
 def evaluate(
     test_annotation_file: str, # The annotation file for the phase
     user_submission_file: str, # * JY: This appears to always be /submission/submission.csv on EvalAI. No matter - load it as a pickle.
     phase_codename: str, # e.g. minival or test
     **kwargs
 ):
     r"""
@@ -203,15 +158,15 @@
             eval_fn = FalconEvaluator.compute_metrics_classification if 'h2' in datasplit else FalconEvaluator.compute_metrics_regression
             try:
                 metrics = eval_fn(pred, tgt, mask)
             except Exception as e:
                 raise ValueError(f"Failed to compute metrics for {datasplit} {in_or_out}: {e}")
             for k in metrics:
                 split_result[f'{HELDIN_OR_OUT_MAP[in_or_out]} {k}'] = metrics[k]
-        result.append({datasplit: split_result})
+        result.append({f'{phase_codename}_split_{datasplit}': split_result})
 
     print(f"Returning result from phase: {phase_codename}: {result}")
     # Out struct according to https://evalai.readthedocs.io/en/latest/evaluation_scripts.html
     return {"result": result, 'submission_result': result[0]}
 
 class FalconEvaluator:
 
@@ -337,25 +292,20 @@
                 } for k in all_targets
             }
             inner_pred['normalized_latency'] = 1 # TODO - CW insert timing code
             pred_payload = {self.dataset.name: inner_pred}
             truth_payload = {self.dataset.name: inner_tgt_spoof}
         else:
             pass
-            # TODO restore
-            # metrics_held_in = self.compute_metrics(all_preds_held_in, all_targets_held_in, all_eval_mask_held_in)
-            # metrics_held_out = self.compute_metrics(all_preds_held_out, all_targets_held_out, all_eval_mask_held_out)
-            # for k, v in metrics_held_in.items():
-                # metrics[f'{HELDIN_OR_OUT_MAP["held_in"]} {k}'] = v
-            # for k, v in metrics_held_out.items():
-                # metrics[f'{HELDIN_OR_OUT_MAP["held_out"]} {k}'] = v            
             
         if USE_PKLS:
+            Path(prediction_path).parent.mkdir(parents=True, exist_ok=True)
             with open(prediction_path, 'wb') as f:
                 pickle.dump(pred_payload, f)
+            Path(gt_path).parent.mkdir(parents=True, exist_ok=True)
             with open(gt_path, 'wb') as f:
                 pickle.dump(truth_payload, f)
             import time
 
             if self.eval_remote:
                 print("Sleeping before exiting for remote eval - feel free to interrupt for local eval.", flush=True)
                 # Gunjan, EvalAI contact says that current static code eval has an issue where the submission dump is only polled by the EvalAI worker comparison script every 5 minutes
```

### Comparing `falcon_challenge-0.2.5/falcon_challenge/interface.py` & `falcon_challenge-0.2.7/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.2.7/falcon_challenge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.5
+Version: 0.2.7
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.2.5/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.2.7/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/assemble_data.py` & `falcon_challenge-0.2.7/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/filtering.py` & `falcon_challenge-0.2.7/preproc/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/h2_preproc.py` & `falcon_challenge-0.2.7/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.2.7/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.2.7/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.2.7/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/m2_preproc.py` & `falcon_challenge-0.2.7/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/merge_answers.py` & `falcon_challenge-0.2.7/preproc/merge_answers.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/nwb_create_utils.py` & `falcon_challenge-0.2.7/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/preproc/zip_data.py` & `falcon_challenge-0.2.7/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.5/setup.py` & `falcon_challenge-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.2.5',
+    version='0.2.7',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

