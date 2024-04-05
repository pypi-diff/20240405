# Comparing `tmp/dalpha_ai_cpu-0.2.9.tar.gz` & `tmp/dalpha_ai_cpu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha_ai_cpu-0.2.9.tar", last modified: Thu Jan 11 11:18:02 2024, max compression
+gzip compressed data, was "dalpha_ai_cpu-0.3.0.tar", last modified: Fri Apr  5 05:46:49 2024, max compression
```

## Comparing `dalpha_ai_cpu-0.2.9.tar` & `dalpha_ai_cpu-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.377110 dalpha_ai_cpu-0.2.9/
--rw-r--r--   0     1024 users      (100)      187 2024-01-11 11:18:02.375110 dalpha_ai_cpu-0.2.9/PKG-INFO
--rw-r--r--   0     1024 users      (100)      996 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/README.md
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.315109 dalpha_ai_cpu-0.2.9/dalpha_ai/
--rw-r--r--   0     1024 users      (100)      672 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/__init__.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.318109 dalpha_ai_cpu-0.2.9/dalpha_ai/core/
--rw-r--r--   0     1024 users      (100)        0 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/__init__.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.327109 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/
--rw-r--r--   0     1024 users      (100)      380 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/__init__.py
--rw-r--r--   0     1024 users      (100)     9979 2024-01-07 16:51:39.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/base_classifier.py
--rw-r--r--   0     1024 users      (100)     4880 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/base_config.py
--rw-r--r--   0     1024 users      (100)     1870 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/base_datamodule.py
--rw-r--r--   0     1024 users      (100)    31221 2024-01-07 16:25:57.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/base_trainer.py
--rw-r--r--   0     1024 users      (100)     1846 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/custom_ops.py
--rw-r--r--   0     1024 users      (100)     1516 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/head_classifier.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.334110 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_classifier/
--rw-r--r--   0     1024 users      (100)      143 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_classifier/__init__.py
--rw-r--r--   0     1024 users      (100)     2841 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_classifier/image_classifier.py
--rw-r--r--   0     1024 users      (100)     2420 2024-01-10 13:56:20.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_classifier/image_config.py
--rw-r--r--   0     1024 users      (100)     2948 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_classifier/image_datamodule.py
--rw-r--r--   0     1024 users      (100)     2558 2024-01-10 14:25:45.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_classifier/image_trainer.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.341110 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_text_classifier/
--rw-r--r--   0     1024 users      (100)      170 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_text_classifier/__init__.py
--rw-r--r--   0     1024 users      (100)     3047 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_text_classifier/image_text_classifier.py
--rw-r--r--   0     1024 users      (100)     4568 2024-01-10 13:56:03.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_text_classifier/image_text_config.py
--rw-r--r--   0     1024 users      (100)     2756 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_text_classifier/image_text_datamodule.py
--rw-r--r--   0     1024 users      (100)     4372 2024-01-10 14:25:54.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_text_classifier/image_text_trainer.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.348110 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/text_classifier/
--rw-r--r--   0     1024 users      (100)      137 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/text_classifier/__init__.py
--rw-r--r--   0     1024 users      (100)     2802 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/text_classifier/text_classifier.py
--rw-r--r--   0     1024 users      (100)     2298 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/text_classifier/text_config.py
--rw-r--r--   0     1024 users      (100)     2534 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/text_classifier/text_datamodule.py
--rw-r--r--   0     1024 users      (100)     2424 2024-01-10 14:26:47.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/text_classifier/text_trainer.py
--rw-r--r--   0     1024 users      (100)    19104 2024-01-10 13:59:08.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/trainer_util.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.354110 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/zeroshot_classifier/
--rw-r--r--   0     1024 users      (100)      128 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/zeroshot_classifier/__init__.py
--rw-r--r--   0     1024 users      (100)    14040 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_classifier.py
--rw-r--r--   0     1024 users      (100)      799 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_config.py
--rw-r--r--   0     1024 users      (100)     1885 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_datamodule.py
--rw-r--r--   0     1024 users      (100)     5118 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/losses.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.362110 dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/
--rw-r--r--   0     1024 users      (100)     2080 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/__init__.py
--rw-r--r--   0     1024 users      (100)    19063 2024-01-11 11:00:59.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/onnx_pipeline.py
--rw-r--r--   0     1024 users      (100)     9839 2024-01-07 12:58:16.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/onnx_util.py
--rw-r--r--   0     1024 users      (100)     7282 2024-01-10 15:42:08.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/pytorch_pipeline.py
--rw-r--r--   0     1024 users      (100)     2175 2024-01-10 14:26:47.000000 dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/util.py
-drwxr-xr-x   0     1024 users      (100)        0 2024-01-11 11:18:02.373110 dalpha_ai_cpu-0.2.9/dalpha_ai_cpu.egg-info/
--rw-r--r--   0     1024 users      (100)      187 2024-01-11 11:18:02.000000 dalpha_ai_cpu-0.2.9/dalpha_ai_cpu.egg-info/PKG-INFO
--rw-r--r--   0     1024 users      (100)     2019 2024-01-11 11:18:02.000000 dalpha_ai_cpu-0.2.9/dalpha_ai_cpu.egg-info/SOURCES.txt
--rw-r--r--   0     1024 users      (100)        1 2024-01-11 11:18:02.000000 dalpha_ai_cpu-0.2.9/dalpha_ai_cpu.egg-info/dependency_links.txt
--rw-r--r--   0     1024 users      (100)      251 2024-01-11 11:18:02.000000 dalpha_ai_cpu-0.2.9/dalpha_ai_cpu.egg-info/requires.txt
--rw-r--r--   0     1024 users      (100)       10 2024-01-11 11:18:02.000000 dalpha_ai_cpu-0.2.9/dalpha_ai_cpu.egg-info/top_level.txt
--rw-r--r--   0     1024 users      (100)       38 2024-01-11 11:18:02.377110 dalpha_ai_cpu-0.2.9/setup.cfg
--rw-r--r--   0     1024 users      (100)      343 2024-01-11 11:17:49.000000 dalpha_ai_cpu-0.2.9/setup.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.899131 dalpha_ai_cpu-0.3.0/
+-rw-r--r--   0     1024 users      (100)      187 2024-04-05 05:46:49.897131 dalpha_ai_cpu-0.3.0/PKG-INFO
+-rw-r--r--   0     1024 users      (100)      660 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/README.md
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.664129 dalpha_ai_cpu-0.3.0/dalpha_ai/
+-rw-r--r--   0     1024 users      (100)      868 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/__init__.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.671129 dalpha_ai_cpu-0.3.0/dalpha_ai/core/
+-rw-r--r--   0     1024 users      (100)        0 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/__init__.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.720129 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/
+-rw-r--r--   0     1024 users      (100)      380 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)    12260 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_classifier.py
+-rw-r--r--   0     1024 users      (100)     5883 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_config.py
+-rw-r--r--   0     1024 users      (100)     2004 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_datamodule.py
+-rw-r--r--   0     1024 users      (100)    43918 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_feedback_trainer.py
+-rw-r--r--   0     1024 users      (100)    31768 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_trainer.py
+-rw-r--r--   0     1024 users      (100)     1846 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/custom_ops.py
+-rw-r--r--   0     1024 users      (100)     1516 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/head_classifier.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.751129 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_classifier/
+-rw-r--r--   0     1024 users      (100)      199 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)     6133 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_classifier/image_classifier.py
+-rw-r--r--   0     1024 users      (100)     4844 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_classifier/image_config.py
+-rw-r--r--   0     1024 users      (100)     5371 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_classifier/image_datamodule.py
+-rw-r--r--   0     1024 users      (100)     5731 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_classifier/image_trainer.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.782130 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_text_classifier/
+-rw-r--r--   0     1024 users      (100)      234 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_text_classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)     6372 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_classifier.py
+-rw-r--r--   0     1024 users      (100)     4731 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_config.py
+-rw-r--r--   0     1024 users      (100)     5650 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_datamodule.py
+-rw-r--r--   0     1024 users      (100)     9605 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_trainer.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.812130 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/text_classifier/
+-rw-r--r--   0     1024 users      (100)      191 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/text_classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)     6017 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/text_classifier/text_classifier.py
+-rw-r--r--   0     1024 users      (100)     2390 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/text_classifier/text_config.py
+-rw-r--r--   0     1024 users      (100)     5127 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/text_classifier/text_datamodule.py
+-rw-r--r--   0     1024 users      (100)     5480 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/text_classifier/text_trainer.py
+-rw-r--r--   0     1024 users      (100)    24444 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/trainer_util.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.835130 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/
+-rw-r--r--   0     1024 users      (100)      128 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/__init__.py
+-rw-r--r--   0     1024 users      (100)    14040 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_classifier.py
+-rw-r--r--   0     1024 users      (100)      799 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_config.py
+-rw-r--r--   0     1024 users      (100)     1885 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_datamodule.py
+-rw-r--r--   0     1024 users      (100)     6562 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/losses.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.864131 dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/
+-rw-r--r--   0     1024 users      (100)     2080 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/__init__.py
+-rw-r--r--   0     1024 users      (100)    19044 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/onnx_pipeline.py
+-rw-r--r--   0     1024 users      (100)     9839 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/onnx_util.py
+-rw-r--r--   0     1024 users      (100)     7335 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/pytorch_pipeline.py
+-rw-r--r--   0     1024 users      (100)     2175 2024-04-05 05:42:18.000000 dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/util.py
+drwxr-xr-x   0     1024 users      (100)        0 2024-04-05 05:46:49.893131 dalpha_ai_cpu-0.3.0/dalpha_ai_cpu.egg-info/
+-rw-r--r--   0     1024 users      (100)      187 2024-04-05 05:46:49.000000 dalpha_ai_cpu-0.3.0/dalpha_ai_cpu.egg-info/PKG-INFO
+-rw-r--r--   0     1024 users      (100)     2070 2024-04-05 05:46:49.000000 dalpha_ai_cpu-0.3.0/dalpha_ai_cpu.egg-info/SOURCES.txt
+-rw-r--r--   0     1024 users      (100)        1 2024-04-05 05:46:49.000000 dalpha_ai_cpu-0.3.0/dalpha_ai_cpu.egg-info/dependency_links.txt
+-rw-r--r--   0     1024 users      (100)      251 2024-04-05 05:46:49.000000 dalpha_ai_cpu-0.3.0/dalpha_ai_cpu.egg-info/requires.txt
+-rw-r--r--   0     1024 users      (100)       10 2024-04-05 05:46:49.000000 dalpha_ai_cpu-0.3.0/dalpha_ai_cpu.egg-info/top_level.txt
+-rw-r--r--   0     1024 users      (100)       38 2024-04-05 05:46:49.901131 dalpha_ai_cpu-0.3.0/setup.cfg
+-rw-r--r--   0     1024 users      (100)      343 2024-04-05 05:46:20.000000 dalpha_ai_cpu-0.3.0/setup.py
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/__init__.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from .core.classifier.text_classifier import (
     TextClassifier,
     TextClassifierConfig,
     TextClassifierModule,
+    FeedbackTextClassifierModule,
+    FeedbackTextClassifier
 )
 
 from .core.classifier.image_classifier import (
     ImageClassifier,
     ImageClassifierConfig,
     ImageClassifierModule,
+    FeedbackImageClassifier,
+    FeedbackImageClassifierModule,
 )
 
 from .core.classifier.image_text_classifier import (
     ImageTextClassifier,
     ImageTextClassifierConfig,
     ImageTextClassifierModule,
+    FeedbackImageTextClassifier,
+    FeedbackImageTextClassifierModule
 )
 
 from .core.classifier.zeroshot_classifier import (
     ZeroshotImageClassifier,
     ZeroshotImageClassifierConfig,
 )
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/base_classifier.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_classifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 from typing import List, Union
 
 import pandas as pd
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import ModelCheckpoint
 
