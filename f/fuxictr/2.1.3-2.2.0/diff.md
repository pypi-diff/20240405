# Comparing `tmp/fuxictr-2.1.3.tar.gz` & `tmp/fuxictr-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuxictr-2.1.3.tar", last modified: Sat Feb 17 01:02:06 2024, max compression
+gzip compressed data, was "dist/fuxictr-2.2.0.tar", last modified: Fri Apr  5 14:22:28 2024, max compression
```

## Comparing `fuxictr-2.1.3.tar` & `fuxictr-2.2.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29940 2024-02-17 01:02:06.000000 fuxictr-2.1.3/PKG-INFO
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    27518 2024-02-17 01:01:56.000000 fuxictr-2.1.3/README.md
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2022-11-14 09:29:53.000000 fuxictr-2.1.3/fuxictr/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6557 2023-05-28 13:18:32.000000 fuxictr-2.1.3/fuxictr/autotuner.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/datasets/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       64 2023-05-16 14:41:26.000000 fuxictr-2.1.3/fuxictr/datasets/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1592 2023-05-16 14:41:36.000000 fuxictr-2.1.3/fuxictr/datasets/avazu.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1231 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/datasets/criteo.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1826 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/datasets/kkbox.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5503 2023-10-13 06:27:47.000000 fuxictr-2.1.3/fuxictr/features.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4369 2023-05-26 10:25:02.000000 fuxictr-2.1.3/fuxictr/metrics.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/preprocess/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       62 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/preprocess/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5712 2024-02-17 01:01:41.000000 fuxictr-2.1.3/fuxictr/preprocess/build_dataset.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18222 2024-02-17 01:01:56.000000 fuxictr-2.1.3/fuxictr/preprocess/feature_processor.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1716 2024-02-17 01:01:56.000000 fuxictr-2.1.3/fuxictr/preprocess/normalizer.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6703 2024-02-17 01:01:56.000000 fuxictr-2.1.3/fuxictr/preprocess/tokenizer.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/pytorch/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2021-08-10 06:39:20.000000 fuxictr-2.1.3/fuxictr/pytorch/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/pytorch/dataloaders/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       91 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/dataloaders/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5645 2024-02-17 01:01:50.000000 fuxictr-2.1.3/fuxictr/pytorch/dataloaders/h5_block_dataloader.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4050 2024-02-17 01:01:41.000000 fuxictr-2.1.3/fuxictr/pytorch/dataloaders/h5_dataloader.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      164 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1463 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/activations.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/attentions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      108 2023-05-31 09:23:26.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/attentions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1810 2023-05-31 09:23:26.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/attentions/dot_product_attention.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1750 2023-05-31 09:23:26.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5616 2023-05-31 09:23:26.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/attentions/target_attention.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/blocks/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      100 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/blocks/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1416 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/blocks/factorization_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1489 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/blocks/logistic_regression.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2740 2023-05-19 04:47:42.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/blocks/mlp_block.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/embeddings/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       71 2024-02-17 01:00:33.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/embeddings/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10164 2024-02-17 01:01:41.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/embeddings/feature_embedding.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6015 2024-02-17 01:01:56.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      244 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4734 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2303 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5228 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/cross_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2940 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/holographic_interaction.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2924 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/inner_product.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2780 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/interaction_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1820 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/layers/pooling.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/pytorch/models/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       78 2023-06-06 11:51:39.000000 fuxictr-2.1.3/fuxictr/pytorch/models/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6804 2023-07-21 14:07:18.000000 fuxictr-2.1.3/fuxictr/pytorch/models/multitask_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12849 2024-02-17 01:00:33.000000 fuxictr-2.1.3/fuxictr/pytorch/models/rank_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5363 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/pytorch/torch_utils.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/tensorflow/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/tensorflow/dataloaders/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       45 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/dataloaders/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3344 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/dataloaders/tf_dataloader.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      107 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      123 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1482 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/factorization_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1517 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/linear.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1673 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/logistic_regression.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3619 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/mlp_block.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/embeddings/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/embeddings/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11938 2023-05-26 06:50:13.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/interactions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       58 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/interactions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2088 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/interactions/cross_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2969 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/interactions/inner_product.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1065 2023-01-27 08:57:12.000000 fuxictr-2.1.3/fuxictr/tensorflow/layers/pooling.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr/tensorflow/models/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       33 2023-05-19 02:03:38.000000 fuxictr-2.1.3/fuxictr/tensorflow/models/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9279 2023-06-08 01:29:48.000000 fuxictr-2.1.3/fuxictr/tensorflow/models/rank_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2730 2023-05-19 02:30:53.000000 fuxictr-2.1.3/fuxictr/tensorflow/tf_utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4649 2023-02-15 05:02:33.000000 fuxictr-2.1.3/fuxictr/utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       21 2024-02-17 01:01:56.000000 fuxictr-2.1.3/fuxictr/version.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr.egg-info/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29940 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr.egg-info/PKG-INFO
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2823 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr.egg-info/SOURCES.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        1 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr.egg-info/dependency_links.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       48 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr.egg-info/requires.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       18 2024-02-17 01:02:06.000000 fuxictr-2.1.3/fuxictr.egg-info/top_level.txt
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/model_zoo/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1420 2023-06-08 03:05:12.000000 fuxictr-2.1.3/model_zoo/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2024-02-17 01:02:06.000000 fuxictr-2.1.3/model_zoo/multitask/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       69 2023-04-18 04:15:15.000000 fuxictr-2.1.3/model_zoo/multitask/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       38 2024-02-17 01:02:06.000000 fuxictr-2.1.3/setup.cfg
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1547 2024-02-17 01:01:56.000000 fuxictr-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-05 14:22:28.000000 fuxictr-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-05 14:22:22.000000 fuxictr-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/autotuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/datasets/avazu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/datasets/criteo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/datasets/kkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/feature_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/npz_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/rank_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/dot_product_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/target_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/feature_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/holographic_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/interaction_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/models/multitask_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/dataloaders/tf_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/model_zoo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/model_zoo/multitask/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 14:22:22.000000 fuxictr-2.2.0/model_zoo/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:22:28.000000 fuxictr-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-05 14:22:22.000000 fuxictr-2.2.0/setup.py
```

### Comparing `fuxictr-2.1.3/PKG-INFO` & `fuxictr-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.1.3
+Version: 2.2.0
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.1.3 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.2.0 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
```

### Comparing `fuxictr-2.1.3/README.md` & `fuxictr-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/autotuner.py` & `fuxictr-2.2.0/fuxictr/autotuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     # enumerate dataset para combinations
     dataset_dict = {k: tune_dict[k] if k in tune_dict else [v] for k, v in dataset_dict.items()}
     dataset_para_keys = list(dataset_dict.keys())
     dataset_para_combs = dict()
     for idx, values in enumerate(itertools.product(*map(dataset_dict.get, dataset_para_keys))):
         dataset_params = dict(zip(dataset_para_keys, values))
