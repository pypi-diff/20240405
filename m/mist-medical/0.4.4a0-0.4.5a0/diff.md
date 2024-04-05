# Comparing `tmp/mist-medical-0.4.4a0.tar.gz` & `tmp/mist-medical-0.4.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mist-medical-0.4.4a0.tar", last modified: Fri Mar 29 17:29:10 2024, max compression
+gzip compressed data, was "mist-medical-0.4.5a0.tar", last modified: Fri Apr  5 18:21:25 2024, max compression
```

## Comparing `mist-medical-0.4.4a0.tar` & `mist-medical-0.4.5a0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.415942 mist-medical-0.4.4a0/
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    33877 2024-03-29 17:29:10.415942 mist-medical-0.4.4a0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    32173 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.407942 mist-medical-0.4.4a0/mist/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.407942 mist-medical-0.4.4a0/mist/analyze_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/analyze_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16741 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/analyze_data/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.407942 mist-medical-0.4.4a0/mist/conversion_tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/conversion_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/conversion_tools/csv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5762 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/conversion_tools/msd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/convert_to_mist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.407942 mist-medical-0.4.4a0/mist/data_loading/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/data_loading/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12303 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/data_loading/dali_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/eval_preds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.411942 mist-medical-0.4.4a0/mist/evaluate_preds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/evaluate_preds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6453 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/evaluate_preds/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.411942 mist-medical-0.4.4a0/mist/inference/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11316 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/inference/main_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3725 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.411942 mist-medical-0.4.4a0/mist/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10087 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.411942 mist-medical-0.4.4a0/mist/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/models/attn_unet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9112 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/models/get_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6272 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/models/layers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/models/mgnets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16466 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/models/nnunet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/models/swin_unetr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/models/unet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2578 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/post_preds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.411942 mist-medical-0.4.4a0/mist/postprocess_preds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/postprocess_preds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8428 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/postprocess_preds/postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.411942 mist-medical-0.4.4a0/mist/preprocess_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/preprocess_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10643 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/preprocess_data/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.415942 mist-medical-0.4.4a0/mist/runtime/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/runtime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8085 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/runtime/args.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7534 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/runtime/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/runtime/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21551 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/runtime/run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21922 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.415942 mist-medical-0.4.4a0/mist/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/scripts/analyze_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/scripts/preprocess_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/scripts/run_all_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/mist/scripts/train_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.415942 mist-medical-0.4.4a0/mist_medical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    33877 2024-03-29 17:29:10.000000 mist-medical-0.4.4a0/mist_medical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-29 17:29:10.000000 mist-medical-0.4.4a0/mist_medical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:29:10.000000 mist-medical-0.4.4a0/mist_medical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-29 17:29:10.000000 mist-medical-0.4.4a0/mist_medical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-29 17:29:10.000000 mist-medical-0.4.4a0/mist_medical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-29 17:29:10.000000 mist-medical-0.4.4a0/mist_medical.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 17:29:10.415942 mist-medical-0.4.4a0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-03-29 17:29:05.000000 mist-medical-0.4.4a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2554 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.374039 mist-medical-0.4.5a0/mist/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.374039 mist-medical-0.4.5a0/mist/analyze_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/analyze_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16741 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/analyze_data/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/conversion_tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/conversion_tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/conversion_tools/csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5762 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/conversion_tools/msd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/convert_to_mist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/data_loading/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/data_loading/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12303 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/data_loading/dali_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/eval_preds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/evaluate_preds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/evaluate_preds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5350 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/evaluate_preds/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11316 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/inference/main_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3689 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/metrics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22757 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/metrics/lookup_tables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18301 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/attn_unet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9112 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/get_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6272 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/mgnets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16466 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/nnunet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/swin_unetr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/unet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2488 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/post_preds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/postprocess_preds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/postprocess_preds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8387 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/postprocess_preds/postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/preprocess_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/preprocess_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10643 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/preprocess_data/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/mist/runtime/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8099 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/args.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7534 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21551 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22443 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/mist/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/analyze_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/preprocess_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/run_all_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/train_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/mist_medical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/setup.py
```

### Comparing `mist-medical-0.4.4a0/mist/analyze_data/analyze.py` & `mist-medical-0.4.5a0/mist/analyze_data/analyze.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/conversion_tools/csv.py` & `mist-medical-0.4.5a0/mist/conversion_tools/csv.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/conversion_tools/msd.py` & `mist-medical-0.4.5a0/mist/conversion_tools/msd.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/convert_to_mist.py` & `mist-medical-0.4.5a0/mist/convert_to_mist.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/data_loading/dali_loader.py` & `mist-medical-0.4.5a0/mist/data_loading/dali_loader.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/eval_preds.py` & `mist-medical-0.4.5a0/mist/eval_preds.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/evaluate_preds/evaluate.py` & `mist-medical-0.4.5a0/mist/evaluate_preds/evaluate.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,43 +2,37 @@
 import json
 import ants
 import pandas as pd
 import numpy as np
 import SimpleITK as sitk
 
 from mist.metrics.metrics import (
-    dice,
-    surface_dice,
-    avg_surface_distance,
-    hausdorff_distance
+    compute_surface_distances,
+    compute_dice_coefficient,
+    compute_robust_hausdorff,
+    compute_surface_dice_at_tolerance,
+    compute_average_surface_distance
 )
 
 from mist.runtime.utils import (
     init_results_df,
     compute_results_stats,
     convert_dict_to_df,
     get_progress_bar
 )
 
 