-from .trainer_util import set_seed
+from .trainer_util import set_seed, sample_stratified
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
 
 def check_dataset(dataset: Union[pd.DataFrame, List[List]], column_list: List[str], train_config=None):
     """
@@ -82,76 +82,101 @@
 
 class BaseClassifier:
     """
     Base class for all classifiers, including text, image, and image-text classifiers
     Args:
         train_dataset (pd.DataFrame or list): training dataset
         val_dataset (pd.DataFrame or list): validation dataset
+        feedback_dataset (pd.DataFrame or list): feedback dataset (optional)
         test_dataset (pd.DataFrame or list): test dataset (optional)
         label_name_list (list): list of label names (optional)
         train_config (ClassifierConfig): training config (optional)
     """
 
     def __init__(
         self,
         train_dataset: Union[pd.DataFrame, List[List]],
         val_dataset: Union[pd.DataFrame, List[List]],
+        feedback_dataset: Union[pd.DataFrame, List[List]] = None,
         test_dataset: Union[pd.DataFrame, List[List]] = None,
         label_name_list: List = None,
         train_config=None,
     ):
         from .text_classifier import TextClassifierConfig
         from .image_classifier import ImageClassifierConfig
         from .image_text_classifier import ImageTextClassifierConfig
 
         self.train_config = train_config
         # Set random seed
         set_seed(self.train_config.seed)
 
         train_dataset = copy.deepcopy(train_dataset)
         val_dataset = copy.deepcopy(val_dataset)
+        feedback_dataset = copy.deepcopy(feedback_dataset)
         test_dataset = copy.deepcopy(test_dataset)
         if type(train_config) == TextClassifierConfig:
             train_dataset = check_dataset(train_dataset, ["text", "label"], train_config)
             val_dataset = check_dataset(val_dataset, ["text", "label"], train_config)
+            if feedback_dataset is not None:
+                feedback_dataset = check_dataset(
+                    feedback_dataset, ["text", "label"], train_config
+                )
             if test_dataset is not None:
                 test_dataset = check_dataset(test_dataset, ["text", "label"], train_config)
             else:
                 logger.warning(
                     "test_dataset is None. Using val_dataset as test_dataset"
                 )
                 test_dataset = copy.deepcopy(val_dataset)
 
+
         elif type(train_config) == ImageClassifierConfig:
             train_dataset = check_dataset(train_dataset, ["img_path", "label"], train_config)
             val_dataset = check_dataset(val_dataset, ["img_path", "label"], train_config)
+            if feedback_dataset is not None:
+                feedback_dataset = check_dataset(
+                    feedback_dataset, ["img_path", "label"], train_config
+                )
             if test_dataset is not None:
                 test_dataset = check_dataset(test_dataset, ["img_path", "label"], train_config)
             else:
                 logger.warning(
                     "test_dataset is None. Using val_dataset as test_dataset"
                 )
                 test_dataset = copy.deepcopy(val_dataset)
 
         elif type(train_config) == ImageTextClassifierConfig:
             train_dataset = check_dataset(train_dataset, ["img_path", "text", "label"], train_config)
             val_dataset = check_dataset(val_dataset, ["img_path", "text", "label"], train_config)
+            if feedback_dataset is not None:
+                feedback_dataset = check_dataset(
+                    feedback_dataset, ["img_path", "text", "label"], train_config
+                )
             if test_dataset is not None:
                 test_dataset = check_dataset(
                     test_dataset, ["img_path", "text", "label"], train_config
                 )
             else:
                 logger.warning(
                     "test_dataset is None. Using val_dataset as test_dataset"
                 )
                 test_dataset = copy.deepcopy(val_dataset)
         else:
             raise ValueError(f"Not supported train_config type: {type(train_config)}")
-
-        self.train_dataset = train_dataset
+        
+        ## If feedback_dataset exists, concat feedback dataset and stratified sample from train dataset
+        if feedback_dataset is not None:
+            sampled_train_dataset = sample_stratified(train_dataset, self.train_config.feedback_iteration * len(feedback_dataset), self.train_config.problem_type)
+            # Add feedback label for distinguishing feedback data
+            sampled_train_dataset["feedback_flag"] = [0] * len(sampled_train_dataset)
+            repeated_feedback_dataset = pd.concat([feedback_dataset] * self.train_config.feedback_iteration, ignore_index=True)
+            repeated_feedback_dataset["feedback_flag"] = [1] * len(repeated_feedback_dataset)
+            self.train_dataset = pd.concat([sampled_train_dataset, repeated_feedback_dataset], ignore_index=True)
+        else:
+            self.train_dataset = train_dataset
         self.val_dataset = val_dataset
         self.test_dataset = test_dataset
 
         # Check number of class when training config num class value is default value.
         if self.train_config.num_class == 0:
             if label_name_list is not None:
                 logger.info("Get number of class with the length of label name list.")
@@ -181,49 +206,62 @@
     def base_train(self):
         """
         Base training function
         """
         if self.train_config.problem_type == "single_label_classification":
             if self.train_config.monitor_topk == "total":
                 monitor_acc = "val/tot_acc"
+                if self.train_config.val_check_interval:
+                    filename = "epoch{epoch:02d}-step{step}-val_totacc={val/tot_acc:.4f}"
+                else:
+                    filename = "epoch{epoch:02d}-val_totacc={val/tot_acc:.4f}"
                 checkpoint_callback = ModelCheckpoint(
                     monitor=monitor_acc,
                     mode="max",
                     save_top_k=self.train_config.save_ckpt_topk,
-                    filename="epoch{epoch:02d}-val_totacc={val/tot_acc:.4f}",
+                    filename=filename,
                     auto_insert_metric_name=False,
                 )
             else:
                 monitor_acc = f"val/acc{self.train_config.monitor_topk}"
+                if self.train_config.val_check_interval:
+                    filename = "epoch{epoch:02d}-step{step}-val_acc={val/monitor_acc:.4f}"
+                else:
+                    filename = "epoch{epoch:02d}-val_acc={val/monitor_acc:.4f}"
                 checkpoint_callback = ModelCheckpoint(
                     monitor=monitor_acc,
                     mode="max",
                     save_top_k=self.train_config.save_ckpt_topk,
-                    filename="epoch{epoch:02d}-val_acc={val/monitor_acc:.4f}",
+                    filename=filename,
                     auto_insert_metric_name=False,
                 )
         else:
             monitor_f1 = f"val/f1"
+            if self.train_config.val_check_interval:
+                filename = "epoch{epoch:02d}-step{step}-val_f1={val/f1:.4f}"
+            else:
+                filename = "epoch{epoch:02d}-val_f1={val/f1:.4f}"
             checkpoint_callback = ModelCheckpoint(
                 monitor=monitor_f1,
                 mode="max",
                 save_top_k=self.train_config.save_ckpt_topk,
-                filename="epoch{epoch:02d}-val_f1={val/f1:.4f}",
+                filename=filename,
                 auto_insert_metric_name=False,
             )
 
         # Define trainer
         self.trainer = pl.Trainer(
             accelerator=self.train_config.device,
             devices=self.train_config.use_device_list,
             precision=self.train_config.precision,
             max_epochs=self.train_config.max_epochs,
             callbacks=[checkpoint_callback],
             num_sanity_val_steps=self.train_config.num_sanity_val_steps,
             check_val_every_n_epoch=self.train_config.check_val_every_n_epoch,
+            val_check_interval=self.train_config.val_check_interval,
             default_root_dir=self.train_config.output_dir,
             strategy="ddp_find_unused_parameters_true",
         )
 
         self.trainer.fit(self.train_module, self.data_module)
 
         print(
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/base_config.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,81 +10,93 @@
 class BaseClassifierConfig:
     """
     Base Classifier Config Class
 
     Args:
         batch_size (int): batch size per GPU, default: 32
         max_epochs (int): max epoch for training, default: 10
