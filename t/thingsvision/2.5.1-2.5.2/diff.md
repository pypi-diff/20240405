# Comparing `tmp/thingsvision-2.5.1.tar.gz` & `tmp/thingsvision-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.5.1.tar", last modified: Thu Apr  4 09:43:35 2024, max compression
+gzip compressed data, was "thingsvision-2.5.2.tar", last modified: Fri Apr  5 10:02:32 2024, max compression
```

## Comparing `thingsvision-2.5.1.tar` & `thingsvision-2.5.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.849491 thingsvision-2.5.1/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.1/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15110 2024-04-04 09:43:35.849237 thingsvision-2.5.1/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14507 2024-04-04 09:43:21.000000 thingsvision-2.5.1/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-04 09:43:35.849608 thingsvision-2.5.1/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.1/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.832114 thingsvision-2.5.1/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.1/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.832928 thingsvision-2.5.1/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.1/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.834575 thingsvision-2.5.1/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.1/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.5.1/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.5.1/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-01 11:25:01.000000 thingsvision-2.5.1/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2851 2024-04-04 09:43:21.000000 thingsvision-2.5.1/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.5.1/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.1/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11635 2024-04-04 09:43:21.000000 thingsvision-2.5.1/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.1/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.1/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.835364 thingsvision-2.5.1/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.1/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.837103 thingsvision-2.5.1/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.1/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.837563 thingsvision-2.5.1/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/core/cka/base.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.838969 thingsvision-2.5.1/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.5.1/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15362 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7683 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.839620 thingsvision-2.5.1/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.1/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.1/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.842341 thingsvision-2.5.1/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.1/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.1/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.1/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.843797 thingsvision-2.5.1/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.1/thingsvision/custom_models/custom.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.844294 thingsvision-2.5.1/thingsvision/custom_models/dreamsim/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.1/thingsvision/custom_models/dreamsim/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.1/thingsvision/custom_models/dreamsim/dreamsim.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.844827 thingsvision-2.5.1/thingsvision/custom_models/harmonization/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.1/thingsvision/custom_models/harmonization/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.1/thingsvision/custom_models/harmonization/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.1/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.1/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.1/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.1/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.1/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.1/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5980 2024-03-19 09:46:42.000000 thingsvision-2.5.1/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.845133 thingsvision-2.5.1/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.1/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.845577 thingsvision-2.5.1/thingsvision/utils/alignment/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.1/thingsvision/utils/alignment/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.1/thingsvision/utils/alignment/transforms.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.845856 thingsvision-2.5.1/thingsvision/utils/checkpointing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.1/thingsvision/utils/checkpointing/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.846995 thingsvision-2.5.1/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.1/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.1/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.1/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.1/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.847223 thingsvision-2.5.1/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.847493 thingsvision-2.5.1/thingsvision/utils/models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.1/thingsvision/utils/models/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.848175 thingsvision-2.5.1/thingsvision/utils/models/dino/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2023-08-08 13:01:35.000000 thingsvision-2.5.1/thingsvision/utils/models/dino/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.1/thingsvision/utils/models/dino/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.1/thingsvision/utils/models/dino/vision_transformer.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.848879 thingsvision-2.5.1/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.1/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.836865 thingsvision-2.5.1/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15110 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2651 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.345260 thingsvision-2.5.2/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.2/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16313 2024-04-05 10:02:32.344832 thingsvision-2.5.2/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15710 2024-04-05 10:02:22.000000 thingsvision-2.5.2/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-05 10:02:32.345387 thingsvision-2.5.2/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.2/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.298564 thingsvision-2.5.2/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.2/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.300908 thingsvision-2.5.2/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.2/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.311948 thingsvision-2.5.2/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.2/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.5.2/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.5.2/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-01 11:25:01.000000 thingsvision-2.5.2/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-05 10:02:22.000000 thingsvision-2.5.2/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.5.2/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.2/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11635 2024-04-04 09:43:21.000000 thingsvision-2.5.2/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.2/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.2/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.313254 thingsvision-2.5.2/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.2/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-05 10:02:22.000000 thingsvision-2.5.2/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.315911 thingsvision-2.5.2/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.2/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.316746 thingsvision-2.5.2/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/core/cka/base.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.320171 thingsvision-2.5.2/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.5.2/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.5.2/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15362 2024-04-04 12:00:22.000000 thingsvision-2.5.2/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.5.2/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.5.2/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8507 2024-04-05 10:02:22.000000 thingsvision-2.5.2/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.321087 thingsvision-2.5.2/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.2/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.2/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.328140 thingsvision-2.5.2/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.2/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.2/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.2/thingsvision/custom_models/alexnet_salobjsub.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.331015 thingsvision-2.5.2/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.2/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.332091 thingsvision-2.5.2/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.2/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.2/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.333356 thingsvision-2.5.2/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.2/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.2/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.2/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.2/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.2/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.2/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.2/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.2/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5980 2024-03-19 09:46:42.000000 thingsvision-2.5.2/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.334004 thingsvision-2.5.2/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.2/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.334976 thingsvision-2.5.2/thingsvision/utils/alignment/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.2/thingsvision/utils/alignment/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.2/thingsvision/utils/alignment/transforms.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.335569 thingsvision-2.5.2/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.2/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.338736 thingsvision-2.5.2/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.2/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.2/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.2/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.2/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.339901 thingsvision-2.5.2/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.340726 thingsvision-2.5.2/thingsvision/utils/models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.2/thingsvision/utils/models/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.342779 thingsvision-2.5.2/thingsvision/utils/models/dino/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2023-08-08 13:01:35.000000 thingsvision-2.5.2/thingsvision/utils/models/dino/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.2/thingsvision/utils/models/dino/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.2/thingsvision/utils/models/dino/vision_transformer.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.343841 thingsvision-2.5.2/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.2/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.2/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-05 10:02:32.315633 thingsvision-2.5.2/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16313 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2651 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-05 10:02:32.000000 thingsvision-2.5.2/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.5.1/LICENSE` & `thingsvision-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/PKG-INFO` & `thingsvision-2.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.1
+Version: 2.5.2
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -104,15 +104,15 @@
 
 
 <!-- Getting Started -->
 ## :running: Getting Started
 
 <!-- Setting up your environment -->
 ### :computer: Setting up your environment