-        if dataset_params["data_format"] == "h5":
+        if dataset_params["data_format"] == "npz":
             dataset_para_combs[dataset_id] = dataset_params
         else:
             hash_id = hashlib.md5("".join(sorted(print_to_json(dataset_params))).encode("utf-8")).hexdigest()[0:8]
             dataset_para_combs[dataset_id + "_{}".format(hash_id)] = dataset_params
 
     # dump dataset para combinations to config file
     dataset_config = os.path.join(config_dir, "dataset_config.yaml")
```

### Comparing `fuxictr-2.1.3/fuxictr/datasets/avazu.py` & `fuxictr-2.2.0/fuxictr/datasets/avazu.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,9 +30,7 @@
         def _convert_weekend(timestamp):
             dt = date(int('20' + timestamp[0:2]), int(timestamp[2:4]), int(timestamp[4:6]))
             return 1 if dt.strftime('%w') in ['6', '0'] else 0
         return df['hour'].apply(_convert_weekend)
 
     def convert_hour(self, df, col_name):
         return df['hour'].apply(lambda x: int(x[6:8]))
-
-
```

### Comparing `fuxictr-2.1.3/fuxictr/datasets/criteo.py` & `fuxictr-2.2.0/fuxictr/datasets/criteo.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,7 @@
         def _convert_to_bucket(value):
             if value > 2:
                 value = int(np.floor(np.log(value) ** 2))
             else:
                 value = int(value)
             return value
         return df[col_name].map(_convert_to_bucket).astype(int)
-
-
-	
-
-
```

### Comparing `fuxictr-2.1.3/fuxictr/datasets/kkbox.py` & `fuxictr-2.2.0/fuxictr/datasets/kkbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,9 +41,7 @@
                 elif age <=50:
                     return "5"
                 elif age <=60:
                     return "6"
                 else:
                     return "7"
         return df[col_name].apply(_bucketize)