+        feedback_iteration (int): feedback iteration, only used for feedback_training, default: 100.
+        e.g. 100 feed back iterations and 5 label, 10 feedback sample -> 100 * 5 * 10 = 5000 samples will be used in train dataset.
         seed (int): random seed, default: 42
         num_class (int): number of class, default: 0
         output_dir (str): output directory, default: 'tmp_classifier'
         device (str): device name, e.g. 'cpu', 'gpu', default: 'gpu'
         use_device_list (Union[str, List[int]]): device list, e.g. 'auto', [0, 1], default: 'auto'
         num_workers (int): number of workers, default: 4
         fc_classifier (Union[str, nn.Module]): fully connected classifier, e.g. 'Base2LinearClassifier', default: 'Base2LinearClassifier'
         label_smoothing_factor (float): label smoothing factor, default: 0.1
+        feedback_ema_decay (float): feedback ema decay, default: 0.9
         gradient_accumulation_steps (int): gradient accumulation steps, default: 1
-        print_topk_list (list): topk list for printing, default: [1, 3, 5]
+        print_topk_list (tuple): topk tuple for printing, default: (1, 3, 5)
         monitor_topk (Union[int, str]): topk for monitoring, default: 1
         save_ckpt_topk (int): topk for saving checkpoint, default: 3
         check_val_every_n_epoch (int): check validation every n epoch, default: 1
+        val_check_interval(int): check validation every n train steps, also saving model checkpoint. default: None,
         num_sanity_val_steps (int): number of sanity validation steps, default: 2
         precision (str): precision, e.g. '16-mixed', '32', default: '16-mixed'
         label_name_list (list): label name list, default: None
         criterion (str): criterion name, e.g. 'cross_entropy', 'focal_loss', default: 'cross_entropy'
         problem_type (str): problem type, e.g. 'single_label_classification', 'multi_label_classification', default: 'single_label_classification'
     """
 
     def __init__(
         self,
         batch_size: int = 32,
         max_epochs: int = 10,
+        feedback_iteration: int = 100,
         seed: int = 42,
         num_class: int = 0,
         output_dir: str = "tmp_classifier",
         device: str = "gpu",
         use_device_list: Union[str, List[int]] = "auto",
         num_workers: int = 4,
         fc_classifier: Union[str, nn.Module] = "Base2LinearClassifier",
         label_smoothing_factor: float = 0.1,
+        feedback_ema_decay: float = 0.9,
         gradient_accumulation_steps: int = 1,
-        print_topk_list: list = [1, 3, 5],
+        print_topk_list: tuple = (1, 3, 5),
         monitor_topk: Union[int, str] = 1,
         save_ckpt_topk: int = 3,
         check_val_every_n_epoch: int = 1,
+        val_check_interval: int = None,
         num_sanity_val_steps: int = 2,
         precision: str = "16-mixed",
         label_name_list: list = None,
         criterion: str = "cross_entropy",
         problem_type: str = "single_label_classification",
+        lr_scheduler: str = "linear_warmup",
     ):
         # Batch size per GPU
         self.batch_size = batch_size
         # Max epoch for training
         self.max_epochs = max_epochs
+        # Feedback iteration, only used for feedback_training
+        self.feedback_iteration = feedback_iteration
         self.seed = seed
         # Num class will be define and be checked at trainer class
         self.num_class = num_class
         self.output_dir = output_dir
         self.device = device
         # Can be GPU Device number e.g. [0, 1]
         self.use_device_list = use_device_list
         self.num_workers = num_workers
         # Can be classifier name string or defined nn.Moudle
         self.fc_classifier = fc_classifier
         self.label_smoothing_factor = label_smoothing_factor
+        self.feedback_ema_decay = feedback_ema_decay
         self.gradient_accumulation_steps = gradient_accumulation_steps
 
-        self.print_topk_list = print_topk_list
+        self.print_topk_list = list(print_topk_list)
         if monitor_topk != "total" and monitor_topk not in print_topk_list:
             raise ValueError("monitor_topk must be in print_topk_list or 'total'")
 
         self.monitor_topk = monitor_topk
         self.save_ckpt_topk = save_ckpt_topk
         self.check_val_every_n_epoch = check_val_every_n_epoch
+        self.val_check_interval = val_check_interval
         self.num_sanity_val_steps = num_sanity_val_steps
         self.precision = precision
         self.label_name_list = label_name_list
 
         if problem_type not in [
             "single_label_classification",
             "multi_label_classification",
@@ -101,15 +113,18 @@
             if criterion not in ["binary_cross_entropy", "binary_focal_loss"]:
                 raise ValueError(
                     f"criterion must be in ['binary_cross_entropy', 'binary_focal_loss'] for multi_label_classification"
                 )
 
         if criterion == "focal_loss" and label_smoothing_factor > 0:
             criterion = "focal_loss_with_label_smoothing"
-
         self.criterion = criterion
 
+        if lr_scheduler not in ["linear_warmup", "constant"]:
+            raise ValueError(f"lr_scheduler must be in ['linear_warmup', 'constant']")
+        self.lr_scheduler = lr_scheduler
+
     def to_dict(self):
         """
         Convert class attributes to dictionary
         """
         return self.__dict__
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/base_datamodule.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_datamodule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
 from torch.utils.data import Dataset
 from typing import Optional
 import torch
 from pytorch_lightning import LightningDataModule
+from typing import Union
 
 
 class BaseDataModule(LightningDataModule):
     """
     Base DataModule for all classification tasks
     Args:
         train_dataset (pd.DataFrame): training dataset
@@ -17,18 +18,20 @@
 
     def __init__(
         self,
         train_dataset: pd.DataFrame,
         val_dataset: pd.DataFrame,
         test_dataset: pd.DataFrame,
         train_config,
+        feedback_dataset: Union[pd.DataFrame, None] = None,
     ):
         super().__init__()
         self.train_dataset = train_dataset
         self.val_dataset = val_dataset
+        self.feedback_dataset = feedback_dataset
         self.test_dataset = test_dataset
         self.batch_size = train_config.batch_size
         self.num_workers = train_config.num_workers
         self.problem_type = train_config.problem_type
         self.num_class = train_config.num_class
 
     def train_dataloader(self):
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/base_trainer.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/base_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,17 @@
         raise NotImplementedError
 
     def forward(self):
         raise NotImplementedError
 
     def configure_optimizers(self):
         raise NotImplementedError
-    
+
     ## Bugfixed in peft 0.7.0 (so we cast lora weights to float, for mixed precision training)