-#### Working locally.
+#### Working locally
 First, create a new `conda environment` with Python version 3.8, 3.9, or 3.10 e.g. by using `conda`:
 
 ```bash
 $ conda create -n thingsvision python=3.9
 $ conda activate thingsvision
 ```
 
@@ -134,15 +134,15 @@
 
 ```bash
 $ pip install dreamsim==0.1.2
 ```
 
 See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for which `DreamSim` models are available in `thingsvision`.
 
-#### Google Colab.
+#### Google Colab
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Basic usage -->
 ### :mag: Basic usage
@@ -220,14 +220,56 @@
     flatten_acts=True,
     output_type="ndarray", # or "tensor" (only applicable to PyTorch models of which CLIP and DINO are ones!)
 )
 
 save_features(features, out_path='path/to/features', file_format='npy') # file_format can be set to "npy", "txt", "mat", "pt", or "hdf5"
 ```
 
+#### Feature extraction with custom data pipeline
+
+##### PyTorch
+
+```python
+module_name = 'visual'
+
+# your custom dataset and dataloader classes come here (for example, a PyTorch data loader)
+my_dataset = ...
+my_dataloader = ...
+
+with extractor.batch_extraction(module_name, output_type="tensor") as e: 
+  for batch in my_dataloader:
+    ... # whatever preprocessing you want to add to the batch
+    feature_batch = e.extract_batch(
+      batch=batch,
+      flatten_acts=True, # flatten 2D feature maps from an early convolutional or attention layer
+      )
+    ... # whatever post-processing you want to add to the extracted features
+```
+
+##### TensorFlow / Keras
+
+```python
+module_name = 'visual'
+
+# your custom dataset and dataloader classes come here (for example, TFRecords files)
+my_dataset = ...
+my_dataloader = ...
+
+for batch in my_dataloader:
+  ... # whatever preprocessing you want to add to the batch
+  feature_batch = extractor.extract_batch(
+    batch=batch,
+    module_name=module_name,
+    flatten_acts=True, # flatten 2D feature maps from an early convolutional or attention layer
+    )
+  ... # whatever post-processing you want to add to the extracted features
+```
+
+#### Human alignment
+
 *Human alignment*: If you want to align the extracted features with human object similarity according to the approach introduced in *[Improving neural network representations using human similiarty judgments](https://proceedings.neurips.cc/paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)* you can optionally `align` the extracted features using the following method:
 
 ```python
 aligned_features = extractor.align(
     features=features,
     module_name=module_name,
     alignment_type="gLocal",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.1 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.5.2 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -64,15 +64,15 @@
 - [DreamSim](https://dreamsim-nights.github.io/) models (see [DreamSim repo]
 (https://github.com/ssundaram21/dreamsim)). The default variant is
 `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`,
 and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for more information
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## :running: Getting Started ### :computer: Setting up your environment ####
-Working locally. First, create a new `conda environment` with Python version
+Working locally First, create a new `conda environment` with Python version
 3.8, 3.9, or 3.10 e.g. by using `conda`: ```bash $ conda create -n thingsvision
 python=3.9 $ conda activate thingsvision ``` Then, activate the environment and
 simply install `thingsvision` via running the following `pip` command in your
 terminal. ```bash $ pip install --upgrade thingsvision $ pip install git+https:
 //github.com/openai/CLIP.git ``` If you want to extract features for
 [harmonized models](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#harmonization) from the [Harmonization repo](https://
@@ -82,15 +82,15 @@
 git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
 attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
 (https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
 github.com/ssundaram21/dreamsim), you have to additionally run the following
 `pip` command in your `thingsvision` environment, ```bash $ pip install
 dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for which `DreamSim` models are available in
-`thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
+`thingsvision`. #### Google Colab Alternatively, you can use Google Colab to
 play around with `thingsvision` by uploading your image data to Google Drive
 (via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
 master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
 colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
 notebooks/tensorflow.ipynb).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
@@ -133,15 +133,30 @@
 extracting features from the image encoder module of CLIP (`visual`), but if
 you don't know which modules are available for a given model, just call
 `extractor.show_model()` to print all the modules. ```python module_name =
 'visual' features = extractor.extract_features( batches=batches,
 module_name=module_name, flatten_acts=True, output_type="ndarray", # or
 "tensor" (only applicable to PyTorch models of which CLIP and DINO are ones!) )
 save_features(features, out_path='path/to/features', file_format='npy') #
-file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` *Human
+file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` #### Feature
+extraction with custom data pipeline ##### PyTorch ```python module_name =
+'visual' # your custom dataset and dataloader classes come here (for example, a
+PyTorch data loader) my_dataset = ... my_dataloader = ... with
+extractor.batch_extraction(module_name, output_type="tensor") as e: for batch
+in my_dataloader: ... # whatever preprocessing you want to add to the batch
+feature_batch = e.extract_batch( batch=batch, flatten_acts=True, # flatten 2D
+feature maps from an early convolutional or attention layer ) ... # whatever
+post-processing you want to add to the extracted features ``` ##### TensorFlow
+/ Keras ```python module_name = 'visual' # your custom dataset and dataloader
+classes come here (for example, TFRecords files) my_dataset = ... my_dataloader
+= ... for batch in my_dataloader: ... # whatever preprocessing you want to add
+to the batch feature_batch = extractor.extract_batch( batch=batch,
+module_name=module_name, flatten_acts=True, # flatten 2D feature maps from an
+early convolutional or attention layer ) ... # whatever post-processing you
+want to add to the extracted features ``` #### Human alignment *Human
 alignment*: If you want to align the extracted features with human object
 similarity according to the approach introduced in *[Improving neural network
 representations using human similiarty judgments](https://
 proceedings.neurips.cc/paper_files/paper/2023/hash/
 9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)* you can optionally
 `align` the extracted features using the following method: ```python
 aligned_features = extractor.align( features=features, module_name=module_name,
```

### Comparing `thingsvision-2.5.1/README.md` & `thingsvision-2.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 <!-- Getting Started -->
 ## :running: Getting Started
 
 <!-- Setting up your environment -->
 ### :computer: Setting up your environment
-#### Working locally.
+#### Working locally
 First, create a new `conda environment` with Python version 3.8, 3.9, or 3.10 e.g. by using `conda`:
 
 ```bash
 $ conda create -n thingsvision python=3.9
 $ conda activate thingsvision
 ```
 
@@ -117,15 +117,15 @@
 
 ```bash
 $ pip install dreamsim==0.1.2
 ```
 
 See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for which `DreamSim` models are available in `thingsvision`.
 
-#### Google Colab.
+#### Google Colab
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Basic usage -->
 ### :mag: Basic usage
@@ -203,14 +203,56 @@
     flatten_acts=True,
     output_type="ndarray", # or "tensor" (only applicable to PyTorch models of which CLIP and DINO are ones!)
 )
 
 save_features(features, out_path='path/to/features', file_format='npy') # file_format can be set to "npy", "txt", "mat", "pt", or "hdf5"
 ```
 
+#### Feature extraction with custom data pipeline
+
+##### PyTorch
+
+```python
+module_name = 'visual'
+
+# your custom dataset and dataloader classes come here (for example, a PyTorch data loader)
+my_dataset = ...
+my_dataloader = ...
+
+with extractor.batch_extraction(module_name, output_type="tensor") as e: 
+  for batch in my_dataloader:
+    ... # whatever preprocessing you want to add to the batch
+    feature_batch = e.extract_batch(
+      batch=batch,
+      flatten_acts=True, # flatten 2D feature maps from an early convolutional or attention layer
+      )
+    ... # whatever post-processing you want to add to the extracted features
+```
+
+##### TensorFlow / Keras
+
+```python
+module_name = 'visual'
+
+# your custom dataset and dataloader classes come here (for example, TFRecords files)
+my_dataset = ...
+my_dataloader = ...
+
+for batch in my_dataloader:
+  ... # whatever preprocessing you want to add to the batch
+  feature_batch = extractor.extract_batch(
+    batch=batch,
+    module_name=module_name,
+    flatten_acts=True, # flatten 2D feature maps from an early convolutional or attention layer
+    )
+  ... # whatever post-processing you want to add to the extracted features
+```
+
+#### Human alignment
+
 *Human alignment*: If you want to align the extracted features with human object similarity according to the approach introduced in *[Improving neural network representations using human similiarty judgments](https://proceedings.neurips.cc/paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)* you can optionally `align` the extracted features using the following method:
 
 ```python
 aligned_features = extractor.align(
     features=features,
     module_name=module_name,
     alignment_type="gLocal",
```

#### html2text {}

```diff
@@ -56,15 +56,15 @@
 - [DreamSim](https://dreamsim-nights.github.io/) models (see [DreamSim repo]
 (https://github.com/ssundaram21/dreamsim)). The default variant is
 `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`,
 and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for more information
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## :running: Getting Started ### :computer: Setting up your environment ####
-Working locally. First, create a new `conda environment` with Python version
+Working locally First, create a new `conda environment` with Python version
 3.8, 3.9, or 3.10 e.g. by using `conda`: ```bash $ conda create -n thingsvision
 python=3.9 $ conda activate thingsvision ``` Then, activate the environment and
 simply install `thingsvision` via running the following `pip` command in your
 terminal. ```bash $ pip install --upgrade thingsvision $ pip install git+https:
 //github.com/openai/CLIP.git ``` If you want to extract features for
 [harmonized models](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#harmonization) from the [Harmonization repo](https://
@@ -74,15 +74,15 @@
 git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
 attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
 (https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
 github.com/ssundaram21/dreamsim), you have to additionally run the following
 `pip` command in your `thingsvision` environment, ```bash $ pip install
 dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for which `DreamSim` models are available in
-`thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
+`thingsvision`. #### Google Colab Alternatively, you can use Google Colab to
 play around with `thingsvision` by uploading your image data to Google Drive
 (via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
 master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
 colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
 notebooks/tensorflow.ipynb).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
@@ -125,15 +125,30 @@
 extracting features from the image encoder module of CLIP (`visual`), but if
 you don't know which modules are available for a given model, just call
 `extractor.show_model()` to print all the modules. ```python module_name =
 'visual' features = extractor.extract_features( batches=batches,
 module_name=module_name, flatten_acts=True, output_type="ndarray", # or
 "tensor" (only applicable to PyTorch models of which CLIP and DINO are ones!) )
 save_features(features, out_path='path/to/features', file_format='npy') #
-file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` *Human
+file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` #### Feature
+extraction with custom data pipeline ##### PyTorch ```python module_name =
+'visual' # your custom dataset and dataloader classes come here (for example, a
+PyTorch data loader) my_dataset = ... my_dataloader = ... with
+extractor.batch_extraction(module_name, output_type="tensor") as e: for batch
+in my_dataloader: ... # whatever preprocessing you want to add to the batch
+feature_batch = e.extract_batch( batch=batch, flatten_acts=True, # flatten 2D
+feature maps from an early convolutional or attention layer ) ... # whatever
+post-processing you want to add to the extracted features ``` ##### TensorFlow
+/ Keras ```python module_name = 'visual' # your custom dataset and dataloader
+classes come here (for example, TFRecords files) my_dataset = ... my_dataloader
+= ... for batch in my_dataloader: ... # whatever preprocessing you want to add
+to the batch feature_batch = extractor.extract_batch( batch=batch,
+module_name=module_name, flatten_acts=True, # flatten 2D feature maps from an
+early convolutional or attention layer ) ... # whatever post-processing you
+want to add to the extracted features ``` #### Human alignment *Human
 alignment*: If you want to align the extracted features with human object
 similarity according to the approach introduced in *[Improving neural network
 representations using human similiarty judgments](https://
 proceedings.neurips.cc/paper_files/paper/2023/hash/
 9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)* you can optionally
 `align` the extracted features using the following method: ```python
 aligned_features = extractor.align( features=features, module_name=module_name,
```

### Comparing `thingsvision-2.5.1/setup.py` & `thingsvision-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.5.2/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.5.2/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.5.2/tests/extractor/extraction/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.5.2/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
-import torch
 
 import numpy as np
+import torch
+
 import tests.helper as helper
-from thingsvision.utils.data import DataLoader
 import thingsvision.core.extraction.helpers as core_helpers
-
+from thingsvision.utils.data import DataLoader
 
 
 class ExtractionPTvsTFTestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         helper.create_test_images()
 
@@ -41,46 +41,45 @@
         pt_model = core_helpers.get_extractor(
             "vgg16", pretrained=False, device=helper.DEVICE, source=pt_source
         )
         pt_model.model = helper.pt_model
         pt_model.backend = pt_backend
 
         layer_name = "relu"
-        expected_features_pt = torch.tensor([[2., 2.], [0., 0.]])
-        expected_features_tf = np.array([[2., 2.], [0, 0.]])
+        expected_features_tf = np.array([[2.0, 2.0], [0, 0.0]])
+        expected_features_pt = torch.tensor([[2.0, 2.0], [0.0, 0.0]])
 
         for i, batch in enumerate(tf_dl):
             tf_features = tf_model.extract_batch(
                 batch=batch,
                 module_name=layer_name,
                 flatten_acts=False,
             )
-            np.testing.assert_allclose(tf_features, expected_features_tf[i][None,:])
-        
-        for i, batch in enumerate(pt_dl):
-            pt_features = pt_model.extract_batch(
-                batch=batch,
-                module_name=layer_name,
-                flatten_acts=False,
-                output_type="tensor",
-            )
-            np.testing.assert_allclose(pt_features, expected_features_pt[i][None,:])
+            expected_features = expected_features_tf[i][None, :]
+            np.testing.assert_allclose(tf_features, expected_features)
+
+        with pt_model.batch_extraction(layer_name, output_type="tensor") as e:
+            for i, batch in enumerate(pt_dl):
+                pt_features = e.extract_batch(
+                    batch=batch,
+                    flatten_acts=False,
+                )
+                expected_features = expected_features_pt[i][None, :]
+                np.testing.assert_allclose(pt_features, expected_features)
 
         layer_name = "relu2"
-        expected_features = np.array([[4., 4.], [0., 0.]])
+        expected_features = np.array([[4.0, 4.0], [0.0, 0.0]])
         for i, batch in enumerate(tf_dl):
             tf_features = tf_model.extract_batch(
                 batch=batch,
                 module_name=layer_name,
                 flatten_acts=False,
             )
-            np.testing.assert_allclose(tf_features, expected_features[i][None,:])
-        
-        for i, batch in enumerate(pt_dl):
-            pt_features = pt_model.extract_batch(
-                batch=batch,
-                module_name=layer_name,
-                flatten_acts=False,
-                output_type="ndarray",
-            )
-            np.testing.assert_allclose(pt_features, expected_features[i][None,:])
-            
+            np.testing.assert_allclose(tf_features, expected_features[i][None, :])
+
+        with pt_model.batch_extraction(layer_name, output_type="ndarray") as e:
+            for i, batch in enumerate(pt_dl):
+                pt_features = e.extract_batch(
+                    batch=batch,
+                    flatten_acts=False,
+                )
+                np.testing.assert_allclose(pt_features, expected_features[i][None, :])
```

### Comparing `thingsvision-2.5.1/tests/extractor/test_load_extractor.py` & `thingsvision-2.5.2/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/tests/extractor/test_transformations.py` & `thingsvision-2.5.2/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/tests/helper.py` & `thingsvision-2.5.2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/tests/test_features.py` & `thingsvision-2.5.2/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/tests/test_rest.py` & `thingsvision-2.5.2/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/core/cka/base.py` & `thingsvision-2.5.2/thingsvision/core/cka/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/core/extraction/base.py` & `thingsvision-2.5.2/thingsvision/core/extraction/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/core/extraction/extractors.py` & `thingsvision-2.5.2/thingsvision/core/extraction/extractors.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/core/extraction/helpers.py` & `thingsvision-2.5.2/thingsvision/core/extraction/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.5.2/thingsvision/core/extraction/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/core/extraction/torch.py` & `thingsvision-2.5.2/thingsvision/core/extraction/torch.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,42 +53,44 @@
             try:
                 self.activations[name] = act.clone().detach()
             except AttributeError:
                 self.activations[name] = act.clone()
 
         return hook
 
-    def register_hook(self, module_name: str) -> None:
+    def _register_hook(self, module_name: str) -> None:
         """Register a forward hook to store activations."""
         for n, m in self.model.named_modules():
             if n == module_name:
                 self.hook_handle = m.register_forward_hook(self.get_activation(n))
                 break
 
     def _unregister_hook(self) -> None:
         self.hook_handle.remove()
 
+    def batch_extraction(self, module_name: str, output_type: str) -> object:
+        return BatchExtraction(
+            extractor=self, module_name=module_name, output_type=output_type
+        )
+
     def extract_batch(
         self,
         batch: TensorType["b", "c", "h", "w"],
-        module_name: str,
         flatten_acts: bool,
-        output_type: str = "tensor",
     ) -> Union[
         TensorType["b", "num_maps", "h_prime", "w_prime"],
         TensorType["b", "t", "d"],
         TensorType["b", "p"],
         TensorType["b", "d"],
     ]:
-        self._module_and_output_check(module_name, output_type)
-        self.register_hook(module_name=module_name)
-        act = self._extract_batch(batch, module_name, flatten_acts)
-        if output_type == "ndarray":
+        act = self._extract_batch(
+            batch=batch, module_name=self.module_name, flatten_acts=flatten_acts
+        )
+        if self.output_type == "ndarray":
             act = self._to_numpy(act)
-        self._unregister_hook()
         return act
 
     @torch.no_grad()
     def _extract_batch(
         self,
         batch: TensorType["b", "c", "h", "w"],
         module_name: str,
@@ -124,15 +126,15 @@
         flatten_acts: bool,
         output_type: str = "ndarray",
         output_dir: Optional[str] = None,
         step_size: Optional[int] = None,
     ):
         self.model = self.model.to(self.device)
         self.activations = {}
-        self.register_hook(module_name=module_name)
+        self._register_hook(module_name=module_name)
         features = super().extract_features(
             batches=batches,
             module_name=module_name,
             flatten_acts=flatten_acts,
             output_type=output_type,
             output_dir=output_dir,
             step_size=step_size,
@@ -226,7 +228,29 @@
         composes += [T.ToTensor(), normalize]
         composition = T.Compose(composes)
 
         return composition
 
     def get_backend(self) -> str:
         return "pt"
+
+
+class BatchExtraction(object):
+
+    def __init__(
+        self, extractor: PyTorchExtractor, module_name: str, output_type: str
+    ) -> None:
+        self.extractor = extractor
+        self.module_name = module_name
+        self.output_type = output_type
+
+    def __enter__(self) -> PyTorchExtractor:
+        self.extractor._module_and_output_check(self.module_name, self.output_type)
+        self.extractor._register_hook(self.module_name)
+        setattr(self.extractor, "module_name", self.module_name)
+        setattr(self.extractor, "output_type", self.output_type)
+        return self.extractor
+
+    def __exit__(self, *args):
+        self.extractor._unregister_hook()
+        delattr(self.extractor, "module_name")
+        delattr(self.extractor, "output_type")
```

### Comparing `thingsvision-2.5.1/thingsvision/core/rsa/helpers.py` & `thingsvision-2.5.2/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.5.2/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.5.2/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.5.2/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.5.2/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/dreamsim/dreamsim.py` & `thingsvision-2.5.2/thingsvision/custom_models/dreamsim/dreamsim.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/harmonization/harmonization.py` & `thingsvision-2.5.2/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.5.2/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/openclip.py` & `thingsvision-2.5.2/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.5.2/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.5.2/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.5.2/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/thingsvision.py` & `thingsvision-2.5.2/thingsvision/thingsvision.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/alignment/transforms.py` & `thingsvision-2.5.2/thingsvision/utils/alignment/transforms.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/checkpointing/__init__.py` & `thingsvision-2.5.2/thingsvision/utils/checkpointing/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/data/__init__.py` & `thingsvision-2.5.2/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/data/data_loader.py` & `thingsvision-2.5.2/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/data/dataset.py` & `thingsvision-2.5.2/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/data/helpers.py` & `thingsvision-2.5.2/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.5.2/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/models/dino/utils.py` & `thingsvision-2.5.2/thingsvision/utils/models/dino/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/models/dino/vision_transformer.py` & `thingsvision-2.5.2/thingsvision/utils/models/dino/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision/utils/storing/helpers.py` & `thingsvision-2.5.2/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.1/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.5.2/thingsvision.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.1
+Version: 2.5.2
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -104,15 +104,15 @@
 
 
 <!-- Getting Started -->
 ## :running: Getting Started
 
 <!-- Setting up your environment -->
 ### :computer: Setting up your environment
-#### Working locally.
+#### Working locally
 First, create a new `conda environment` with Python version 3.8, 3.9, or 3.10 e.g. by using `conda`:
 
 ```bash
 $ conda create -n thingsvision python=3.9
 $ conda activate thingsvision
 ```
 
@@ -134,15 +134,15 @@
 
 ```bash
 $ pip install dreamsim==0.1.2
 ```
 
 See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for which `DreamSim` models are available in `thingsvision`.
 
-#### Google Colab.
+#### Google Colab
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Basic usage -->
 ### :mag: Basic usage
@@ -220,14 +220,56 @@
     flatten_acts=True,
     output_type="ndarray", # or "tensor" (only applicable to PyTorch models of which CLIP and DINO are ones!)
 )
 
 save_features(features, out_path='path/to/features', file_format='npy') # file_format can be set to "npy", "txt", "mat", "pt", or "hdf5"
 ```
 
+#### Feature extraction with custom data pipeline
+
+##### PyTorch
+
+```python
+module_name = 'visual'
+
+# your custom dataset and dataloader classes come here (for example, a PyTorch data loader)
+my_dataset = ...
+my_dataloader = ...
+
+with extractor.batch_extraction(module_name, output_type="tensor") as e: 
+  for batch in my_dataloader:
+    ... # whatever preprocessing you want to add to the batch
+    feature_batch = e.extract_batch(
+      batch=batch,
+      flatten_acts=True, # flatten 2D feature maps from an early convolutional or attention layer
+      )
+    ... # whatever post-processing you want to add to the extracted features
+```
+
+##### TensorFlow / Keras
+
+```python
+module_name = 'visual'
+
+# your custom dataset and dataloader classes come here (for example, TFRecords files)
+my_dataset = ...
+my_dataloader = ...
+
+for batch in my_dataloader:
+  ... # whatever preprocessing you want to add to the batch
+  feature_batch = extractor.extract_batch(
+    batch=batch,
+    module_name=module_name,
+    flatten_acts=True, # flatten 2D feature maps from an early convolutional or attention layer
+    )
+  ... # whatever post-processing you want to add to the extracted features
+```
+
+#### Human alignment
+
 *Human alignment*: If you want to align the extracted features with human object similarity according to the approach introduced in *[Improving neural network representations using human similiarty judgments](https://proceedings.neurips.cc/paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)* you can optionally `align` the extracted features using the following method:
 
 ```python
 aligned_features = extractor.align(
     features=features,
     module_name=module_name,
     alignment_type="gLocal",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.1 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.5.2 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -64,15 +64,15 @@
 - [DreamSim](https://dreamsim-nights.github.io/) models (see [DreamSim repo]
 (https://github.com/ssundaram21/dreamsim)). The default variant is
 `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`,
 and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for more information
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## :running: Getting Started ### :computer: Setting up your environment ####
-Working locally. First, create a new `conda environment` with Python version
+Working locally First, create a new `conda environment` with Python version
 3.8, 3.9, or 3.10 e.g. by using `conda`: ```bash $ conda create -n thingsvision
 python=3.9 $ conda activate thingsvision ``` Then, activate the environment and
 simply install `thingsvision` via running the following `pip` command in your
 terminal. ```bash $ pip install --upgrade thingsvision $ pip install git+https:
 //github.com/openai/CLIP.git ``` If you want to extract features for
 [harmonized models](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#harmonization) from the [Harmonization repo](https://
@@ -82,15 +82,15 @@
 git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
 attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
 (https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
 github.com/ssundaram21/dreamsim), you have to additionally run the following
 `pip` command in your `thingsvision` environment, ```bash $ pip install
 dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for which `DreamSim` models are available in
-`thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
+`thingsvision`. #### Google Colab Alternatively, you can use Google Colab to
 play around with `thingsvision` by uploading your image data to Google Drive
 (via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
 master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
 colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
 notebooks/tensorflow.ipynb).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
@@ -133,15 +133,30 @@
 extracting features from the image encoder module of CLIP (`visual`), but if
 you don't know which modules are available for a given model, just call
 `extractor.show_model()` to print all the modules. ```python module_name =
 'visual' features = extractor.extract_features( batches=batches,
 module_name=module_name, flatten_acts=True, output_type="ndarray", # or
 "tensor" (only applicable to PyTorch models of which CLIP and DINO are ones!) )
 save_features(features, out_path='path/to/features', file_format='npy') #
-file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` *Human
+file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` #### Feature
+extraction with custom data pipeline ##### PyTorch ```python module_name =
+'visual' # your custom dataset and dataloader classes come here (for example, a
+PyTorch data loader) my_dataset = ... my_dataloader = ... with
+extractor.batch_extraction(module_name, output_type="tensor") as e: for batch
+in my_dataloader: ... # whatever preprocessing you want to add to the batch
+feature_batch = e.extract_batch( batch=batch, flatten_acts=True, # flatten 2D
+feature maps from an early convolutional or attention layer ) ... # whatever
+post-processing you want to add to the extracted features ``` ##### TensorFlow
+/ Keras ```python module_name = 'visual' # your custom dataset and dataloader
+classes come here (for example, TFRecords files) my_dataset = ... my_dataloader
+= ... for batch in my_dataloader: ... # whatever preprocessing you want to add
+to the batch feature_batch = extractor.extract_batch( batch=batch,
+module_name=module_name, flatten_acts=True, # flatten 2D feature maps from an
+early convolutional or attention layer ) ... # whatever post-processing you
+want to add to the extracted features ``` #### Human alignment *Human
 alignment*: If you want to align the extracted features with human object
 similarity according to the approach introduced in *[Improving neural network
 representations using human similiarty judgments](https://
 proceedings.neurips.cc/paper_files/paper/2023/hash/
 9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)* you can optionally
 `align` the extracted features using the following method: ```python
 aligned_features = extractor.align( features=features, module_name=module_name,
```

### Comparing `thingsvision-2.5.1/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.5.2/thingsvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