-
-
```

### Comparing `fuxictr-2.1.3/fuxictr/features.py` & `fuxictr-2.2.0/fuxictr/features.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/metrics.py` & `fuxictr-2.2.0/fuxictr/metrics.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/preprocess/build_dataset.py` & `fuxictr-2.2.0/fuxictr/preprocess/build_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # =========================================================================
+# Copyright (C) 2024. FuxiCTR Authors. All rights reserved.
 # Copyright (C) 2022. Huawei Technologies Co., Ltd. All rights reserved.
 # 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -11,30 +12,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========================================================================
 
 
-import h5py
 import os
 import logging
 import numpy as np
 import gc
 import multiprocessing as mp
 
 
-def save_h5(darray_dict, data_path):
-    logging.info("Saving data to h5: " + data_path)
-    os.makedirs(os.path.dirname(data_path), exist_ok=True)
-    with h5py.File(data_path, 'w') as hf:
-        for key, arr in darray_dict.items():
-            hf.create_dataset(key, data=arr)
-
-
 def split_train_test(train_ddf=None, valid_ddf=None, test_ddf=None, valid_size=0, 
                      test_size=0, split_type="sequential"):
     num_samples = len(train_ddf)
     train_size = num_samples
     instance_IDs = np.arange(num_samples)
     if split_type == "random":
         np.random.shuffle(instance_IDs)
@@ -51,41 +43,47 @@
         valid_ddf = train_ddf.loc[instance_IDs[train_size:], :].reset_index()
         instance_IDs = instance_IDs[0:train_size]
     if valid_size > 0 or test_size > 0:
         train_ddf = train_ddf.loc[instance_IDs, :].reset_index()
     return train_ddf, valid_ddf, test_ddf
 
 
+def save_npz(darray_dict, data_path):
+    logging.info("Saving data to npz: " + data_path)
+    os.makedirs(os.path.dirname(data_path), exist_ok=True)
+    np.savez(data_path, **darray_dict)
+
+
 def transform_block(feature_encoder, df_block, filename, preprocess=False):
     if preprocess:
         df_block = feature_encoder.preprocess(df_block)
     darray_dict = feature_encoder.transform(df_block)