-    def cast_lora_to_float(self, model):
+    def cast_lora_to_float(self, model: nn.Module):
         for name, mod in model.named_modules():
             if ("lora_" in name) and hasattr(mod, "weight"):
                 mod.weight.data = mod.weight.data.float()
             if ("lora_" in name) and hasattr(mod, "bias") and (mod.bias is not None):
                 mod.bias.data = mod.bias.data.float()
             if ("modules_to_save" in name) and isinstance(mod, nn.Linear):
                 mod.weight.data = mod.weight.data.float()
@@ -229,22 +229,27 @@
             data_config = timm.data.resolve_model_data_config(model)
             train_transforms = timm.data.create_transform(
                 **data_config, is_training=True
             )
             val_transforms = timm.data.create_transform(
                 **data_config, is_training=False
             )
-            data_config['scale'] = (self.train_config.crop_ratio, 1.0)
+            data_config["scale"] = (self.train_config.crop_ratio, 1.0)
             timm_flag = True
             config = None
             # self.train_config.timm = True
         else:
             timm_flag = False
 
-            from transformers import AutoImageProcessor, AutoModel, CLIPModel, AutoConfig
+            from transformers import (
+                AutoImageProcessor,
+                AutoModel,
+                CLIPModel,
+                AutoConfig,
+            )
 
             model = AutoModel.from_pretrained(backbone_name)
             if isinstance(model, CLIPModel):
                 model = model.vision_model
                 # Cannot converted with huggingface
                 timm_flag = True
             model = TransformerWrapper(model)
@@ -257,37 +262,37 @@
                         3,
                         image_processor.crop_size["height"],
                         image_processor.crop_size["width"],
                     ),
                     "mean": image_processor.image_mean,
                     "std": image_processor.image_std,
                     "interpolation": _pil_interpolation_to_str[
-                        image_processor.resample,
-                    "scale":  (self.train_config.crop_ratio, 1.0)
+                        image_processor.resample
                     ],
+                    "scale": (self.train_config.crop_ratio, 1.0),
                 }
             elif hasattr(image_processor, "size"):
                 data_config = {
                     "input_size": (
                         3,
                         image_processor.size["height"],
                         image_processor.size["width"],
                     ),
                     "mean": image_processor.image_mean,
                     "std": image_processor.image_std,
                     "interpolation": _pil_interpolation_to_str[
                         image_processor.resample
                     ],
-                    "scale": (self.train_config.crop_ratio, 1.0)
+                    "scale": (self.train_config.crop_ratio, 1.0),
                 }
             else:
                 raise ValueError(
                     f"'size' and 'crop_size' does not exist in current Image processor. Current image processor: {image_processor}"
                 )
-            
+
             train_transforms = timm.data.create_transform(
                 **data_config,
                 auto_augment=self.train_config.auto_augment,
                 is_training=True,
             )
             val_transforms = timm.data.create_transform(
                 **data_config, is_training=False
@@ -299,14 +304,15 @@
 
         return model, train_transforms, val_transforms, data_config, timm_flag, config
 
     def text_forward(
         self,
         input_texts: List[str],
         backbone: nn.Module,
+        classifier_head: nn.Module,
         initial_config: AutoConfig,
         freeze: bool = False,
         eval: bool = False,
         classifier: bool = True,
     ):
         """
         Forward function for text model
@@ -335,15 +341,15 @@
             with torch.no_grad():
                 backbone_outputs = backbone(**inputs)
                 backbone_outputs = TextClassifierSelectToken(
                     backbone_outputs, inputs=inputs, configs=initial_config
                 )
                 if not classifier:
                     return backbone_outputs
-                logits = self.classifier_head(backbone_outputs)
+                logits = classifier_head(backbone_outputs)
             return logits
         else:
             if freeze:
                 # Do not compute gradient for backbone weights
                 with torch.no_grad():
                     backbone_outputs = backbone(**inputs)
                     backbone_outputs = TextClassifierSelectToken(
@@ -354,22 +360,23 @@
                 backbone_outputs = backbone(**inputs)
                 backbone_outputs = TextClassifierSelectToken(
                     backbone_outputs, inputs=inputs, configs=initial_config
                 )
 
             if not classifier:
                 return backbone_outputs
-            logits = self.classifier_head(backbone_outputs)
+            logits = classifier_head(backbone_outputs)
 
             return logits
 
     def image_forward(
         self,
         input_img_paths: List[str],
         backbone: nn.Module,
+        classifier_head: nn.Module,
         freeze: bool = False,
         eval: bool = False,
         classifier: bool = True,
     ):
         """
         Forward function for image model
 
@@ -386,15 +393,15 @@
                 device=self.device,
                 transforms=self.val_transforms,
             )
             with torch.no_grad():
                 backbone_outputs = backbone.forward(inputs)
                 if not classifier:
                     return backbone_outputs
-                logits = self.classifier_head(backbone_outputs)
+                logits = classifier_head(backbone_outputs)
             return logits
         else:
             inputs = ImageClassifierInputPreprocess(
                 input_img_paths,
                 device=self.device,
                 transforms=self.train_transforms,
             )
@@ -405,15 +412,15 @@
             # LORA and full fine-tuning case.
             else:
                 backbone_outputs = backbone.forward(inputs)
 
             if not classifier:
                 return backbone_outputs
 
-            logits = self.classifier_head(backbone_outputs)
+            logits = classifier_head(backbone_outputs)
 
             return logits
 
     def training_step(self, batch, batch_idx):
         """
         Training step for LightningModule
         """
@@ -806,18 +813,26 @@
             for name, params in backbone.named_parameters():
                 backbone_pg.append(params)
             optimizer.add_param_group(
                 {"params": backbone_pg, "lr": backbone_learning_rate}
             )
         return optimizer
 
-    def get_lr_scheduler(self, optimizer):
+    def get_lr_scheduler(self, optimizer, lr_scheduler_type: str):
         """
         Get the learning rate scheduler (Currently supporting only linear warmup, will be adding more in future)
         """
-        lr_scheduler = get_linear_schedule_with_warmup(
-            optimizer=optimizer,
-            num_warmup_steps=0.06 * self.trainer.estimated_stepping_batches,
-            num_training_steps=self.trainer.estimated_stepping_batches,
-        )
+        if lr_scheduler_type == "linear_warmup":
+            lr_scheduler = get_linear_schedule_with_warmup(
+                optimizer=optimizer,
+                num_warmup_steps=0.06 * self.trainer.estimated_stepping_batches,
+                num_training_steps=self.trainer.estimated_stepping_batches,
+            )
+        elif lr_scheduler_type == "constant":
+            lambda_constant = lambda epoch: 1.0
+            lr_scheduler = torch.optim.lr_scheduler.LambdaLR(
+                optimizer, lr_lambda=lambda_constant
+            )
+        else:
+            raise ValueError(f"lr_scheduler_type {lr_scheduler_type} is not supported.")
 
         return lr_scheduler
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/custom_ops.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/custom_ops.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/head_classifier.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/head_classifier.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_classifier/image_config.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/text_classifier/text_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,61 @@
+import torch
 import logging
 from ..base_config import BaseClassifierConfig
 
 logger = logging.getLogger(__name__)
 
 
-class ImageClassifierConfig(BaseClassifierConfig):
+class TextClassifierConfig(BaseClassifierConfig):
     """
-    Image Classifier Config.
-    Containing all the hyperparameters for training and inference.
+    Text Classifier Config.
 
     Args:
-        backbone_name (str): Name of the backbone model. Defaults to "eva_large_patch14_196.in22k_ft_in22k_in1k".
-        classifier_learning_rate (float): Learning rate for the classifier. Defaults to 1e-3.
-        backbone_learning_rate (float): Learning rate for the backbone. Defaults to 4e-5.
-        freeze (bool): Freeze the backbone. Defaults to False.
-        lora (bool): Use LoRA. Defaults to False.
-        lora_r (int): LoRA r. Defaults to 16.
-        lora_alpha (int): LoRA alpha. Defaults to 16.
-        lora_target_modules (str): LoRA target modules. Defaults to ["qkv"].
-        lora_dropout (float): LoRA dropout. Defaults to 0.1.
-        auto_augment (str): Image augmentation method. Defaults to "rand-n3-mstd1".
-        crop_ratio (float): Minimum crop ratio for when augmentate image, default: 0.9.
+        text_prompt (str): Text prompt for the task, default: "{}의 상품 종류는?".
+        backbone_name (str): Name of the backbone model, default: "EleutherAI/polyglot-ko-1.3b".
+        classifier_learning_rate (float): Learning rate for the classifier, default: 1e-3.
+        backbone_learning_rate (float): Learning rate for the backbone, default: 3e-4.
+        freeze (bool): Whether to freeze the backbone, default: False.
+        lora (bool): Whether to use LoRA for the backbonㄷ, default: True.
+        lora_r (int): LoRA r parameter, default: 16.
+        lora_alpha (int): LoRA alpha parameter, default: 16.
+        lora_target_modules (list): LoRA target modules, default: ["query_key_value"].
+        lora_dropout (float): LoRA dropout, default: 0.1.
     """
 
     def __init__(
         self,
-        backbone_name: str = "eva_large_patch14_196.in22k_ft_in22k_in1k",
+        text_prompt: str = "{}의 상품 종류는?",
+        backbone_name: str = "EleutherAI/polyglot-ko-1.3b",
         classifier_learning_rate: float = 1e-3,
-        backbone_learning_rate: float = 4e-5,
+        backbone_learning_rate: float = 3e-4,
         freeze: bool = False,
-        lora: bool = False,
+        lora: bool = True,
         lora_r: int = 16,
         lora_alpha: int = 16,
-        lora_target_modules: str = ["qkv"],
+        lora_target_modules: list = None,
         lora_dropout: float = 0.1,
-        auto_augment: str = "rand-n3-mstd1",
-        crop_ratio: float = 0.9,
         **kwargs
     ):
         super().__init__(**kwargs)