-def get_dtms_for_eval(mask_npy, spacing):
-    mask = sitk.Cast(sitk.GetImageFromArray(mask_npy.T), sitk.sitkUInt8)
-    mask.SetSpacing(spacing)
+def get_worst_case_haus(mask_npy, spacing):
+    width = mask_npy.shape[0] * spacing[0]
+    height = mask_npy.shape[1] * spacing[1]
+    depth = mask_npy.shape[2] * spacing[2]
+    return np.sqrt(width ** 2 + height ** 2 + depth ** 2)
 
-    dtm = sitk.Abs(sitk.SignedMaurerDistanceMap(mask, squaredDistance=False, useImageSpacing=True))
-    return dtm
 
-
-def get_surface_contour_for_eval(mask_npy):
-    mask = sitk.Cast(sitk.GetImageFromArray(mask_npy.T), sitk.sitkUInt8)
-    mask_surface = sitk.LabelContour(mask)
-    return mask_surface
-
-
-def evaluate_single_example(pred, truth, patient_id, config, metrics, normalize_hd, use_native_spacing):
+def evaluate_single_example(pred, truth, patient_id, config, metrics, use_native_spacing):
     # Get dice and hausdorff distances for final prediction
     row_dict = dict()
     row_dict['id'] = patient_id
 
     # Read prediction and truth nifti files
     pred = ants.image_read(pred)
     truth = ants.image_read(truth)
@@ -61,62 +55,57 @@
         for label in class_labels:
             pred_label = (pred == label).astype("uint8")
             mask_label = (truth == label).astype("uint8")
 
             pred_temp += pred_label
             truth_temp += mask_label
 
-        # Get DTMs once - we don't recompute them for multiple metrics
-        if "haus95" in metrics or "avg_surf" in metrics or "surf_dice" in metrics:
-            truth_dtm = get_dtms_for_eval(truth_temp, spacing)
-            pred_dtm = get_dtms_for_eval(pred_temp, spacing)
-        else:
-            truth_dtm = None
-            pred_dtm = None
-
-        if "avg_surf" in metrics or "surf_dice" in metrics:
-            truth_surface = get_surface_contour_for_eval(truth_temp)
-            pred_surface = get_surface_contour_for_eval(pred_temp)
-        else:
-            truth_surface = None
-            pred_surface = None
+        # Test surface_distances package
+        truth_temp = truth_temp.astype("bool")
+        pred_temp = pred_temp.astype("bool")
+        distances = compute_surface_distances(truth_temp, pred_temp, spacing)
 
+        temp_truth_sum = truth_temp.sum()
+        temp_pred_sum = pred_temp.sum()
         if "dice" in metrics:
-            row_dict['{}_dice'.format(key)] = dice(truth_temp,
-                                                   pred_temp)
-        if "surf_dice" in metrics:
-            row_dict["{}_surf_dice".format(key)] = surface_dice(truth,
-                                                                pred,
-                                                                spacing,
-                                                                tolerance=1.0,
-                                                                truth_dtm=truth_dtm,
-                                                                pred_dtm=pred_dtm,
-                                                                truth_surface=truth_surface,
-                                                                pred_surface=pred_surface)
+            if temp_truth_sum == 0 and temp_pred_sum == 0:
+                dice_coef = 1.0
+            elif bool(temp_truth_sum == 0) ^ bool(temp_pred_sum == 0):
+                dice_coef = 0.0
+            else:
+                dice_coef = compute_dice_coefficient(truth_temp, pred_temp)
+            row_dict["{}_dice".format(key)] = dice_coef
         if "haus95" in metrics:
-            row_dict['{}_haus95'.format(key)] = hausdorff_distance(truth_temp,
-                                                                   pred_temp,
-                                                                   spacing,
-                                                                   normalize=normalize_hd,
-                                                                   percentile=95,
-                                                                   truth_dtm=truth_dtm,
-                                                                   pred_dtm=pred_dtm)
+            if temp_truth_sum == 0 and temp_pred_sum == 0:
+                haus95_dist = 0.0
+            elif bool(temp_truth_sum == 0) ^ bool(temp_pred_sum == 0):
+                haus95_dist = get_worst_case_haus(truth_temp, spacing)
+            else:
+                haus95_dist = compute_robust_hausdorff(distances, percent=95)
+            row_dict["{}_haus95".format(key)] = haus95_dist
+        if "surf_dice" in metrics:
+            if temp_truth_sum == 0 and temp_pred_sum == 0:
+                surf_dice_coef = 1.0
+            elif bool(temp_truth_sum == 0) ^ bool(temp_pred_sum == 0):
+                surf_dice_coef = 0.0
+            else:
+                surf_dice_coef = compute_surface_dice_at_tolerance(distances, tolerance_mm=1.0)
+            row_dict["{}_surf_dice".format(key)] = surf_dice_coef
         if "avg_surf" in metrics:
-            row_dict['{}_avg_surf'.format(key)] = avg_surface_distance(truth_temp,
-                                                                       pred_temp,
-                                                                       spacing,
-                                                                       normalize=normalize_hd,
-                                                                       truth_dtm=truth_dtm,
-                                                                       pred_dtm=pred_dtm,
-                                                                       truth_surface=truth_surface,
-                                                                       pred_surface=pred_surface)
+            if temp_truth_sum == 0 and temp_pred_sum == 0:
+                avg_surf_dist = 0.0
+            elif bool(temp_truth_sum == 0) ^ bool(temp_pred_sum == 0):
+                avg_surf_dist = get_worst_case_haus(truth_temp, spacing)
+            else:
+                avg_surf_dist = compute_average_surface_distance(distances)
+            row_dict["{}_avg_surf".format(key)] = avg_surf_dist
     return row_dict
 
 
-def evaluate(config_json, paths, source_dir, output_csv, metrics, normalize_hd, use_native_spacing):
+def evaluate(config_json, paths, source_dir, output_csv, metrics, use_native_spacing):
     with open(config_json, 'r') as file:
         config = json.load(file)
 
     if not isinstance(paths, pd.DataFrame):
         # Convert input to pandas dataframe
         if '.csv' in paths:
             paths = pd.read_csv(paths)
@@ -146,13 +135,12 @@
             truth = paths.loc[paths['id'].astype(str) == patient_id].iloc[0]['mask']
 
             eval_results = evaluate_single_example(pred,
                                                    truth,
                                                    patient_id,
                                                    config,
                                                    metrics,
-                                                   normalize_hd,
                                                    use_native_spacing)
             results_df = pd.concat([results_df, pd.DataFrame(eval_results, index=[0])], ignore_index=True)
 
     results_df = compute_results_stats(results_df)
     results_df.to_csv(output_csv, index=False)
```

### Comparing `mist-medical-0.4.4a0/mist/inference/main_inference.py` & `mist-medical-0.4.5a0/mist/inference/main_inference.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/main.py` & `mist-medical-0.4.5a0/mist/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         mist_trainer.fit()
 
         evaluate(args.data,
                  os.path.join(args.results, "train_paths.csv"),
                  os.path.join(args.results, "predictions", "train", "raw"),
                  os.path.join(args.results, "results.csv"),
                  args.metrics,
-                 args.normalize_hd,
                  args.use_native_spacing)
 
     if args.exec_mode == "all" or args.exec_mode == "train":
         if has_test_data(args.data):
             test_df = get_files_df(args.data, "test")
             test_df.to_csv(os.path.join(args.results, "test_paths.csv"), index=False)
```

### Comparing `mist-medical-0.4.4a0/mist/models/attn_unet.py` & `mist-medical-0.4.5a0/mist/models/attn_unet.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/models/get_model.py` & `mist-medical-0.4.5a0/mist/models/get_model.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/models/layers.py` & `mist-medical-0.4.5a0/mist/models/layers.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/models/mgnets.py` & `mist-medical-0.4.5a0/mist/models/mgnets.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/models/nnunet.py` & `mist-medical-0.4.5a0/mist/models/nnunet.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/models/swin_unetr.py` & `mist-medical-0.4.5a0/mist/models/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/models/unet.py` & `mist-medical-0.4.5a0/mist/models/unet.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/post_preds.py` & `mist-medical-0.4.5a0/mist/post_preds.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
           type=non_negative_int,
           help="How many of top connected components to keep")
     p.arg("--morph-cleanup-iterations",
           default=2,
           type=non_negative_int,
           help="How many iterations for morphological cleaning")
     p.arg("--fill-label", type=non_negative_int, help="Fill label for fill holes transformation")