-    save_h5(darray_dict, os.path.join(feature_encoder.data_dir, filename))
+    save_npz(darray_dict, os.path.join(feature_encoder.data_dir, filename))
 
 
-def transform_h5(feature_encoder, ddf, filename, preprocess=False, block_size=0):
+def transform(feature_encoder, ddf, filename, preprocess=False, block_size=0):
     if block_size > 0:
         pool = mp.Pool(mp.cpu_count() // 2)
         block_id = 0
         for idx in range(0, len(ddf), block_size):
             df_block = ddf[idx: (idx + block_size)]
             pool.apply_async(transform_block, args=(feature_encoder,
                                                     df_block,
-                                                    '{}/part_{}.h5'.format(filename, block_id),
+                                                    '{}/part_{:05d}.npz'.format(filename, block_id),
                                                     preprocess))
             block_id += 1
         pool.close()
         pool.join()
     else:
-        transform_block(feature_encoder, ddf, filename + ".h5", preprocess)
+        transform_block(feature_encoder, ddf, filename, preprocess)
 
 
 def build_dataset(feature_encoder, train_data=None, valid_data=None, test_data=None, valid_size=0, 
                   test_size=0, split_type="sequential", data_block_size=0, **kwargs):
-    """ Build feature_map and transform h5 data """
+    """ Build feature_map and transform data """
 
     feature_map_json = os.path.join(feature_encoder.data_dir, "feature_map.json")
     if os.path.exists(feature_map_json):
         logging.warn("Skip rebuilding {}. Please delete it manually if rebuilding is required." \
                      .format(feature_map_json))
     else:
         # Load csv data
@@ -99,33 +97,33 @@
             test_ddf = feature_encoder.read_csv(test_data, **kwargs)
             train_ddf, valid_ddf, test_ddf = split_train_test(train_ddf, valid_ddf, test_ddf, 
                                                             valid_size, test_size, split_type)
         
         # fit and transform train_ddf
         train_ddf = feature_encoder.preprocess(train_ddf)
         feature_encoder.fit(train_ddf, **kwargs)
-        transform_h5(feature_encoder, train_ddf, 'train', preprocess=False, block_size=data_block_size)
+        transform(feature_encoder, train_ddf, 'train', preprocess=False, block_size=data_block_size)
         del train_ddf
         gc.collect()
 
         # Transfrom valid_ddf
         if valid_ddf is None and (valid_data is not None):
             valid_ddf = feature_encoder.read_csv(valid_data, **kwargs)
         if valid_ddf is not None:
-            transform_h5(feature_encoder, valid_ddf, 'valid', preprocess=True, block_size=data_block_size)
+            transform(feature_encoder, valid_ddf, 'valid', preprocess=True, block_size=data_block_size)
             del valid_ddf
             gc.collect()
 
         # Transfrom test_ddf
         if test_ddf is None and (test_data is not None):
             test_ddf = feature_encoder.read_csv(test_data, **kwargs)
         if test_ddf is not None:
-            transform_h5(feature_encoder, test_ddf, 'test', preprocess=True, block_size=data_block_size)
+            transform(feature_encoder, test_ddf, 'test', preprocess=True, block_size=data_block_size)
             del test_ddf
             gc.collect()
-        logging.info("Transform csv data to h5 done.")
+        logging.info("Transform csv data to npz done.")
     
     # Return processed data splits
     return os.path.join(feature_encoder.data_dir, "train"), \
            os.path.join(feature_encoder.data_dir, "valid"), \
            os.path.join(feature_encoder.data_dir, "test") if (
            test_data or test_size > 0) else None
```

### Comparing `fuxictr-2.1.3/fuxictr/preprocess/feature_processor.py` & `fuxictr-2.2.0/fuxictr/preprocess/feature_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import pandas as pd
 import pickle
 import os
 import logging
 import json
 import re
 import shutil
+from pathlib import Path
 import sklearn.preprocessing as sklearn_preprocess
 from fuxictr.features import FeatureMap
 from .tokenizer import Tokenizer
 from .normalizer import Normalizer
 
 
 class FeatureProcessor(object):
@@ -126,17 +127,18 @@
         os.makedirs(self.data_dir, exist_ok=True)
         for col in self.feature_cols:
             name = col["name"]
             if "pretrained_emb" in col:
                 logging.info("Loading pretrained embedding: " + name)
                 if "pretrain_dim" in col:
                     self.feature_map.features[name]["pretrain_dim"] = col["pretrain_dim"]
+                ext = Path(col["pretrained_emb"]).suffix
                 shutil.copy(col["pretrained_emb"],
-                            os.path.join(self.data_dir, "pretrained_{}.h5".format(name)))
-                self.feature_map.features[name]["pretrained_emb"] = "pretrained_{}.h5".format(name)
+                            os.path.join(self.data_dir, "pretrained_{}{}".format(name, ext)))
+                self.feature_map.features[name]["pretrained_emb"] = "pretrained_{}{}".format(name, ext)
                 self.feature_map.features[name]["freeze_emb"] = col.get("freeze_emb", True)
                 self.feature_map.features[name]["pretrain_usage"] = col.get("pretrain_usage", "init")
                 tokenizer = self.processor_dict[name + "::tokenizer"]
                 tokenizer.load_pretrained_vocab(self.dtype_dict[name], col["pretrained_emb"])
                 self.processor_dict[name + "::tokenizer"] = tokenizer
                 self.feature_map.features[name]["vocab_size"] = tokenizer.vocab_size()
 
@@ -150,14 +152,17 @@
                     tokenizer = self.processor_dict[name + "::tokenizer"]
                     tokenizer.vocab = self.processor_dict[spec["share_embedding"] + "::tokenizer"].vocab
                     self.processor_dict[name + "::tokenizer"] = tokenizer
                     self.feature_map.features[name].update({"oov_idx": tokenizer.vocab["__OOV__"],
                                                             "vocab_size": tokenizer.vocab_size()})
                 else:
                     self.feature_map.total_features += self.feature_map.features[name]["vocab_size"]
+                if "pretrained_emb" not in spec: # "oov_idx" not used without pretrained_emb
+                    del self.feature_map.features[name]["oov_idx"]
+
         self.feature_map.num_fields = self.feature_map.get_num_fields()
         self.feature_map.set_column_index()
         self.save_pickle(self.pickle_file)
         self.save_vocab(self.vocab_file)
         self.feature_map.save(self.json_file)
         logging.info("Set feature processor done.")