-
+        # 태스크에 맞게 text prompt 수정 필수!
+        self.text_prompt = text_prompt
         self.backbone_name = backbone_name
         self.classifier_learning_rate = classifier_learning_rate
         self.backbone_learning_rate = backbone_learning_rate
+
         self.freeze = freeze
         self.lora = lora
         if self.freeze and self.lora:
             raise ValueError(
                 "freezing backbone and using lora cannot be True at the same time"
             )
 
         self.lora_r = lora_r
         self.lora_alpha = lora_alpha
-        self.lora_target_modules = lora_target_modules
+        if lora_target_modules is None:
+            self.lora_target_modules = ["query_key_value"]
+        else:
+            self.lora_target_modules = lora_target_modules
         self.lora_dropout = lora_dropout
-
-        # Image augmentation method
-        self.auto_augment = auto_augment
-        self.crop_ratio = crop_ratio
-        # Boolean to check if the model is loaded from transformers or timm, will be set in trainer
-        self.timm = None
+        # Boolean to check if the model is loaded from transformers or timm, default value is False for TextClassifier
+        self.timm = False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_classifier/image_datamodule.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_classifier/image_datamodule.py`

 * *Files 26% similar despite different names*

```diff
@@ -64,25 +64,96 @@
         train_dataset: pd.DataFrame,
         val_dataset: pd.DataFrame,
         test_dataset: pd.DataFrame,
         train_config: ImageClassifierConfig,
     ):
         super().__init__(train_dataset, val_dataset, test_dataset, train_config)
 
-        self.train_dataset = train_dataset
-        self.val_dataset = val_dataset
-        self.test_dataset = test_dataset
-        self.batch_size = train_config.batch_size
-        self.num_workers = train_config.num_workers
-        self.problem_type = train_config.problem_type
-        self.num_class = train_config.num_class
 
     def setup(self, stage: Optional[str] = None):
         self.trainset = ImageClassifierDataset(
             self.train_dataset, self.problem_type, self.num_class
         )
         self.valset = ImageClassifierDataset(
             self.val_dataset, self.problem_type, self.num_class
         )
         self.testset = ImageClassifierDataset(
             self.test_dataset, self.problem_type, self.num_class
         )
+
+
+class FeedbackImageClassifierDataset(Dataset):
+    """
+    Feedback Image Classifier Dataset.
+
+    Args:
+        data (pd.DataFrame): Dataframe containing image path and label.
+        problem_type (str): Problem type, either "single_label_classification" or "multi_label_classification".
+        num_class (int): Number of classes.
+    """
+
+    def __init__(self, data: pd.DataFrame, problem_type: str, num_class: int):
+        super().__init__()
+        self.img_path_list = data["img_path"].tolist()
+        self.label_list = data["label"].tolist()
+        self.feedback_flag_list = data["feedback_flag"].tolist()
+        self.problem_type = problem_type
+        self.num_class = num_class
+
+    def __getitem__(self, idx):
+        input_img_path = self.img_path_list[idx]
+        label = self.label_list[idx]
+        feedback_flag = self.feedback_flag_list[idx]
+
+        if self.problem_type == "multi_label_classification":
+            target = torch.zeros(self.num_class)
+            # Case for single label, but want to use multi-label loss (e.g. BCE)
+            if type(label) != list:
+                label = [label]
+            for lab in label:
+                # negative sample
+                if lab == -1:
+                    continue
+                target[lab] = 1
+
+            return input_img_path, target, feedback_flag
+        # single label classification
+        else:
+            return input_img_path, label, feedback_flag
+
+    def __len__(self):
+        return len(self.label_list)
+
+
+
+class FeedbackImageClassifierDataModule(BaseDataModule):
+    """
+    Feedback Image Classifier Data Module.
+
+    Args:
+        train_dataset (pd.DataFrame): Training dataset (containing original train data and feedback data).
+        val_dataset (pd.DataFrame): Validation dataset.
+        test_dataset (pd.DataFrame): Test dataset.
+        train_config (ImageClassifierConfig): ImageClassifierConfig.
+    """
+
+    def __init__(
+        self,
+        train_dataset: pd.DataFrame,
+        val_dataset: pd.DataFrame,
+        test_dataset: pd.DataFrame,
+        train_config: ImageClassifierConfig,
+    ):
+        super().__init__(train_dataset, val_dataset, test_dataset, train_config)
+
+    def setup(self, stage: Optional[str] = None):
+        self.trainset = FeedbackImageClassifierDataset(
+            self.train_dataset, self.problem_type, self.num_class
+        )
+        # Use same dataset for validation with and without feedback
+        self.valset = ImageClassifierDataset(
+            self.val_dataset, self.problem_type, self.num_class
+        )
+        # Use same dataset for test with and without feedback
+        self.testset = ImageClassifierDataset(
+            self.test_dataset, self.problem_type, self.num_class
+        )
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_text_classifier/image_text_config.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_text_classifier/image_text_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         text_freeze (bool): Freeze text backbone, default: False.
         image_lora (bool): Use LoRA for image backbone, default: True.
         text_lora (bool): Use LoRA for text backbone, default: True.
         image_lora_r (int): LoRA r for image backbone, default: 16.
         text_lora_r (int): LoRA r for text backbone, default: 16.
         image_lora_alpha (int): LoRA alpha for image backbone, default: 16.
         text_lora_alpha (int): LoRA alpha for text backbone, default: 16.
-        image_lora_target_modules (str): LoRA target modules for image backbone, default: ["qkv"].
-        text_lora_target_modules (str): LoRA target modules for text backbone, default: ["query", "key", "value"].
+        image_lora_target_modules (list): LoRA target modules for image backbone, default: ["qkv"].
+        text_lora_target_modules (list): LoRA target modules for text backbone, default: ["query_key_value"].
         image_lora_dropout (float): LoRA dropout for image backbone, default: 0.1.
         text_lora_dropout (float): LoRA dropout for text backbone, default: 0.1.
         auto_augment (str): Auto augment for image backbone, default: "rand-m9-mstd0.5-inc1".
         crop_ratio (float): Minimum crop ratio for image backbone when augmentation image, default: 0.9.
     """
 
     def __init__(
@@ -43,20 +43,16 @@
         text_freeze: bool = False,
         image_lora: bool = True,
         text_lora: bool = True,
         image_lora_r: int = 16,
         text_lora_r: int = 16,
         image_lora_alpha: int = 16,
         text_lora_alpha: int = 16,
-        image_lora_target_modules: str = ["qkv"],
-        text_lora_target_modules: str = [
-            "query",
-            "key",
-            "value",
-        ],
+        image_lora_target_modules: list = None,
+        text_lora_target_modules: list = None,
         image_lora_dropout: float = 0.1,
         text_lora_dropout: float = 0.1,
         auto_augment: str = "rand-n3-mstd1",
         crop_ratio: float = 0.9,
         **kwargs
     ):
         super().__init__(**kwargs)
@@ -82,18 +78,24 @@
                 "freezing backbone and using lora for text backbone cannot be True at the same time"
             )
 
         self.image_lora_r = image_lora_r
         self.text_lora_r = text_lora_r
         self.image_lora_alpha = image_lora_alpha
         self.text_lora_alpha = text_lora_alpha
-        self.image_lora_target_modules = image_lora_target_modules
-        self.text_lora_target_modules = text_lora_target_modules
+        if image_lora_target_modules is None:
+            self.image_lora_target_modules = ["qkv"]
+        else:
+            self.image_lora_target_modules = image_lora_target_modules
+        if text_lora_target_modules is None:
+            self.text_lora_target_modules = ["query_key_value"]
+        else:
+            self.text_lora_target_modules = text_lora_target_modules
         self.image_lora_dropout = image_lora_dropout
         self.text_lora_dropout = text_lora_dropout
         # Image Augmentation
         self.auto_augment = auto_augment
         self.crop_ratio = crop_ratio
-        
+
         # Boolean to check if the model is loaded from transformers or timm, will be set in trainer
         self.text_timm = False
         self.image_timm = None
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/image_text_classifier/image_text_trainer.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/image_classifier/image_trainer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,40 @@
+import logging
 import torch
-from ..head_classifier import *
 
-from .image_text_config import ImageTextClassifierConfig
+from ..head_classifier import *
+from .image_config import ImageClassifierConfig
 from ..base_trainer import BaseClassifierModule
+from ..base_feedback_trainer import FeedbackBaseClassifierModule
 
+logger = logging.getLogger(__name__)
 
-class ImageTextClassifierModule(BaseClassifierModule):
+
+class ImageClassifierModule(BaseClassifierModule):
     """