-    p.boolean_flag("--normalize-hd", default=False, help="Normalize Hausdorff distances")
     p.arg("--metrics",
           nargs="+",
           default=["dice", "haus95"],
           choices=["dice", "surf_dice", "haus95", "avg_surf"],
           help="List of metrics to use for evaluation")
     p.boolean_flag("--use-native-spacing",
                    default=False,
```

### Comparing `mist-medical-0.4.4a0/mist/postprocess_preds/postprocess.py` & `mist-medical-0.4.5a0/mist/postprocess_preds/postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 
         # Evaluate new predictions
         evaluate(self.config_file,
                  self.train_paths,
                  self.dest_dir,
                  self.new_results_csv,
                  self.metrics,
-                 self.args.normalize_hd,
                  self.args.use_native_spacing)
 
         # Compute improvement score
         new_results_df = pd.read_csv(self.new_results_csv)
         score = compute_improvement_score(self.base_results_df, new_results_df, self.metrics)
         return score
```

### Comparing `mist-medical-0.4.4a0/mist/predict.py` & `mist-medical-0.4.5a0/mist/predict.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/preprocess_data/preprocess.py` & `mist-medical-0.4.5a0/mist/preprocess_data/preprocess.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/runtime/args.py` & `mist-medical-0.4.5a0/mist/runtime/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,23 +74,24 @@
     p.arg("--max-patch-size", default=[256, 256, 256], nargs="+", type=int, help="Max patch size")
     p.arg("--val-percent", type=float_0_1, default=0.1, help="Percentage of training data used for validation")
     p.arg("--learning-rate", type=float, default=0.0003, help="Learning rate")
     p.arg("--exp_decay", type=float, default=0.9999, help="Exponential decay factor")
     p.arg("--lr-scheduler",
           type=str,
           default="constant",
-          choices=["constant", "cosine_warm_restarts", "exponential"],
+          choices=["constant", "polynomial", "cosine", "cosine_warm_restarts", "exponential"],
           help="Learning rate scheduler")
     p.arg("--cosine-first-steps",
           type=positive_int,
           default=500,
           help="Length of a cosine decay cycle in steps, only with cosine_annealing scheduler")
 
     # Optimizer
-    p.arg("--optimizer", type=str, default="adam", choices=["sgd", "adam", "adamw"], help="Optimizer")
+    p.arg("--optimizer", type=str, default="adam", choices=["adam", "sgd", "adamw"], help="Optimizer")
+    p.arg("--sgd-momentum", type=float_0_1, default=0, help="Momentum for SGD")
     p.boolean_flag("--clip-norm", default=False, help="Use gradient clipping")
     p.arg("--clip-norm-max", type=float, default=1.0, help="Max threshold for global norm clipping")
 
     # Neural network parameters
     p.arg("--model",
           type=str,
           default="nnunet",
@@ -168,15 +169,14 @@
 
     # Evaluation
     p.arg("--metrics",
           nargs="+",
           default=["dice", "haus95"],
           choices=["dice", "surf_dice", "haus95", "avg_surf"],
           help="List of metrics to use for evaluation")
-    p.boolean_flag("--normalize-hd", default=False, help="Normalize Hausdorff distances")
     p.boolean_flag("--use-native-spacing",
                    default=False,
                    help="Use native image spacing to compute Hausdorff distances")
 
     # Uncertainty
     p.boolean_flag("--output-std", default=False, help="Output standard deviation for ensemble predictions")
```

### Comparing `mist-medical-0.4.4a0/mist/runtime/loss.py` & `mist-medical-0.4.5a0/mist/runtime/loss.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/runtime/progress_bar.py` & `mist-medical-0.4.5a0/mist/runtime/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/runtime/run.py` & `mist-medical-0.4.5a0/mist/runtime/run.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/runtime/utils.py` & `mist-medical-0.4.5a0/mist/runtime/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,27 +154,34 @@
         df = pd.concat([df, pd.DataFrame(row_dict, index=[0])], ignore_index=True)
     return df
 
 
 def get_lr_schedule(args, optimizer):
     if args.lr_scheduler == "constant":
         return torch.optim.lr_scheduler.ConstantLR(optimizer, factor=1)
+    elif args.lr_scheduler == "polynomial":
+        return torch.optim.lr_scheduler.PolynomialLR(optimizer,
+                                                     total_iters=args.steps_per_epoch*args.epochs,
+                                                     power=0.9)
     elif args.lr_scheduler == "cosine_warm_restarts":
         return torch.optim.lr_scheduler.CosineAnnealingWarmRestarts(optimizer,
                                                                     T_0=args.cosine_first_steps,
                                                                     T_mult=2)
+    elif args.lr_scheduler == "cosine":
+        return torch.optim.lr_scheduler.CosineAnnealingLR(optimizer,
+                                                          T_max=args.steps_per_epoch*args.epochs)
     elif args.lr_scheduler == "exponential":
         return torch.optim.lr_scheduler.ExponentialLR(optimizer, gamma=args.exp_decay)
     else:
         raise ValueError("Invalid learning rate scheduler")
 
 
 def get_optimizer(args, model):
     if args.optimizer == "sgd":
-        return torch.optim.SGD(params=model.parameters(), lr=args.learning_rate)
+        return torch.optim.SGD(params=model.parameters(), lr=args.learning_rate, momentum=args.sgd_momentum)
     elif args.optimizer == "adam":
         return torch.optim.Adam(params=model.parameters(), lr=args.learning_rate)
     elif args.optimizer == "adamw":
         return torch.optim.AdamW(params=model.parameters(), lr=args.learning_rate)
     else:
         raise ValueError("Invalid optimizer")
 
@@ -279,19 +286,19 @@
     # Get final statistics
     mean_row = {"id": "Mean"}
     std_row = {"id": "Std"}
     percentile50_row = {"id": "Median"}
     percentile25_row = {"id": "25th Percentile"}
     percentile75_row = {"id": "75th Percentile"}
     for col in results_df.columns[1:]:
-        mean_row[col] = np.mean(results_df[col])
-        std_row[col] = np.std(results_df[col])
-        percentile25_row[col] = np.percentile(results_df[col], 25)
-        percentile50_row[col] = np.percentile(results_df[col], 50)
-        percentile75_row[col] = np.percentile(results_df[col], 75)
+        mean_row[col] = np.nanmean(results_df[col])
+        std_row[col] = np.nanstd(results_df[col])
+        percentile25_row[col] = np.nanpercentile(results_df[col], 25)
+        percentile50_row[col] = np.nanpercentile(results_df[col], 50)
+        percentile75_row[col] = np.nanpercentile(results_df[col], 75)
 
     results_df = pd.concat([results_df, pd.DataFrame(mean_row, index=[0])], ignore_index=True)
     results_df = pd.concat([results_df, pd.DataFrame(std_row, index=[0])], ignore_index=True)
     results_df = pd.concat([results_df, pd.DataFrame(percentile25_row, index=[0])], ignore_index=True)
     results_df = pd.concat([results_df, pd.DataFrame(percentile50_row, index=[0])], ignore_index=True)
     results_df = pd.concat([results_df, pd.DataFrame(percentile75_row, index=[0])], ignore_index=True)
     return results_df
```

### Comparing `mist-medical-0.4.4a0/mist/scripts/run_all_entrypoint.py` & `mist-medical-0.4.5a0/mist/scripts/run_all_entrypoint.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist/scripts/train_entrypoint.py` & `mist-medical-0.4.5a0/mist/scripts/train_entrypoint.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.4a0/mist_medical.egg-info/SOURCES.txt` & `mist-medical-0.4.5a0/mist_medical.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 mist/data_loading/__init__.py
 mist/data_loading/dali_loader.py
 mist/evaluate_preds/__init__.py
 mist/evaluate_preds/evaluate.py
 mist/inference/__init__.py
 mist/inference/main_inference.py
 mist/metrics/__init__.py
+mist/metrics/lookup_tables.py
 mist/metrics/metrics.py
 mist/models/__init__.py
 mist/models/attn_unet.py
 mist/models/get_model.py
 mist/models/layers.py
 mist/models/mgnets.py
 mist/models/nnunet.py
```

### Comparing `mist-medical-0.4.4a0/pyproject.toml` & `mist-medical-0.4.5a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mist-medical"
-version = "0.4.4-alpha"
+version = "0.4.5-alpha"
 requires-python = ">= 3.8"
 description = "MIST is a simple, fully automated framework for 3D medical imaging segmentation."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Adrian Celaya", email = "aecelaya@rice.edu"},
     {name = "David Fuentes", email = "dtfuentes@mdanderson.org"},
```