```

### Comparing `fuxictr-2.1.3/fuxictr/preprocess/normalizer.py` & `fuxictr-2.2.0/fuxictr/preprocess/normalizer.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/preprocess/tokenizer.py` & `fuxictr-2.2.0/fuxictr/preprocess/tokenizer.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/dataloaders/h5_dataloader.py` & `fuxictr-2.2.0/fuxictr/pytorch/dataloaders/npz_block_dataloader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # =========================================================================
+# Copyright (C) 2023-2024. FuxiCTR Authors. All rights reserved.
 # Copyright (C) 2022. Huawei Technologies Co., Ltd. All rights reserved.
 # 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,82 +13,78 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========================================================================
 
 
 import numpy as np
-from torch.utils import data
-from fuxictr.utils import load_h5
+from itertools import chain
 import torch
-import logging
+from torch.utils import data
+import glob
 
 
-class Dataset(data.Dataset):
-    def __init__(self, feature_map, data_path):
+class BlockDataPipe(data.IterDataPipe):
+    def __init__(self, block_datapipe, feature_map):
         self.feature_map = feature_map
-        self.darray = self.load_data_array(data_path)
+        self.block_datapipe = block_datapipe
         
-    def __getitem__(self, index):
-        return self.darray[index, :]
-    
-    def __len__(self):
-        return self.darray.shape[0]
-
-    def load_data_array(self, data_path):
-        data_dict = load_h5(data_path) # dict of arrays from h5
+    def load_data(self, data_path):
+        data_dict = np.load(data_path)
         data_arrays = []
         all_cols = list(self.feature_map.features.keys()) + self.feature_map.labels
         for col in all_cols:
             array = data_dict[col]
             if array.ndim == 1:
                 data_arrays.append(array.reshape(-1, 1))
             else:
                 data_arrays.append(array)
         data_tensor = torch.from_numpy(np.hstack(data_arrays))
         return data_tensor
 
-
-class DataLoader(data.DataLoader):
-    def __init__(self, feature_map, data_path, batch_size=32, shuffle=False, num_workers=1, **kwargs):
-        if not data_path.endswith(".h5"):
-            data_path += ".h5"
-        self.dataset = Dataset(feature_map, data_path)
-        super(DataLoader, self).__init__(dataset=self.dataset, batch_size=batch_size,
-                                         shuffle=shuffle, num_workers=num_workers)
-        self.num_samples = len(self.dataset)
-        self.num_batches = int(np.ceil(self.num_samples * 1.0 / self.batch_size))
+    def read_block(self, data_block):
+        darray = self.load_data(data_block)
+        for idx in range(darray.shape[0]):
+            yield darray[idx, :]
+
+    def __iter__(self):
+        worker_info = data.get_worker_info()
+        if worker_info is None: # single-process data loading
+            block_list = self.block_datapipe
+        else: # in a worker process
+            block_list = [
+                block
+                for idx, block in enumerate(self.block_datapipe)
+                if idx % worker_info.num_workers == worker_info.id
+            ]
+        return chain.from_iterable(map(self.read_block, block_list))
+
+
+class NpzBlockDataLoader(data.DataLoader):
+    def __init__(self, feature_map, data_path, batch_size=32, shuffle=False,
+                 num_workers=1, buffer_size=100000, **kwargs):
+        data_blocks = glob.glob(data_path + "/*.npz")
+        assert len(data_blocks) > 0, f"invalid data_path: {data_path}"
+        if len(data_blocks) > 1:
+            data_blocks.sort() # sort by part name
+        self.data_blocks = data_blocks
+        self.num_blocks = len(self.data_blocks)
+        self.feature_map = feature_map
+        self.batch_size = batch_size
+        self.num_batches, self.num_samples = self.count_batches_and_samples()
+        datapipe = BlockDataPipe(data_blocks, feature_map)
+        if shuffle:
+            datapipe = datapipe.shuffle(buffer_size=buffer_size)
+        super(NpzBlockDataLoader, self).__init__(dataset=datapipe, batch_size=batch_size,
+                                                 num_workers=num_workers)
 
     def __len__(self):
         return self.num_batches
 