-    Image Text Classifier Module.
+    Image Classifier for training and inference.
 
     Args:
-        train_config (ImageTextClassifierConfig): ImageTextClassifierConfig.
+        train_config (ImageClassifierConfig): ImageClassifierConfig.
     """
 
-    def __init__(self, train_config: ImageTextClassifierConfig):
+    def __init__(self, train_config: ImageClassifierConfig):
         super().__init__(train_config)
 
         (
-            self.image_backbone,
+            self.backbone,
             self.train_transforms,
             self.val_transforms,
-            self.image_data_config,
-            self.train_config.image_timm,
-            self.image_initial_config,
-            self.text_backbone,
-            self.tokenizer,
-            self.text_initial_config,
-            self.delete_input_key_list,
+            self.data_config,
+            self.train_config.timm,
+            self.initial_config,
         ) = self.get_model()
-        # Concat embedding
-        self.image_embedding_size = self.image_backbone.forward(
-            torch.randn(self.image_data_config["input_size"]).unsqueeze(0)
+        self.embedding_size = self.backbone.forward(
+            torch.randn(self.data_config["input_size"]).unsqueeze(0)
         ).shape[-1]
-        self.text_embedding_size = self.text_initial_config.hidden_size
-        self.embedding_size = self.image_embedding_size + self.text_embedding_size
 
         # Define classifier
         if type(self.train_config.fc_classifier) == str:
             classifier_class = globals()[self.train_config.fc_classifier]
             self.classifier_head = classifier_class(
                 self.embedding_size, self.train_config.num_class
             )
@@ -46,80 +43,144 @@
                 self.embedding_size, self.train_config.num_class
             )
 
         self.save_hyperparameters()
 
     def get_model(self):
         """
-        Get model from config.
-        Return image_backbone, train_transforms, val_transforms, image_initial_config, image_timm, text_backbone, tokenizer, text_initial_config, delete_input_key_list
+        Get model, train transforms, val transforms, initial config, and timm flag.
         """
-        # Get Text Models
-        get_text_model_result = self.get_text_model(
-            self.train_config.text_backbone_name,
-            self.train_config.text_freeze,
-            self.train_config.text_lora,
-            self.train_config.text_lora_r,
-            self.train_config.text_lora_alpha,
-            self.train_config.text_lora_target_modules,
-            self.train_config.text_lora_dropout,
-        )
-        get_image_model_result = self.get_image_model(
-            self.train_config.image_backbone_name,
-            self.train_config.image_freeze,
-            self.train_config.image_lora,
-            self.train_config.image_lora_r,
-            self.train_config.image_lora_alpha,
-            self.train_config.image_lora_target_modules,
-            self.train_config.image_lora_dropout,
+        return self.get_image_model(
+            self.train_config.backbone_name,
+            self.train_config.freeze,
+            self.train_config.lora,
+            self.train_config.lora_r,
+            self.train_config.lora_alpha,
+            self.train_config.lora_target_modules,
+            self.train_config.lora_dropout,
         )
 
-        return get_image_model_result + get_text_model_result
-
     # model forward
-    def forward(self, input_img_paths, input_texts, eval=False, classifier=True):
-        image_backbone_outputs = self.image_forward(
+    def forward(
+        self,
+        input_img_paths,
+        backbone=None,
+        classifier_head=None,
+        eval=False,
+        classifier=True,
+    ):
+        if backbone is None:
+            backbone = self.backbone
+        if classifier_head is None:
+            classifier_head = self.classifier_head
+        return self.image_forward(
             input_img_paths,
-            self.image_backbone,
-            self.train_config.image_freeze,
+            backbone,
+            classifier_head,
+            self.train_config.freeze,
             eval=eval,
-            classifier=False,
-        )
-        text_backbone_outputs = self.text_forward(
-            input_texts,
-            self.text_backbone,
-            self.text_initial_config,
-            self.train_config.text_freeze,
-            eval=eval,
-            classifier=False,
+            classifier=classifier,
         )
 
-        backbone_outputs = torch.cat(
-            [image_backbone_outputs, text_backbone_outputs], dim=1
+    def configure_optimizers(self):
+        optimizer = self.classifier_head_optimizers()
+        optimizer = self.add_optimizers(
+            optimizer,
+            self.backbone,
+            self.train_config.freeze,
+            self.train_config.lora,
+            self.train_config.backbone_learning_rate,
         )
-        if classifier:
-            logits = self.classifier_head(backbone_outputs)
 
-            return logits
+        lr_scheduler = self.get_lr_scheduler(optimizer, self.train_config.lr_scheduler)
+
+        return [optimizer], [{"scheduler": lr_scheduler}]
+
+
+class FeedbackImageClassifierModule(FeedbackBaseClassifierModule):
+    """
+    FeedbackImage Classifier for training and inference.
+
+    Args:
+        train_config (ImageClassifierConfig): ImageClassifierConfig.
+    """
+
+    def __init__(self, train_config: ImageClassifierConfig):
+        super().__init__(train_config)
+
+        (
+            self.backbone,
+            self.train_transforms,
+            self.val_transforms,
+            self.data_config,
+            self.train_config.timm,
+            self.initial_config,
+        ) = self.get_model()
+        self.embedding_size = self.backbone.forward(
+            torch.randn(self.data_config["input_size"]).unsqueeze(0)
+        ).shape[-1]
+
+        # Define classifier
+        if type(self.train_config.fc_classifier) == str:
+            classifier_class = globals()[self.train_config.fc_classifier]
+            self.classifier_head = classifier_class(
+                self.embedding_size, self.train_config.num_class
+            )
         else:
-            return backbone_outputs
+            self.classifier_head = self.train_config.fc_classifier(
+                self.embedding_size, self.train_config.num_class
+            )
+
+        self.save_hyperparameters()
+
+    def get_model(self):
+        """
+        Get model, train transforms, val transforms, initial config, and timm flag.
+        """
+        return self.get_image_model(
+            self.train_config.backbone_name,
+            self.train_config.freeze,
+            self.train_config.lora,
+            self.train_config.lora_r,
+            self.train_config.lora_alpha,
+            self.train_config.lora_target_modules,
+            self.train_config.lora_dropout,
+        )
+
+    # model forward
+    def forward(
+        self,
+        input_img_paths,
+        backbone=None,
+        classifier_head=None,
+        eval=False,
+        classifier=True,
+    ):
+        if backbone is None:
+            if type(self.backbone) == nn.ModuleList:
+                backbone = self.backbone[0]
+            else:
+                backbone = self.backbone
+        if classifier_head is None:
+            classifier_head = self.classifier_head
+        return self.image_forward(
+            input_img_paths,
+            backbone,
+            classifier_head,
+            self.train_config.freeze,
+            eval=eval,
+            classifier=classifier,
+        )
 
     def configure_optimizers(self):
         optimizer = self.classifier_head_optimizers()
         optimizer = self.add_optimizers(
             optimizer,
-            self.text_backbone,
-            self.train_config.text_freeze,
-            self.train_config.text_lora,
-            self.train_config.text_backbone_learning_rate,
-        )
-        optimizer = self.add_optimizers(
-            optimizer,
-            self.image_backbone,
-            self.train_config.image_freeze,
-            self.train_config.image_lora,
-            self.train_config.image_backbone_learning_rate,
+            self.backbone,
+            self.train_config.freeze,
+            self.train_config.lora,
+            self.train_config.backbone_learning_rate,
         )
 
-        lr_scheduler = self.get_lr_scheduler(optimizer)
+        lr_scheduler = self.get_lr_scheduler(optimizer, self.train_config.lr_scheduler)
 
         return [optimizer], [{"scheduler": lr_scheduler}]
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/text_classifier/text_datamodule.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/text_classifier/text_datamodule.py`

 * *Files 23% similar despite different names*

```diff
@@ -74,7 +74,82 @@
         )
         self.valset = TextClassifierDataset(
             self.val_dataset, self.problem_type, self.num_class
         )
         self.testset = TextClassifierDataset(
             self.test_dataset, self.problem_type, self.num_class
         )
+        
+class FeedbackTextClassifierDataset(Dataset):
+    """
+    Feedback Text Classifier Dataset.
+
+    Args:
+        data (pd.DataFrame): Dataframe with columns ["text", "label"].
+        problem_type (str): Problem type, either "multi_label_classification" or "single_label_classification".
+        num_class (int): Number of classes.
+    """
+
+    def __init__(self, data: pd.DataFrame, problem_type: str, num_class: int):
+        super().__init__()
+        self.text_list = data["text"].tolist()
+        self.label_list = data["label"].tolist()
+        self.feedback_flag_list = data["feedback_flag"].tolist()
+        self.problem_type = problem_type
+        self.num_class = num_class
+
+    def __getitem__(self, idx):
+        input_text = self.text_list[idx]
+        label = self.label_list[idx]
+        feedback_flag = self.feedback_flag_list[idx]
+
+        if self.problem_type == "multi_label_classification":
+            target = torch.zeros(self.num_class)
+            # Case for single label, but want to use multi-label loss (e.g. BCE)
+            if type(label) != list:
+                label = [label]
+            for lab in label:
+                # negative sample
+                if lab == -1:
+                    continue
+                target[lab] = 1
+
+            return input_text, target, feedback_flag
+
+        # single label classification
+        else:
+            return input_text, label, feedback_flag
+
+    def __len__(self):
+        return len(self.label_list)
+
+
+class FeedbackTextClassifierDataModule(BaseDataModule):
+    """
+    Feedback Text Classifier Data Module.
+
+    Args:
+        train_dataset (pd.DataFrame): Training dataset (containing original train data and feedback data).
+        val_dataset (pd.DataFrame): Validation dataset.
+        test_dataset (pd.DataFrame): Test dataset.
+        train_config (TextClassifierConfig): TextClassifierConfig.
+    """
+
+    def __init__(
+        self,
+        train_dataset: pd.DataFrame,
+        val_dataset: pd.DataFrame,
+        test_dataset: pd.DataFrame,
+        train_config: TextClassifierConfig,
+    ):
+        super().__init__(train_dataset, val_dataset, test_dataset, train_config)
+
+    def setup(self, stage: Optional[str] = None):
+        self.trainset = FeedbackTextClassifierDataset(
+            self.train_dataset, self.problem_type, self.num_class
+        )
+        self.valset = TextClassifierDataset(
+            self.val_dataset, self.problem_type, self.num_class
+        )
+        self.testset = TextClassifierDataset(
+            self.test_dataset, self.problem_type, self.num_class
+        )
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/trainer_util.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/trainer_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,18 +10,46 @@
 from PIL import Image
 import requests
 from optimum.onnxruntime import ORTModel
 import json
 import logging
 from easydict import EasyDict
 from transformers import AutoConfig
+import torch.nn.functional as F  ## hm
+from copy import deepcopy
+import torch.nn as nn
+
 
 logger = logging.getLogger(__name__)
 
 
+def sample_stratified(df, n_samples_per_label, problem_type):
+    """
+    Returns a stratified sample of rows from the dataframe, ensuring that each 'label' value is
+    equally represented according to n_samples_per_label.
+
+    Parameters:
+    - df: DataFrame to sample from.
+    - n_samples_per_label: Number of samples to draw for each label.
+
+    Returns:
+    - Stratified sample of the dataframe.
+    """
+    # Group by 'label' and sample n_samples_per_label from each group
+    df_copy = df.copy()
+    if problem_type == "multi_label_classification":
+        # select random label in label_list
+        df_copy["label"] = df_copy["label"].apply(lambda x: random.choice(x))
+    sampled_df = df_copy.groupby("label", group_keys=False).apply(
+        lambda x: x.sample(min(len(x), n_samples_per_label))
+    )
+
+    return sampled_df
+
+
 def set_seed(seed: int):
     """
     Helper function for reproducible behavior to set the seed in `random`, `numpy`, `torch` and/or `tf` (if installed).
 
     Args:
         seed (`int`): The seed to set.
     """
@@ -113,15 +141,15 @@
         text_backbone_save_module.save_pretrained(os.path.join(save_dir, "text"))
         # Save Tokenizer
         train_module.tokenizer.save_pretrained(os.path.join(save_dir, "text"))
         train_module.text_initial_config.save_pretrained(os.path.join(save_dir, "text"))
 
         # with open(os.path.join(save_dir, "image", "config.json"), "w") as f:
         #     json.dump(train_module.image_initial_config, f)
-            
+
         if train_module.image_initial_config is not None:
             train_module.image_initial_config.save_pretrained(save_dir)
 
         # Save validation transform with pickle
         with open(os.path.join(save_dir, "image", "val_transforms.pkl"), "wb") as f:
             pickle.dump(train_module.val_transforms, f)
 
@@ -164,18 +192,20 @@
         classifier_head_save_module,
         dummy_input,
         os.path.join(save_dir, "classifier_head.onnx"),
         input_names=["embeddings"],
         output_names=["logits"],
         dynamic_axes={"embeddings": {0: "batch_size"}, "logits": {0: "batch_size"}},
     )
-    
+
     ## Classifier save to ckpt
-    
-    torch.save(classifier_head_save_module, os.path.join(save_dir, "classifier_head.ckpt"))
+
+    torch.save(
+        classifier_head_save_module, os.path.join(save_dir, "classifier_head.ckpt")
+    )
 
 
 def export_onnx(model_type: str, save_dir: str, device: str = "gpu"):
     """
     Export Huggingface backbone model to onnx format.
     Args:
         model_type (`str`): Model type string, e.g. "TextClassifier", "ImageClassifier", "ImageTextClassifier"
@@ -388,29 +418,31 @@
     """
     inputs = []
     # PIL open image then preprocess with augmentation.
     for img_path in input_img_paths:
         if type(img_path) == str:
             try:
                 if img_path.startswith("https:"):
-                    input_img = Image.open(requests.get(img_path, stream=True).raw).convert(
-                        "RGB"
-                    )
+                    input_img = Image.open(
+                        requests.get(img_path, stream=True).raw
+                    ).convert("RGB")
                 else:
                     input_img = Image.open(img_path).convert("RGB")
             except:
                 logger.warning(
                     f"Cannot open image {img_path}, use zero padding image instead"
                 )
                 input_img = Image.fromarray(np.zeros((224, 224, 3), dtype=np.uint8))
-        ### 보통 inference할 때만 사용. -> pil image 자체가 input인 경우. 
+        ### 보통 inference할 때만 사용. -> pil image 자체가 input인 경우.
         elif isinstance(img_path, Image.Image):
             input_img = img_path.convert("RGB")
         else:
-            raise TypeError("Not supported input type for image classifier. Only support img path or pil image.")
+            raise TypeError(
+                "Not supported input type for image classifier. Only support img path or pil image."
+            )
         input_tensor = transforms(input_img).to(device)
         inputs.append(input_tensor)
 
     return torch.stack(inputs)
 
 
 def TextClassifierInputPreprocess(
@@ -473,12 +505,132 @@
     ):
         last_hidden_state = backbone_outputs[0]
         if type(last_hidden_state) == np.ndarray:
             last_hidden_state = torch.from_numpy(last_hidden_state)
         selected_tokens = last_hidden_state[:, 0]
 
         return selected_tokens
+    ##  hm
+    elif configs.model_type == "mpnet":
+        # print('============= you are here =============')
+        def mean_pooling(model_output, attention_mask):
+            token_embeddings = model_output[0]
+            input_mask_expanded = (
+                attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
+            )
+            return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(
+                input_mask_expanded.sum(1), min=1e-9
+            )
+
+        attention_mask = inputs["attention_mask"]
+
+        if type(backbone_outputs) == np.ndarray:
+            backbone_outputs = torch.from_numpy(backbone_outputs)
+
+        selected_tokens = mean_pooling(backbone_outputs, attention_mask)
+        selected_tokens = F.normalize(selected_tokens, p=2, dim=1)
+
+        return selected_tokens
 
     else:
         raise NotImplementedError(
             f"{configs.model_type} selecting token method is not implemented."
         )
+
+
+def is_parallel(model):
+    """check if model is in parallel mode."""
+
+    parallel_type = (
+        nn.parallel.DataParallel,
+        nn.parallel.DistributedDataParallel,
+    )
+    return isinstance(model, parallel_type)
+
+
+def copy_attr(a, b, include=(), exclude=()):
+    # Copy attributes from b to a, options to only include [...] and to exclude [...]
+    for k, v in b.__dict__.items():
+        if (len(include) and k not in include) or k.startswith("_") or k in exclude:
+            continue
+        else:
+            setattr(a, k, v)
+
+
+class ModelEMA:
+    """
+    Model Exponential Moving Average from https://github.com/rwightman/pytorch-image-models
+    Keep a moving average of everything in the model state_dict (parameters and buffers).
+    This is intended to allow functionality like
+    https://www.tensorflow.org/api_docs/python/tf/train/ExponentialMovingAverage
+    A smoothed version of the weights is necessary for some training schemes to perform well.
+    This class is sensitive where it is initialized in the sequence of model init,
+    GPU assignment and distributed training wrappers.
+    """
+
+    def __init__(self, models, decay=0.9999, updates=0):
+        """
+        Args:
+            models (tuple of nn.Module): model list to apply EMA.
+            decay (float): ema decay reate.
+            updates (int): counter of EMA updates.
+        """
+        # Create EMA(FP32)
+        self.ema = ()
+        self.updates = ()
+        self.decay = decay
+        for model in models:
+            ema = deepcopy(model.module if is_parallel(model) else model).eval()
+            self.ema = self.ema + (ema,)
+            # decay exponential ramp (to help early epochs)
+            # self.decay = lambda x: decay * (1 - math.exp(-x / 2000))
+            for p in ema.parameters():
+                p.requires_grad_(False)
+
+        self.updates = (updates,) * len(models)
+
+    def update(self, models):
+        # Update EMA parameters
+        self.updates += 1
+        for idx, model in enumerate(models):
+            with torch.no_grad():
+                # d = self.decay(self.updates)
+                d = self.decay
+                msd = (
+                    model.module.state_dict()
+                    if is_parallel(model)
+                    else model.state_dict()
+                )  # model state_dict
+                for k, v in self.ema[idx].state_dict().items():
+                    if v.dtype.is_floating_point:
+                        v *= d
+                        v += (1.0 - d) * msd[k].detach()
+
+    @staticmethod
+    def update_attr(
+        updating_models,
+        cand_models,
+        include=(),
+        exclude=("process_group", "reducer", "training"),
+    ):
+        for updating_model, cand_model in zip(updating_models, cand_models):
+            # Update EMA attributes
+            copy_attr(updating_model, cand_model, include, exclude)
+
+
+def find_indices_based_on_max_and_label(tensor, labels, threshold):
+    # 각 행의 최대값과 그 인덱스를 계산
+    max_values, max_indices = torch.max(tensor, dim=1)
+
+    # 조건 1: 최대값이 threshold보다 큰 경우
+    condition1 = max_values > threshold
+
+    # 조건 2: 최대값의 인덱스가 labels와 일치하는 경우
+    condition2 = max_indices == labels
+
+    # 두 조건을 모두 만족하는 경우
+    valid_indices = torch.where(condition1 & condition2)[0]
+
+    # 두 조건 중 하나라도 만족하지 않는 경우
+    invalid_indices = torch.where(~(condition1 & condition2))[0]
+
+    return valid_indices, invalid_indices
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_classifier.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_classifier.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_config.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_config.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_datamodule.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/classifier/zeroshot_classifier/zeroshot_image_datamodule.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/losses.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/losses.py`

 * *Files 26% similar despite different names*

```diff
@@ -158,14 +158,44 @@
         torch.Tensor: binary cross entropy with logits
     """
     return F.binary_cross_entropy_with_logits(
         inputs, targets
     )  # , pos_weight=pos_weight.to(inputs.device))
 
 