-
-class H5DataLoader(object):
-    def __init__(self, feature_map, stage="both", train_data=None, valid_data=None, test_data=None,
-                 batch_size=32, shuffle=True, **kwargs):
-        logging.info("Loading data...")
-        train_gen = None
-        valid_gen = None
-        test_gen = None
-        self.stage = stage
-        if stage in ["both", "train"]:
-            train_gen = DataLoader(feature_map, train_data, batch_size=batch_size, shuffle=shuffle, **kwargs)
-            logging.info("Train samples: total/{:d}, blocks/{:d}".format(train_gen.num_samples, 1))
-            if valid_data:  
-                valid_gen = DataLoader(feature_map, valid_data, batch_size=batch_size, shuffle=False, **kwargs)
-                logging.info("Validation samples: total/{:d}, blocks/{:d}".format(valid_gen.num_samples, 1))
-        if stage in ["both", "test"]:
-            if test_data:
-                test_gen = DataLoader(feature_map, test_data, batch_size=batch_size, shuffle=False, **kwargs)
-                logging.info("Test samples: total/{:d}, blocks/{:d}".format(test_gen.num_samples, 1))
-        self.train_gen, self.valid_gen, self.test_gen = train_gen, valid_gen, test_gen
-
-    def make_iterator(self):
-        if self.stage == "train":
-            logging.info("Loading train and validation data done.")
-            return self.train_gen, self.valid_gen
-        elif self.stage == "test":
-            logging.info("Loading test data done.")
-            return self.test_gen
-        else:
-            logging.info("Loading data done.")
-            return self.train_gen, self.valid_gen, self.test_gen
+    def count_batches_and_samples(self):
+        num_samples = 0
+        num_batches = 0
+        for block_path in self.data_blocks:
+            block_size = np.load(block_path)[self.feature_map.labels[0]].shape[0]
+            num_samples += block_size
+            num_batches += int(np.ceil(block_size * 1.0 / self.batch_size))
+        return num_batches, num_samples
```

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/activations.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/activations.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/attentions/dot_product_attention.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/attentions/squeeze_excitation.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/attentions/target_attention.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/target_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/blocks/factorization_machine.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/blocks/logistic_regression.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/blocks/mlp_block.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/embeddings/feature_embedding.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,22 @@
 
     def reset_parameters(self, embedding_initializer):
         if self.pretrain_usage in ["sum", "concat"]:
             nn.init.zeros_(self.id_embedding.weight) # set oov token embeddings to zeros
             embedding_initializer(self.id_embedding.weight[1:self.oov_idx, :])
 
     def get_pretrained_embedding(self, pretrain_path):
-        with h5py.File(pretrain_path, 'r') as hf:
-            keys = hf["key"][:]
-            embeddings = hf["value"][:]
         logging.info("Loading pretrained_emb: {}".format(pretrain_path))
+        if pretrain_path.endswith("h5"):
+            with h5py.File(pretrain_path, 'r') as hf:
+                keys = hf["key"][:]
+                embeddings = hf["value"][:]
+        elif pretrain_path.endswith("npz"):
+            npz = np.load(pretrain_path)
+            keys, embeddings = npz["key"], npz["value"]
         return keys, embeddings
 
     def load_feature_vocab(self, vocab_path, feature_name):
         with io.open(vocab_path, "r", encoding="utf-8") as fd:
             vocab = json.load(fd)
             vocab_type = type(list(vocab.items())[1][0]) # get key dtype
         return vocab[feature_name], vocab_type
```

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/bilinear_interaction.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/bilinear_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/cross_net.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/holographic_interaction.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/holographic_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/inner_product.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/interactions/interaction_machine.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/interaction_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/layers/pooling.py` & `fuxictr-2.2.0/fuxictr/pytorch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/models/multitask_model.py` & `fuxictr-2.2.0/fuxictr/pytorch/models/multitask_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/pytorch/models/rank_model.py` & `fuxictr-2.2.0/fuxictr/pytorch/models/rank_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             self._best_metric = monitor_value
             if self._save_best_only:
                 logging.info("Save best model: monitor({})={:.6f}"\
                              .format(self._monitor_mode, monitor_value))
                 self.save_weights(self.checkpoint)
         if self._stopping_steps >= self._early_stop_patience:
             self._stop_training = True
-            logging.info("********* Epoch=={} early stop *********".format(self._epoch_index + 1))
+            logging.info("********* Epoch={} early stop *********".format(self._epoch_index + 1))
         if not self._save_best_only:
             self.save_weights(self.checkpoint)
 
     def eval_step(self):
         logging.info('Evaluation @epoch {} - batch {}: '.format(self._epoch_index + 1, self._batch_index + 1))
         val_logs = self.evaluate(self.valid_gen, metrics=self._monitor.get_metrics())
         self.checkpoint_and_earlystop(val_logs)
```

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/dataloaders/tf_dataloader.py` & `fuxictr-2.2.0/fuxictr/tensorflow/dataloaders/tf_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/factorization_machine.py` & `fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/linear.py` & `fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/linear.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/logistic_regression.py` & `fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/layers/blocks/mlp_block.py` & `fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/layers/embeddings/feature_embedding.py` & `fuxictr-2.2.0/fuxictr/tensorflow/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/layers/interactions/cross_net.py` & `fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/layers/interactions/inner_product.py` & `fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/layers/pooling.py` & `fuxictr-2.2.0/fuxictr/tensorflow/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/models/rank_model.py` & `fuxictr-2.2.0/fuxictr/tensorflow/models/rank_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/tensorflow/tf_utils.py` & `fuxictr-2.2.0/fuxictr/tensorflow/tf_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.1.3/fuxictr/utils.py` & `fuxictr-2.2.0/fuxictr/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import os
 import logging
 import logging.config
 import yaml
 import glob
 import json
 from collections import OrderedDict
-import h5py
 
 
 def load_config(config_dir, experiment_id):
     params = load_model_config(config_dir, experiment_id)
     data_params = load_dataset_config(config_dir, params['dataset_id'])
     params.update(data_params)
     return params
@@ -101,16 +100,7 @@
         value = 0
         for k, v in self.kv_pairs.items():
             value += logs.get(k, 0) * v
         return value
 
     def get_metrics(self):
         return list(self.kv_pairs.keys())
-
-def load_h5(data_path, verbose=0):
-    if verbose == 0:
-        logging.info('Loading data from h5: ' + data_path)
-    data_dict = dict()
-    with h5py.File(data_path, 'r') as hf:
-        for key in hf.keys():
-            data_dict[key] = hf[key][:]
-    return data_dict
```

### Comparing `fuxictr-2.1.3/fuxictr.egg-info/PKG-INFO` & `fuxictr-2.2.0/fuxictr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.1.3
+Version: 2.2.0
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.1.3 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.2.0 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
```

### Comparing `fuxictr-2.1.3/fuxictr.egg-info/SOURCES.txt` & `fuxictr-2.2.0/fuxictr.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 fuxictr/preprocess/build_dataset.py
 fuxictr/preprocess/feature_processor.py
 fuxictr/preprocess/normalizer.py
 fuxictr/preprocess/tokenizer.py
 fuxictr/pytorch/__init__.py
 fuxictr/pytorch/torch_utils.py
 fuxictr/pytorch/dataloaders/__init__.py
-fuxictr/pytorch/dataloaders/h5_block_dataloader.py
-fuxictr/pytorch/dataloaders/h5_dataloader.py
+fuxictr/pytorch/dataloaders/npz_block_dataloader.py
+fuxictr/pytorch/dataloaders/npz_dataloader.py
+fuxictr/pytorch/dataloaders/rank_dataloader.py
 fuxictr/pytorch/layers/__init__.py
 fuxictr/pytorch/layers/activations.py
 fuxictr/pytorch/layers/pooling.py
 fuxictr/pytorch/layers/attentions/__init__.py
 fuxictr/pytorch/layers/attentions/dot_product_attention.py
 fuxictr/pytorch/layers/attentions/squeeze_excitation.py
 fuxictr/pytorch/layers/attentions/target_attention.py
@@ -63,9 +64,8 @@
 fuxictr/tensorflow/layers/embeddings/__init__.py
 fuxictr/tensorflow/layers/embeddings/feature_embedding.py
 fuxictr/tensorflow/layers/interactions/__init__.py
 fuxictr/tensorflow/layers/interactions/cross_net.py
 fuxictr/tensorflow/layers/interactions/inner_product.py
 fuxictr/tensorflow/models/__init__.py
 fuxictr/tensorflow/models/rank_model.py
-model_zoo/__init__.py
 model_zoo/multitask/__init__.py
```

### Comparing `fuxictr-2.1.3/setup.py` & `fuxictr-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setuptools.setup(
     name="fuxictr",
-    version="2.1.3",
+    version="2.2.0",
     author="RECZOO",
     author_email="reczoo@users.noreply.github.com",
     description="A configurable, tunable, and reproducible library for CTR prediction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/reczoo/FuxiCTR",
     download_url='https://github.com/reczoo/FuxiCTR/tags',
```