+def cross_entropy_from_probabilities(true_distributions, pred_distributions):
+    """
+    Calculates the cross entropy between two probability distributions that have already been applied with softmax.
+
+    Parameters:
+    - true_distributions: The actual distribution (target distribution). A PyTorch tensor.
+    - pred_distributions: The predicted distribution. A PyTorch tensor.
+
+    Returns:
+    - The cross entropy value between the two distributions. (scalar)
+    """
+    # 두 분포 간의 cross entropy 계산
+    cross_entropy = -torch.sum(true_distributions * torch.log(pred_distributions + 1e-9)) # / true_distributions.size(0)
+    return cross_entropy
+
+def binary_cross_entropy_from_probabilities(true_distributions, pred_distributions):
+    """
+    Calculates the binary cross entropy between two probability distributions that have already been applied with softmax.
+
+    Parameters:
+    - true_distributions: The actual distribution (target distribution). A PyTorch tensor.
+    - pred_distributions: The predicted distribution. A PyTorch tensor.
+
+    Returns:
+    - The binary cross entropy value between the two distributions. (scalar)
+    """
+    # 두 분포 간의 binary cross entropy 계산
+    binary_cross_entropy = -torch.sum(true_distributions * torch.log(pred_distributions + 1e-9) + (1 - true_distributions) * torch.log(1 - pred_distributions + 1e-9)) # / true_distributions.size(0)
+    return binary_cross_entropy
+
 LOSSES = {
     "cross_entropy": F.cross_entropy,
     "focal_loss": focal_loss,
     "focal_loss_with_label_smoothing": focal_loss_with_label_smoothing,
     "binary_cross_entropy": bce_with_logits,
     "binary_focal_loss": binary_focal_loss,
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/__init__.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/onnx_pipeline.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/onnx_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             only_backbone (bool, optional): Only return backbone output embedding. Defaults to False.
         """
         if only_backbone and last_embedding:
             raise ValueError(
                 "only_backbone and last_embedding cannot be True at the same time."
             )
 
-        if type(inputs) == str:
+        if type(inputs) != list:
             inputs = [inputs]
 
         preprocessed_inputs = TextClassifierInputPreprocess(
             inputs,
             text_prompt=self.text_prompt,
             device=self.device,
             tokenizer=self.tokenizer,
@@ -274,15 +274,15 @@
             only_backbone (bool, optional): Only return backbone output embedding. Defaults to False.
         """
         if only_backbone and last_embedding:
             return ValueError(
                 "only_backbone and last_embedding cannot be True at the same time."
             )
 
-        if type(inputs) == str:
+        if type(inputs) != list:
             inputs = [inputs]
 
         #  preprocessed_inputs = TextClassifierInputPreprocess(
         #     inputs,
         #     text_prompt=self.text_prompt,
         #     device=self.device,
         #     tokenizer=self.tokenizer,
@@ -320,15 +320,14 @@
             emb = F.relu(emb)
             return emb.detach().cpu().numpy()
 
         # CLassifier ort input preprocess
         classifier_ort_input_dict = classifier_onnx_preprocess(
             self.classifier_ort_session, embeddings
         )
-        breakpoint()
         logits = onnx_inference(
             self.classifier_ort_session, classifier_ort_input_dict, self.device
         )
 
         return postprocess(
             logits, topk, self.label_name_list, return_logits, sigmoid, temperature
         )
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/onnx_util.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/onnx_util.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/pytorch_pipeline.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/pytorch_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         model_class = globals()[train_module_name]
         ckpt_path = os.path.join(save_dir, "model.ckpt")
         self.pretrained_model = model_class.load_from_checkpoint(
             ckpt_path, map_location=self.device
         )
         self.pretrained_model.eval()
 
+        self.label_name_list = self.pretrained_model.train_config.label_name_list
+
     def __call__(
         self,
         inputs: Union[str, List[str]],
         topk: int = 1,
         return_logits: bool = False,
         sigmoid: bool = False,
         only_backbone: bool = False,
@@ -162,15 +164,15 @@
                         return emb.detach().cpu().numpy()
                     with torch.autocast(self.autocast_device):
                         logits = self.pretrained_model.forward(inputs, eval=True)
 
         return postprocess(
             logits,
             topk,
-            self.pretrained_model.train_config.label_name_list,
+            self.label_name_list,
             return_logits,
             sigmoid,
             temperature,
         )
 
     def backbone_to_float32(self):
         self.pretrained_model = self.pretrained_model.float()
```

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai/core/pipeline/util.py` & `dalpha_ai_cpu-0.3.0/dalpha_ai/core/pipeline/util.py`

 * *Files identical despite different names*

### Comparing `dalpha_ai_cpu-0.2.9/dalpha_ai_cpu.egg-info/SOURCES.txt` & `dalpha_ai_cpu-0.3.0/dalpha_ai_cpu.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 dalpha_ai/__init__.py
 dalpha_ai/core/__init__.py
 dalpha_ai/core/losses.py
 dalpha_ai/core/classifier/__init__.py
 dalpha_ai/core/classifier/base_classifier.py
 dalpha_ai/core/classifier/base_config.py
 dalpha_ai/core/classifier/base_datamodule.py
+dalpha_ai/core/classifier/base_feedback_trainer.py
 dalpha_ai/core/classifier/base_trainer.py
 dalpha_ai/core/classifier/custom_ops.py
 dalpha_ai/core/classifier/head_classifier.py
 dalpha_ai/core/classifier/trainer_util.py
 dalpha_ai/core/classifier/image_classifier/__init__.py
 dalpha_ai/core/classifier/image_classifier/image_classifier.py
 dalpha_ai/core/classifier/image_classifier/image_config.py
```

