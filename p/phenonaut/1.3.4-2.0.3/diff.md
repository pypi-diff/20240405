# Comparing `tmp/phenonaut-1.3.4.tar.gz` & `tmp/phenonaut-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenonaut-1.3.4.tar", last modified: Mon Mar 27 08:57:34 2023, max compression
+gzip compressed data, was "phenonaut-2.0.3.tar", last modified: Fri Apr  5 11:52:07 2024, max compression
```

## Comparing `phenonaut-1.3.4.tar` & `phenonaut-2.0.3.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.285813 phenonaut-1.3.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-02-13 21:12:15.000000 phenonaut-1.3.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       88 2023-02-16 15:43:59.000000 phenonaut-1.3.4/NOTICE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2625 2023-03-27 08:57:34.285813 phenonaut-1.3.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2053 2023-03-27 08:55:07.000000 phenonaut-1.3.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.245812 phenonaut-1.3.4/phenonaut/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      321 2023-03-17 12:55:49.000000 phenonaut-1.3.4/phenonaut/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      654 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/__main__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.245812 phenonaut-1.3.4/phenonaut/data/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      167 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/data/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    78632 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/data/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3053 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/data/platemap_querier.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      599 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/data/recipes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.245812 phenonaut-1.3.4/phenonaut/metrics/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      188 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/metrics/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8567 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/metrics/distances.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14267 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/metrics/measures.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9335 2023-03-17 12:54:23.000000 phenonaut-1.3.4/phenonaut/metrics/non_ds_phenotypic_metrics.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    81034 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/metrics/performance.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17467 2023-03-17 12:54:23.000000 phenonaut-1.3.4/phenonaut/metrics/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.265812 phenonaut-1.3.4/phenonaut/output/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      255 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/output/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2242 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/output/boxplot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8306 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/output/heatmap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/output/pair_plot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    32839 2023-02-13 21:12:16.000000 phenonaut-1.3.4/phenonaut/output/ph0_pptx_template.pptx
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    31496 2023-02-13 21:12:16.000000 phenonaut-1.3.4/phenonaut/output/ph0_pptx_template_desc.pptx
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4864 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/output/pptx.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9783 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/output/scatter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2538 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/output/spreadsheet.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1123 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/output/visualisation_base.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.269812 phenonaut-1.3.4/phenonaut/packaged_datasets/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      333 2023-03-17 12:55:49.000000 phenonaut-1.3.4/phenonaut/packaged_datasets/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24771 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/packaged_datasets/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6540 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/packaged_datasets/breast_cancer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    28170 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/packaged_datasets/cmap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8687 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/packaged_datasets/iris.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11035 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/packaged_datasets/lincs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9494 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/packaged_datasets/metadata_moa.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26493 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/packaged_datasets/tcga.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    48915 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/phenonaut.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.273812 phenonaut-1.3.4/phenonaut/predict/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      121 2023-02-13 21:12:16.000000 phenonaut-1.3.4/phenonaut/predict/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.277813 phenonaut-1.3.4/phenonaut/predict/default_predictors/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/default_predictors/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3117 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/default_predictors/classifiers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2242 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/default_predictors/multiregressors.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.277813 phenonaut-1.3.4/phenonaut/predict/default_predictors/pytorch_models/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      163 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/default_predictors/pytorch_models/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9492 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/default_predictors/pytorch_models/dave.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4258 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/default_predictors/pytorch_models/multiregressor_nn.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2599 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/default_predictors/regressors.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17903 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/optuna_functions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18631 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/predict_utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4377 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/predictor_dataclasses.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21424 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/predict/profile.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.281813 phenonaut-1.3.4/phenonaut/transforms/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      301 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/transforms/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23124 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/transforms/dimensionality_reduction.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      461 2023-02-15 14:16:19.000000 phenonaut-1.3.4/phenonaut/transforms/generic_transformations.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5512 2023-03-27 08:52:12.000000 phenonaut-1.3.4/phenonaut/transforms/imputers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24722 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/transforms/preparative.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6728 2023-03-27 08:53:39.000000 phenonaut-1.3.4/phenonaut/transforms/supervised_transformer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38335 2023-02-15 14:51:28.000000 phenonaut-1.3.4/phenonaut/transforms/transformer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3126 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53339 2023-02-16 15:43:59.000000 phenonaut-1.3.4/phenonaut/workflow.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.285813 phenonaut-1.3.4/phenonaut.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2625 2023-03-27 08:57:33.000000 phenonaut-1.3.4/phenonaut.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2380 2023-03-27 08:57:33.000000 phenonaut-1.3.4/phenonaut.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-03-27 08:57:33.000000 phenonaut-1.3.4/phenonaut.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      237 2023-03-27 08:57:33.000000 phenonaut-1.3.4/phenonaut.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2023-03-27 08:57:33.000000 phenonaut-1.3.4/phenonaut.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      186 2023-02-15 15:44:16.000000 phenonaut-1.3.4/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1216 2023-03-27 08:57:34.289813 phenonaut-1.3.4/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-27 08:57:34.285813 phenonaut-1.3.4/test/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6001 2023-03-27 08:53:39.000000 phenonaut-1.3.4/test/test_dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      291 2023-03-17 12:54:23.000000 phenonaut-1.3.4/test/test_metrics.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9882 2023-03-27 08:53:39.000000 phenonaut-1.3.4/test/test_phenonaut_obj.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1654 2023-02-15 14:16:19.000000 phenonaut-1.3.4/test/test_prediction.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3058 2023-03-27 08:53:39.000000 phenonaut-1.3.4/test/test_preparation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2870 2023-02-15 14:16:19.000000 phenonaut-1.3.4/test/test_transformations.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.969483 phenonaut-2.0.3/
+-rw-rw-rw-   0        0        0    11358 2024-04-05 11:38:20.000000 phenonaut-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0       87 2024-04-05 11:38:20.000000 phenonaut-2.0.3/NOTICE
+-rw-rw-rw-   0        0        0    15899 2024-04-05 11:52:07.968483 phenonaut-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2024-04-05 11:38:20.000000 phenonaut-2.0.3/README.md
+-rw-rw-rw-   0        0        0     2318 2024-04-05 11:38:20.000000 phenonaut-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:52:07.969483 phenonaut-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.882483 phenonaut-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.894484 phenonaut-2.0.3/src/phenonaut/
+-rw-rw-rw-   0        0        0      343 2024-04-05 11:38:18.000000 phenonaut-2.0.3/src/phenonaut/__init__.py
+-rw-rw-rw-   0        0        0      669 2024-04-05 11:38:18.000000 phenonaut-2.0.3/src/phenonaut/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.922482 phenonaut-2.0.3/src/phenonaut/data/
+-rw-rw-rw-   0        0        0      167 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/data/__init__.py
+-rw-rw-rw-   0        0        0    82065 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/data/dataset.py
+-rw-rw-rw-   0        0        0     3154 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/data/platemap_querier.py
+-rw-rw-rw-   0        0        0      599 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/data/recipes.py
+-rw-rw-rw-   0        0        0       46 2024-04-05 11:38:18.000000 phenonaut-2.0.3/src/phenonaut/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.930483 phenonaut-2.0.3/src/phenonaut/metrics/
+-rw-rw-rw-   0        0        0      188 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/metrics/__init__.py
+-rw-rw-rw-   0        0        0     8648 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/metrics/distances.py
+-rw-rw-rw-   0        0        0    14409 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/metrics/measures.py
+-rw-rw-rw-   0        0        0     9841 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/metrics/non_ds_phenotypic_metrics.py
+-rw-rw-rw-   0        0        0    94367 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/metrics/performance.py
+-rw-rw-rw-   0        0        0    17725 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/metrics/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.938484 phenonaut-2.0.3/src/phenonaut/output/
+-rw-rw-rw-   0        0        0      255 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/__init__.py
+-rw-rw-rw-   0        0        0     2511 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/boxplot.py
+-rw-rw-rw-   0        0        0     8390 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/heatmap.py
+-rw-rw-rw-   0        0        0      406 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/pair_plot.py
+-rw-rw-rw-   0        0        0    32839 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/ph0_pptx_template.pptx
+-rw-rw-rw-   0        0        0    31496 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/ph0_pptx_template_desc.pptx
+-rw-rw-rw-   0        0        0     4903 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/pptx.py
+-rw-rw-rw-   0        0        0     9716 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/scatter.py
+-rw-rw-rw-   0        0        0     2583 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/spreadsheet.py
+-rw-rw-rw-   0        0        0     1125 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/output/visualisation_base.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.945483 phenonaut-2.0.3/src/phenonaut/packaged_datasets/
+-rw-rw-rw-   0        0        0      315 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/packaged_datasets/__init__.py
+-rw-rw-rw-   0        0        0    24786 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/packaged_datasets/base.py
+-rw-rw-rw-   0        0        0     6527 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/packaged_datasets/breast_cancer.py
+-rw-rw-rw-   0        0        0    28381 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/packaged_datasets/cmap.py
+-rw-rw-rw-   0        0        0     8673 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/packaged_datasets/iris.py
+-rw-rw-rw-   0        0        0    11095 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/packaged_datasets/lincs.py
+-rw-rw-rw-   0        0        0     9631 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/packaged_datasets/metadata_moa.py
+-rw-rw-rw-   0        0        0    27152 2024-04-05 11:38:20.000000 phenonaut-2.0.3/src/phenonaut/packaged_datasets/tcga.py
+-rw-rw-rw-   0        0        0    51451 2024-04-05 11:38:18.000000 phenonaut-2.0.3/src/phenonaut/phenonaut.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.949483 phenonaut-2.0.3/src/phenonaut/predict/
+-rw-rw-rw-   0        0        0      121 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.953483 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/
+-rw-rw-rw-   0        0        0        0 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/__init__.py
+-rw-rw-rw-   0        0        0     3097 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/classifiers.py
+-rw-rw-rw-   0        0        0     2279 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/multiregressors.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.955484 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/pytorch_models/
+-rw-rw-rw-   0        0        0      163 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/pytorch_models/__init__.py
+-rw-rw-rw-   0        0        0     9758 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/pytorch_models/dave.py
+-rw-rw-rw-   0        0        0     4155 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/pytorch_models/multiregressor_nn.py
+-rw-rw-rw-   0        0        0     2634 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/default_predictors/regressors.py
+-rw-rw-rw-   0        0        0    18374 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/optuna_functions.py
+-rw-rw-rw-   0        0        0    19065 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/predict_utils.py
+-rw-rw-rw-   0        0        0     4593 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/predictor_dataclasses.py
+-rw-rw-rw-   0        0        0    22405 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/predict/profile.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.962483 phenonaut-2.0.3/src/phenonaut/transforms/
+-rw-rw-rw-   0        0        0      301 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/transforms/__init__.py
+-rw-rw-rw-   0        0        0    24064 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/transforms/dimensionality_reduction.py
+-rw-rw-rw-   0        0        0      463 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/transforms/generic_transformations.py
+-rw-rw-rw-   0        0        0     5519 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/transforms/imputers.py
+-rw-rw-rw-   0        0        0    25106 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/transforms/preparative.py
+-rw-rw-rw-   0        0        0     6873 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/transforms/supervised_transformer.py
+-rw-rw-rw-   0        0        0    39579 2024-04-05 11:38:19.000000 phenonaut-2.0.3/src/phenonaut/transforms/transformer.py
+-rw-rw-rw-   0        0        0     3127 2024-04-05 11:38:18.000000 phenonaut-2.0.3/src/phenonaut/utils.py
+-rw-rw-rw-   0        0        0    53718 2024-04-05 11:38:18.000000 phenonaut-2.0.3/src/phenonaut/workflow.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.919484 phenonaut-2.0.3/src/phenonaut.egg-info/
+-rw-rw-rw-   0        0        0    15899 2024-04-05 11:52:07.000000 phenonaut-2.0.3/src/phenonaut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2518 2024-04-05 11:52:07.000000 phenonaut-2.0.3/src/phenonaut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:52:07.000000 phenonaut-2.0.3/src/phenonaut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      458 2024-04-05 11:52:07.000000 phenonaut-2.0.3/src/phenonaut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 11:52:07.000000 phenonaut-2.0.3/src/phenonaut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:07.967483 phenonaut-2.0.3/test/
+-rw-rw-rw-   0        0        0     6645 2024-04-05 11:38:20.000000 phenonaut-2.0.3/test/test_dataset.py
+-rw-rw-rw-   0        0        0     1456 2024-04-05 11:38:20.000000 phenonaut-2.0.3/test/test_metrics.py
+-rw-rw-rw-   0        0        0     9921 2024-04-05 11:38:20.000000 phenonaut-2.0.3/test/test_phenonaut_obj.py
+-rw-rw-rw-   0        0        0     1656 2024-04-05 11:38:20.000000 phenonaut-2.0.3/test/test_prediction.py
+-rw-rw-rw-   0        0        0     3210 2024-04-05 11:38:20.000000 phenonaut-2.0.3/test/test_preparation.py
+-rw-rw-rw-   0        0        0     2919 2024-04-05 11:38:20.000000 phenonaut-2.0.3/test/test_transformations.py
```

### Comparing `phenonaut-1.3.4/LICENSE` & `phenonaut-2.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `phenonaut-1.3.4/README.md` & `phenonaut-2.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # Phenonaut
 
-A toolkit for multi-omic phenotypic space exploration. 
+A toolkit for multi-omic phenotypic space exploration.
+
 
 
 ## Description
 <img style="float: right;" src="phenonaut.png">
 
-Phenonaut is a framework for applying workflows to multi-omics data. Originally targeting high-content imaging and the exploration of phenotypic space, with different visualisations and metrics, Phenonaut allows now operates in a data agnostic manner, allowing users to describe their data (potentially multi-view/multi-omics) and apply a series of generic or specialised data-centric transforms and measures.  
+Phenonaut is a framework for applying workflows to multi-omics data. Originally targeting high-content imaging and the exploration of phenotypic space, with different visualisations and metrics, Phenonaut allows now operates in a data agnostic manner, allowing users to describe their data (potentially multi-view/multi-omics) and apply a series of generic or specialised data-centric transforms and measures.
+
 
 Phenonaut operates in 2 modes:
 
 - As a Python package, importable and callable within custom scripts.
 - Operating on a workflow defined in either YAML, or JSON, allowing integration of complex chains of Phenonaut instructions to be integrated into existing workflows and pipelines. When built as a package and installed, workflows can be executed with:
 ```python -m phenonaut workflow.yml``` .
 
+After installing phenonaut into a kernel, dont forget to register it with Jupyter:
+```python -m ipykernel install --user --name=<ENVIRONMENT NAME>```
+
 
 ## Structrure
-Datasets are read into the dataset class, aided by a yaml file describing the underlying data (see config/ for example yaml data definition files). Pandas dataframes are created representing the data (a Phenonaut object may hold multiple dataset objects), along with two additional pieces of data. 
+Datasets are read into the dataset class, aided by a yaml file describing the underlying data (see config/ for example yaml data definition files). Pandas dataframes are created representing the data (a Phenonaut object may hold multiple dataset objects), along with two additional pieces of data.
 1) A features list, accessible with .features property of a dataframe. Initially defined by the data definition workflow.
 2) perturbation_column, optional column which gives a unique ID to the treatment performed on the well/vial/data.
 3) Metadata, optional dictionary containing metadata for the dataset.
 
-## Documentation
-
-[Start here](https://carragherlab.github.io/phenonaut/)
-- [User guide](https://carragherlab.github.io/phenonaut/userguide.html)
-- [API documentation](https://carragherlab.github.io/phenonaut/phenonaut.html)
-- [Publication examples](https://carragherlab.github.io/phenonaut/publication_examples.html)
-- [Workflow mode](https://carragherlab.github.io/phenonaut/workflow_guide.html)
-
+Example usage in Python programs, and in workflow/scripted modes coming soon.
 
 
-Copyright © The University of Edinburgh, 2023.
+Copyright © The University of Edinburgh, 2024.
 
 Development has been supported by GSK.
```

### Comparing `phenonaut-1.3.4/phenonaut/__main__.py` & `phenonaut-2.0.3/src/phenonaut/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
 """
 Phenonaut workflows are an alternative way of running phenonaut transforms allowing
 the processing of data as defined in YAML or JSON workflow files.
 """
-from phenonaut.workflow import Workflow
-from pathlib import Path
 import argparse
+from pathlib import Path
+
+from phenonaut.workflow import Workflow
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Run a Phenonaut workflow")
-    parser.add_argument("workflow_path", help="YAML or JSON file containing Phenonaut workflow")
+    parser.add_argument(
+        "workflow_path", help="YAML or JSON file containing Phenonaut workflow"
+    )
     args = parser.parse_args()
 
     workflow_path = Path(args.workflow_path)
 
     ph0_workflow = Workflow(workflow_path)
```

### Comparing `phenonaut-1.3.4/phenonaut/data/dataset.py` & `phenonaut-2.0.3/src/phenonaut/data/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# Copyright © The University of Edinburgh, 2023.
+# Copyright © The University of Edinburgh, 2024.
 # Development has been supported by GSK.
 
-from scipy.spatial.distance import cdist
+import re
+from collections import namedtuple
+from collections.abc import Callable
+from copy import deepcopy
+from hashlib import sha256
 from inspect import signature
+from itertools import product as itertools_product
 from pathlib import Path
-from typing import Callable, Optional, Union
-import pandas as pd
+from typing import List, Optional, Union
+
 import numpy as np
+import pandas as pd
 from pandas.errors import DataError
+from scipy.spatial.distance import cdist
 
-from copy import deepcopy
-from itertools import product as itertools_product
-from collections import namedtuple
 from phenonaut import data
 from phenonaut.utils import load_dict
-from hashlib import sha256
-import re
 
 TransformationHistory = namedtuple("TransformationHistory", ["features", "description"])
 
 
 class Dataset:
 
     """Dataset constructor
@@ -73,55 +75,61 @@
     DataError
         Metadata could not be used to parse input CSV
     """
 
     def __init__(
         self,
         dataset_name: str,
-        input_file_path_or_df: Union[Path, str, pd.DataFrame] = None,
+        input_file_path_or_df: Optional[Union[Path, str, pd.DataFrame]] = None,
         metadata: Union[dict, Path, str] = {},
         kind: Optional[str] = None,
         init_hash: Optional[Union[str, bytes]] = None,
         h5_key: Optional[str] = None,
         features: Optional[list[str]] = None,
     ):
         self.name = dataset_name
         self._history = []
         self._metadata = {}
         self._features = []
         self.df = None
         self.callable_functions = list(
             x for x in dir(Dataset) if callable(getattr(Dataset, x)) and x[0] != "_"
         )
-        metadata=deepcopy(metadata)
+        metadata = deepcopy(metadata)
         features_can_be_an_empty_list = False
 
         if features is not None:
             if metadata is None:
-                metadata={}
+                metadata = {}
 
             if "features" in metadata:
                 raise ValueError(
                     f"'features' argument was not None in construction of new Dataset (named {dataset_name}), and metadata contained a features entry, please use only one"
                 )
-            metadata['features']=features.copy()
+            metadata["features"] = features.copy()
 
         if metadata is not None:
-            if metadata.get("features", None) == []:
-                features_can_be_an_empty_list = True
+            metadata_features=metadata.get("features", None)
+            if metadata_features is not None:
+                if not isinstance(metadata_features, list):
+                    raise ValueError(f"metadata features should be of type list, it was of type: {type(metadata_features)}")
+                if metadata_features == []:
+                    features_can_be_an_empty_list = True
 
         if init_hash is None:
             self.sha256 = sha256()
         else:
             if isinstance(init_hash, bytes):
                 self.sha256 = sha256(init_hash)
             elif isinstance(init_hash, str):
                 self.sha256 = sha256(init_hash.encode("utf-8"))
             else:
-                raise ValueError(f"The given argument init_hash was not a bytes array or a string")
+                raise ValueError(
+                    f"The given argument init_hash was not a bytes array or a string"
+                )
         # If file path is a string, make it a Path
         if isinstance(input_file_path_or_df, str):
             input_file_path_or_df = Path(input_file_path_or_df)
 
         # Allow creation of a blank Dataset object when None is supplied for csv_file_path
         if input_file_path_or_df is None:
             self.__update_hash()
@@ -129,21 +137,25 @@
 
         # Load metadata.
         # If str, change to path, check exists, load yaml file defining metadata
         # Can also be a dictionary, which is allowed, or None, relying on defaults.
         if isinstance(metadata, (Path, str)):
             metadata = load_dict(metadata)
         if metadata is None:
-            metadata={}
+            metadata = {}
 
         if kind is not None:
             from .recipes import kinds
 
             regularised_kind = (
-                kind.lower().replace(" ", "").replace("-", "").replace("_", "").replace(".", "")
+                kind.lower()
+                .replace(" ", "")
+                .replace("-", "")
+                .replace("_", "")
+                .replace(".", "")
             )
             if regularised_kind not in kinds:
                 raise ValueError(
                     f"Dataset kind given in kind argument was '{kind}',"
                     f" but this was not found in phenonaut. Usable kind arguments are: {kinds.keys()}"
                 )
             metadata = {**kinds[regularised_kind], **metadata}
@@ -153,15 +165,17 @@
             metadata["skip_row_numbers"] = [metadata["skip_row_numbers"]]
         if isinstance(metadata.get("header_row_number"), int):
             metadata["header_row_number"] = [metadata["header_row_number"]]
 
         if isinstance(input_file_path_or_df, Path):
             if input_file_path_or_df.suffix == ".h5":
                 if "key" not in metadata:
-                    raise KeyError("Attempting to load hdf5 file, but no key was given in metadata")
+                    raise KeyError(
+                        "Attempting to load hdf5 file, but no key was given in metadata"
+                    )
                 self.df = pd.read_hdf(input_file_path_or_df, h5_key)
             else:
                 # Read the CSV file into a pandas DataFrame. It needs to be read in
                 # before features are set because the user may be using
                 # features_prefix, so we need to examine column names to obtain
                 # feature names
 
@@ -229,15 +243,17 @@
                     func_name, func_args = t[0], (t[1],)
                 else:
                     func_name, func_args = t
             if len(t) > 2:
                 func_name, func_args = t[0], t[1:]
 
             if func_name not in self.callable_functions:
-                raise KeyError(f"'transforms' contains an unknown function: '{func_name}'")
+                raise KeyError(
+                    f"'transforms' contains an unknown function: '{func_name}'"
+                )
 
             if isinstance(func_args, dict):
                 getattr(self, func_name)(**func_args)
             else:
                 getattr(self, func_name)(*func_args)
 
         if "features" in metadata and "initial_features" in metadata:
@@ -277,15 +293,17 @@
                         if str(column_name).startswith(tuple(features_prefix))
                     ]
                 )
 
             if features_regex is not None:
                 metadata["initial_features"].extend(
                     f
-                    for f in list(filter(re.compile(features_regex).match, self.df.columns.values))
+                    for f in list(
+                        filter(re.compile(features_regex).match, self.df.columns.values)
+                    )
                     if f not in metadata["initial_features"]
                 )
 
             if len(metadata["initial_features"]) == 0:
                 message = f"No column headers found with specified prefix(es): {features_prefix}, or matching features_regex {features_regex}, first 10 column headers were: {self.df.columns[:10]}"
                 raise DataError(message)
 
@@ -309,15 +327,17 @@
         # ['f1', 'f2a', 'f03', 'f10', 'f13']
         # ignoring zero padding etc.
         def natural_sort_convert_digit_or_str(x):
             return int(x) if x.isdigit() else x.lower()
 
         metadata["initial_features"] = sorted(
             metadata["initial_features"],
-            key=lambda x: [natural_sort_convert_digit_or_str(c) for c in re.split("([0-9]+)", x)],
+            key=lambda x: [
+                natural_sort_convert_digit_or_str(c) for c in re.split("([0-9]+)", x)
+            ],
         )
 
         # Check all specified features are present in the DataFrame
         missing_features = []
         for feature in metadata["initial_features"]:
             if feature not in self.df.columns:
                 print(f"Specified feature ({feature}) not found in columns")
@@ -392,27 +412,27 @@
                 "Setting features requires a tuple to be supplied of the form:([features], 'history message')"
             )
         if len(features_and_message_tuple) != 2:
             raise AttributeError(
                 "Supplied tuple did not have 2 elements. Setting features requires a tuple to be supplied of the form:([features], 'history message')"
             )
         if len(features_and_message_tuple[0]) == 0:
-            print(f"Features list is empty, message was {features_and_message_tuple[1]}")
+            print(
+                f"Features list is empty, message was {features_and_message_tuple[1]}"
+            )
         if not isinstance(features_and_message_tuple[1], str):
             raise AttributeError(
                 "Message (second tuple element) must be of type str. Setting features requires a tuple to be supplied of the form:([features], 'history message')"
             )
 
         self._history.append(TransformationHistory(*features_and_message_tuple))
         self._features = list(features_and_message_tuple[0])
         self.__update_hash()
 
-    def get_history(
-        self,
-    ) -> list[TransformationHistory]:
+    def get_history(self) -> list[TransformationHistory]:
         """Get dataset history
 
         Returns
         -------
         list[TransformationHistory]
             List of TransformationHistory (named tuples) which contain a list
             of features as the first element and then a plain text description
@@ -479,20 +499,22 @@
         """
         self._metadata["perturbation_column"] = perturbation_column
         self.features = (
             self.features,
             f"Updated perturbation column, perturbation column is now {perturbation_column}",
         )
 
-    def get_unique_perturbations(
-        self,
-    ):
+    def get_unique_perturbations(self):
         if self.perturbation_column is None:
             return None
-        return [t for t in self.df[self.perturbation_column].unique() if not pd.isna(t) and t != ""]
+        return [
+            t
+            for t in self.df[self.perturbation_column].unique()
+            if not pd.isna(t) and t != ""
+        ]
 
     def get_feature_ranges(self, pad_by_percent: Union[float, int]) -> tuple:
         """Get the ranges of feature columns
 
         Parameters
         ----------
         pad_by_percent : Union[float, int]
@@ -525,15 +547,17 @@
         -------
         list[str]
             Returns list of Dataset columns which are not currently features.
         """
         return list(set(self.df.columns.unique().values) - set(self.features))
 
     def drop_columns(
-        self, column_labels: Union[str, list[str], tuple[str]], reason: Optional[str] = None
+        self,
+        column_labels: Union[str, list[str], tuple[str]],
+        reason: Optional[str] = None,
     ) -> None:
         """Drop columns inplace, update features if needed and set new history.
 
         Intelligently drop columns from the dataset (inplace). If any of those
         columns were listed as features, then remove them from the features list
         and set a new new history.  Updating features and new history only
         happens if it needs to (removed column was a feature). Updaing of
@@ -562,20 +586,27 @@
         if isinstance(column_labels, str):
             column_labels = [column_labels]
         features_removed = set(self.features).intersection(set(column_labels))
 
         self.df.drop(columns=column_labels, inplace=True)
 
         reason_message = (
-            f", reason = {reason}" if reason is not None and len(features_removed) > 0 else ""
+            f", reason = {reason}"
+            if reason is not None and len(features_removed) > 0
+            else ""
         )
 
         if len(features_removed) > 0:
-            new_features = [feat for feat in self.features if feat not in features_removed]
-            self.features = new_features, f"Dropped columns ({column_labels}) {reason_message}"
+            new_features = [
+                feat for feat in self.features if feat not in features_removed
+            ]
+            self.features = (
+                new_features,
+                f"Dropped columns ({column_labels}) {reason_message}",
+            )
 
     def drop_rows(self, row_indices: pd.Index) -> None:
         """Drop rows inplace given a set of indices.
 
         Intelligently drop rows from the dataset (inplace). Updating of
         rows will not cause hash update as features are unchanged.
 
@@ -680,28 +711,22 @@
             in self.df[self._metadata.get("perturbation_column", None)]
         ):
             query_or_perturbation_name = (
                 f"{self.perturbation_column}=='{query_or_perturbation_name}'"
             )
         if groupby is None:
             self.df[self.features] = _perform_df_transform(
-                self.df,
-                self.df.query(query_or_perturbation_name),
-                self.features,
-                func,
+                self.df, self.df.query(query_or_perturbation_name), self.features, func
             )
         else:
             grouped_df_results = []
             for _, g in self.df.groupby(groupby):
                 grouped_df_results.append(
                     _perform_df_transform(
-                        g,
-                        query_or_perturbation_name,
-                        self.features,
-                        func,
+                        g, query_or_perturbation_name, self.features, func
                     )
                 )
             self.df = pd.concat(grouped_df_results)
 
         self.features = (
             self.features,
             f"Subtracted features of rows matching perturbation: {query_or_perturbation_name}, func={func}",
@@ -736,15 +761,17 @@
             grouped by for application of the transformation on a group-by group
             basis. This is very useful if neededing to subtract median DMSO
             perturbation features on a plate-by-plate basis, whereby the column
             containing plateIDs would be supplied.  Multiple column names may
             also be supplied.
         """
         self.subtract_func_results_on_features(
-            query_or_perturbation_name=query_or_perturbation_name, groupby=groupby, func="median"
+            query_or_perturbation_name=query_or_perturbation_name,
+            groupby=groupby,
+            func="median",
         )
 
     def subtract_mean(
         self, query_or_perturbation_name: str, groupby: Optional[Union[str, list[str]]]
     ) -> None:
         """Subtract the mean of rows identified in the query from features
 
@@ -772,43 +799,53 @@
             grouped by for application of the transformation on a group-by group
             basis. This is very useful if neededing to subtract mean DMSO
             perturbation features on a plate-by-plate basis, whereby the column
             containing plateIDs would be supplied.  Multiple column names may
             also be supplied.
         """
         self.subtract_func_results_on_features(
-            query_or_perturbation_name=query_or_perturbation_name, groupby=groupby, func="mean"
+            query_or_perturbation_name=query_or_perturbation_name,
+            groupby=groupby,
+            func="mean",
         )
 
     def divide_median(self, query: str) -> None:
         """Divide dataset features by the median of rows identified in the query
 
         Useful function for normalising to controls.
 
         Parameters
         ----------
         query : str
             Pandas style query to retrieve rows from which medians are
             calculated.
         """
-        self.df[self.features] = self.data / self.df.query(query)[self.features].median()
-        self.features = self.features, f"Divided by median of rows matching query: {query}"
+        self.df[self.features] = (
+            self.data / self.df.query(query)[self.features].median()
+        )
+        self.features = (
+            self.features,
+            f"Divided by median of rows matching query: {query}",
+        )
 
     def divide_mean(self, query: str) -> None:
         """Divide dataset features by the mean of rows identified in the query
 
         Useful function for normalising to controls.
 
         Parameters
         ----------
         query : str
             Pandas style query to retrieve rows from which means are calculated.
         """
         self.df[self.features] = self.data / self.df.query(query)[self.features].mean()
-        self.features = self.features, f"Divided by mean of rows matching query: {query}"
+        self.features = (
+            self.features,
+            f"Divided by mean of rows matching query: {query}",
+        )
 
     def distance_df(
         self,
         candidate_dataset: "Dataset",
         metric: Union[str, Callable] = "euclidean",
         return_best_n_indexes_and_score: Optional[int] = None,
         lower_is_better=True,
@@ -855,39 +892,41 @@
         if not all([f in candidate_dataset.features for f in self.features]):
             raise ValueError("Datasets do not share common features")
 
         dist_mat = cdist(self.data, candidate_dataset.df[self.features], metric=metric)
 
         if return_best_n_indexes_and_score is None:
             return pd.DataFrame(
-                data=dist_mat, index=self.df.index, columns=candidate_dataset.df.index.to_list()
+                data=dist_mat,
+                index=self.df.index,
+                columns=candidate_dataset.df.index.to_list(),
             )
 
         else:
             if lower_is_better:
                 top_n = list(
                     map(
                         lambda x: np.unravel_index(x, dist_mat.shape),
-                        np.argsort(dist_mat, axis=None)[:return_best_n_indexes_and_score],
+                        np.argsort(dist_mat, axis=None)[
+                            :return_best_n_indexes_and_score
+                        ],
                     )
                 )
             else:
                 top_n = list(
                     map(
                         lambda x: np.unravel_index(x, dist_mat.shape),
-                        np.argsort(dist_mat, axis=None)[-return_best_n_indexes_and_score:],
+                        np.argsort(dist_mat, axis=None)[
+                            -return_best_n_indexes_and_score:
+                        ],
                     )
                 )[::-1]
         return [(loc, dist_mat[loc[0], loc[1]]) for loc in top_n]
 
-    def get_ds_from_query(
-        self,
-        name: str,
-        query: str,
-    ):
+    def get_ds_from_query(self, name: str, query: str):
         """Make a new Dataset object from a pandas style query.
 
         Parameters
         ----------
         name : str
             Name of new dataset
         query : str
@@ -916,30 +955,34 @@
         tmp_hash_object = self.sha256.copy()
         self.sha256 = None
         new_ds = deepcopy(self)
         self.sha256 = tmp_hash_object
         new_ds.sha256 = self.sha256.copy()
         return new_ds
 
-    def filter_columns_with_prefix(self, column_prefix: Union[str, list], keep: bool = False):
+    def filter_columns_with_prefix(
+        self, column_prefix: Union[str, list], keep: bool = False
+    ):
         """Filter columns based on prefix
 
         Parameters
         ----------
         column_prefix : Union[str, list]
             Prefix for columns as a string, or alternatively, a list of string
             prefixes
         keep : bool, optional
             If true, only columns matching the prefix are kept, if false, these
             columns are removed, by default False
         """
         column_names = []
         if isinstance(column_prefix, list):
             column_prefix = tuple(column_prefix)
-        column_names = [c for c in self.df.columns.values if c.startswith(column_prefix)]
+        column_names = [
+            c for c in self.df.columns.values if c.startswith(column_prefix)
+        ]
         self.filter_columns(column_names, keep=keep)
 
     def filter_columns(self, column_names: list, keep=True, regex=False):
         """Filter dataframe columns
 
         Parameters
         ----------
@@ -949,15 +992,17 @@
             Keep columns listed in column_names, if false, then the opposite
             happens and these columns are removed, by default True.
         """
 
         if regex:
             new_column_names = []
             for pattern in column_names:
-                for match in list(filter(re.compile(pattern).match, self.df.columns.values)):
+                for match in list(
+                    filter(re.compile(pattern).match, self.df.columns.values)
+                ):
                     if match not in new_column_names:
                         new_column_names.append(match)
             column_names = new_column_names
 
         if len(column_names) == 0:
             return
         if keep:
@@ -975,15 +1020,17 @@
             if len(features_to_remove) > 0:
                 self.features = (
                     [f for f in self.features if f not in features_to_remove],
                     f"Features removed due to filtering of columns, columns removed were {column_names=}, which removed the following features {features_to_remove}",
                 )
             self.df = self.df.drop(column_names, axis=1)
 
-    def filter_rows(self, query_column: str, values: Union[list, str], keep: bool = True):
+    def filter_rows(
+        self, query_column: str, values: Union[list, str], keep: bool = True
+    ):
         """Filter dataframe rows
 
         Parameters
         ----------
         query_column : str
             Column name which is being filtered on
         values : Union[list, str]
@@ -1029,19 +1076,22 @@
             Dictionary of the form {'old_name':'new_name'}
         """
         self.df.rename(columns=from_to, inplace=True)
         if len(self._history) != 0:
             self.features = self.features, f"Renamed columns: {from_to}"
 
         # Renamed column might be a feature, if so, then rename the feature
-        from_to_in_features = {k_f: from_to[k_f] for k_f in from_to if k_f in self.features}
+        from_to_in_features = {
+            k_f: from_to[k_f] for k_f in from_to if k_f in self.features
+        }
         if len(from_to_in_features) > 0:
-            self.features = [
-                from_to_in_features.get(f, f) for f in self.features
-            ], "New features set by renaming columns ({from_to_dict})"
+            self.features = (
+                [from_to_in_features.get(f, f) for f in self.features],
+                "New features set by renaming columns ({from_to_dict})",
+            )
 
     def df_to_csv(self, output_path: Union[Path, str], **kwargs):
         """Write DataFrame to CSV
 
         Convenience function to write the underlying DataFrame to a CSV.  Additional
         arguments will be passed to the Pandas.DataFrame.to_csv function.
 
@@ -1097,15 +1147,17 @@
             splits = self.df[split_by_column].unique()
             for split in splits:
                 if split == np.nan:
                     continue
                 split_output_path = (
                     output_dir / f"{file_prefix}{split}{file_suffix}{file_extension}"
                 )
-                self.df.query(f"{split_by_column} == '{split}'").to_csv(split_output_path, **kwargs)
+                self.df.query(f"{split_by_column} == '{split}'").to_csv(
+                    split_output_path, **kwargs
+                )
 
     def add_well_id(
         self,
         numerical_column_name: str = "COLUMN",
         numerical_row_name: str = "ROW",
         plate_type: int = 384,
         new_well_column_name: str = "Well",
@@ -1151,45 +1203,49 @@
         if plate_type == 384:
             MAX_ROWS = 16
             MAX_COLUMNS = 24
             row_map = {n: chr(n + 64) for n in range(1, MAX_ROWS + 1)}
             column_map = {n: f"{n}".zfill(2) for n in range(1, MAX_COLUMNS + 1)}
 
         # Make sure to cast to a list, otherwise it is consumed upon use/iteration
-        all_possible_well_ids = list(itertools_product(row_map.keys(), column_map.keys()))
+        all_possible_well_ids = list(
+            itertools_product(row_map.keys(), column_map.keys())
+        )
         numerical_column = self.df[numerical_column_name].astype(int)
         numerical_row = self.df[numerical_row_name].astype(int)
         if numerical_column.max() > MAX_COLUMNS:
             raise DataError(
                 f"Column value {numerical_column.max()} is greater than maximum for {plate_type} well plate of {MAX_COLUMNS}"
             )
         if numerical_row.max() > MAX_ROWS:
             raise DataError(
                 f"Row value {numerical_row.max()} is greater than maximum for {plate_type} well plate of {MAX_ROWS}"
             )
 
-        self.df[new_well_column_name] = numerical_row.apply(lambda x: row_map[x]).astype(
-            str
-        ) + numerical_column.apply(lambda x: column_map[x]).astype(str)
+        self.df[new_well_column_name] = numerical_row.apply(
+            lambda x: row_map[x]
+        ).astype(str) + numerical_column.apply(lambda x: column_map[x]).astype(str)
 
         if add_empty_wells:
             if plate_barcode_column is None:
                 all_well_ids = list(zip(numerical_row, numerical_column))
-                missing_wells = list((set(all_possible_well_ids) - set(all_well_ids)))
+                missing_wells = list(set(all_possible_well_ids) - set(all_well_ids))
                 if len(missing_wells) > 0:
                     additional_data = pd.DataFrame.from_dict(
                         {
                             numerical_row_name: [w[0] for w in missing_wells],
                             numerical_column_name: [w[1] for w in missing_wells],
                             new_well_column_name: [
                                 row_map[w[0]] + column_map[w[1]] for w in missing_wells
                             ],
                         }
                     )
-                    self.df = pd.concat([self.df, additional_data], axis=0, ignore_index=True)
+                    self.df = pd.concat(
+                        [self.df, additional_data], axis=0, ignore_index=True
+                    )
                     if not no_sort:
                         self.df = self.df.sort_values([new_well_column_name])
             else:
                 for plate in self.df[plate_barcode_column].unique():
                     if plate is np.nan:
                         continue
                     plate_df = self.df.query(f"{plate_barcode_column} == '{plate}'")
@@ -1206,20 +1262,23 @@
 
                     if len(missing_wells) > 0:
                         additional_wells = pd.DataFrame.from_dict(
                             {
                                 numerical_row_name: [w[0] for w in missing_wells],
                                 numerical_column_name: [w[1] for w in missing_wells],
                                 new_well_column_name: [
-                                    row_map[w[0]] + column_map[w[1]] for w in missing_wells
+                                    row_map[w[0]] + column_map[w[1]]
+                                    for w in missing_wells
                                 ],
                                 plate_barcode_column: [w[2] for w in missing_wells],
                             }
                         )
-                        self.df = pd.concat([self.df, additional_wells], axis=0, ignore_index=True)
+                        self.df = pd.concat(
+                            [self.df, additional_wells], axis=0, ignore_index=True
+                        )
                         if not no_sort:
                             self.df = self.df.sort_values(
                                 [plate_barcode_column, new_well_column_name]
                             )
         self.features = (
             self.features,
             f"Added well IDs, {numerical_column_name=}, {numerical_row_name=}, {plate_type=}, {new_well_column_name}, {add_empty_wells=}, {plate_barcode_column=}, {no_sort=}",
@@ -1227,15 +1286,15 @@
 
     def subtract_median_perturbation(
         self,
         perturbation_label: str,
         per_column_name: Optional[str] = None,
         new_features_prefix: str = "SMP_",
     ):
-        """Subtract the median perturbation from all features
+        r"""Subtract the median perturbation from all features
 
         Useful for normalisation within a well/plate format. The median feature
         may be identified through the per_column_name variable, and perturbation
         label. Newly generated features may have their prefixes controled via
         the new_features_prefix argument.
 
         Parameters
@@ -1256,18 +1315,20 @@
             self.df[new_features] = self.data - self.df.median(axis=0)
         else:
             for unique_plate in self.df[per_column_name].unique():
                 medians = self.df.loc[
                     self.df[per_column_name] == unique_plate, self.features
                 ].median(axis=0)
                 self.df.loc[
-                    self.df[self.df[per_column_name] == unique_plate].index, new_features
+                    self.df[self.df[per_column_name] == unique_plate].index,
+                    new_features,
                 ] = (
                     self.df.loc[
-                        self.df[self.df[per_column_name] == unique_plate].index, self.features
+                        self.df[self.df[per_column_name] == unique_plate].index,
+                        self.features,
                     ]
                     - medians
                 ).values
         self.features = (
             new_features,
             f"Subtracted median perturbation {perturbation_label=}, {per_column_name=}",
         )
@@ -1343,15 +1404,17 @@
             Incorrect number of new column names given in new_columns.
         """
         if isinstance(column, int):
             column = self.df.columns.tolist()[column]
         pat_count = self.df[column].str.count("_").unique().tolist()
         if len(pat_count) != 1:
             different_count_indexes = [
-                self.df.loc[self.df.loc[self.df[column].str.count(pat) == c].index[0], column]
+                self.df.loc[
+                    self.df.loc[self.df[column].str.count(pat) == c].index[0], column
+                ]
                 for c in pat_count
             ]
 
             raise DataError(
                 f"Attempting to split {column} column on '{pat}', "
                 f"but column does not contain a consistent count of '{pat}',"
                 f" contained: {pat_count} instances, from {column} values such as:\n"
@@ -1365,20 +1428,66 @@
             )
 
         self.df[new_columns] = self.df[column].str.split(pat, expand=True)
 
     def pivot(self, feature_names_column: str, values_column: str):
         self.df = self.df.pivot_table(
             values=values_column,
-            index=[c for c in self.df.columns if c not in [feature_names_column, values_column]],
+            index=[
+                c
+                for c in self.df.columns
+                if c not in [feature_names_column, values_column]
+            ],
             columns=feature_names_column,
         )
         self.df.reset_index(inplace=True)
         self.df.columns.name = ""
 
+    def groupby(self, by: Union[str, List[str]]):
+        """Returns multiple new Dataset objects by splitting on columns
+
+        Akin to performing groupby on a pd.DataFrame, split a dataset on one or many
+        columns and return a list of Phenonaut Datasets containing the information
+        contained within each unique split.
+
+        Parameters
+        ----------
+        by : Union[str, list[str]]
+            If a string, then this is used as a column name upon which to group the
+            dataset and return unique classes based on this column.  A list of strings
+            is also allowed, enabling grouping of datasets by multiple columns, such as
+            ['timepoint', 'concentration']
+
+        Returns
+        -------
+        List[phenonaut.Dataset]
+            A list of new phenonaut.Dataset objects split on the value(s) of the by
+            argument
+        """
+        metadata = self._metadata
+        metadata["initial_features"] = self.features
+        if isinstance(by, str):
+            by = [by]
+        new_datasets = [
+            Dataset(
+                f"{self.name}_groupby_{','.join(by)}_{','.join([str(item) for item in index]) if not isinstance(index, str) else str(index)}",
+                df,
+                metadata=self._metadata,
+            )
+            for index, df in self.df.groupby(by)
+        ]
+        for ds in new_datasets:
+            ds.history.append(
+                TransformationHistory(
+                    ds.features,
+                    f"Dataset split with groupby on {by}, and taking value(s) {[ds.df[b].unique()[0] for b in by]}",
+                )
+            )
+        return new_datasets
+
     def new_aggregated_dataset(
         self,
         identifier_columns: list[str],
         new_dataset_name: str = "Merged rows dataset",
         transformation_lookup: dict[str, Union[Callable, str]] = None,
         tranformation_lookup_default_value: Union[str, Callable] = "mean",
     ):
@@ -1453,51 +1562,59 @@
                 np.dtype("O"): lambda x: ",".join([f"{item}" for item in set(x)])
             }
         dtypes_dict = {n: dt for n, dt in zip(self.df.columns, self.df.dtypes)}
         transforms = {
             c: transformation_lookup.get(dt, tranformation_lookup_default_value)
             for c, dt in zip(self.df.columns, self.df.dtypes)
         }
-        merged_df = self.df.copy().groupby(identifier_columns, as_index=False).aggregate(transforms)
+        merged_df = (
+            self.df.copy()
+            .groupby(identifier_columns, as_index=False)
+            .aggregate(transforms)
+        )
 
         for id_col_name in identifier_columns:
-            merged_df[id_col_name] = merged_df[id_col_name].astype(dtypes_dict[id_col_name])
+            merged_df[id_col_name] = merged_df[id_col_name].astype(
+                dtypes_dict[id_col_name]
+            )
         tmp_metadata = self._metadata.copy()
         if "features_prefix" in tmp_metadata:
             del tmp_metadata["features_prefix"]
         if "initial_features" in tmp_metadata:
             del tmp_metadata["initial_features"]
         tmp_metadata["features"] = self.features
 
         new_ds = Dataset(
-            dataset_name=new_dataset_name, input_file_path_or_df=merged_df, metadata=tmp_metadata
+            dataset_name=new_dataset_name,
+            input_file_path_or_df=merged_df,
+            metadata=tmp_metadata,
         )
         new_ds._history = self.get_history()
         new_ds.features = (
             self.features,
             f"Merged rows of the dataset, using columns {identifier_columns}",
         )
         return new_ds
 
-    def __update_hash(
-        self,
-    ):
+    def __update_hash(self):
         self.sha256.update(self.name.encode("utf-8"))
         self.sha256.update(
-            ";".join(f"{','.join(feat)}:{t_hist}" for feat, t_hist in self.get_history()).encode(
-                "utf-8"
-            )
+            ";".join(
+                f"{','.join(feat)}:{t_hist}" for feat, t_hist in self.get_history()
+            ).encode("utf-8")
         )
         self.sha256.update("".join(self._metadata).encode("utf-8"))
         self.sha256.update(",".join(self.features).encode("utf-8"))
         if self.df is not None:
             self.sha256.update(self.df.values.tobytes())
             self.sha256.update(self.df.columns.values.tobytes())
 
-    def remove_features_with_outliers(self, outlier_cutoff=15.0, remove_data: bool = False):
+    def remove_features_with_outliers(
+        self, outlier_cutoff=15.0, remove_data: bool = False
+    ):
         """Removes feature columns containing values greater than given cutoff
 
         By default, any feature containing a value greater than 15 is removed. This cutoff can
         be raised and lowered as appropriate.
 
         Parameters
         ----------
@@ -1511,15 +1628,16 @@
             changed. By default False.
         """
         outlier_features = self.data.columns[
             self.data.apply(lambda x: x.abs().max() >= outlier_cutoff)
         ].tolist()
         if remove_data:
             self.drop_columns(
-                outlier_features, reason=f"outlier feature columns, cutoff={outlier_cutoff}"
+                outlier_features,
+                reason=f"outlier feature columns, cutoff={outlier_cutoff}",
             )
         else:
             self.features = (
                 [f for f in self.features if f not in outlier_features],
                 f"Dropped columns ({outlier_features}) outlier feature columns, cutoff={outlier_cutoff}",
             )
 
@@ -1527,15 +1645,15 @@
         self,
         blocklist: Union[Path, str, list[str]],
         skip_first_line_in_file: bool = True,
         erase_data: bool = True,
         apply_to_non_features: bool = True,
         remove_prefixed: bool = True,
     ):
-        """Remove blocklisted features/columns from a Dataset
+        r"""Remove blocklisted features/columns from a Dataset
 
         Allows removal of predefined feature blocklists.  Featurisation may generate
         features which are to be excluded from analysis as standard. This is the case
         with cellular images featurised with cell profiler. As such, there are a set
         of blocklist feautures which are often applied. This function allows
         specification of a list of features for removal (in the form of a list),
         or a string or path object denoting the location of a file containing this
@@ -1591,60 +1709,67 @@
 
         if isinstance(blocklist, str):
             if blocklist == "CellProfiler":
                 import requests
 
                 blocklist = [
                     blf
-                    for blf in requests.get("https://figshare.com/ndownloader/files/23661539")
+                    for blf in requests.get(
+                        "https://figshare.com/ndownloader/files/23661539"
+                    )
                     .content.decode()
                     .split("\n")[1:]
                     if len(blf) > 1
                 ]
             else:
                 blocklist = Path(blocklist)
         if isinstance(blocklist, Path):
             if not blocklist.exists():
-                raise FileNotFoundError(f"Specified blocklist file {blocklist} does not exist")
+                raise FileNotFoundError(
+                    f"Specified blocklist file {blocklist} does not exist"
+                )
             with open(blocklist) as f:
                 blocklist = [line.rstrip() for line in f]
             if skip_first_line_in_file:
                 blocklist = blocklist[1:]
 
         if not erase_data:
             # Only removing features
             if remove_prefixed:
                 features_to_keep = [
                     f
                     for f in self.features
-                    if f not in blocklist and not any([f.endswith(f"_{b}") for b in blocklist])
+                    if f not in blocklist
+                    and not any([f.endswith(f"_{b}") for b in blocklist])
                 ]
             else:
                 features_to_keep = [f for f in self.features if f not in blocklist]
             self.features = (
                 features_to_keep,
                 f"Removed blocklist features ({list(set(self.features)-set(features_to_keep))})",
             )
             return
         else:
             if apply_to_non_features:
                 if remove_prefixed:
                     to_remove = [
                         c
                         for c in self.df.columns
-                        if c in blocklist or any([c.endswith(f"_{b}") for b in blocklist])
+                        if c in blocklist
+                        or any([c.endswith(f"_{b}") for b in blocklist])
                     ]
                 else:
                     to_remove = [c for c in self.df.columns if c in blocklist]
             else:
                 if remove_prefixed:
                     to_remove = [
                         f
                         for f in self.df.columns
-                        if f in blocklist or any([f.endswith(f"_{b}") for b in blocklist])
+                        if f in blocklist
+                        or any([f.endswith(f"_{b}") for b in blocklist])
                     ]
                 else:
                     to_remove = [f for f in self.df.columns if f in blocklist]
             self.filter_columns(to_remove, keep=False)
 
     def remove_low_variance_features(self, freq_cutoff=0.05, unique_cutoff=0.01):
         """Exclude low information content features.
@@ -1686,26 +1811,32 @@
 
         # Subset dataframe
 
         # Features containing massively overrepresented common values
         features_to_remove_freq = self.data.apply(
             lambda x: _violates_frequency_cutoff(x, freq_cutoff)
         )
-        features_to_remove_freq = features_to_remove_freq[features_to_remove_freq].index.tolist()
+        features_to_remove_freq = features_to_remove_freq[
+            features_to_remove_freq
+        ].index.tolist()
 
         # Features with values too common
         unique_ratio = self.data.nunique() / self.df.shape[0]
-        features_to_remove_unique = unique_ratio[unique_ratio < unique_cutoff].index.tolist()
+        features_to_remove_unique = unique_ratio[
+            unique_ratio < unique_cutoff
+        ].index.tolist()
 
         self.drop_columns(
             list(set(features_to_remove_freq + features_to_remove_unique)),
             reason=": filtered low variance features",
         )
 
-    def drop_nans_with_cutoff(self, axis: Optional[int] = None, nan_cutoff: float = 0.1) -> None:
+    def drop_nans_with_cutoff(
+        self, axis: Optional[int] = None, nan_cutoff: float = 0.1
+    ) -> None:
         """
         Drop rows or columns containing NaN or Inf values above a specified cutoff percentage.
 
         Parameters:
         -----------
         axis: Optional[int], default=None
             Axis along which to drop NaN or Inf values. If None, both rows and columns are dropped.
@@ -1777,15 +1908,17 @@
         group = group.replace([np.inf, -np.inf], np.nan)
 
         if groupby_col is None:
             imputed_group = impute_fn(group)
             self.df[self.features] = imputed_group
 
         else:
-            imputed_groups = group.groupby(groupby_col, group_keys=False).apply(impute_fn)
+            imputed_groups = group.groupby(groupby_col, group_keys=False).apply(
+                impute_fn
+            )
             self.df[self.features + groupby_col] = imputed_groups
 
         if groupby_col is not None:
             self.features = (
                 self.features,
                 f"Removed invalid entries by nan and inf handling on group column {groupby_col}",
             )
@@ -1816,9 +1949,11 @@
         tuple[pd.DataFrame, list[str], str]
             Tuple containing the Dataframe, a list of features and the
             perturbation column name.
         """
         return (
             self.df,
             self.features,
-            self._metadata.get("perturbation_column", None) if quiet else self.perturbation_column,
+            self._metadata.get("perturbation_column", None)
+            if quiet
+            else self.perturbation_column,
         )
```

### Comparing `phenonaut-1.3.4/phenonaut/data/platemap_querier.py` & `phenonaut-2.0.3/src/phenonaut/data/platemap_querier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
 from pathlib import Path
-import pandas as pd
 from typing import Union
+
 import numpy as np
+import pandas as pd
 
 
 class PlatemapQuerier:
     plate_to_cpd_to_well_dict = {}
     platemap_files = None
 
     def __init__(
         self,
         platemap_directory: Union[str, Path],
         platemap_csv_files: Union[list, str, Path] = None,
         plate_name_before_underscore_in_filename=True,
     ):
-
         self.platemap_files = []
         if platemap_directory is None:
             if platemap_csv_files is None:
                 raise FileNotFoundError("No platemaps given")
             if isinstance(platemap_csv_files, str):
                 platemap_csv_files = [Path(platemap_csv_files)]
             if isinstance(platemap_csv_files, Path):
@@ -40,30 +40,35 @@
                 raise FileNotFoundError(f"{platemap_directory} is not a directory")
             self.platemap_files = list(platemap_directory.glob("*.csv"))
 
         for csv_file in self.platemap_files:
             plate_name = csv_file.stem
             if plate_name_before_underscore_in_filename:
                 plate_name = plate_name.split("_")[0]
-            df = pd.read_csv(csv_file, index_col=0).rename(columns={"Unnamed: 0": "Column"})
+            df = pd.read_csv(csv_file, index_col=0).rename(
+                columns={"Unnamed: 0": "Column"}
+            )
             self.plate_to_cpd_to_well_dict[plate_name] = self._platemap_to_dict(df)
 
         if len(self.plate_to_cpd_to_well_dict.keys()) == 0:
             raise FileNotFoundError("No suitable platemaps found")
 
     def _platemap_to_dict(self, plate):
         d = {}
         for column_label, column in plate.iteritems():
             for row, val in enumerate(column):
                 if str(val) == "nan":
                     continue
                 if val not in d.keys():
                     d[val] = []
                 d[val].append(
-                    (plate.index.values[row], plate.columns.values[int(column_label) - 1])
+                    (
+                        plate.index.values[row],
+                        plate.columns.values[int(column_label) - 1],
+                    )
                 )
         return d
 
     def get_compound_locations(self, cpd, plates: Union[str, list] = None):
         locations = []
         if isinstance(plates, str):
             plates = [plates]
```

### Comparing `phenonaut-1.3.4/phenonaut/data/recipes.py` & `phenonaut-2.0.3/src/phenonaut/data/recipes.py`

 * *Files identical despite different names*

### Comparing `phenonaut-1.3.4/phenonaut/metrics/distances.py` & `phenonaut-2.0.3/src/phenonaut/metrics/distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from typing import List, Tuple, Union, Optional
+from typing import List, Optional, Tuple, Union
 
-from pandas.errors import DataError
-
-from phenonaut.data import Dataset, dataset
+import numpy as np
 import pandas as pd
-
-from scipy.spatial.distance import pdist, cdist, cityblock
+from pandas.errors import DataError
 from scipy.linalg import inv
-import numpy as np
 from scipy.spatial import distance
+from scipy.spatial.distance import cdist, cityblock, pdist
 from sklearn.covariance import EmpiricalCovariance, MinCovDet
 
+from phenonaut.data import Dataset, dataset
+
 
 def treatment_spread_euclidean(
     data: Dataset,
     perturbation_column: Optional[str] = None,
     perturbations: Optional[List[str]] = None,
 ) -> dict[str:float]:
     """Calculate the euclidean spreat of perturbation repeats
@@ -36,30 +35,36 @@
     """
     if perturbation_column is None and data.perturbation_column is None:
         raise DataError(
             "Dataset does not have a perturbation column set and none was supplied to treatment_spread_euclidean"
         )
     if perturbation_column is None:
         perturbation_column = data.perturbation_column
-    perturbations = data.get_unique_perturbations() if perturbations is None else perturbations
+    perturbations = (
+        data.get_unique_perturbations() if perturbations is None else perturbations
+    )
 
     return {
         t: np.sum(
-            pdist(dataset.df.query(f"{data.perturbation_column} == '{t}'")[data.features]),
+            pdist(
+                dataset.df.query(f"{data.perturbation_column} == '{t}'")[data.features]
+            ),
             axis=None,
         )
         for t in perturbations
     }
 
 
 def mahalanobis(
     point: Union[List[float], np.ndarray, pd.DataFrame],
     cloud: Union[List[List[float]], np.ndarray, pd.DataFrame],
     pvals: bool = False,
-    covariance: Union[np.ndarray, EmpiricalCovariance, MinCovDet, None] = EmpiricalCovariance(),
+    covariance: Union[
+        np.ndarray, EmpiricalCovariance, MinCovDet, None
+    ] = EmpiricalCovariance(),
 ):
     """Measure the Mahalanobis distance between a point and a cloud
 
     The Mahalanobis distance calculation is particularly sensitive to outliers,
     which results in large changes in covariance matrix calculation. For this
     reason, robust covarience estimators may be suppplied to the method. Whilst
     a common recomendation is to calculate the sqrt of the Mahalanobis distance,
@@ -119,15 +124,17 @@
         elif isinstance(covariance, np.ndarray):
             cov_mat = covariance
         else:
             raise ValueError(
                 f"cov argument should be one of np.ndarray, None, or a subclass of sklearn.covariance.EmpiricalCovariance, it was {type(covariance)}"
             )
         difference = point - np.mean(cloud, axis=0)
-        mahl_d = np.diag(np.dot(np.dot(difference, np.linalg.inv(cov_mat)), difference.T))
+        mahl_d = np.diag(
+            np.dot(np.dot(difference, np.linalg.inv(cov_mat)), difference.T)
+        )
     if len(mahl_d) == 1:
         mahl_d = mahl_d[0]
     if not pvals:
         return mahl_d
     else:
         from scipy.stats import chi2
```

### Comparing `phenonaut-1.3.4/phenonaut/metrics/measures.py` & `phenonaut-2.0.3/src/phenonaut/metrics/measures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from pandas import DataFrame
-from phenonaut.data import Dataset
+from typing import Optional, Union
+
 import numpy as np
-from typing import Union, Optional
+from pandas import DataFrame
 
+from phenonaut.data import Dataset
 from phenonaut.phenonaut import Phenonaut
 
 
 def _scalar_projection_and_rejection(a: np.ndarray, b: np.ndarray):
     """Return two scalar projection and rejection lists of a(s) onto b.
 
     Scalar projection and rejection calculated from:
@@ -203,15 +204,17 @@
         dataset.df.eval(
             f"{target_perturbation_column_name} == '{target_perturbation_column_value}'"
         ),
         dataset.features,
     ].median(axis=0)
 
     if median_target_phenotype.isnull().values.any():
-        raise ValueError(f"Target phenotype contained null values: {median_target_phenotype}")
+        raise ValueError(
+            f"Target phenotype contained null values: {median_target_phenotype}"
+        )
 
     # a is a point in phenotypic space - actually the entire dataframe as all is
     # calculated in one call.
     a = dataset.data
     # get scalar projection and rejection values.
     (
         scalar_projection_values,
@@ -352,38 +355,45 @@
     # If Dataset, then make df with just required features
     if isinstance(dataset, Dataset):
         if features is None:
             features = list(dataset.features)
         if target_feature in features:
             features.remove(target_feature)
         if target_feature not in dataset.df.columns:
-            raise ValueError("Given target_feature was not found in the supplied Dataset")
+            raise ValueError(
+                "Given target_feature was not found in the supplied Dataset"
+            )
         dataset = dataset.df[features + [target_feature]]
 
     elif isinstance(dataset, DataFrame):
         if features is None:
             raise ValueError(
                 "DataFrame provided to feature_correlation_to_target, but no features_list"
             )
         if target_feature not in dataset.columns:
-            raise ValueError("Given target_feature was not found in the supplied Dataset")
+            raise ValueError(
+                "Given target_feature was not found in the supplied Dataset"
+            )
         dataset = dataset[features + [target_feature]]
     else:
         raise TypeError(
             "dataset argument to feature_correlation_to_target was not of type Phenonaut, Dataset, or DataFrame"
         )
 
     coefs = {
         column_name: dataset[column_name].corr(dataset[target_feature], method=method)
         for column_name in features
     }
 
     if return_dataframe:
         return (
             DataFrame.from_dict(
-                {"index": coefs.keys(), f"correlation_to_{target_feature}": coefs.values()}
+                {
+                    "index": coefs.keys(),
+                    f"correlation_to_{target_feature}": coefs.values(),
+                }
             )
             .set_index("index")
             .sort_values(by=f"correlation_to_{target_feature}", ascending=False)
         )
     else:
         return coefs
```

### Comparing `phenonaut-1.3.4/phenonaut/metrics/non_ds_phenotypic_metrics.py` & `phenonaut-2.0.3/src/phenonaut/metrics/non_ds_phenotypic_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+from collections.abc import Callable
+from dataclasses import dataclass
+from typing import Optional, Tuple, Union
 
-
-from typing import Union, Callable, Tuple, Optional
-from scipy.spatial.distance import cityblock
 import numpy as np
+from scipy.spatial.distance import cityblock, cosine, euclidean
 from scipy.stats import rankdata, spearmanr
-from dataclasses import dataclass
-from scipy.spatial.distance import euclidean, cityblock, cosine
 
-def calc_zhang_scores(anchor:np.array, queries:np.array)->Union[float, np.ndarray]:
 
+def calc_zhang_scores(anchor: np.array, queries: np.array) -> Union[float, np.ndarray]:
     """Calculate Zhang scores between two np.ndarrays
 
     Implementation of the Zhang method for comparing L1000/CMAP signatures.
     Zhang, Shu-Dong, and Timothy W. Gant. "A simple and robust method for
     connecting small-molecule drugs using gene-expression signatures." BMC
     bioinformatics 9.1 (2008): 1-10.
     Implemented by Steven Shave, following above paper as a reference
@@ -30,203 +29,238 @@
     Returns
     -------
     Union[float, np.ndarray]
         If anchor and candidate array ndims are both 1, then a single float
         representing the Zhang score is returned. If one input array has ndims
         of  2 (and the other has ndims of 1), then a 1-D np.ndarray is
         returned. If both inputs are 2-D, then a 2D MxN array is returned, where
-        M is the 
+        M is the
 
 
-    """    
+    """
     if queries is None:
         queries = anchor
-    if anchor.ndim!=1:
-        if anchor.ndim==2:
-            multi_anchor_results=np.full((anchor.shape[0], queries.shape[0]), np.nan)
+    if anchor.ndim != 1:
+        if anchor.ndim == 2:
+            multi_anchor_results = np.full((anchor.shape[0], queries.shape[0]), np.nan)
             for i in range(anchor.shape[0]):
-                multi_anchor_results[i,:]=calc_zhang_scores(anchor[i],queries)
+                multi_anchor_results[i, :] = calc_zhang_scores(anchor[i], queries)
             return multi_anchor_results
         else:
-            raise ValueError(f"Anchor should be a 1D array, it had shape: {anchor.shape}")
-    anchor_profile=rankdata(np.abs(anchor), axis=-1)*np.sign(anchor)
-    if queries.ndim==1:
-        queries.reshape(1,-1)
-    if queries.shape[-1]!=anchor.shape[-1]:
-        raise ValueError(f"Different number of features found in anchor ({anchor.shape[-1]}) and queries ({queries.shape[-1]})")
-    query_profiles=rankdata(np.abs(queries), axis=-1)*np.sign(queries)
-    return np.sum(anchor_profile*query_profiles, axis=-1)/np.sum(anchor_profile**2, axis=-1)
-
-def calc_zhang_scores_all_v_all(anchor:np.array):
-    anchor=np.array(anchor)
-    if anchor.ndim==2:
-        multi_anchor_results=np.full((anchor.shape[0], anchor.shape[0]), np.nan)
-        query_profiles=rankdata(np.abs(anchor), axis=-1)*np.sign(anchor)
+            raise ValueError(
+                f"Anchor should be a 1D array, it had shape: {anchor.shape}"
+            )
+    anchor_profile = rankdata(np.abs(anchor), axis=-1) * np.sign(anchor)
+    if queries.ndim == 1:
+        queries.reshape(1, -1)
+    if queries.shape[-1] != anchor.shape[-1]:
+        raise ValueError(
+            f"Different number of features found in anchor ({anchor.shape[-1]}) and queries ({queries.shape[-1]})"
+        )
+    query_profiles = rankdata(np.abs(queries), axis=-1) * np.sign(queries)
+    return np.sum(anchor_profile * query_profiles, axis=-1) / np.sum(
+        anchor_profile**2, axis=-1
+    )
+
+
+def calc_zhang_scores_all_v_all(anchor: np.array):
+    anchor = np.array(anchor)
+    if anchor.ndim == 2:
+        multi_anchor_results = np.full((anchor.shape[0], anchor.shape[0]), np.nan)
+        query_profiles = rankdata(np.abs(anchor), axis=-1) * np.sign(anchor)
         for i in range(anchor.shape[0]):
-            anchor_profile=rankdata(np.abs(anchor[i]), axis=-1)*np.sign(anchor[i])
-            multi_anchor_results[i,:]=np.sum(anchor_profile*query_profiles, axis=-1)/np.sum(anchor_profile**2, axis=-1)
+            anchor_profile = rankdata(np.abs(anchor[i]), axis=-1) * np.sign(anchor[i])
+            multi_anchor_results[i, :] = np.sum(
+                anchor_profile * query_profiles, axis=-1
+            ) / np.sum(anchor_profile**2, axis=-1)
         return multi_anchor_results
     else:
         raise ValueError(f"Anchor should be a 2D array, it had shape: {anchor.shape}")
 
-def calc_spearmansrank_scores(anchor:np.array, queries:np.array)->Union[float, np.ndarray]:
+
+def calc_spearmansrank_scores(
+    anchor: np.array, queries: np.array
+) -> Union[float, np.ndarray]:
     # Standardise inputs to np arrays
-    anchor=np.array(anchor)
+    anchor = np.array(anchor)
     if queries is None:
         queries = np.array(anchor)
     else:
-        queries=np.array(queries)
-    
-    if anchor.ndim==1:
-        if queries.ndim==1:
+        queries = np.array(queries)
+
+    if anchor.ndim == 1:
+        if queries.ndim == 1:
             return spearmanr(anchor, queries).correlation
         else:
             return np.array([spearmanr(anchor, q).correlation for q in queries])
     else:
-        if anchor.ndim!=2:
+        if anchor.ndim != 2:
             raise ValueError("Anchor should be 1D or 2D, it was {anchor.ndim}D")
-        if queries.ndim==1:
-            queries=queries.reshape(1,-1)
-        results_array=np.empty((anchor.shape[0], queries.shape[0]))
+        if queries.ndim == 1:
+            queries = queries.reshape(1, -1)
+        results_array = np.empty((anchor.shape[0], queries.shape[0]))
 
         for i in range(anchor.shape[0]):
-            results_array[i]=np.array([spearmanr(anchor[i], q).correlation for q in queries])
+            results_array[i] = np.array(
+                [spearmanr(anchor[i], q).correlation for q in queries]
+            )
         return results_array
 
 
-def calc_connectivity_scores(anchor:np.array, queries:np.array)->Union[float, np.ndarray]:
+def calc_connectivity_scores(
+    anchor: np.array, queries: np.array
+) -> Union[float, np.ndarray]:
     # Standardise inputs to np arrays
-    anchor=np.array(anchor)
+    anchor = np.array(anchor)
     if queries is None:
         queries = np.array(anchor)
     else:
-        queries=np.array(queries)
+        queries = np.array(queries)
 
-    if anchor.ndim==1:
-        if queries.ndim==1:
-            return np.sum(np.sign(anchor)==np.sign(queries))/len(anchor)
+    if anchor.ndim == 1:
+        if queries.ndim == 1:
+            return np.sum(np.sign(anchor) == np.sign(queries)) / len(anchor)
         else:
-            return np.array([np.sum(np.sign(anchor)==np.sign(q))/len(anchor) for q in queries])
+            return np.array(
+                [np.sum(np.sign(anchor) == np.sign(q)) / len(anchor) for q in queries]
+            )
     else:
-        if anchor.ndim!=2:
+        if anchor.ndim != 2:
             raise ValueError("Anchor should be 1D or 2D, it was {anchor.ndim}D")
-        if queries.ndim==1:
-            queries=queries.reshape(1,-1)
-        results_array=np.empty((anchor.shape[0], queries.shape[0]))
+        if queries.ndim == 1:
+            queries = queries.reshape(1, -1)
+        results_array = np.empty((anchor.shape[0], queries.shape[0]))
 
         for i in range(anchor.shape[0]):
-            results_array[i]=np.array([np.sum(np.sign(anchor[i])==np.sign(q))/len(anchor[i]) for q in queries])
+            results_array[i] = np.array(
+                [
+                    np.sum(np.sign(anchor[i]) == np.sign(q)) / len(anchor[i])
+                    for q in queries
+                ]
+            )
         return results_array
 
+
 class PhenotypicMetric:
     """Metrics evaluate one profile/feature vector against another
-    
+
     SciPy and other libraries traditionally supply distance metrics, like
     Manhattan, Euclidean etc. These are typically unbound in their max value,
     but not always, for example; cosine distance with a maximum dissimilarity of
     1.  Scientific literature is also full of similarity metrics, where a high
     value indicates most similarity - the opposite of a similarity metric. This
     dataclass coerces metrics into a standard form, with .similarity and
     .distance functions to turn any metric into a similarity or distance metric.
-    
+
     This allows the definition of something like the Zhang similarity metric,
     which ranges from -1 to 1, indicating most dissimilarity and most similarity
     respectively. Calling the metric defined by this Zhang function will return
     the traditional Zhang metric value - ranging from -1 to 1.
 
     The methods similarity and distance will also be added
-    
+
     Calling distance will return a value between 0 and 1, with 0 being most
     similar and 1 being most dissimilar.
 
     Calling similarity will return a value between 0 and 1, with 1 being the
     most similar and 0 being the most different.
-    
+
     """
 
     def __init__(
         self,
         name: str,
         method: Union[Callable, str],
-        range:Tuple[float, float],
-        higher_is_better:bool=True,
-        ):
-        self.name=name
-        self.func=method
-        self.range=range
-        self.higher_is_better=higher_is_better
+        range: Tuple[float, float],
+        higher_is_better: bool = True,
+    ):
+        self.name = name
+        self.func = method
+        self.range = range
+        self.higher_is_better = higher_is_better
         if isinstance(self.func, str):
-            self.is_magic_string=True
+            self.is_magic_string = True
         else:
-            self.is_magic_string=False
+            self.is_magic_string = False
         if not any(np.isinf(self.range)):
-            self.scalable=True
+            self.scalable = True
         else:
-            self.scalable=False
+            self.scalable = False
 
     def __repr__(self) -> str:
         return self.name
+
     def __str__(self) -> str:
         return self.name
 
     def __call__(self, anchor, query):
-        anchor=np.array(anchor)
-        query=np.array(query)
-        if anchor.ndim!=1:
-            raise ValueError(f"Expected anchor to have 1 dimension, it had {anchor.ndim}")
-        if query.ndim==2:
+        anchor = np.array(anchor)
+        query = np.array(query)
+        if anchor.ndim != 1:
+            raise ValueError(
+                f"Expected anchor to have 1 dimension, it had {anchor.ndim}"
+            )
+        if query.ndim == 2:
             return np.array([self.__call__(anchor, row) for row in query])
         return self.func(anchor, query)
 
     def scale(self, score):
-        return (score-self.range[0])/(self.range[1]-self.range[0])
-
+        return (score - self.range[0]) / (self.range[1] - self.range[0])
 
     def distance(self, anchor, query):
-        score=self.__call__(anchor, query)
-        
+        score = self.__call__(anchor, query)
+
         if self.scalable:
-            score=self.scale(score)
+            score = self.scale(score)
             if self.higher_is_better:
-                return 1.0-score
+                return 1.0 - score
             return score
         else:
             if self.higher_is_better:
-                return 1.0/score
+                return 1.0 / score
             return score
 
     def similarity(self, anchor, query):
-        score=self.__call__(anchor, query)
+        score = self.__call__(anchor, query)
         if self.scalable:
-            score=self.scale(score)
+            score = self.scale(score)
             if self.higher_is_better:
                 return score
             else:
-                return 1-score
+                return 1 - score
         else:
             if self.higher_is_better:
                 return score
             else:
                 if isinstance(score, float):
-                    if score==0:
+                    if score == 0:
                         return 1
-                    return 1./score
-                return 1./np.clip(score, np.finfo(float).eps, None)
+                    return 1.0 / score
+                return 1.0 / np.clip(score, np.finfo(float).eps, None)
 
-non_ds_phenotypic_metrics={
-    'Connectivity':PhenotypicMetric('Connectivity',calc_connectivity_scores,(-1,1)),
-    'Rank':PhenotypicMetric('Rank',calc_spearmansrank_scores,(-1,1)),
-    'Zhang':PhenotypicMetric('Zhang',calc_zhang_scores,(-1,1)),
-    'Euclidean':PhenotypicMetric('Euclidean',euclidean,(0,np.inf), higher_is_better=False),
-    'Manhattan':PhenotypicMetric('Manhattan',cityblock,(0,np.inf), higher_is_better=False),
-    'Cosine': PhenotypicMetric('Cosine',cosine, (0,2), higher_is_better=False),
+
+non_ds_phenotypic_metrics = {
+    "Connectivity": PhenotypicMetric("Connectivity", calc_connectivity_scores, (-1, 1)),
+    "Rank": PhenotypicMetric("Rank", calc_spearmansrank_scores, (-1, 1)),
+    "Zhang": PhenotypicMetric("Zhang", calc_zhang_scores, (-1, 1)),
+    "Euclidean": PhenotypicMetric(
+        "Euclidean", euclidean, (0, np.inf), higher_is_better=False
+    ),
+    "Manhattan": PhenotypicMetric(
+        "Manhattan", cityblock, (0, np.inf), higher_is_better=False
+    ),
+    "Cosine": PhenotypicMetric("Cosine", cosine, (0, 2), higher_is_better=False),
 }
 
 # Metrics with magic values - magic values referrs to the fast methods which  scipy's pdist/cidist use
-metrics_with_magic_values={
-    'Rank':PhenotypicMetric('Rank','spearman',(-1,1)),
-    'Euclidean':PhenotypicMetric('Euclidean','euclidean',(0,np.inf), higher_is_better=False),
-    'Manhattan':PhenotypicMetric('Manhattan','cityblock',(0,np.inf), higher_is_better=False),
-    'Cosine':PhenotypicMetric('Cosine', 'cosine', (0,2), higher_is_better=False),
-    'Connectivity':PhenotypicMetric('Connectivity',calc_connectivity_scores,(-1,1)),
-    'Zhang':PhenotypicMetric('Zhang',calc_zhang_scores,(-1,1)),
-}
+metrics_with_magic_values = {
+    "Rank": PhenotypicMetric("Rank", "spearman", (-1, 1)),
+    "Euclidean": PhenotypicMetric(
+        "Euclidean", "euclidean", (0, np.inf), higher_is_better=False
+    ),
+    "Manhattan": PhenotypicMetric(
+        "Manhattan", "cityblock", (0, np.inf), higher_is_better=False
+    ),
+    "Cosine": PhenotypicMetric("Cosine", "cosine", (0, 2), higher_is_better=False),
+    "Connectivity": PhenotypicMetric("Connectivity", calc_connectivity_scores, (-1, 1)),
+    "Zhang": PhenotypicMetric("Zhang", calc_zhang_scores, (-1, 1)),
+}
```

### Comparing `phenonaut-1.3.4/phenonaut/metrics/performance.py` & `phenonaut-2.0.3/src/phenonaut/metrics/performance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,46 @@
+import json
+from collections import namedtuple
+from collections.abc import Callable
+from pathlib import Path
+from random import choice, choices, sample
+from timeit import default_timer as timer
+from typing import Optional, Union, List
+from scipy.spatial.distance import mahalanobis
 import numpy as np
 import pandas as pd
-from phenonaut.data import Dataset
-from phenonaut import Phenonaut
-from typing import Optional, Union, Callable
-import numpy as np
-from random import sample, choice, choices
-from scipy.spatial.distance import pdist
 from joblib import Parallel, delayed
-from progressbar import progressbar
-from pathlib import Path
-from collections import namedtuple
-import json
-from phenonaut.metrics.non_ds_phenotypic_metrics import PhenotypicMetric
+import multiprocessing as mp
+from tqdm import tqdm
+from scipy.spatial.distance import pdist
 from sklearn.metrics import silhouette_score as sklearn_silhouette_score
-from timeit import default_timer as timer
+from scipy import linalg
+from phenonaut import Phenonaut
+from ..errors import NotEnoughRowsError
+from phenonaut.data import Dataset
+from phenonaut.metrics.non_ds_phenotypic_metrics import PhenotypicMetric
+from sklearn.decomposition import PCA
+
 
 _ReplicateData = namedtuple(
     "_ReplicateData",
-    ["index", "cardinality", "matching_median_dist", "null_nth_percentile_or_null_distribution"],
+    [
+        "index",
+        "cardinality",
+        "matching_median_dist",
+        "null_nth_percentile_or_null_distribution",
+        "replicate_all_to_all_distances",
+    ],
+    defaults=[np.nan],
 )
 
 
-def _check_performance_path_and_gen_if_needed(filename, args_dict: dict, prefix:str) -> Path:
+def _check_performance_path_and_gen_if_needed(
+    filename, args_dict: dict, prefix: str
+) -> Path:
     """Private function, check target performance_path
 
     It could be a directory, in which case, generate a suitable filename
     from args_dict.  If a file, then just return it.  If a bool, then
     generate a suitable filename.
 
     Parameters
@@ -104,15 +119,17 @@
     replicate_query: Optional[str] = None,
     null_query_or_df: Optional[Union[str, pd.DataFrame]] = None,
     similarity_metric: Union[str, Callable] = "spearman",
     n_iters: int = 1000,
     min_cardinality: int = 2,
     max_cardinality: int = 50,
     return_full_profiles: bool = False,
+    include_replicate_pairwise_distances_in_df: bool = False,
     percentile_cutoff: int = 95,
+    random_state: Union[int, np.random.Generator] = 42,
 ):
     """Private function to obtain replicating info for a single treatment
 
     Parameters
     ----------
     df : pd.DataFrame
         Input pd.DataFrame
@@ -157,64 +174,81 @@
         finding pairwise all-to-all distances of non-matching compounds, this
         argument allows setting an upper bound cutoff after which, the repeats
         are shuffled and max_cardinality samples drawn to create a synthetic set of
         max_cardinality repeats. This is very useful when using a demanding similarity
         method as it cuts the evaluations dramatically. By default 50.
     return_full_profiles : bool, optional
         Instead of a percentile cutoff value, return the full null distribution, by default False.
+    include_replicate_pairwise_distances_in_df : bool
+        If True, then pairwise replicate distances are included in the full performance dataframe.
+        Has no effect if return_full_performance_df is False
     percentile_cutoff : int
         Percentile of the null distribution over which the matching replicates must score to be
         considered replicating. Should range from 0 to 100. By default 95.
-
+    random_state : Union[int, np.random.Generator]
+        Random state which should be used when performing sampling operations. Can be a
+        np.random.Generator, or an int (in which case, a np.random.Generator) is
+        instantiated with it.  If attempting reproducible results, run without parallelisation by
+        settiung the use_joblib_parallelisation argument to False, by default 42
     Returns
     -------
     _ReplicateData
         Named tuple containing information on the replicate performance of the tuple.
         If return_full_profiles is True, then named tuples contain the full null
-        distribution, if False, then just np.nan in this position.
+        distribution, if False, then just np.nan in this position. Additionally, if
+        include_replicate_pairwise_distances_in_df is True, then replicate pairwise
+        distances are included, if False then this property is np.nan.
         _ReplicateData has the following fields:
         - index (multiindex identifier - eg a tuple of compoundID and dose
         - cardinality - number of repeats included in calculation
         - matching_median_dist - median all to all score of the replicates
         - null_nth_percentile_or_null_distribution - Nth percentile cutoff of
             the null distribution or if requested (return_full_profiles = True),
             the full null distribution.
+        - replicate_all_to_all_distances - if requested, then an array of replicate
+            pairwise distances is present here, otherwise np.nan
     """
+    np_rng = np.random.default_rng(random_state)
 
     matching_multiindex, matching_indices = g_indices
     replicate_frame = df.iloc[matching_indices]
 
     # Early exit if required, before further checks
     if len(matching_indices) < 2 or len(matching_indices) < min_cardinality:
-        return _ReplicateData(matching_multiindex, len(matching_indices), np.nan, np.nan)
+        return _ReplicateData(
+            matching_multiindex, len(matching_indices), np.nan, np.nan
+        )
 
     if replicate_query is not None:
         replicate_frame = replicate_frame.query(replicate_query)
 
     # If replicate_criteria_not contains fields not to match on, then we must regenerate 'matching_indices'
     if len(replicate_criteria_not) > 0:
         matching_indices = [
-            choice(nmi)
+            np_rng.choice(nmi)
             for nmi in [
-                i_idx for i_idx in replicate_frame.groupby(replicate_criteria_not).indices.values()
+                i_idx
+                for i_idx in replicate_frame.groupby(
+                    replicate_criteria_not
+                ).indices.values()
             ]
         ]
         replicate_frame = replicate_frame.iloc[matching_indices]
 
     cardinality = replicate_frame.shape[0]
     # If only 1 compound, then it is not replicating
     if cardinality == 1:
         return _ReplicateData(matching_multiindex, cardinality, np.nan, np.nan)
     # If less than required cardinality, then return as non-replicating
     if cardinality < min_cardinality:
         return _ReplicateData(matching_multiindex, cardinality, np.nan, np.nan)
 
     # If matching cardinality is > max_cardinality, then resample to max_cardinality
     if cardinality > max_cardinality:
-        replicate_frame = replicate_frame.sample(n=max_cardinality)
+        replicate_frame = replicate_frame.sample(n=max_cardinality, random_state=np_rng)
         cardinality = max_cardinality
 
     if cardinality < 2:
         return _ReplicateData(matching_multiindex, cardinality, np.nan, np.nan)
 
     # Compose query for selecting null distribution. This can be as simple as
     # not equal to the same compound/pert_id as the matched compound, or include
@@ -249,48 +283,59 @@
     # generate a dictionary (pert_name_to_idx_dict), allowing mapping from pert_name
     # to indexes (0 -indexed np array)
     null_pert_names = null_df[replicate_criteria[0]]
     pert_name_to_idx_dict = {pname: [] for pname in null_pert_names.unique()}
     for i, pert_name in enumerate(null_pert_names):
         pert_name_to_idx_dict[pert_name].append(i)
     if len(pert_name_to_idx_dict) < 2 or len(pert_name_to_idx_dict) < min_cardinality:
-        return _ReplicateData(matching_multiindex, len(matching_indices), np.nan, np.nan)
+        return _ReplicateData(
+            matching_multiindex, len(matching_indices), np.nan, np.nan
+        )
 
     if cardinality > len(pert_name_to_idx_dict):
         print(
-            f"Number of unique non-matching compounds ({len(pert_name_to_idx_dict)}) was less than the number of repeats ({cardinality}) for {matching_multiindex}, running with a reduced cardinality of {len(pert_name_to_idx_dict)}"
+            f"Number of unique non-matching compounds ({len(pert_name_to_idx_dict)})"
+            f" was less than the number of repeats ({cardinality}) for"
+            f" {matching_multiindex}, running with a reduced cardinality of"
+            f" {len(pert_name_to_idx_dict)}"
         )
         cardinality = len(pert_name_to_idx_dict)
-        replicate_frame = replicate_frame.sample(n=cardinality)
+        replicate_frame = replicate_frame.sample(n=cardinality, random_state=np_rng)
 
     # Calculate matched repeat score
     if similarity_metric == "spearman":
-        matching_median_dist = np.median(
-            np.corrcoef(np.argsort(np.argsort(replicate_frame[features].values)))[
-                np.triu_indices(cardinality, k=1)
-            ]
-        )
+        replicate_scores = np.corrcoef(
+            np.argsort(np.argsort(replicate_frame[features].values))
+        )[np.triu_indices(cardinality, k=1)]
+        matching_median_dist = np.median(replicate_scores)
     else:
-        matching_median_dist = np.median(
-            pdist(replicate_frame[features].values, metric=similarity_metric)
+        replicate_scores = pdist(
+            replicate_frame[features].values, metric=similarity_metric
         )
+        matching_median_dist = np.median(replicate_scores)
 
     # If c is cardinality, choose c non-matching compounds. For each c, choose a
     # random repeat index r. Compose list of length n_iters x c.
     indices = [
-        choice(pert_name_to_idx_dict[cpd])
+        np_rng.choice(pert_name_to_idx_dict[cpd])
         for _ in range(n_iters)
-        for cpd in sample(list(pert_name_to_idx_dict.keys()), cardinality)
+        for cpd in np_rng.choice(
+            list(pert_name_to_idx_dict.keys()), cardinality, replace=False
+        )
     ]
 
     if len(indices) < 2:
-        return _ReplicateData(matching_multiindex, len(matching_indices), np.nan, np.nan)
+        return _ReplicateData(
+            matching_multiindex, len(matching_indices), np.nan, np.nan
+        )
 
     # Extract the profiles then reahape to a 3D array n_iters x cardinality x features
-    profiles = null_df[features].values[indices].reshape(n_iters, cardinality, len(features))
+    profiles = (
+        null_df[features].values[indices].reshape(n_iters, cardinality, len(features))
+    )
 
     # Calculate the null distribution
     if similarity_metric == "spearman":
         null_distribution = np.array(
             [
                 np.median(
                     np.corrcoef(np.argsort(np.argsort(profiles[p])))[
@@ -298,24 +343,28 @@
                     ]
                 )
                 for p in range(n_iters)
             ]
         )
     else:
         null_distribution = np.array(
-            [np.median(pdist(profiles[p], metric=similarity_metric)) for p in range(n_iters)]
+            [
+                np.median(pdist(profiles[p], metric=similarity_metric))
+                for p in range(n_iters)
+            ]
         )
-
+    # print(include_replicate_pairwise_distances_in_df)
     return _ReplicateData(
         matching_multiindex,
         cardinality,
         matching_median_dist,
         null_distribution
         if return_full_profiles
         else np.percentile(null_distribution, float(percentile_cutoff)),
+        replicate_scores if include_replicate_pairwise_distances_in_df else np.nan,
     )
 
 
 def _inspect_compact(
     df: pd.DataFrame,
     features: list[str],
     g_indices: list[int],
@@ -403,25 +452,30 @@
     """
 
     matching_multiindex, matching_indices = g_indices
     replicate_frame = df.iloc[matching_indices]
 
     # Early exit if required, before further checks
     if len(matching_indices) < 2 or len(matching_indices) < min_cardinality:
-        return _ReplicateData(matching_multiindex, len(matching_indices), np.nan, np.nan)
+        return _ReplicateData(
+            matching_multiindex, len(matching_indices), np.nan, np.nan
+        )
 
     if replicate_query is not None:
         replicate_frame = replicate_frame.query(replicate_query)
 
     # If replicate_criteria_not contains fields not to match on, then we must regenerate 'matching_indices'
     if len(replicate_criteria_not) > 0:
         matching_indices = [
             choice(nmi)
             for nmi in [
-                i_idx for i_idx in replicate_frame.groupby(replicate_criteria_not).indices.values()
+                i_idx
+                for i_idx in replicate_frame.groupby(
+                    replicate_criteria_not
+                ).indices.values()
             ]
         ]
         replicate_frame = replicate_frame.iloc[matching_indices]
 
     cardinality = replicate_frame.shape[0]
     # If only 1 compound, then it is not replicating
     if cardinality == 1:
@@ -457,66 +511,67 @@
         for gbn in null_criteria_not:
             tmp_val = tmp_matched_cpd_row[gbn]
             if isinstance(tmp_val, (float, int)):
                 null_criteria_query_list.append(f"{gbn}!={tmp_val}")
             else:
                 null_criteria_query_list.append(f"{gbn}!='{tmp_val}'")
 
-    if len(null_criteria_query_list)>0:
+    if len(null_criteria_query_list) > 0:
         null_df = df.query(" and ".join(null_criteria_query_list))
     else:
         null_df = df
 
     if isinstance(null_query_or_df, pd.DataFrame):
-        if len(null_criteria_query_list)==0:
+        if len(null_criteria_query_list) == 0:
             null_df = null_query_or_df
         else:
             null_df = null_query_or_df.query(" and ".join(null_criteria_query_list))
     elif isinstance(null_query_or_df, str):
-        if len(null_criteria_query_list)==0:
+        if len(null_criteria_query_list) == 0:
             null_df = df.query(null_query_or_df)
         else:
-            null_df = df.query(" and ".join(null_criteria_query_list)).query(null_query_or_df)
+            null_df = df.query(" and ".join(null_criteria_query_list)).query(
+                null_query_or_df
+            )
     else:
-        if len(null_criteria_query_list)>0:
+        if len(null_criteria_query_list) > 0:
             null_df = df.query(" and ".join(null_criteria_query_list))
         else:
             null_df = df
 
-
     # generate a dictionary (pert_name_to_idx_dict), allowing mapping from pert_name
     # to indexes (0 -indexed np array)
     null_pert_names = null_df[replicate_criteria[0]]
     pert_name_to_idx_dict = {pname: [] for pname in null_pert_names.unique()}
 
-
     # Calculate matched repeat score
     if similarity_metric == "spearman":
         matching_median_dist = np.median(
             np.corrcoef(np.argsort(np.argsort(replicate_frame[features].values)))[
                 np.triu_indices(cardinality, k=1)
             ]
         )
     else:
         matching_median_dist = np.median(
             pdist(replicate_frame[features].values, metric=similarity_metric)
         )
 
     # If c is cardinality, choose c non-matching compounds. For each c, choose a
     # random repeat index r. Compose list of length n_iters x c.
-    indices = [
-        choices(range(null_df.shape[0]), k=cardinality)
-        for _ in range(n_iters)
-    ]
+    indices = [choices(range(null_df.shape[0]), k=cardinality) for _ in range(n_iters)]
 
     if len(indices) < 2:
-        return _ReplicateData(matching_multiindex, len(matching_indices), np.nan, np.nan)
+        return _ReplicateData(
+            matching_multiindex, len(matching_indices), np.nan, np.nan
+        )
 
     # Extract the profiles then reahape to a 3D array n_iters x cardinality x features
-    profiles = null_df[features].values[indices].reshape(n_iters, cardinality, len(features))
+    profiles = (
+        null_df[features].values[indices].reshape(n_iters, cardinality, len(features))
+    )
 
     # Calculate the null distribution
     if similarity_metric == "spearman":
         null_distribution = np.array(
             [
                 np.median(
                     np.corrcoef(np.argsort(np.argsort(profiles[p])))[
@@ -524,15 +579,18 @@
                     ]
                 )
                 for p in range(n_iters)
             ]
         )
     else:
         null_distribution = np.array(
-            [np.median(pdist(profiles[p], metric=similarity_metric)) for p in range(n_iters)]
+            [
+                np.median(pdist(profiles[p], metric=similarity_metric))
+                for p in range(n_iters)
+            ]
         )
 
     return _ReplicateData(
         matching_multiindex,
         cardinality,
         matching_median_dist,
         null_distribution
@@ -574,47 +632,58 @@
     -------
     tuple[pd.DataFrame, list[str], Union[str, Callable], list[str], list[str]]
         Tuple containing the required DataFrame, features, similarity_metric,
         replicate_criteria, null_criteria, and null_criteria_not.
 
     """
     if isinstance(ds, (Phenonaut, Dataset)):
-        df, features, ret_pert_column = ds.get_df_features_perturbation_column(quiet=True)
+        df, features, ret_pert_column = ds.get_df_features_perturbation_column(
+            quiet=True
+        )
         if ret_pert_column is not None and perturbation_column is None:
             perturbation_column = ret_pert_column
         if perturbation_column is None:
             raise ValueError(
-                "No perturbation column found in Dataset, and the purturbation_column argument was None. Please pass it as an argument, or set on the Dataset - e.g.: ds.perturbation_column='pert_iname'"
+                "No perturbation column found in Dataset, and the purturbation_column"
+                " argument was None. Please pass it as an argument, or set on the"
+                " Dataset - e.g.: ds.perturbation_column='pert_iname'"
             )
     elif isinstance(ds, pd.DataFrame):
         if features is None:
             raise ValueError("Must supply features if operating on a raw pd.DataFrame")
         df = ds
         if perturbation_column is None:
             raise ValueError(
-                "No perturbation column set. Purturbation_column argument was None, and it is not discoverable from a pd.DataFrame. Please pass it as an argument"
+                "No perturbation column set. Purturbation_column argument was None, and"
+                " it is not discoverable from a pd.DataFrame. Please pass it as an"
+                " argument"
             )
     else:
         raise ValueError(
-            f"ds must be a Phenonaut object, a phenonaut.Dataset or a pd.DataFrame, it was {type(ds)}"
+            "ds must be a Phenonaut object, a phenonaut.Dataset or a pd.DataFrame, it"
+            f" was {type(ds)}"
         )
     replicate_criteria = [] if replicate_criteria is None else replicate_criteria
     replicate_criteria = (
-        [replicate_criteria] if isinstance(replicate_criteria, str) else replicate_criteria
+        [replicate_criteria]
+        if isinstance(replicate_criteria, str)
+        else replicate_criteria
     )
     replicate_criteria = (
         [perturbation_column] + replicate_criteria
         if perturbation_column not in replicate_criteria
         else replicate_criteria
     )
 
     null_criteria = [] if null_criteria is None else null_criteria
     null_criteria = [null_criteria] if isinstance(null_criteria, str) else null_criteria
 
-    replicate_criteria_not = [] if replicate_criteria_not is None else replicate_criteria_not
+    replicate_criteria_not = (
+        [] if replicate_criteria_not is None else replicate_criteria_not
+    )
     replicate_criteria_not = (
         [replicate_criteria_not]
         if isinstance(replicate_criteria_not, str)
         else replicate_criteria_not
     )
 
     null_criteria_not = [] if null_criteria_not is None else null_criteria_not
@@ -646,20 +715,22 @@
     n_iters: int = 1000,
     similarity_metric: Union[str, Callable] = "spearman",
     similarity_metric_higher_is_better: bool = True,
     min_cardinality: int = 2,
     max_cardinality: int = 50,
     include_cardinality_violating_compounds_in_calculation: bool = False,
     return_full_performance_df: bool = False,
+    include_replicate_pairwise_distances_in_df: bool = False,
     additional_captured_params: Optional[dict] = None,
     similarity_metric_name: Optional[str] = None,
     performance_df_file: Optional[Union[str, Path]] = None,
-    percentile_cutoff:Optional[int] = None,
+    percentile_cutoff: Optional[int] = None,
     use_joblib_parallelisation: bool = True,
     n_jobs: int = -1,
+    random_state: Union[int, np.random.Generator] = 42,
 ):
     """Calculate percent replicating
 
     Percent replicating is defined by Way et. al. in:
     Way, Gregory P., et al. "Morphology and gene expression profiling provide complementary
     information for mapping cell state." Cell systems 13.11 (2022): 911-923.
     or on bioRxiv:
@@ -796,14 +867,17 @@
         by min_cardinality (and are therefore deemed not replicating) are included in the final
         reported percent replicating statistics. If False, then they are not included as
         non-replicating and simply ignored as if they were not present in the dataset. By default
         False.
     return_full_performance_df : bool
         If True, then a tuple is returned with the percent replicating score in the first position,
         and a pd.DataFrame containing full information on each repeat. By default False
+    include_replicate_pairwise_distances_in_df : bool
+        If True, then pairwise replicate distances are included in the full performance dataframe.
+        Has no effect if return_full_performance_df is False
     performance_df_file : Optional[Union[str, Path, bool]]
         If return_full_performance_df is True and a Path or str is given as an argument to this
         parameter, then the performance DataFrame is written out to a CSV file using this filename.
         If True is passed here, then the a filename will be constructed from function arguments,
         attempting to capture the run details. If an auto-generated file with this name exists,
         then an error is raised and no calculations are performed. In addition to the output CSV,
         a json file is also written capturing arguments that the function was called with. So if
@@ -828,32 +902,48 @@
         similarity_metric_higher_is_better==False. By default None.
     use_joblib_parallelisation : bool
         If True, then use joblib to parallelise evaluation of compounds. By default True.
     n_jobs : int, optional
         The n_jobs argument is passed to joblib for parallel execution and defines the number of
         threads to use.  A value of -1 denotes that the system should determine how many jobs to run.
         By default -1.
+    random_state : Union[int, np.random.Generator]
+        Random state which should be used when performing sampling operations. Can be a
+        np.random.Generator, or an int (in which case, a np.random.Generator) is
+        instantiated with it.  If attempting reproducible results, run without parallelisation by
+        settiung the use_joblib_parallelisation argument to False, by default 42
 
     Returns
     -------
     Union[float, tuple[float, pd.DataFrame]]
         If return_full_performance_df is False, then only the percent replicating is returned.
         If True, then a tuple is returned, with percent replicating in the first position, and a
         pd.DataFrame in the second position containing the median repeat scores, as well as median
         null distribution scores in an easy to analyse format.
 
     """
+
+    if isinstance(random_state, int):
+        random_state = np.random.default_rng(random_state)
+    if not isinstance(random_state, np.random.Generator):
+        raise ValueError(
+            "random_state should be an int or a np.random.Generator, it was"
+            f" {type(random_state)}"
+        )
     start_time = timer()
     if max_cardinality < min_cardinality:
         raise ValueError(
-            f"Error, max_cardinality ({max_cardinality}) may not be less than min_cardinality ({min_cardinality})"
+            f"Error, max_cardinality ({max_cardinality}) may not be less than"
+            f" min_cardinality ({min_cardinality})"
         )
-    if percentile_cutoff is not None and percentile_cutoff < 1 :
+    if percentile_cutoff is not None and percentile_cutoff < 1:
         print(
-            "WARNING: percentile_cutoff < 1. For the 95th percentile, this should be 95, not 0.95. This function calls np.percentile, which behaves the same, expecting a number between 0 and 100 to specify the cutoff."
+            "WARNING: percentile_cutoff < 1. For the 95th percentile, this should be"
+            " 95, not 0.95. This function calls np.percentile, which behaves the same,"
+            " expecting a number between 0 and 100 to specify the cutoff."
         )
     (
         df,
         features,
         replicate_criteria,
         null_criteria,
         replicate_criteria_not,
@@ -878,28 +968,35 @@
         }
         if similarity_metric in special_similarity_metrics_higher_better_lookup:
             if (
                 special_similarity_metrics_higher_better_lookup[similarity_metric]
                 != similarity_metric_higher_is_better
             ):
                 print(
-                    f"Warning, special similarity metric value {similarity_metric} passed with similarity_metric_higher_is_better = {similarity_metric_higher_is_better}, changing similarity_metric_higher_is_better to {special_similarity_metrics_higher_better_lookup[similarity_metric]}"
+                    "Warning, special similarity metric value"
+                    f" {similarity_metric} passed with"
+                    " similarity_metric_higher_is_better ="
+                    f" {similarity_metric_higher_is_better}, changing"
+                    " similarity_metric_higher_is_better to"
+                    f" {special_similarity_metrics_higher_better_lookup[similarity_metric]}"
+                )
+                similarity_metric_higher_is_better = (
+                    not similarity_metric_higher_is_better
                 )
-                similarity_metric_higher_is_better = not similarity_metric_higher_is_better
         if similarity_metric_name is None:
             similarity_metric_name = similarity_metric
 
     if isinstance(similarity_metric, PhenotypicMetric):
         similarity_metric_higher_is_better = similarity_metric.higher_is_better
         similarity_metric_name = similarity_metric.name
         if similarity_metric.is_magic_string:
             similarity_metric = similarity_metric.func
 
     if percentile_cutoff is None:
-        percentile_cutoff=95 if similarity_metric_higher_is_better else 5
+        percentile_cutoff = 95 if similarity_metric_higher_is_better else 5
 
     inspect_replicating_additional_args = {
         "df": df,
         "features": features,
         "replicate_query": replicate_query,
         "replicate_criteria": replicate_criteria,
         "replicate_criteria_not": replicate_criteria_not,
@@ -907,21 +1004,25 @@
         "null_criteria": null_criteria,
         "null_criteria_not": null_criteria_not,
         "similarity_metric": similarity_metric,
         "n_iters": n_iters,
         "min_cardinality": min_cardinality,
         "max_cardinality": max_cardinality,
         "return_full_profiles": return_full_performance_df,
+        "include_replicate_pairwise_distances_in_df": include_replicate_pairwise_distances_in_df,
         "percentile_cutoff": percentile_cutoff,
+        "random_state": random_state,
     }
 
     df_groupby_indices_and_items = (
         df.groupby(replicate_criteria).indices.items()
         if restrict_evaluation_query is None
-        else df.query(restrict_evaluation_query).groupby(replicate_criteria).indices.items()
+        else df.query(restrict_evaluation_query)
+        .groupby(replicate_criteria)
+        .indices.items()
     )
 
     # Run in parallel
     if use_joblib_parallelisation:
         pr_results = Parallel(n_jobs=n_jobs)(
             delayed(_inspect_replicating)(
                 **(inspect_replicating_additional_args), **{"g_indices": g_indices}
@@ -934,28 +1035,29 @@
         )
     # Or not
     else:
         pr_results = [
             _inspect_replicating(
                 **(inspect_replicating_additional_args), **{"g_indices": g_indices}
             )
-            for g_indices in progressbar(df_groupby_indices_and_items)
+            for g_indices in tqdm(df_groupby_indices_and_items)
             if (
                 len(g_indices) >= min_cardinality
                 or include_cardinality_violating_compounds_in_calculation
             )
         ]
 
     # Remove compounds which did not make it through cardinality filters (as specified through args)
     if not include_cardinality_violating_compounds_in_calculation:
         pr_results = [r for r in pr_results if not np.isnan(r.matching_median_dist)]
 
     if len(pr_results) == 0:
         print(
-            "No suitable compounds were found for calculation of any replicating compounds, reporting as such"
+            "No suitable compounds were found for calculation of any replicating"
+            " compounds, reporting as such"
         )
 
     def _determine_replicating(
         null_dist, rep_val, similarity_metric_higher_is_better, percentile_cutoff
     ) -> int:
         if isinstance(null_dist, np.ndarray):
             null_dist = np.percentile(null_dist, percentile_cutoff)
@@ -964,30 +1066,33 @@
         if similarity_metric_higher_is_better:
             return 1 if rep_val > null_dist else 0
         else:
             return 1 if rep_val < null_dist else 0
 
     if len(pr_results) == 0:
         print(
-            "No suitable compounds were found for calculation of any replicating compounds, reporting as such"
+            "No suitable compounds were found for calculation of any replicating"
+            " compounds, reporting as such"
         )
 
     if return_full_performance_df:
         res_df = pd.DataFrame(
             data=[
                 (
                     prd.cardinality,
                     _determine_replicating(
                         prd.null_nth_percentile_or_null_distribution,
                         prd.matching_median_dist,
                         similarity_metric_higher_is_better,
                         percentile_cutoff,
                     ),
                     prd.matching_median_dist,
-                    np.percentile(prd.null_nth_percentile_or_null_distribution, percentile_cutoff),
+                    np.percentile(
+                        prd.null_nth_percentile_or_null_distribution, percentile_cutoff
+                    ),
                 )
                 for prd in pr_results
             ],
             columns=[
                 "cardinality",
                 "is_replicating",
                 "median_replicate_score",
@@ -1002,14 +1107,39 @@
                 else np.full(n_iters, np.nan)
                 for prd in pr_results
             ],
             columns=[f"null_{ni}" for ni in range(1, n_iters + 1)],
             index=[prd.index for prd in pr_results],
         )
         res_df = pd.concat([res_df, null_d_df], axis=1)
+
+        if include_replicate_pairwise_distances_in_df:
+            max_cardinality_in_results = np.max(
+                [
+                    len(prtuple.replicate_all_to_all_distances)
+                    for prtuple in pr_results
+                    if isinstance(prtuple.replicate_all_to_all_distances, np.ndarray)
+                ]
+            )
+            replicate_pairwise_scores_df = pd.DataFrame(
+                data=np.full((len(pr_results), max_cardinality_in_results), np.nan),
+                index=res_df.index,
+                columns=[
+                    f"replicate_pairwise_score_{ni}"
+                    for ni in range(1, max_cardinality_in_results + 1)
+                ],
+            )
+            for prtuple_i, prtuple in enumerate(pr_results):
+                if isinstance(prtuple.replicate_all_to_all_distances, np.ndarray):
+                    replicate_pairwise_scores_df.iloc[
+                        prtuple_i, : len(prtuple.replicate_all_to_all_distances)
+                    ] = prtuple.replicate_all_to_all_distances
+
+            res_df = pd.concat([res_df, replicate_pairwise_scores_df], axis=1)
+
         if performance_df_file is not None and performance_df_file != False:
             run_parameters_dict = {
                 "ds.df.shape": df.shape,
                 "perturbation_column": perturbation_column,
                 "replicate_query": replicate_query,
                 "replicate_criteria": replicate_criteria,
                 "replicate_criteria_not": replicate_criteria_not,
@@ -1073,15 +1203,14 @@
                     for prd in pr_results
                 ]
             )
             / len(pr_results)
         ) * 100
 
 
-
 def percent_compact(
     ds: Union[Dataset, Phenonaut, pd.DataFrame],
     perturbation_column: Optional[str] = None,
     replicate_criteria: Optional[Union[str, list[str]]] = None,
     replicate_query: Optional[str] = None,
     replicate_criteria_not: Optional[Union[str, list[str]]] = None,
     null_query_or_df: Optional[Union[str, pd.DataFrame]] = None,
@@ -1095,15 +1224,15 @@
     min_cardinality: int = 2,
     max_cardinality: int = 50,
     include_cardinality_violating_compounds_in_calculation: bool = False,
     return_full_performance_df: bool = False,
     additional_captured_params: Optional[dict] = None,
     similarity_metric_name: Optional[str] = None,
     performance_df_file: Optional[Union[str, Path]] = None,
-    percentile_cutoff:Optional[int] = None,
+    percentile_cutoff: Optional[int] = None,
     use_joblib_parallelisation: bool = True,
     n_jobs: int = -1,
 ):
     """Calculate percent compact
 
     Compactness is defined by the spread of compound repeats compared to a randomly sampled
     background distribution.  For a given compound, its cardinality (num replicates), reffered
@@ -1280,19 +1409,22 @@
         pd.DataFrame in the second position containing the median repeat scores, as well as median
         null distribution scores in an easy to analyse format.
 
     """
     start_time = timer()
     if max_cardinality < min_cardinality:
         raise ValueError(
-            f"Error, max_cardinality ({max_cardinality}) may not be less than min_cardinality ({min_cardinality})"
+            f"Error, max_cardinality ({max_cardinality}) may not be less than"
+            f" min_cardinality ({min_cardinality})"
         )
-    if percentile_cutoff is not None and percentile_cutoff < 1 :
+    if percentile_cutoff is not None and percentile_cutoff < 1:
         print(
-            "WARNING: percentile_cutoff < 1. For the 95th percentile, this should be 95, not 0.95. This function calls np.percentile, which behaves the same, expecting a number between 0 and 100 to specify the cutoff."
+            "WARNING: percentile_cutoff < 1. For the 95th percentile, this should be"
+            " 95, not 0.95. This function calls np.percentile, which behaves the same,"
+            " expecting a number between 0 and 100 to specify the cutoff."
         )
     (
         df,
         features,
         replicate_criteria,
         null_criteria,
         replicate_criteria_not,
@@ -1317,28 +1449,35 @@
         }
         if similarity_metric in special_similarity_metrics_higher_better_lookup:
             if (
                 special_similarity_metrics_higher_better_lookup[similarity_metric]
                 != similarity_metric_higher_is_better
             ):
                 print(
-                    f"Warning, special similarity metric value {similarity_metric} passed with similarity_metric_higher_is_better = {similarity_metric_higher_is_better}, changing similarity_metric_higher_is_better to {special_similarity_metrics_higher_better_lookup[similarity_metric]}"
+                    "Warning, special similarity metric value"
+                    f" {similarity_metric} passed with"
+                    " similarity_metric_higher_is_better ="
+                    f" {similarity_metric_higher_is_better}, changing"
+                    " similarity_metric_higher_is_better to"
+                    f" {special_similarity_metrics_higher_better_lookup[similarity_metric]}"
+                )
+                similarity_metric_higher_is_better = (
+                    not similarity_metric_higher_is_better
                 )
-                similarity_metric_higher_is_better = not similarity_metric_higher_is_better
         if similarity_metric_name is None:
             similarity_metric_name = similarity_metric
 
     if isinstance(similarity_metric, PhenotypicMetric):
         similarity_metric_higher_is_better = similarity_metric.higher_is_better
         similarity_metric_name = similarity_metric.name
         if similarity_metric.is_magic_string:
             similarity_metric = similarity_metric.func
 
     if percentile_cutoff is None:
-        percentile_cutoff=95 if similarity_metric_higher_is_better else 5
+        percentile_cutoff = 95 if similarity_metric_higher_is_better else 5
 
     inspect_compact_additional_args = {
         "df": df,
         "features": features,
         "replicate_query": replicate_query,
         "replicate_criteria": replicate_criteria,
         "replicate_criteria_not": replicate_criteria_not,
@@ -1352,15 +1491,17 @@
         "return_full_profiles": return_full_performance_df,
         "percentile_cutoff": percentile_cutoff,
     }
 
     df_groupby_indices_and_items = (
         df.groupby(replicate_criteria).indices.items()
         if restrict_evaluation_query is None
-        else df.query(restrict_evaluation_query).groupby(replicate_criteria).indices.items()
+        else df.query(restrict_evaluation_query)
+        .groupby(replicate_criteria)
+        .indices.items()
     )
 
     # Run in parallel
     if use_joblib_parallelisation:
         compactness_results = Parallel(n_jobs=n_jobs)(
             delayed(_inspect_compact)(
                 **inspect_compact_additional_args, **{"g_indices": g_indices}
@@ -1373,28 +1514,31 @@
         )
     # Or not
     else:
         compactness_results = [
             _inspect_compact(
                 **inspect_compact_additional_args, **{"g_indices": g_indices}
             )
-            for g_indices in progressbar(df_groupby_indices_and_items)
+            for g_indices in tqdm(df_groupby_indices_and_items)
             if (
                 len(g_indices) >= min_cardinality
                 or include_cardinality_violating_compounds_in_calculation
             )
         ]
 
     # Remove compounds which did not make it through cardinality filters (as specified through args)
     if not include_cardinality_violating_compounds_in_calculation:
-        compactness_results = [r for r in compactness_results if not np.isnan(r.matching_median_dist)]
+        compactness_results = [
+            r for r in compactness_results if not np.isnan(r.matching_median_dist)
+        ]
 
     if len(compactness_results) == 0:
         print(
-            "No suitable compounds were found for calculation of any replicating compounds, reporting as such"
+            "No suitable compounds were found for calculation of any replicating"
+            " compounds, reporting as such"
         )
 
     def _determine_compact(
         null_dist, rep_val, similarity_metric_higher_is_better, percentile_cutoff
     ) -> int:
         if isinstance(null_dist, np.ndarray):
             null_dist = np.percentile(null_dist, percentile_cutoff)
@@ -1403,30 +1547,33 @@
         if similarity_metric_higher_is_better:
             return 1 if rep_val > null_dist else 0
         else:
             return 1 if rep_val < null_dist else 0
 
     if len(compactness_results) == 0:
         print(
-            "No suitable compounds were found for calculation of any replicating compounds, reporting as such"
+            "No suitable compounds were found for calculation of any replicating"
+            " compounds, reporting as such"
         )
 
     if return_full_performance_df:
         res_df = pd.DataFrame(
             data=[
                 (
                     prd.cardinality,
                     _determine_compact(
                         prd.null_nth_percentile_or_null_distribution,
                         prd.matching_median_dist,
                         similarity_metric_higher_is_better,
                         percentile_cutoff,
                     ),
                     prd.matching_median_dist,
-                    np.percentile(prd.null_nth_percentile_or_null_distribution, percentile_cutoff),
+                    np.percentile(
+                        prd.null_nth_percentile_or_null_distribution, percentile_cutoff
+                    ),
                 )
                 for prd in compactness_results
             ],
             columns=[
                 "cardinality",
                 "is_compact",
                 "median_replicate_score",
@@ -1511,86 +1658,263 @@
                     )
                     for prd in compactness_results
                 ]
             )
             / len(compactness_results)
         ) * 100
 
+
 def silhouette_score(
     ds: Union[Dataset, Phenonaut, pd.DataFrame],
     perturbation_column: Union[str, None],
     replicate_criteria: Optional[Union[str, list[str]]] = None,
     features: Optional[list[str]] = None,
     similarity_metric: Union[str, Callable] = "euclidean",
     similarity_metric_higher_is_better: bool = True,
-    return_full_performance_df: bool = False,):
-
-
+    return_full_performance_df: bool = False,
+):
     if isinstance(similarity_metric, str):
         # Inbuilt fast methods, lookup table for higher_is_better
         special_similarity_metrics_higher_better_lookup = {
             "spearman": True,
             "euclidean": False,
             "cityblock": False,
             "cosine": False,
         }
         if similarity_metric in special_similarity_metrics_higher_better_lookup:
             if (
                 special_similarity_metrics_higher_better_lookup[similarity_metric]
                 != similarity_metric_higher_is_better
             ):
                 print(
-                    f"Warning, special similarity metric value {similarity_metric} passed with similarity_metric_higher_is_better = {similarity_metric_higher_is_better}, changing similarity_metric_higher_is_better to {special_similarity_metrics_higher_better_lookup[similarity_metric]}"
+                    "Warning, special similarity metric value"
+                    f" {similarity_metric} passed with"
+                    " similarity_metric_higher_is_better ="
+                    f" {similarity_metric_higher_is_better}, changing"
+                    " similarity_metric_higher_is_better to"
+                    f" {special_similarity_metrics_higher_better_lookup[similarity_metric]}"
+                )
+                similarity_metric_higher_is_better = (
+                    not similarity_metric_higher_is_better
                 )
-                similarity_metric_higher_is_better = not similarity_metric_higher_is_better
 
     if isinstance(similarity_metric, PhenotypicMetric):
         similarity_metric_higher_is_better = similarity_metric.higher_is_better
         if similarity_metric.is_magic_string:
             similarity_metric = similarity_metric.func
 
-
-    if isinstance(ds,Phenonaut):
-        ds=ds[-1]
+    if isinstance(ds, Phenonaut):
+        ds = ds[-1]
     if isinstance(ds, Dataset):
-        df=ds.df
-        features=ds.features
+        df = ds.df
+        features = ds.features
 
         if perturbation_column is None:
             if ds.perturbation_column is None:
-                raise ValueError("No pertuabtion column set, and no perturbation_column argument given")
-            perturbation_column=ds.perturbation_column
-    else: # Must be df-like
+                raise ValueError(
+                    "No pertuabtion column set, and no perturbation_column argument"
+                    " given"
+                )
+            perturbation_column = ds.perturbation_column
+    else:  # Must be df-like
         if perturbation_column is None:
-            raise ValueError("Must provide a perturbation_column argument when supplying a DataFrame")
+            raise ValueError(
+                "Must provide a perturbation_column argument when supplying a DataFrame"
+            )
         if features is None:
-            raise ValueError("Must provide features argument when supplying a DataFrame")
-        df=df
+            raise ValueError(
+                "Must provide features argument when supplying a DataFrame"
+            )
+        df = df
 
-    group_by=[perturbation_column]
+    group_by = [perturbation_column]
     if replicate_criteria is not None:
         if isinstance(replicate_criteria, str):
-            replicate_criteria=[replicate_criteria]
+            replicate_criteria = [replicate_criteria]
         group_by.extend(replicate_criteria)
 
-    gb=df.groupby(group_by)
-    n_clusters=len(gb)
-
-    scores=np.eye(n_clusters)
-    scores[scores==1]=np.nan
+    gb = df.groupby(group_by)
+    n_clusters = len(gb)
 
+    scores = np.eye(n_clusters)
+    scores[scores == 1] = np.nan
 
     for i, (group_name_a, indices_a) in enumerate(gb.indices.items()):
         for j, (group_name_b, indices_b) in enumerate(gb.indices.items()):
-            if group_name_a==group_name_b:
+            if group_name_a == group_name_b:
                 continue
-            X=np.vstack([
-            df.iloc[indices_a][features], df.iloc[indices_b][features]])
-            labels=[*([group_name_a]*len(indices_a)), *([group_name_b]*len(indices_b))]
-            scores[i,j]=sklearn_silhouette_score(X, labels, metric=similarity_metric)
-    scores_df=pd.DataFrame(data=scores, index=list(gb.indices.keys()), columns=list(gb.indices.keys()))
-    scores_df["mean_silhouette_score"]=np.nanmean(scores, axis=1)
+            X = np.vstack([df.iloc[indices_a][features], df.iloc[indices_b][features]])
+            labels = [
+                *([group_name_a] * len(indices_a)),
+                *([group_name_b] * len(indices_b)),
+            ]
+            scores[i, j] = sklearn_silhouette_score(X, labels, metric=similarity_metric)
+    scores_df = pd.DataFrame(
+        data=scores, index=list(gb.indices.keys()), columns=list(gb.indices.keys())
+    )
+    scores_df["mean_silhouette_score"] = np.nanmean(scores, axis=1)
     if return_full_performance_df:
-        return scores_df['mean_silhouette_score'].mean(), scores_df
+        return scores_df["mean_silhouette_score"].mean(), scores_df
     else:
-        return scores_df['mean_silhouette_score'].mean()
+        return scores_df["mean_silhouette_score"].mean()
+
+
+def mp_value_score(
+    ds: Union[Dataset, Phenonaut],
+    ds_groupby: Union[str, List[str]],
+    reference_perturbation_query: str,
+    pca_explained_variance: float = 0.99,
+    std_scaler_columns: bool = True,
+    std_scaler_rows: bool = False,
+    n_iters: int = 1000,
+    random_state: int = 42,
+    raise_error_for_low_count_groups: bool = True,
+):
+    """Get mp-value score performance DataFrame for a dataset
 
+    Implementation of the mp-value score from the paper:
+        Hutz JE, Nelson T, Wu H, et al. The Multidimensional Perturbation Value: A
+        Single Metric to Measure Similarity and Activity of Treatments in
+        High-Throughput Multidimensional Screens. Journal of Biomolecular Screening.
+        2013;18(4):367-377. doi:10.1177/1087057112469257.
+
+    The paper mentions normalising by rows as well as columns. This is not appropriate
+    for some data types like DRUG-seq, and so this is not enabled by default.
+    Additionally, a default fraction explained variance for the PCA operation has been
+    set to 0.99 so that the PCA may explain 99 % of variance.
+
+    This implementation differs somewhat to the one in pycytominer_eval which deviates
+    from the paper definition and does not perform a mixin of the covariance matrices
+    for treatment and control.
+
+    Parameters
+    ----------
+    ds : Union[Dataset, Phenonaut]
+        Phenonaut dataset or Phenonaut object upon which to perform the mp_value_score
+        calculation. If a Phenonaut object is passed, then the dataset at position -1
+        (usually the last added is used)
+    ds_groupby: Pandas style groupby to apply on the ds. Normally this is the column
+        name of a unique compound identifier. Can also be a list, containing the unique
+        compound identifier column name, along with a concentration or timepoint column.
+    reference_perturbation_query : reference_perturbation_query
+        Pandas style query which may be run on ds to extract the reference set of points
+        in phenotypic space, against which all other grouped perturbations are compared.
+    pca_explained_variance: float
+        This argument is passed to scikit's PCA object and specifices the % variance
+        that the returned components should capture. The original paper aims for 90 % ev
+        we aim by default for 99 %. Should be expressed as a float between 0 and 1.
+        By default 0.99
+    std_scaler_columns: bool
+        Apply standard scaler to columns. By default True
+    std_scaler_rows: bool
+        Apply standard scaler to rows. By default False
+    n_iters : int
+        Number of iterations iterations to perform in statistical test to derive
+        p-value, by default 1000
+    n_jobs : int, optional
+        Calculations will be run in parallel by providing the number of processors to
+        use. If n_jobs is None, then this is autodetected by the system. By default None
+    random_state : int
+        Random seed to use for initialisation of rng, enabling reproducible runs
+    raise_error_for_low_count_groups : bool
+        Calculation of mp_value scores requires more than three samples to be in each
+        group. If raise_error_for_low_count_groups is True, then an error is raised upon
+        encountering such a group as no mp_value score can be calculated. If False, then
+        a simple warning is printed and the returned p-value and mahalanobis distance in
+        the results dataframe are both np.nan. By default True
+    """
+
+    if isinstance(ds, Phenonaut):
+        ds = ds[-1]
+    vehicle_data = ds.df.query(reference_perturbation_query)[ds.features].values
+    if len(vehicle_data) < 3:
+        raise NotEnoughRowsError(
+            f"Vehicle had {len(vehicle_data)} rows. 3 or more are required for the"
+            " mp_value_score calculation. It is highly likely that the query string"
+            " passed as reference_perturbation_query does not return any dataframe"
+            " rows. Try running the supplied query on your dataset.df and see if"
+            f" anything is returned.  Query was: {reference_perturbation_query}"
+        )
+    len_veh_data = vehicle_data.shape[0]
+    grouped_df = ds.df.groupby(ds_groupby)
+
+    mp_value_score_results_df = pd.DataFrame()
+
+    for group_identifier, group_df in grouped_df:
+        print("Working on", group_identifier, len(group_df))
+        if len(group_df) < 3:
+            if raise_error_for_low_count_groups:
+                raise NotEnoughRowsError(
+                    f"Group '{group_identifier}' contained only {len(group_df)} rows. 3"
+                    " or more are required for the mp_value_score calculation. To"
+                    " continue processing when small groups like this are encountered,"
+                    " call mp_value_score again with raise_error_for_low_count_groups"
+                    " = False"
+                )
+            print(
+                f"WARNING, Group '{group_identifier}' contained only"
+                f" {len(group_df)} rows. 3 or more are required for the mp_value_score"
+                " calculation. np.nan values will be included in results. Continuing"
+                " as raise_error_for_low_count_groups was False."
+            )
+            mp_value_score_results_df.loc[
+                group_identifier, ["mahalanobis_distance", "mp_value"]
+            ] = (np.nan, np.nan)
+            continue
+        # Reseed RNG for every group otherwise the order of groups would influenc
+        # mp_value scores
+        np_rng = np.random.default_rng(random_state)
+
+        trt_data = group_df[ds.features].values
+        len_trt_data = trt_data.shape[0]
+        X = np.vstack([trt_data, vehicle_data])
+        # Scale data
+        if std_scaler_columns:
+            X = (X - X.mean(axis=0)) / np.std(X, axis=0)
+        if std_scaler_rows:
+            X = (X - X.mean(axis=1)) / np.std(X, axis=1)
+
+        pca = PCA(n_components=pca_explained_variance, svd_solver="full")
+        X = pca.fit_transform(X)
+        X = X * pca.explained_variance_ratio_
+
+        # Compute covariance matrices of the scaled data and add them before inverting for
+        # calculation of mahalanobis distances
+        cov_trt = (np.cov(X[:len_trt_data].T)) * (
+            len_trt_data / (len_trt_data + len_veh_data)
+        )
+        cov_veh = (np.cov(X[len_trt_data:].T)) * (
+            len_veh_data / (len_trt_data + len_veh_data)
+        )
+        inv_cov = linalg.inv(cov_trt + cov_veh)
+
+        veh_pca_mean = np.mean(X[len_trt_data:], axis=0)
+        original_m_dist = mahalanobis(
+            np.mean(X[:len_trt_data], axis=0), veh_pca_mean, inv_cov
+        )
+
+        original_labels = np.array([1] * len_trt_data + [0] * len_veh_data)
+        cur_labels = original_labels.copy()
+        perturbed_distances = np.empty(n_iters)
+        for i in range(n_iters):
+            np_rng.shuffle(cur_labels)
+            while np.all(cur_labels[:len_trt_data]):
+                np_rng.shuffle(cur_labels)
+            not_cur_labels = np.logical_not(cur_labels)
+            pcov_trt = np.cov(X[np.where(cur_labels)].T) * (
+                len_trt_data / (len_trt_data + len_veh_data)
+            )
+            pcov_veh = np.cov(X[np.where(not_cur_labels)].T) * (
+                len_veh_data / (len_trt_data + len_veh_data)
+            )
+            pinv_cov = linalg.inv(pcov_trt + pcov_veh)
+
+            perturbed_distances[i] = mahalanobis(
+                np.mean(X[np.where(cur_labels)], axis=0),
+                np.mean(X[np.where(not_cur_labels)], axis=0),
+                pinv_cov,
+            )
+            mp_value = np.mean([v > original_m_dist for v in perturbed_distances])
+        mp_value_score_results_df.loc[
+            group_identifier, ["mahalanobis_distance", "mp_value"]
+        ] = (original_m_dist, mp_value)
+    return mp_value_score_results_df
```

### Comparing `phenonaut-1.3.4/phenonaut/metrics/utils.py` & `phenonaut-2.0.3/src/phenonaut/metrics/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import pandas as pd
+import json
+from pathlib import Path
+from typing import Union
+
 import numpy as np
+import pandas as pd
 from joblib import Parallel, delayed
-from typing import Union
-from pathlib import Path
-import json
+
 
 def percent_replicating_results_dataframe_to_percentile_vs_percent_replicating(
     df: pd.DataFrame,
     percentile_range: tuple[int, int] = (0, 101),
     percentile_step_size: int = 1,
     return_counts: bool = False,
-    n_jobs:int=-1,
+    n_jobs: int = -1,
     similarity_metric_higher_is_better: bool = True,
-
 ) -> tuple[np.ndarray, np.ndarray]:
     """Get x,y arrays for cutoff vs % replicating plots
 
     Reads a DataFrame from phenonaut.metrics.performance.percent_replicating
     when run with return_full_performance_df = True, and generates a tuple of
     x and y coordinates, allowing plotting of percentile cutoff vs percent
     replicating.
@@ -47,60 +48,70 @@
     -------
     tuple[np.ndarray, np.ndarray]
         Tuple containing 2 np.ndarrays, the first being percentile cutoff, and
         the second being mathching % replicating values (or count of replicating
         compounds if return_counts=True)
     """
     num_in_null = len(
-        [1 for nc in df.columns if nc.startswith("null_") and not nc.endswith("_percentile")]
+        [
+            1
+            for nc in df.columns
+            if nc.startswith("null_") and not nc.endswith("_percentile")
+        ]
     )
     x = np.arange(*percentile_range)
     y = []
 
     def _assign_pr(r, p, similarity_metric_higher_is_better):
         if isinstance(r[-num_in_null], str):
             return 0
         if similarity_metric_higher_is_better:
             if r["median_replicate_score"] > np.percentile(r[-num_in_null:], p):
                 return 1
             else:
                 return 0
         else:
-            if r["median_replicate_score"] < np.percentile(r[-num_in_null:], 100-p):
+            if r["median_replicate_score"] < np.percentile(r[-num_in_null:], 100 - p):
                 return 1
             else:
                 return 0
 
     def _get_pr(df, p, similarity_metric_higher_is_better):
-        return (p, np.sum(df.apply(_assign_pr, p=p, axis=1, similarity_metric_higher_is_better=similarity_metric_higher_is_better)))
+        return (
+            p,
+            np.sum(
+                df.apply(
+                    _assign_pr,
+                    p=p,
+                    axis=1,
+                    similarity_metric_higher_is_better=similarity_metric_higher_is_better,
+                )
+            ),
+        )
 
-    if df.shape[0]==0:
+    if df.shape[0] == 0:
         return x, np.full(x.shape, np.nan)
     results = Parallel(n_jobs=n_jobs)(
-        delayed(_get_pr)(
-            df,
-            percentile,
-            similarity_metric_higher_is_better,
-        )
+        delayed(_get_pr)(df, percentile, similarity_metric_higher_is_better)
         for percentile in x
     )
 
     sorted(results)
     y = np.array([r[1] for r in results])
-    return (x, (y / df.shape[0])*100) if not return_counts else (x,y)
+    return (x, (y / df.shape[0]) * 100) if not return_counts else (x, y)
 
 
 def percent_replicating_summarise_results(
     file_or_dir: Union[Path, str],
     dir_glob: str = "pr_*.csv",
     if_no_json_use_filename_to_derive_info: bool = True,
-    get_percent_replicating:bool=True,
+    get_percent_replicating: bool = True,
 ) -> Union[None, pd.DataFrame]:
     """Summarise percent replicating results
-    
+
     Parameters
     ----------
     file_or_dir : Union[Path, str]
         Percent replicating results file, or directory containing results files.
     dir_glob : str, optional
         Glob to use in searching directories for percent replicating results
         files, by default "pr_*.csv".
@@ -113,15 +124,15 @@
         run on a file (not a directory). By default True.
     Returns
     -------
     Union[Tuple[float, int], pd.DataFrame]
         Either a tuple containing the percent replicating and number of records
         contributing to that score (if run on a single file), or a pd.DataFrame
         summarising results (if run on a directory).
-    """    
+    """
 
     def _getpr_and_len(f):
         df = pd.read_csv(f)
         if df.shape[0] == 0:
             return 0.0, 0
         return (np.sum(df.is_replicating) / df.shape[0]) * 100, df.shape[0]
 
@@ -144,83 +155,90 @@
             "replicate_query_or_df",
             "null_criteria",
             "null_criteria_not",
             "null_query_or_df",
             "n_contributing",
         ]
 
-        series_list=[]
+        series_list = []
         for file in files:
             if get_percent_replicating:
                 calculated_pr, len_df = _getpr_and_len(file)
             else:
                 calculated_pr, len_df = (None, None)
             if file.with_suffix(".json").exists():
                 d = json.load(open(file.with_suffix(".json")))
-                columns=standard_columns.copy()
-                new_data=[
-                        str(file),
-                        d["similarity_metric_name"],
-                        d['similarity_metric_higher_is_better'],
-                        calculated_pr,
-                        d["replicate_criteria"],
-                        d["replicate_criteria_not"],
-                        d["replicate_query"],
-                        d["null_criteria"],
-                        d["null_criteria_not"] if d["null_criteria_not"]!=[] else np.nan,
-                        d["null_query_or_df"],
-                        len_df,
+                columns = standard_columns.copy()
+                new_data = [
+                    str(file),
+                    d["similarity_metric_name"],
+                    d["similarity_metric_higher_is_better"],
+                    calculated_pr,
+                    d["replicate_criteria"],
+                    d["replicate_criteria_not"],
+                    d["replicate_query"],
+                    d["null_criteria"],
+                    d["null_criteria_not"] if d["null_criteria_not"] != [] else np.nan,
+                    d["null_query_or_df"],
+                    len_df,
                 ]
-                
-                additional_data=d.get("additional_captured_params", None)
+
+                additional_data = d.get("additional_captured_params", None)
                 if isinstance(additional_data, dict):
-                    for k,v in additional_data.items():
+                    for k, v in additional_data.items():
                         columns.append(k)
                         new_data.append(v)
                 series_list.append(pd.Series(data=new_data, index=columns))
-                
+
             else:
                 if if_no_json_use_filename_to_derive_info:
                     fstr = file.stem
                     if fstr.startswith("pr__"):
                         similarity_metric = "Spearman"
                     similarity_metric = fstr.split("__")[0].split("_")
                     cell_lines = fstr.split("__")[1]
                     matching = fstr.split("__matching")[1]
                     if "__" in matching:
                         matching = matching.split("__")[0]
-                    nullmatch = "" if "__nullmatch" not in fstr else fstr.split("__nullmatch")[1]
+                    nullmatch = (
+                        ""
+                        if "__nullmatch" not in fstr
+                        else fstr.split("__nullmatch")[1]
+                    )
                     if "__" in nullmatch:
                         nullmatch = nullmatch.split("__")[0]
-                    columns=standard_columns.copy()
+                    columns = standard_columns.copy()
                     columns.append("CellLine")
-                    new_data=[
-                            str(file),
-                            similarity_metric,
-                            calculated_pr,
-                            matching,
-                            nullmatch,
-                            len_df,
-                            cell_lines,
+                    new_data = [
+                        str(file),
+                        similarity_metric,
+                        calculated_pr,
+                        matching,
+                        nullmatch,
+                        len_df,
+                        cell_lines,
                     ]
                     series_list.append(pd.Series(data=new_data, index=columns))
-        if len(series_list)<2:
+        if len(series_list) < 2:
             return pd.DataFrame(series_list).T
-        return pd.concat(series_list, axis=1).T.set_index("filename").sort_values('percent_replicating', ascending=False).dropna(axis='columns')
-
-
+        return (
+            pd.concat(series_list, axis=1)
+            .T.set_index("filename")
+            .sort_values("percent_replicating", ascending=False)
+            .dropna(axis="columns")
+        )
 
 
 def percent_compact_summarise_results(
     file_or_dir: Union[Path, str],
     dir_glob: str = "pc_*.csv",
-    get_percent_compact:bool=True,
+    get_percent_compact: bool = True,
 ) -> Union[None, pd.DataFrame]:
     """Summarise percent compact results
-    
+
     Parameters
     ----------
     file_or_dir : Union[Path, str]
         Percent compact results file, or directory containing results files.
     dir_glob : str, optional
         Glob to use in searching directories for percent replicating results
         files, by default "pc_*.csv".
@@ -229,15 +247,15 @@
         effect if run on a file (not a directory). By default True.
     Returns
     -------
     Union[Tuple[float, int], pd.DataFrame]
         Either a tuple containing the percent compact and number of records
         contributing to that score (if run on a single file), or a pd.DataFrame
         summarising results (if run on a directory).
-    """    
+    """
 
     def _getpc_and_len(f):
         df = pd.read_csv(f)
         if df.shape[0] == 0:
             return 0.0, 0
         return (np.sum(df.is_compact) / df.shape[0]) * 100, df.shape[0]
 
@@ -260,75 +278,62 @@
             "replicate_query_or_df",
             "null_criteria",
             "null_criteria_not",
             "null_query_or_df",
             "n_contributing",
         ]
 
-        series_list=[]
+        series_list = []
         for file in files:
             if get_percent_compact:
                 calculated_pc, len_df = _getpc_and_len(file)
             else:
                 calculated_pc, len_df = (None, None)
             d = json.load(open(file.with_suffix(".json")))
-            columns=standard_columns.copy()
-            new_data=[
-                    str(file),
-                    d["similarity_metric_name"],
-                    d['similarity_metric_higher_is_better'],
-                    calculated_pc,
-                    d["replicate_criteria"],
-                    d["replicate_criteria_not"],
-                    d["replicate_query"],
-                    d["null_criteria"],
-                    d["null_criteria_not"] if d["null_criteria_not"]!=[] else np.nan,
-                    d["null_query_or_df"],
-                    len_df,
+            columns = standard_columns.copy()
+            new_data = [
+                str(file),
+                d["similarity_metric_name"],
+                d["similarity_metric_higher_is_better"],
+                calculated_pc,
+                d["replicate_criteria"],
+                d["replicate_criteria_not"],
+                d["replicate_query"],
+                d["null_criteria"],
+                d["null_criteria_not"] if d["null_criteria_not"] != [] else np.nan,
+                d["null_query_or_df"],
+                len_df,
             ]
-            
-            additional_data=d.get("additional_captured_params", None)
+
+            additional_data = d.get("additional_captured_params", None)
             if isinstance(additional_data, dict):
-                for k,v in additional_data.items():
+                for k, v in additional_data.items():
                     columns.append(k)
                     new_data.append(v)
             series_list.append(pd.Series(data=new_data, index=columns))
-                
-            
-        if len(series_list)<2:
-            return pd.DataFrame(series_list).T
-        return pd.concat(series_list, axis=1).T.set_index("filename").sort_values('percent_compact', ascending=False).dropna(axis='columns')
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
 
+        if len(series_list) < 2:
+            return pd.DataFrame(series_list).T
+        return (
+            pd.concat(series_list, axis=1)
+            .T.set_index("filename")
+            .sort_values("percent_compact", ascending=False)
+            .dropna(axis="columns")
+        )
 
 
 def percent_replicating_results_dataframe_to_95pct_confidence_interval(
     df: pd.DataFrame,
-    percentile_cutoff:Union[int, float, list[Union[int, float]]]=95,
-    n_resamples:int=1000,
+    percentile_cutoff: Union[int, float, list[Union[int, float]]] = 95,
+    n_resamples: int = 1000,
     similarity_metric_higher_is_better: bool = True,
-    n_jobs:int=-1,
+    n_jobs: int = -1,
 ) -> Union[list[tuple[float, float]], tuple[float, float]]:
     """Get confidence interval at given percentile cutoff for percent replicating results
-    
+
     Reads a DataFrame from phenonaut.metrics.performance.percent_replicating
     and performs bootstrapping, sampling from the null distribution to assign a
     confidence interval at the given cutoff, or list of cutoffs.  Returns a tuple
     containing upper and lower 95 % confidence interval bounds.  If multiple
     percentile cutoffs are supplied, then a list containing tuples for each is returned.
 
     Parameters
@@ -354,73 +359,116 @@
     Union[list[tuple[float, float]], tuple[float, float]]
         Tuple containing 2 values, the first being the lower confidence interval
         and the second being the higher confidence interval.  If multiple
         percentile cutoffs are given, then a list of tuples at each percentile
         cutoff will be returned.
     """
     num_in_null = len(
-        [1 for nc in df.columns if nc.startswith("null_") and not nc.endswith("_percentile")]
+        [
+            1
+            for nc in df.columns
+            if nc.startswith("null_") and not nc.endswith("_percentile")
+        ]
     )
 
-    if df.shape[0]==0:
-        return [None for _ in range(len(percentile_cutoff))] if isinstance(percentile_cutoff, (np.ndarray, list, tuple)) else None
-    
+    if df.shape[0] == 0:
+        return (
+            [None for _ in range(len(percentile_cutoff))]
+            if isinstance(percentile_cutoff, (np.ndarray, list, tuple))
+            else None
+        )
+
     def _assign_pr(r, p, similarity_metric_higher_is_better):
         if isinstance(r[-num_in_null], str):
             return 0
         if similarity_metric_higher_is_better:
             if r["median_replicate_score"] > np.percentile(r[-num_in_null:], p):
                 return 1
             else:
                 return 0
         else:
-            if r["median_replicate_score"] < np.percentile(r[-num_in_null:], 100-p):
+            if r["median_replicate_score"] < np.percentile(r[-num_in_null:], 100 - p):
                 return 1
             else:
                 return 0
 
-
     def _get_pr(df, p, similarity_metric_higher_is_better):
-        if df.shape[0]==0:
+        if df.shape[0] == 0:
             return np.nan
-        return np.sum(df.apply(_assign_pr, p=p, axis=1, similarity_metric_higher_is_better=similarity_metric_higher_is_better))/df.shape[0]
+        return (
+            np.sum(
+                df.apply(
+                    _assign_pr,
+                    p=p,
+                    axis=1,
+                    similarity_metric_higher_is_better=similarity_metric_higher_is_better,
+                )
+            )
+            / df.shape[0]
+        )
 
     def _get_null(row):
         if isinstance(row[-num_in_null], str):
             print(row[-num_in_null])
             return np.full(num_in_null, np.nan)
         else:
             return np.array(row[-num_in_null:])
 
-    if isinstance(percentile_cutoff,(float, int)):
-        percentile_cutoff=[percentile_cutoff]
-    bootstrap_results=[]
-    null_distributions=np.apply_along_axis(_get_null,1, df.values)
+    if isinstance(percentile_cutoff, (float, int)):
+        percentile_cutoff = [percentile_cutoff]
+    bootstrap_results = []
+    null_distributions = np.apply_along_axis(_get_null, 1, df.values)
+
     def _pfunc_higher_is_better(percentile_cutoff):
-        return (np.sum(repeat_medians>np.percentile(np.apply_along_axis(lambda x: np.random.choice(x, num_in_null, replace=True), 1, null_distributions), percentile_cutoff, axis=1))/repeat_medians.shape[0])*100
+        return (
+            np.sum(
+                repeat_medians
+                > np.percentile(
+                    np.apply_along_axis(
+                        lambda x: np.random.choice(x, num_in_null, replace=True),
+                        1,
+                        null_distributions,
+                    ),
+                    percentile_cutoff,
+                    axis=1,
+                )
+            )
+            / repeat_medians.shape[0]
+        ) * 100
 
     def _pfunc_higher_is_not_better(percentile_cutoff):
-        ndist=np.apply_along_axis(lambda x: np.random.choice(x, num_in_null, replace=True), 1, null_distributions)
-        return (np.sum(repeat_medians<np.percentile(ndist, 100-percentile_cutoff, axis=1))/repeat_medians.shape[0])*100
+        ndist = np.apply_along_axis(
+            lambda x: np.random.choice(x, num_in_null, replace=True),
+            1,
+            null_distributions,
+        )
+        return (
+            np.sum(
+                repeat_medians < np.percentile(ndist, 100 - percentile_cutoff, axis=1)
+            )
+            / repeat_medians.shape[0]
+        ) * 100
 
-    repeat_medians=df.median_replicate_score.values
+    repeat_medians = df.median_replicate_score.values
     for p in percentile_cutoff:
-        #repeat_pr=np.empty(n_resamples)
+        # repeat_pr=np.empty(n_resamples)
         if similarity_metric_higher_is_better:
-            repeat_pr=Parallel(n_jobs=n_jobs)(delayed(_pfunc_higher_is_better)(p) for _ in range(n_resamples))
+            repeat_pr = Parallel(n_jobs=n_jobs)(
+                delayed(_pfunc_higher_is_better)(p) for _ in range(n_resamples)
+            )
 
-            # for repeat_i in progressbar(range(n_resamples), prefix="Bootstrapping null distributions"):
-            #     ndist=np.apply_along_axis(lambda x: np.random.choice(x, num_in_null, replace=True), 1, null_distributions)
-            #     repeat_pr[repeat_i]=(np.sum(repeat_medians>np.percentile(ndist, percentile_cutoff, axis=1))/repeat_medians.shape[0])*100
         else:
-            repeat_pr=Parallel(n_jobs=-1)(delayed(_pfunc_higher_is_not_better)(p) for _ in range(n_resamples))
-            
-            # for repeat_i in progressbar(range(n_resamples), prefix="Bootstrapping null distributions"):
-            #     ndist=np.apply_along_axis(lambda x: np.random.choice(x, num_in_null, replace=True), 1, null_distributions)
-            #     repeat_pr[repeat_i]=(np.sum(repeat_medians<np.percentile(ndist, 100-percentile_cutoff, axis=1))/repeat_medians.shape[0])*100
-
-        bootstrap_results.append((np.mean(repeat_pr), np.percentile(repeat_pr, 2.5), np.percentile(repeat_pr, 97.5)))
-    if len(bootstrap_results)==1:
+            repeat_pr = Parallel(n_jobs=-1)(
+                delayed(_pfunc_higher_is_not_better)(p) for _ in range(n_resamples)
+            )
+
+        bootstrap_results.append(
+            (
+                np.mean(repeat_pr),
+                np.percentile(repeat_pr, 2.5),
+                np.percentile(repeat_pr, 97.5),
+            )
+        )
+    if len(bootstrap_results) == 1:
         return bootstrap_results[0]
     else:
         return bootstrap_results
-
```

### Comparing `phenonaut-1.3.4/phenonaut/output/boxplot.py` & `phenonaut-2.0.3/src/phenonaut/output/boxplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from matplotlib import pyplot as plt
 from pathlib import Path
-from typing import Union, Optional
+from typing import Optional, Union
+
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-import matplotlib.pyplot as plt
+from matplotlib import pyplot as plt
 
 
 def write_boxplot_to_file(
     df: pd.DataFrame,
     x_label_in_df: str,
     y_label_in_df: str,
     output_file: Union[str, Path],
     title="Boxplot",
     x_label: Optional[str] = None,
     y_label: Optional[str] = None,
     figsize=(10, 6.18),
+    orient: Optional[str] = None,
 ):
     """Write a boxplot to a file
 
     Boxplot generation from pd.DataFrames using the Seaborn library
 
     Parameters
     ----------
@@ -43,23 +45,27 @@
     y_label : Optional[str], optional
         Optionally, override the use of the y-label present in the dataframe
         and display a different one on the axis. If None, the the value of
         y_label_in_df is used. By default None.
     figsize : tuple, optional
         Optional tuple of image height-width (in inches - as dictated by
         matplotlib/seaborn), by default (10, 6.18).
+    orient : str, optional
+        'h' or 'v' accepted and passed to seaborn to orient boxplots
+        horizontally or vertically respectively.  If None, then the
+        best orientation is guessed.  By default None.
     """
     sns.set(rc={"figure.figsize": figsize})
     tidy_df = df.replace(" ", r"\n", regex=True)
 
     if isinstance(output_file, str):
         output_file = Path(output_file)
     if not output_file.parent.exists():
         output_file.parent.mkdir(parents=True)
-    ax = sns.boxplot(x=x_label_in_df, y=y_label_in_df, data=tidy_df)
+    ax = sns.boxplot(x=x_label_in_df, y=y_label_in_df, data=tidy_df, orient=orient)
     if x_label is not None:
         ax.set(xlabel=x_label)
     if y_label is not None:
         ax.set(ylabel=y_label)
 
     ax.set_title(title)
     fig = ax.get_figure()
```

### Comparing `phenonaut-1.3.4/phenonaut/output/heatmap.py` & `phenonaut-2.0.3/src/phenonaut/output/heatmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
 from copy import deepcopy
-from matplotlib import pyplot as plt
-
-from pathlib import Path
-from typing import Tuple, Union, Optional, List
-import numpy as np
 from pathlib import Path
-from typing import Union, Optional
+from typing import List, Optional, Tuple, Union
+
 import numpy as np
 import pandas as pd
 import seaborn as sns
-
-from matplotlib.ticker import StrMethodFormatter
+from matplotlib import pyplot as plt
 from matplotlib.colors import Colormap
+from matplotlib.ticker import StrMethodFormatter
 
 
 def write_heatmap_from_df(
     df: pd.DataFrame,
     title: str,
     output_file: Union[str, Path],
     axis_labels: tuple[str, str] = ("", ""),
@@ -102,23 +98,21 @@
         If True, then position the colour bar on the left. If False, then
         position the colour bar on the right. By default False.
     sns_colour_palette : Optional[Colormap], optional
         Optionally, supply a seaborn colour map for use in the colour bar. By
         default None.
     """
 
-    padding = {
-        "top": 0.25,
-        "bottom": 1.24,
-        "element_height": 0.60,
-    }
+    padding = {"top": 0.25, "bottom": 1.24, "element_height": 0.60}
     if figsize is None:
         figsize = (
             10.0,
-            padding["top"] + padding["bottom"] + padding["element_height"] * df.shape[0],
+            padding["top"]
+            + padding["bottom"]
+            + padding["element_height"] * df.shape[0],
         )
     if (transpose is None and df.shape[0] > df.shape[1]) or transpose:
         df = deepcopy(df.transpose())
     # Turn column and row labels with spaces into multiline items
     df = df.rename(
         columns={c: c.replace(" ", "\n") for c in df.columns if isinstance(c, str)},
         index={
@@ -140,15 +134,20 @@
                     ]
                 )
                 .reshape(df.values.shape)
                 .tolist()
             )
         else:
             annot = (
-                np.array([f"{val:{annotation_format_string_value}}" for val in df.values.ravel()])
+                np.array(
+                    [
+                        f"{val:{annotation_format_string_value}}"
+                        for val in df.values.ravel()
+                    ]
+                )
                 .reshape(df.values.shape)
                 .tolist()
             )
 
     fig, ax = plt.subplots(figsize=figsize, facecolor="w")
     if highlight_best:
         mask = df.values == np.nanmax(df.values)
@@ -176,15 +175,19 @@
             if sns_colour_palette is None
             else sns_colour_palette,
             mask=negated_mask,
             annot=annot,
             linewidths=0.02,
             ax=ax,
             fmt="",
-            annot_kws={"fontsize": annotation_best_fontsize, "style": "italic", "weight": "bold"},
+            annot_kws={
+                "fontsize": annotation_best_fontsize,
+                "style": "italic",
+                "weight": "bold",
+            },
             cbar=False,
             vmin=np.nanmin(df.values) if vmin is None else vmin,
             vmax=np.nanmax(df.values) if vmax is None else vmax,
             cbar_kws=dict(location="left") if put_cbar_on_left else None,
         )
     else:
         sns.heatmap(
```

### Comparing `phenonaut-1.3.4/phenonaut/output/ph0_pptx_template.pptx` & `phenonaut-2.0.3/src/phenonaut/output/ph0_pptx_template.pptx`

 * *Files identical despite different names*

### Comparing `phenonaut-1.3.4/phenonaut/output/ph0_pptx_template_desc.pptx` & `phenonaut-2.0.3/src/phenonaut/output/ph0_pptx_template_desc.pptx`

 * *Files identical despite different names*

### Comparing `phenonaut-1.3.4/phenonaut/output/pptx.py` & `phenonaut-2.0.3/src/phenonaut/output/pptx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from typing import Union, Optional
+import datetime
 from pathlib import Path
+from typing import Optional, Union
+
 import pkg_resources
-import datetime
 
 try:
     import pptx
 except ImportError as ie:
-    raise (f"Import Error - python-pptx functionality called, but it is not installed {ie}")
+    raise (
+        f"Import Error - python-pptx functionality called, but it is not installed {ie}"
+    )
 
 
 class PhenonautPPTX:
     """Phenonaut PPTX class
 
     Allows the creation of PPTX presentation files through insertion of images into slides.
 
@@ -77,15 +80,17 @@
         self.pres = pptx.Presentation(template_file)
         slide = self.pres.slides.add_slide(self.pres.slide_layouts[0])
         slide.shapes.title.text = cover_title
         slide.placeholders[1].text = cover_subtitle
         slide.placeholders[
             13
         ].text = f"Generated: {datetime.datetime.now().strftime('%d/%m/%Y, %H:%M:%S')}"
-        slide.placeholders[14].text = experiment_hash if experiment_hash is not None else "Hash: NA"
+        slide.placeholders[14].text = (
+            experiment_hash if experiment_hash is not None else "Hash: NA"
+        )
 
     def add_image_slide(
         self,
         title: str,
         img_file: Union[Path, str],
         width: Optional[Union[int, float]] = None,
         height: Optional[Union[int, float]] = None,
```

### Comparing `phenonaut-1.3.4/phenonaut/output/scatter.py` & `phenonaut-2.0.3/src/phenonaut/output/scatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from typing import List, Optional, Union, Tuple
 from pathlib import Path
-from pandas.errors import DataError
+from typing import List, Optional, Tuple, Union
 
-from phenonaut import data, output
-from matplotlib import pyplot as plt
+import pandas as pd
 import seaborn as sns
-from phenonaut import Phenonaut
+from matplotlib import pyplot as plt
+from pandas.errors import DataError
+
+from phenonaut import Phenonaut, data, output
 from phenonaut.data import Dataset
 
 from .visualisation_base import PhenonautVisualisation
-import pandas as pd
 
 
 class Scatter(PhenonautVisualisation):
     """Phenonaut scatter visualisation object.
 
     The object should be constructed, and then its add member function used
     to add points to the scatter.  It may then be saved by calling save, or
@@ -120,17 +120,15 @@
         for var in [
             x
             for x in self.__init__.__code__.co_varnames
             if x not in ("self", "figure_config", "var") and x not in self.config.keys()
         ]:
             self.config[var] = eval(var)
 
-
-
-        self.fig, self.ax = plt.subplots(1,1,figsize = figsize)
+        self.fig, self.ax = plt.subplots(1, 1, figsize=figsize)
         self.marker_size = marker_size
 
     def add(
         self,
         dataset: Union[Dataset, Phenonaut],
         perturbations: Optional[List[str]] = None,
         markers: Union[dict, list, bool] = True,
@@ -188,43 +186,37 @@
             y=dataset.features[1],
             style=dataset.perturbation_column,
             hue=dataset.perturbation_column,
             s=marker_size,
             markers=markers,
             ax=self.ax,
         )
-        #self._decorate_figure()
-        #plt.show()
+        # self._decorate_figure()
+        # plt.show()
 
-    def _decorate_figure(
-        self,
-    ):
+    def _decorate_figure(self):
         """Internal helper function for axis decoration"""
         if self.config.get("show_legend", True):
             self.ax.legend()
         else:
             self.ax.get_legend().remove()
 
         self.ax.set_xlabel(self.config.get("xlabel", ""))
         self.ax.set_ylabel(self.config.get("ylabel", ""))
         axis_ranges = self.config.get("axis_ranges", ((None, None), (None, None)))
         self.ax.set_xlim(axis_ranges[0])
         self.ax.set_ylim(axis_ranges[1])
         self.ax.set_title(self.config.get("title", "2D scatter"))
         plt.tight_layout()
 
-    def show(
-        self,
-    ):
+    def show(self):
         """Show the plot on the screen"""
         self._decorate_figure()
         plt.show()
 
-
-
     def save_figure(self, output_image_path: Union[Path, str], **savefig_kwargs):
         """Save the current scatter plot to PNG/SVG file
 
         Saving of the image is achieved using the matplotlib plt.savefig. After
         the output filename, any argument/option may be given that is also
         valid in calls to plt.savefig.
 
@@ -236,16 +228,14 @@
         self._decorate_figure()
         if isinstance(output_image_path, str):
             output_image_path = Path(output_image_path)
         if not output_image_path.parent.exists():
             output_image_path.parent.mkdir(parents=True)
         plt.savefig(output_image_path, **savefig_kwargs)
 
-    def __del__(
-        self,
-    ):
+    def __del__(self):
         """Delete scatter
 
         Ensures plt.cla and clf are called upon Scatter object deletion
         """
         plt.cla()
         plt.clf()
```

### Comparing `phenonaut-1.3.4/phenonaut/output/spreadsheet.py` & `phenonaut-2.0.3/src/phenonaut/output/spreadsheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from typing import Union
 from pathlib import Path
+from typing import Union
+
 import pandas as pd
 
 
 def write_xlsx(
     output_file: Union[Path, str],
     dfs: Union[pd.DataFrame, list[pd.DataFrame], dict[str, pd.DataFrame]],
     df_names: Union[tuple, str] = None,
@@ -41,27 +42,31 @@
     if isinstance(output_file, str):
         output_file = Path(output_file)
     if isinstance(output_file, Path):
         output_file = output_file.resolve()
         if not output_file.parent.exists():
             output_file.parent.mkdir(parents=True)
     else:
-        raise ValueError(f"output_file should have been a Path or str, it was {type(output_file)}")
+        raise ValueError(
+            f"output_file should have been a Path or str, it was {type(output_file)}"
+        )
 
     if isinstance(dfs, dict):
         df_names = list(dfs.keys())
         dfs = list(dfs.values())
 
     if isinstance(dfs, pd.DataFrame):
         dfs = [dfs]
 
     if df_names is None:
         df_names = [f"Sheet{i+1}" for i in range(len(dfs))]
     if isinstance(df_names, str):
         df_names = [df_names]
     if len(dfs) > len(df_names):
         num_to_add = len(dfs) - len(df_names)
-        df_names.extend([f"Sheet{i+1}" for i in range(len(df_names), len(df_names) + num_to_add)])
+        df_names.extend(
+            [f"Sheet{i+1}" for i in range(len(df_names), len(df_names) + num_to_add)]
+        )
 
     with pd.ExcelWriter(output_file) as writer:
         for df, sheet_name in zip(dfs, df_names):
             df.to_excel(writer, sheet_name=sheet_name)
```

### Comparing `phenonaut-1.3.4/phenonaut/output/visualisation_base.py` & `phenonaut-2.0.3/src/phenonaut/output/visualisation_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import json
+from pathlib import Path
 from typing import Optional, Union
+
 import yaml
-from pathlib import Path
-import json
+
 from phenonaut.utils import load_dict
 
 
 class PhenonautVisualisation:
     """Base class for Phenonaut visualisations.
 
     Constructor allows supply of a plot_config dictionary, which is then stored
```

### Comparing `phenonaut-1.3.4/phenonaut/packaged_datasets/base.py` & `phenonaut-2.0.3/src/phenonaut/packaged_datasets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import gzip
+import shutil
+import urllib.request
 from abc import ABC, abstractclassmethod, abstractmethod
+from collections.abc import Callable
 from os import path
 from pathlib import Path
 from time import sleep
-from typing import Callable, List, Tuple, Union, Optional
-import urllib.request
+from typing import List, Optional, Tuple, Union
 from urllib.error import URLError
-from progressbar import progressbar
-import shutil
-import gzip
+
+from tqdm import tqdm
 
 
 class PackagedDataset(ABC):
     """PackagedDataset base class for all downloaded Datasets
 
     Inherited by Phenonaut classes which supply public datasets in the same
     way that pytorch allows easy access to MNIST and FashionMNIST etc,
@@ -184,15 +186,17 @@
         """
         if val is None:
             self._raw_data_dir = self.root
             return
         if isinstance(val, str):
             val = Path(val)
         if not isinstance(val, Path):
-            raise TypeError(f"raw_data_dir should be of type Path or str, but was {type(val)}")
+            raise TypeError(
+                f"raw_data_dir should be of type Path or str, but was {type(val)}"
+            )
         if self._raw_data_dir_relative_to_root:
             self._raw_data_dir = (self.root / val).resolve()
         else:
             self._raw_data_dir = val.resolve()
 
     def _download(
         self,
@@ -281,45 +285,45 @@
         if max_attempts == 0:
             if all(fi[0] in non_critical_urls for fi in failed_items):
                 return
             else:
                 raise URLError(
                     f"Cannot make any more download attempts, {len(tasks)} tasks remain, they were:\n {tasks}. Set download=False to process what was downloaded"
                 )
-        for source, destination in progressbar(tasks, redirect_stdout=True):
+        for source, destination in tqdm(tasks):
             try:
                 self._download(source, destination)
             except Exception as e:
                 print(e)
                 print(f"Failed to get {source}, will retry ")
                 failed_items.append((source, destination))
         if len(failed_items) > 0:
             sleep(retry_pause_seconds)
             self._batch_download(
                 failed_items,
                 max_attempts=max_attempts - 1,
                 retry_pause_seconds=retry_pause_seconds,
             )
 
-    def _processed_dataset_exists(self, required_files: List[Path]) -> bool:
+    def _processed_dataset_exists(self, required_files: list[Path]) -> bool:
         """Checks if all listed files are present in the dataset root directory
 
         Parameters
         ----------
         required_files : List[Path]
             List of file names to check exist in dataset root directory
 
         Returns
         -------
         bool
             True if all files were found in root of dataset directory
         """
         return all([(self.root / file).exists() for file in required_files])
 
-    def _raw_dataset_exists(self, required_files: List[Path]) -> bool:
+    def _raw_dataset_exists(self, required_files: list[Path]) -> bool:
         """Checks if all listed files are present in the raw_data_dir of dataset
 
         Parameters
         ----------
         required_files : List[Path]
             List of file names to check exist in raw_data_dir of dataset
```

### Comparing `phenonaut-1.3.4/phenonaut/packaged_datasets/breast_cancer.py` & `phenonaut-2.0.3/src/phenonaut/packaged_datasets/breast_cancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import datetime
+import gzip
+import pathlib
+import shutil
+import tarfile
 from collections import namedtuple
 from pathlib import Path
-import pathlib
 from typing import List, NamedTuple, Optional, Union
-from ..data import Dataset
+
+import h5py
+import numpy as np
 import pandas as pd
-from .base import PackagedDataset
-import gzip, tarfile
-import shutil
 from sklearn.datasets import load_breast_cancer
 
-import pandas as pd
-import numpy as np
-import h5py
-import datetime
+from ..data import Dataset
+from .base import PackagedDataset
 
 
 class BreastCancer(PackagedDataset):
     """Breast Cancer Dataset from scikit-learn
 
     This PackagedDataset provides the Breast Cancer dataset from
     scikit-learn. This is also known as the Breast cancer Wisconsin
```

### Comparing `phenonaut-1.3.4/phenonaut/packaged_datasets/cmap.py` & `phenonaut-2.0.3/src/phenonaut/packaged_datasets/cmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import datetime
+import gzip
+import json
 from collections import namedtuple
 from pathlib import Path
 from typing import List, Optional, Union
-from ..data import Dataset
+
+import h5py
+import numpy as np
 import pandas as pd
+
+from ..data import Dataset
 from .base import PackagedDataset
-import gzip
-import pandas as pd
-import numpy as np
-import h5py
-import datetime
-import json
 
 
 class CMAP(PackagedDataset):
     """CMAP (Level 5)- ConnectivityMap dataset - https://clue.io/
 
     CMAP is a repository of L1000 profiles measured from small molecule and
     crisper perturbations. This CMAP packaged dataset supplies an interface
@@ -100,15 +101,14 @@
         self,
         root: Union[Path, str],
         download: bool = False,
         raw_data_dir: Optional[Union[Path, str]] = Path("raw_data"),
         rm_downloaded_data: bool = True,
         landmark_only: bool = True,
     ):
-
         super().__init__(root, raw_data_dir)
         self.name = "CMAP"
         self.landmark_only = landmark_only
         self.processed_h5_file = self.root / "cmap_phenonaut.h5"
 
         if not download and not self.processed_h5_file.exists():
             raise FileNotFoundError(
@@ -190,15 +190,17 @@
                     "destination": self.root / req_file.compressed_filename,
                     "extract": True,
                 },
             )
 
         # Make sure the large GCTX file is present
         CMAP_GCTX_GZ_URL = "https://ftp.ncbi.nlm.nih.gov/geo/series/GSE70nnn/GSE70138/suppl/GSE70138_Broad_LINCS_Level5_COMPZ_n118050x12328_2017-03-06.gctx.gz"
-        CMAP_GCTX_GZ_FILENAME = "GSE70138_Broad_LINCS_Level5_COMPZ_n118050x12328_2017-03-06.gctx"
+        CMAP_GCTX_GZ_FILENAME = (
+            "GSE70138_Broad_LINCS_Level5_COMPZ_n118050x12328_2017-03-06.gctx"
+        )
         self._call_if_file_missing(
             self.root / CMAP_GCTX_GZ_FILENAME,
             self._download,
             {
                 "source": CMAP_GCTX_GZ_URL,
                 "destination": self.root / (CMAP_GCTX_GZ_FILENAME + ".gz"),
                 "extract": True,
@@ -221,18 +223,22 @@
         print(f"{datetime.datetime.now()} Merging")
         self._sig_info = pd.read_csv(
             self.root / "GSE70138_Broad_LINCS_sig_info_2017-03-06.txt",
             sep="\t",
             index_col=[0],
         )
         pert_dose = (
-            self._sig_info["pert_idose"].apply(lambda x: x.replace(" um", "").strip()).astype(float)
+            self._sig_info["pert_idose"]
+            .apply(lambda x: x.replace(" um", "").strip())
+            .astype(float)
         )
         self._sig_info["pert_idose"] = np.where(pert_dose < 0, np.nan, pert_dose)
-        self._df = self._df.merge(self._sig_info, left_index=True, right_index=True, copy=False)
+        self._df = self._df.merge(
+            self._sig_info, left_index=True, right_index=True, copy=False
+        )
 
         h5_store = pd.HDFStore(self.processed_h5_file, "w", complevel=0)
         h5_store["df"] = self._df
 
         h5_store["gene_info"] = pd.read_csv(
             self.root / "GSE70138_Broad_LINCS_gene_info_2017-03-06.txt",
             sep="\t",
@@ -423,15 +429,14 @@
         download: bool = False,
         raw_data_dir: Optional[Union[Path, str]] = Path("raw_data"),
         rm_downloaded_data: bool = True,
         landmark_only: bool = True,
         allowed_treatment_types: Union[str, list[str]] = ["trt_cp", "ctl_vehicle"],
         allowed_treatment_times: Union[str, list[str]] = "24 h",
     ):
-
         super().__init__(root, raw_data_dir)
         self.name = "CMAP_Level4"
         self.landmark_only = landmark_only
         self.processed_h5_file = self.root / "cmap_level4_phenonaut.h5"
 
         if isinstance(allowed_treatment_types, str):
             allowed_treatment_types = [allowed_treatment_types]
@@ -477,17 +482,15 @@
 
         Downloads the large compressed data file, decompresses it, extracts the
         data into a pd.DataFrame, merges the sig_info data file which includes
         data on the perturbation type.
 
         """
 
-        CMAP_GCTX_GZ_FILENAME = (
-            "GSE70138_Broad_LINCS_Level4_ZSPCINF_mlr12k_n345976x12328_2017-03-06.gctx.gz"
-        )
+        CMAP_GCTX_GZ_FILENAME = "GSE70138_Broad_LINCS_Level4_ZSPCINF_mlr12k_n345976x12328_2017-03-06.gctx.gz"
         # Make sure the required files to make the dataset exist
         DownloadableFileInfo = namedtuple(
             "DownloadableFileInfo", ["filename", "compressed_filename", "url"]
         )
         required_files = [
             DownloadableFileInfo(
                 "GSE70138_Broad_LINCS_gene_info_2017-03-06.txt",
@@ -533,15 +536,17 @@
 
         sig_info = pd.read_csv(
             self.raw_data_dir / "GSE70138_Broad_LINCS_sig_info_2017-03-06.txt.gz",
             sep="\t",
             index_col=[0],
         )
         pert_dose = (
-            sig_info["pert_idose"].apply(lambda x: x.replace(" um", "").strip()).astype(float)
+            sig_info["pert_idose"]
+            .apply(lambda x: x.replace(" um", "").strip())
+            .astype(float)
         )
         sig_info["pert_idose_uM"] = np.where(pert_dose < 0, np.nan, pert_dose)
         gene_info = pd.read_csv(
             self.raw_data_dir / "GSE70138_Broad_LINCS_gene_info_2017-03-06.txt.gz",
             sep="\t",
             index_col=[0],
         )
@@ -560,30 +565,39 @@
         big_df.columns = big_df.columns.map(lambda x: x.decode("utf8"))
         print(f"{datetime.datetime.now()} ..done")
 
         # Drop non-landmark features/genes if needed (by default we do)
         if self.landmark_only:
             big_df = big_df.drop(
                 columns=[str(g) for g in gene_info.query("pr_is_lm==0").index.tolist()]
-            ).rename(columns={str(n): gene_info.loc[n, "pr_gene_symbol"] for n in gene_info.index})
+            ).rename(
+                columns={
+                    str(n): gene_info.loc[n, "pr_gene_symbol"] for n in gene_info.index
+                }
+            )
 
         # Define and write out features
-        features = [gn for gn in big_df.columns if gn in gene_info.pr_gene_symbol.unique().tolist()]
+        features = [
+            gn
+            for gn in big_df.columns
+            if gn in gene_info.pr_gene_symbol.unique().tolist()
+        ]
 
         print("Adding metadata")
         old_columns = sig_info.columns.values.tolist()
-        ssi = sig_info.distil_id.str.split(
-            "|",
-            expand=True,
-        )
+        ssi = sig_info.distil_id.str.split("|", expand=True)
         sig_info = pd.concat([sig_info, ssi], axis=1)
         sig_info = sig_info.rename(
             columns={
                 v: f"sample_id_{v}"
-                for v in [cn for cn in sig_info.columns.values.tolist() if cn not in old_columns]
+                for v in [
+                    cn
+                    for cn in sig_info.columns.values.tolist()
+                    if cn not in old_columns
+                ]
             }
         )
         new_siginfo = pd.concat(
             [
                 sig_info.set_index(f"sample_id_{n}").drop(
                     columns=[
                         c
```

### Comparing `phenonaut-1.3.4/phenonaut/packaged_datasets/iris.py` & `phenonaut-2.0.3/src/phenonaut/packaged_datasets/iris.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import datetime
+import gzip
+import pathlib
+import shutil
+import tarfile
 from collections import namedtuple
 from pathlib import Path
-import pathlib
 from typing import List, NamedTuple, Optional, Union
-from ..data import Dataset
+
+import h5py
+import numpy as np
 import pandas as pd
-from .base import PackagedDataset
-import gzip, tarfile
-import shutil
 from sklearn.datasets import load_iris
 
-import pandas as pd
-import numpy as np
-import h5py
-import datetime
+from ..data import Dataset
+from .base import PackagedDataset
 
 
 class Iris(PackagedDataset):
     """IRIS dataset Scikit learn
 
     This PackagedDataset provides the Iris dataset from scikit-learn, with
     unique iris entries, each with four features each, and finally a target
@@ -62,15 +63,14 @@
     def __init__(
         self,
         root: Union[Path, str],
         download: bool = False,
         raw_data_dir: Optional[Union[Path, str]] = Path("raw_data"),
         rm_downloaded_data: bool = True,
     ):
-
         super().__init__(root, raw_data_dir)
         self.name = "Iris"
         self.processed_h5_file = self.root / "IRIS_phenonaut.h5"
 
         # If the dataset is missing, get it
         self._call_if_file_missing(self.processed_h5_file, self._make, None)
```

### Comparing `phenonaut-1.3.4/phenonaut/packaged_datasets/lincs.py` & `phenonaut-2.0.3/src/phenonaut/packaged_datasets/lincs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import datetime
+import gzip
+import pathlib
+import shutil
+import tarfile
 from collections import namedtuple
 from pathlib import Path
-import pathlib
 from typing import List, NamedTuple, Optional, Union
-from ..data import Dataset
+
+import h5py
+import numpy as np
 import pandas as pd
+
+from ..data import Dataset
 from .base import PackagedDataset
-import gzip, tarfile
-import shutil
-import pandas as pd
-import numpy as np
-import h5py
-import datetime
 
 
 class LINCS_Cell_Painting(PackagedDataset):
     """LINCS Cell Painting Dataset - https://clue.io/
 
     This PackagedDataset provides supplies the following pd.DataFrames
     (queryable by calling the inherited ".keys" method):
@@ -147,15 +149,17 @@
                     "destination": self.root / req_file.compressed_filename,
                     "extract": True,
                 },
             )
 
         # Make sure the large GCTX file is present
         CMAP_GCTX_GZ_URL = "https://ftp.ncbi.nlm.nih.gov/geo/series/GSE70nnn/GSE70138/suppl/GSE70138_Broad_LINCS_Level5_COMPZ_n118050x12328_2017-03-06.gctx.gz"
-        CMAP_GCTX_GZ_FILENAME = "GSE70138_Broad_LINCS_Level5_COMPZ_n118050x12328_2017-03-06.gctx"
+        CMAP_GCTX_GZ_FILENAME = (
+            "GSE70138_Broad_LINCS_Level5_COMPZ_n118050x12328_2017-03-06.gctx"
+        )
         self._call_if_file_missing(
             self.root / CMAP_GCTX_GZ_FILENAME,
             self._download,
             {
                 "source": CMAP_GCTX_GZ_URL,
                 "destination": self.root / (CMAP_GCTX_GZ_FILENAME + ".gz"),
                 "extract": True,
@@ -178,18 +182,22 @@
         print(f"{datetime.datetime.now()} Merging")
         self._sig_info = pd.read_csv(
             self.root / "GSE70138_Broad_LINCS_sig_info_2017-03-06.txt",
             sep="\t",
             index_col=[0],
         )
         pert_dose = (
-            self._sig_info["pert_idose"].apply(lambda x: x.replace(" um", "").strip()).astype(float)
+            self._sig_info["pert_idose"]
+            .apply(lambda x: x.replace(" um", "").strip())
+            .astype(float)
         )
         self._sig_info["pert_idose"] = np.where(pert_dose < 0, np.nan, pert_dose)
-        self._df = self._df.merge(self._sig_info, left_index=True, right_index=True, copy=False)
+        self._df = self._df.merge(
+            self._sig_info, left_index=True, right_index=True, copy=False
+        )
 
         h5_store = pd.HDFStore(self.processed_h5_file, "w", complevel=0)
         h5_store["df"] = self._df
 
         h5_store["gene_info"] = pd.read_csv(
             self.root / "GSE70138_Broad_LINCS_gene_info_2017-03-06.txt",
             sep="\t",
```

### Comparing `phenonaut-1.3.4/phenonaut/packaged_datasets/metadata_moa.py` & `phenonaut-2.0.3/src/phenonaut/packaged_datasets/metadata_moa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import datetime
+import gzip
+import pathlib
+import shutil
+import tarfile
 from collections import namedtuple
 from pathlib import Path
-import pathlib
 from typing import List, NamedTuple, Optional, Union
-from ..data import Dataset
+
+import h5py
+import numpy as np
 import pandas as pd
-from .base import PackagedDataset
-import gzip, tarfile
-import shutil
 from sklearn.datasets import load_iris
 
-import pandas as pd
-import numpy as np
-import h5py
-import datetime
+from ..data import Dataset
+from .base import PackagedDataset
 
 
 class MetadataJUMPMOACompounds(PackagedDataset):
     """DataFrame supplier for JUMP consortium MOA compound set
 
     This PackagedDataset provides access to a pd.DataFrame containing information
     on the JUMP MOA compound selection. Further information is available here:
-    
+
     https://github.com/jump-cellpainting/JUMP-MOA
 
     Parameters
     ----------
     root : Union[Path, str]
         Local directory containing the prepared dataset. If the dataset is
         not found here and the argument download=True is not given, then an
@@ -75,56 +76,64 @@
         Parameters
         ----------
         remove_intermediates : bool, optional
             If true, then the downloaded archive is removed, by default False
         """
         self._download(
             "https://raw.githubusercontent.com/jump-cellpainting/JUMP-MOA/master/JUMP-MOA_compound_metadata.tsv",
-            self.raw_data_dir/"JUMP-MOA_compound_metadata.tsv",
+            self.raw_data_dir / "JUMP-MOA_compound_metadata.tsv",
             mkdir=True,
             skip_if_exists=True,
         )
 
         from io import StringIO
-        replace_df_string="moa,new,old\nHMGCR inhibitor,delta-Tocotrienol,Compound1\nkinesin inhibitor,ispinesib,Compound2\nBCL inhibitor,ABT-737,Compound3\nPARP inhibitor,veliparib,Compound4\nIGF-1 inhibitor,NVP-AEW541,Compound5\ntricyclic antidepressant,dosulepin,Compound6\nFGFR inhibitor,BLU9931,Compound7\nphosphodiesterase inhibitor,quazinone,Compound8\n"
-        replace_df=pd.read_csv(StringIO(replace_df_string), sep=',')
 
-        df=pd.read_csv(self.raw_data_dir/"JUMP-MOA_compound_metadata.tsv", sep='\t', dtype=str).set_index("pert_iname").rename(index={old:new for old, new in replace_df[['old', 'new']].values})
+        replace_df_string = "moa,new,old\nHMGCR inhibitor,delta-Tocotrienol,Compound1\nkinesin inhibitor,ispinesib,Compound2\nBCL inhibitor,ABT-737,Compound3\nPARP inhibitor,veliparib,Compound4\nIGF-1 inhibitor,NVP-AEW541,Compound5\ntricyclic antidepressant,dosulepin,Compound6\nFGFR inhibitor,BLU9931,Compound7\nphosphodiesterase inhibitor,quazinone,Compound8\n"
+        replace_df = pd.read_csv(StringIO(replace_df_string), sep=",")
+
+        df = (
+            pd.read_csv(
+                self.raw_data_dir / "JUMP-MOA_compound_metadata.tsv",
+                sep="\t",
+                dtype=str,
+            )
+            .set_index("pert_iname")
+            .rename(index={old: new for old, new in replace_df[["old", "new"]].values})
+        )
         h5_store = pd.HDFStore(self.processed_h5_file, "w", complevel=9)
 
         h5_store["/JUMP_MOA_compounds"] = df
 
         h5_store["/creation_date"] = pd.Series(str(datetime.datetime.now()))
 
         h5_store.close()
 
         self.register_df_key("JUMP_MOA_compounds")
 
-    def __call__(self)->pd.DataFrame:
+    def __call__(self) -> pd.DataFrame:
         return self.get_df(None)
 
-
     def get_df(self, key: str) -> pd.DataFrame:
         """Get supporting dataframe
 
         Parameters
         ----------
         key : str
             Key of pd.DataFrame.
 
         Returns
         -------
         pd.DataFrame
             Requested pd.DataFrame from h5 store
         """
         store = pd.HDFStore(self.processed_h5_file)
-        if key=="" or key is None:
+        if key == "" or key is None:
             df = store["/JUMP_MOA_compounds"].copy()
         else:
-            df=store["/" + key].copy()
+            df = store["/" + key].copy()
         store.close()
         return df
 
     def get_ds(self, key: str) -> Dataset:
         """Get supporting dataframe
 
         Parameters
@@ -137,25 +146,20 @@
         Dataset
             Requested Phenonaut Dataset from h5 store, with the correctly set
             features and metadata
         """
         return None
 
 
-
-
-
-
-
 class MetadataBROADLincsCellPaintingMOAs(PackagedDataset):
     """DataFrame supplier for BROAD Lincs Cell Painting assigned MOAs
 
     This PackagedDataset provides access to a pd.DataFrame containing information
     on the BROAD institutes LINCS Cell Paiting compound MOA assignment.
-    
+
     This data is located in the broadinstitute/lincs-cell-painting GitHub repository
     under metadata/moa/repurposing_simple.tsv.
 
     https://raw.githubusercontent.com/broadinstitute/lincs-cell-painting/master/metadata/moa/repurposing_simple.tsv
 
     Commentary on creation of this resource which may be useful is also available
     here:
@@ -210,56 +214,56 @@
         Parameters
         ----------
         remove_intermediates : bool, optional
             If true, then the downloaded archive is removed, by default False
         """
         self._download(
             "https://raw.githubusercontent.com/broadinstitute/lincs-cell-painting/master/metadata/moa/repurposing_simple.tsv",
-            self.raw_data_dir/"repurposing_simple.tsv",
+            self.raw_data_dir / "repurposing_simple.tsv",
             mkdir=True,
             skip_if_exists=True,
         )
 
-        df=pd.read_csv(self.raw_data_dir/"repurposing_simple.tsv", sep='\t', dtype=str).set_index("pert_iname")
+        df = pd.read_csv(
+            self.raw_data_dir / "repurposing_simple.tsv", sep="\t", dtype=str
+        ).set_index("pert_iname")
         h5_store = pd.HDFStore(self.processed_h5_file, "w", complevel=9)
 
         h5_store["/Broad_MOA_compounds"] = df
 
         h5_store["/creation_date"] = pd.Series(str(datetime.datetime.now()))
 
         h5_store.close()
 
         self.register_df_key("Broad_MOA_compounds")
 
-    def __call__(self)->pd.DataFrame:
+    def __call__(self) -> pd.DataFrame:
         return self.get_df(None)
 
-
     def get_df(self, key: str) -> pd.DataFrame:
         """Get supporting dataframe
 
         Parameters
         ----------
         key : str
             Key of pd.DataFrame.
 
         Returns
         -------
         pd.DataFrame
             Requested pd.DataFrame from h5 store
         """
         store = pd.HDFStore(self.processed_h5_file)
-        if key=="" or key is None:
-            df=store["/Broad_MOA_compounds"].copy()
+        if key == "" or key is None:
+            df = store["/Broad_MOA_compounds"].copy()
         else:
-            df= store["/" + key].copy()
+            df = store["/" + key].copy()
         store.close()
         return df
 
-
     def get_ds(self, key: str) -> Dataset:
         """Get supporting dataframe
 
         Parameters
         ----------
         key : str
             Key of Phenonaut Dataset.
```

### Comparing `phenonaut-1.3.4/phenonaut/packaged_datasets/tcga.py` & `phenonaut-2.0.3/src/phenonaut/packaged_datasets/tcga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import datetime
+import shutil
 from collections import namedtuple
+from collections.abc import Callable
 from pathlib import Path
-from typing import Callable, Optional, Type, Union
+from typing import Optional, Type, Union
 
-from ..data import Dataset
+import h5py
+import numpy as np
+import pandas as pd
 from pandas.io.parsers import read_csv
+
+from ..data import Dataset
 from .base import PackagedDataset
-import shutil
-import pandas as pd
-import numpy as np
-import h5py
-import datetime
 
 
 class TCGA(PackagedDataset):
     """TCGA - The Cancer Genome Atlas, packaged dataset
 
     The TCGA dataset captures a snapshot of The Cancer Genome Atlas, from
     the TCGA website:
@@ -151,15 +153,17 @@
         download: bool = False,
         raw_data_dir: Optional[Union[Path, str]] = Path("raw_data"),
         rm_downloaded_data: bool = True,
         rm_intermediates: bool = True,
         prediction_target: Optional[str] = None,
         num_pca_dims: Union[int, None] = 10,
         vif_filter_cutoff: Optional[float] = None,
-        custom_transformation_func_and_name_tuple: Optional[tuple[Callable, str]] = None,
+        custom_transformation_func_and_name_tuple: Optional[
+            tuple[Callable, str]
+        ] = None,
     ):
         # List of clinical tumor types within TCGA
         self.tumor_list = [
             "ACC",
             "BLCA",
             "BRCA",
             "CESC",
@@ -210,25 +214,29 @@
             raise ValueError(
                 "custom_transformation_func_and_name_tuple must be a tuple of the form tuple[Callable, str] where str is a short descriptive string to be used in the filename - such as 'UMAP' or 'LDA'"
             )
 
         if custom_transformation_func_and_name_tuple is None:
             self.custom_transformation_func = None
             self.processed_h5_file = (
-                self.root / f"tcga_pca{num_pca_dims}_VIF{self.vif_filter_cutoff}_phenonaut.h5"
+                self.root
+                / f"tcga_pca{num_pca_dims}_VIF{self.vif_filter_cutoff}_phenonaut.h5"
             )
             self.metadata_h5_file = (
                 self.root
                 / f"tcga_pca{num_pca_dims}_VIF{self.vif_filter_cutoff}_metadata_phenonaut.h5"
             )
             self.num_pca_dims = num_pca_dims
         else:
-            self.custom_transformation_func = custom_transformation_func_and_name_tuple[0]
+            self.custom_transformation_func = custom_transformation_func_and_name_tuple[
+                0
+            ]
             self.processed_h5_file = (
-                self.root / f"tcga_{custom_transformation_func_and_name_tuple[1]}_phenonaut.h5"
+                self.root
+                / f"tcga_{custom_transformation_func_and_name_tuple[1]}_phenonaut.h5"
             )
             self.metadata_h5_file = (
                 self.root
                 / f"tcga_{custom_transformation_func_and_name_tuple[1]}_metadata_phenonaut.h5"
             )
 
         # If the dataset is missing, get it
@@ -248,15 +256,17 @@
             )
 
         store = pd.HDFStore(self.processed_h5_file)
         for key in store.keys():
             if key != "/clinical_decisions":
                 self.register_ds_key(key[1:])
         self.register_df_key("clinical_decisions")
-        self.clinical_decisions_df = store["clinical_decisions"].set_index("Hybridization REF")
+        self.clinical_decisions_df = store["clinical_decisions"].set_index(
+            "Hybridization REF"
+        )
         store.close()
 
     def _make_dataset(
         self,
         download: bool = False,
         rm_downloaded_data: bool = True,
         rm_intermediates: bool = True,
@@ -271,30 +281,34 @@
         if download:
             self.__download_TCGA()
         self.__decompress_TCGA()
         self.__merge_data()
         self.__perform_pca_write_h5()
 
     def __download_TCGA(self):
-        remote_base_url = "https://gdac.broadinstitute.org/runs/stddata__2016_01_28/data/"
+        remote_base_url = (
+            "https://gdac.broadinstitute.org/runs/stddata__2016_01_28/data/"
+        )
         filename_suffixes = [
             "Methylation_Preprocess.Level_3.2016012800.0.0.tar.gz",
             "miRseq_Preprocess.Level_3.2016012800.0.0.tar.gz",
             "mRNAseq_Preprocess.Level_3.2016012800.0.0.tar.gz",
             "RPPA_AnnotateWithGene.Level_3.2016012800.0.0.tar.gz",
             "Clinical_Pick_Tier1.Level_4.2016012800.0.0.tar.gz",
         ]
 
         download_tasks = []
         print(f"{download_tasks=}")
         for tumor in self.tumor_list:
             filename_prefix = f"gdac.broadinstitute.org_{tumor}"
             for filename in [f"{filename_prefix}.{fns}" for fns in filename_suffixes]:
                 if not (self.raw_data_dir / Path(filename)).exists():
-                    print(f"Download task: {remote_base_url}{tumor}/20160128/{filename}")
+                    print(
+                        f"Download task: {remote_base_url}{tumor}/20160128/{filename}"
+                    )
                     download_tasks.append(
                         (
                             f"{remote_base_url}{tumor}/20160128/{filename}",
                             self.raw_data_dir / filename,
                         )
                     )
         print(f"Downloading {len(download_tasks)} files")
@@ -356,15 +370,19 @@
                 {"skiprows": [1]},
                 "methylation.csv",
                 2,
                 "Hybridization REF",
                 lambda x: x.lower()[:-3],
             ),
             "mRNA": self.TCGA_MetadataTuple(
-                list(self.raw_data_dir.glob("**/*.uncv2.mRNAseq_RSEM_normalized_log2.txt")),
+                list(
+                    self.raw_data_dir.glob(
+                        "**/*.uncv2.mRNAseq_RSEM_normalized_log2.txt"
+                    )
+                ),
                 {},
                 "mRNAseq_RSEM.csv",
                 1,
                 "gene",
                 lambda x: x.lower()[:-3],
             ),
         }
@@ -375,42 +393,49 @@
                 f"{datetime.datetime.now().strftime('%H:%M:%S')}: Processing {dataset_name} ... ",
                 end="",
             )
             self.__merge_TCGA_files(metadata)
             print(f"{datetime.datetime.now().strftime('%H:%M:%S')}")
 
     def __merge_TCGA_files(self, dataset_metadata: TCGA_MetadataTuple):
-
         if not (self.tmp_dir / dataset_metadata.output_file_name).exists():
             TARGET_TREATMENT_ID = "Hybridization REF"
             dfs = []
             for file in dataset_metadata.files:
                 tumor = str(file.name)[: file.name.find(".")]
 
                 print(f"{tumor}")
 
-                tmp = pd.read_csv(file, sep="\t", header=[0], **dataset_metadata.load_csv_kwargs)
+                tmp = pd.read_csv(
+                    file, sep="\t", header=[0], **dataset_metadata.load_csv_kwargs
+                )
                 tmp = tmp.T.reset_index()
                 tmp.columns = tmp.iloc[0, 0:]
-                tmp = tmp.iloc[dataset_metadata.header_offset :, :].reset_index(drop=True)
+                tmp = tmp.iloc[dataset_metadata.header_offset :, :].reset_index(
+                    drop=True
+                )
                 tmp[TARGET_TREATMENT_ID] = tmp[dataset_metadata.treatment_id].apply(
                     dataset_metadata.treatment_lambda
                 )
                 tmp["disease_code"] = tumor
                 dfs.append(tmp)
 
             merged_df = (
                 pd.concat(dfs)
                 .drop(columns=["Composite Element REF"], errors="ignore")
                 .replace(r"^\s*$", np.nan, regex=True)
             )
             if dataset_metadata.treatment_id != TARGET_TREATMENT_ID:
-                merged_df = merged_df.drop(columns=[dataset_metadata.treatment_id], errors="ignore")
+                merged_df = merged_df.drop(
+                    columns=[dataset_metadata.treatment_id], errors="ignore"
+                )
             del dfs
-            merged_df.to_csv(self.tmp_dir / dataset_metadata.output_file_name, index=False)
+            merged_df.to_csv(
+                self.tmp_dir / dataset_metadata.output_file_name, index=False
+            )
             del merged_df
 
     def __perform_pca_write_h5(self):
         from sklearn.decomposition import PCA
         from sklearn.preprocessing import StandardScaler
 
         store = pd.HDFStore(self.processed_h5_file, "w")
@@ -426,30 +451,39 @@
                 "methylation.csv",
             ]
         ]:
             if self.custom_transformation_func is not None:
                 self.custom_transformation_func(file_path, store)
             else:
                 dataset_type = (
-                    str(file_path.name).split("_")[0].replace(".csv", "").replace("seq", "")
+                    str(file_path.name)
+                    .split("_")[0]
+                    .replace(".csv", "")
+                    .replace("seq", "")
                 )
                 index_column = "Hybridization REF"
                 print(f"Performing dimensionality reduction on {file_path}")
                 df = pd.read_csv(file_path)
                 df = df[df[index_column].astype(str).str.startswith("tcga")]
                 df = df.drop_duplicates(subset=[index_column])
                 df = df[np.asarray(list(df))[df.isna().sum(axis=0) == 0]]
                 df = df.set_index(index_column)
 
                 features = sorted(
-                    [f for f in df.columns.values if f not in [index_column, "disease_code"]]
+                    [
+                        f
+                        for f in df.columns.values
+                        if f not in [index_column, "disease_code"]
+                    ]
                 )
 
                 if self.vif_filter_cutoff is not None:
-                    from phenonaut.transforms.preparative import RemoveHighestCorrelatedThenVIF
+                    from phenonaut.transforms.preparative import (
+                        RemoveHighestCorrelatedThenVIF,
+                    )
 
                     tmp_ds = Dataset("tmp_df", df, {"features": features})
                     print("Num features in dataset:", len(tmp_ds.features))
                     # If there are too many features, then we cannot analyse all
                     # correlations and must abandon
                     if len(tmp_ds.features) <= 1000:
                         r_high_then_vif = RemoveHighestCorrelatedThenVIF(verbose=True)
@@ -592,14 +626,16 @@
         """
         if new_df_column_name is None:
             new_df_column_name = clinical_decision_column
 
         cd_series = self.clinical_decisions_df[clinical_decision_column]
         if custom_func is not None:
             cd_series = cd_series.map(custom_func)
-        df = df.join(cd_series).rename(columns={clinical_decision_column: new_df_column_name})
+        df = df.join(cd_series).rename(
+            columns={clinical_decision_column: new_df_column_name}
+        )
 
         if remove_incomplete_rows:
             df = df[~df[new_df_column_name].isin([np.nan, np.inf, -np.inf])]
         if dtype is not None:
             df[new_df_column_name] = df[new_df_column_name].astype(dtype)
         return df
```

### Comparing `phenonaut-1.3.4/phenonaut/phenonaut.py` & `phenonaut-2.0.3/src/phenonaut/phenonaut.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import gzip
+import pickle
 import warnings
+from base64 import b64encode
+from collections.abc import Callable, Iterable
+from copy import deepcopy
+from hashlib import sha256
+from itertools import combinations as itertools_combinations
+from pathlib import Path
 from random import random
+from typing import List, Optional, Union, Literal
+
+import pandas as pd
 from pandas.errors import DataError
+from sklearn.utils import Bunch
+
 from phenonaut import data
 from phenonaut.data import Dataset
-from typing import Callable, Iterable, List, Optional, Union
-from pathlib import Path
-import pandas as pd
-from itertools import combinations as itertools_combinations
-from sklearn.utils import Bunch
 from phenonaut.packaged_datasets.base import PackagedDataset
-import pickle
-from copy import deepcopy
-import gzip
 from phenonaut.utils import check_path
-from hashlib import sha256
-from base64 import b64encode
 
 
 class Phenonaut:
     """Phenonaut object constructor
 
     Holds multiple datasets of different type, applys transforms, load and
     tracking operations.
@@ -94,36 +97,44 @@
         subsequent experiments. Building up a provable chain along the way.
         By default None, implying an empty bytes array.
     """
 
     def __init__(
         self,
         dataset: Optional[
-            Union[Dataset, list[Dataset], PackagedDataset, Bunch, pd.DataFrame, Path, str]
+            Union[
+                Dataset, list[Dataset], PackagedDataset, Bunch, pd.DataFrame, Path, str
+            ]
         ] = None,
         name: str = "Phenonaut object",
         kind: Optional[str] = None,
         packaged_dataset_name_filter: Optional[Union[list[str], str]] = None,
         metadata: Optional[Union[dict, list[dict]]] = {},
-        features : Optional[list[str]] = None,
+        features: Optional[list[str]] = None,
         dataframe_name: Optional[Union[str, list[str]]] = None,
         init_hash: Optional[Union[str, bytes]] = None,
     ):
-        metadata=deepcopy(metadata)
-        if isinstance(metadata, dict) and 'features' not in metadata and features is not None:
-            metadata['features']=features.copy()
+        metadata = deepcopy(metadata)
+        if (
+            isinstance(metadata, dict)
+            and "features" not in metadata
+            and features is not None
+        ):
+            metadata["features"] = features.copy()
         if init_hash is None:
             self.init_hash = b""
         else:
             if isinstance(init_hash, bytes):
                 self.init_hash = init_hash
             elif isinstance(init_hash, str):
                 self.init_hash = init_hash.encode("utf-8")
             else:
-                raise ValueError(f"The given argument init_hash was not a bytes array or a string")
+                raise ValueError(
+                    f"The given argument init_hash was not a bytes array or a string"
+                )
         self.datasets = []
         self.name = name
         if dataset is None:
             return
         if isinstance(dataset, Phenonaut):
             for ds in dataset.datasets:
                 self.datasets.append(ds.copy())
@@ -173,15 +184,18 @@
         # If Path or string, then read it in
         if isinstance(dataset, (Path, str)):
             if isinstance(dataset, str):
                 dataset = Path(dataset)
             if dataframe_name is None:
                 dataframe_name = str(dataset)
             dataset = Dataset(
-                dataset_name=dataframe_name, input_file_path_or_df=dataset, metadata=metadata, kind=kind
+                dataset_name=dataframe_name,
+                input_file_path_or_df=dataset,
+                metadata=metadata,
+                kind=kind,
             )
 
         # If its a Dataset, or list of datasets, directly add it to self.datasets.
         if isinstance(dataset, (Dataset, pd.DataFrame)):
             dataset = [dataset]
         if isinstance(dataset, list):
             ds_types = list(set(map(type, dataset)))
@@ -214,15 +228,19 @@
                     metadata = [metadata.copy() for dm in range(len(dataset))]
                 if len(metadata) != len(dataset):
                     raise ValueError(
                         f"dataset_metadata contained {len(metadata)} metadata dictionaries, but dataset contained {len(dataset)} pd.DataFrames"
                     )
                 for ds_name, df, ds_metadata in zip(dataframe_name, dataset, metadata):
                     self.datasets.append(
-                        Dataset(dataset_name=ds_name, input_file_path_or_df=df, metadata=ds_metadata)
+                        Dataset(
+                            dataset_name=ds_name,
+                            input_file_path_or_df=df,
+                            metadata=ds_metadata,
+                        )
                     )
                 return
 
             if name is not None:
                 self.name = name
             return
         # If a packaged dataset has been passed, then load it
@@ -268,15 +286,17 @@
         KeyError
             Dataset with the supplied name was not found
         ValueError
             Invalid dataset index
         """
         if isinstance(dataset, str):
             if dataset not in self.keys():
-                raise KeyError(f"'{dataset}' not found as a name in datasets ({self.keys()})")
+                raise KeyError(
+                    f"'{dataset}' not found as a name in datasets ({self.keys()})"
+                )
             return self.datasets[self.keys().index(dataset)]
         elif isinstance(dataset, int):
             return self.datasets[dataset]
         elif isinstance(dataset, (list, tuple)):
             return [self[ds] for ds in dataset]
         else:
             raise ValueError(
@@ -323,15 +343,17 @@
         ------
         KeyError
             Dataset of that name not found
 
         """
         if isinstance(key, str):
             if key not in self.keys():
-                raise KeyError(f"'{key}' not found as a name in datasets ({self.keys()})")
+                raise KeyError(
+                    f"'{key}' not found as a name in datasets ({self.keys()})"
+                )
             del self.datasets[self.keys().index(key)]
             return
         elif isinstance(key, int):
             del self.datasets[key]
             return
 
     def __iter__(self):
@@ -360,15 +382,14 @@
         DataError
             No datasets loaded
         """
         if self.datasets is None or self.datasets == []:
             raise DataError("Attempt to get data, but no dataset loaded")
         return self.datasets[-1].data
 
-
     @property
     def ds(self) -> Dataset:
         """Return the dataset with the highest index in phenonaut.datasets
 
         Returns
         -------
         Dataset
@@ -432,17 +453,21 @@
         for ds in self.datasets:
             combined_ds_hash.update(ds.sha256.digest())
             phenonaut_object_hash.update(ds.sha256.digest())
         phenonaut_object_hash.update(self.name.encode("utf-8"))
 
         return {
             "datasets": ds_hashes,
-            "combined_datasets_hash": b64encode(combined_ds_hash.digest()).decode("utf-8"),
+            "combined_datasets_hash": b64encode(combined_ds_hash.digest()).decode(
+                "utf-8"
+            ),
             "phenonaut_object_name": self.name,
-            "phenonaut_object_hash": b64encode(phenonaut_object_hash.digest()).decode("utf-8"),
+            "phenonaut_object_hash": b64encode(phenonaut_object_hash.digest()).decode(
+                "utf-8"
+            ),
         }
 
     def __delete__(self) -> None:
         """Deconstructor for Phenonaut object
 
         Upon deconstruction of a Phenonaut object, a hash dictionary is
         retrieved and printed to standard output.
@@ -479,19 +504,25 @@
         features : Optional[list[str]]
             Optionally supply a list of features here. If None, then the
             features/feature finding related keys in metadata are used. You may
             also explicitly supply an empty list to explicitly specify that the
             dataset has no features. This is not recommended.
         """
         if dataset_name is None and metadata is not None:
-            dataset_name = metadata.pop("dataset_name", f"Dataset {len(self.datasets)+1}")
+            dataset_name = metadata.pop(
+                "dataset_name", f"Dataset {len(self.datasets)+1}"
+            )
         if features != None:
             metadata["features"] = features
         self.datasets.append(
-            Dataset(dataset_name=dataset_name, input_file_path_or_df=input_file_path, metadata=metadata)
+            Dataset(
+                dataset_name=dataset_name,
+                input_file_path_or_df=input_file_path,
+                metadata=metadata,
+            )
         )
 
     def combine_datasets(
         self,
         dataset_ids_to_combine: Optional[Union[list[str], list[int]]] = None,
         new_name: Optional[str] = None,
         features: list = None,
@@ -542,33 +573,34 @@
             for ds in datasets_to_combine[1:]:
                 if ds.features != features:
                     raise DataError(
                         f"Different features found when combining datasets\n{features}\nvs\n{ds.features}"
                     )
         if new_name is None:
             new_name = f"Combined_dataset from datasets[{dataset_ids_to_combine}]"
-        self.datasets.append(Dataset(dataset_name=new_name, input_file_path_or_df=None, metadata=None))
+        self.datasets.append(
+            Dataset(dataset_name=new_name, input_file_path_or_df=None, metadata=None)
+        )
         self.datasets[-1].df = new_df
         self.datasets[-1]._metadata = new_metadata
         self.datasets[-1].features = (
             features,
             f"Combined datasets at dataset indexes: {dataset_ids_to_combine}",
         )
 
-    def get_dataset_names(self,)->list[str]:
+    def get_dataset_names(self) -> list[str]:
         """Get a list of dataset names
 
         Returns
         -------
         list[str]
             List containing the names of datasets within this Phenonaut object.
         """
         return self.keys()
 
-
     def get_dataset_index_from_name(
         self, name: Union[str, list[str], tuple[str]]
     ) -> Union[int, list[int]]:
         """Get dataset index from name
 
         Given the name of a dataset, return the index of it in datasets list.
         Accepts single string query, or a list/tuple of names to return lists
@@ -745,15 +777,15 @@
 
     def subtract_median_perturbation(
         self,
         perturbation_label: str,
         per_column_name: Optional[str] = None,
         new_features_prefix: str = "SMP_",
     ):
-        """Subtract the median perturbation from all features for all datasets.
+        r"""Subtract the median perturbation from all features for all datasets.
 
         Useful for normalisation within a well/plate format. The median feature
         may be identified through the per_column_name variable, and perturbation
         label. Newly generated features may have their prefixes controled via
         the new_features_prefix argument.
 
         Parameters
@@ -767,17 +799,15 @@
         new_features_prefix : str
             Prefix for new features, each with the median perturbation
             subtracted. By default 'SMP\_' (for subtracted median perturbation).
 
         """
         for ds in self.datasets:
             ds.subtract_median_perturbation(
-                perturbation_label,
-                per_column_name,
-                new_features_prefix,
+                perturbation_label, per_column_name, new_features_prefix
             )
 
     def get_dataset_combinations(
         self,
         min_datasets: Optional[int] = None,
         max_datasets: Optional[int] = None,
         return_indexes: bool = False,
@@ -845,15 +875,15 @@
         composite_identifier_columns: list[str],
         datasets: Union[Iterable[int], Iterable[str], int, str] = -1,
         new_names_or_prefix: Union[list[str], tuple[str], str] = "Aggregated_",
         inplace: bool = False,
         transformation_lookup: dict[str, Union[Callable, str]] = None,
         tranformation_lookup_default_value: Union[str, Callable] = "mean",
     ):
-        """Aggregate multiple or single phenonaut dataset rows
+        r"""Aggregate multiple or single phenonaut dataset rows
 
         If we have a Phenonaut object containing data derived from 2 fields of
         view from a microscopy image, a sensible approach is averaging features.
         If we have the DataFrame below, we may merge FOV 1 and FOV 2, taking the
         mean of all features.  As strings such as filenames should be kept, they
         are concatenated together, separated by a comma, unless the strings are
         the same, in which case just one is used.
@@ -926,21 +956,27 @@
         tranformation_lookup_default_value : Union[str, Callable]
             Transformation to apply if the data type is not found in the
             transformation_lookup_dictionary, can be a callable or string to
             pandas defined string to function shortcut mappings.
             By default "mean".
 
         """
+        if isinstance(composite_identifier_columns, str):
+            composite_identifier_columns = [composite_identifier_columns]
 
         if isinstance(datasets, (int, str)):
             datasets = [datasets]
-        datasets = list(datasets)  # In case generator is consumed by new_names_or_prefix below.
+        datasets = list(
+            datasets
+        )  # In case generator is consumed by new_names_or_prefix below.
 
         if isinstance(new_names_or_prefix, str):
-            new_names_or_prefix = [f"{new_names_or_prefix}{self[idx].name}" for idx in datasets]
+            new_names_or_prefix = [
+                f"{new_names_or_prefix}{self[idx].name}" for idx in datasets
+            ]
 
         if len(new_names_or_prefix) != len(datasets):
             raise ValueError(
                 f"Expected new_names_or_prefix to have the same number of elements as number datasets being worked on. Was {len(new_names_or_prefix)}, when it should be ({len(datasets)})"
             )
         for dsi, new_ds_name in zip(datasets, new_names_or_prefix):
             new_ds = self[dsi].new_aggregated_dataset(
@@ -950,94 +986,17 @@
                 tranformation_lookup_default_value=tranformation_lookup_default_value,
             )
             if inplace:
                 self[dsi] = new_ds
             else:
                 self.datasets.append(new_ds)
 
-    def merge_datasets(
-        self,
-        ids: Optional[Union[list, tuple]] = None,
-        common_merge_columns: Optional[list[str]] = None,
-        new_dataset_name: str = "merged_dataset",
-    ):
-        """Merge Datasets within a Phenonaut object
-
-        With multiple views of an underlying biological system, it is often
-        useful to merge different datasets, for example, DRUG-seq with
-        CellProfiler or similar imaging data. This function merges Datasets
-        and adds the resultant Dataset to the Phenonaut object.  DataFrames are
-        assumed to have common columns which allow the merge to proceed.
-
-        Underneath the hood, Phenonaut uses Panda's pd.merge function, and then
-        handles features and other Phenonaut specific data like features.
-
-        Parameters
-        ----------
-        ids : Optional[Union[list, tuple]], optional
-            A list or tuple containing two indexes, or dataset names contained
-            within the Phenonaut object which should be merged. If None, then
-            it is assumed that the Phenonaut object contains only 2 datasets,
-            and their indexes are then used.  If more than 2 datasets are found
-            and ids is None, then an error is raised. By default None.
-        common_merge_columns : Optional[list[str]], optional
-            Merge datasets on common columns, found within each dataset. This may
-            be things like a treatment ID, WellID, PlateID, etc. If None, then
-            both Datasets are looked at and common columns identified. By
-            default None.
-        new_dataset_name : str, optional
-            Name for the new dataset, by default "merged_dataset".
-
-        Raises
-        ------
-        ValueError
-            The ids argument was None, but more than 2 datasets were found in
-            the Phenonaut object, please specify which Datasets should be
-            merged.
-        ValueError
-            The ids argument contained more than 2 elements.
-        ValueError
-            Datasets contain common feature columns, cannot merge.
-        ValueError
-            No common columns found to perform merge.
-
-        """
-        if ids is None:
-            ids = self.get_dataset_index_from_name(self.keys())
-            if len(ids) != 2:
-                raise ValueError(
-                    f"merge_datasets merges 2 Datasets at a time.  ids was None, and there are {len(ids)} datasets in this Phenonaut object"
-                )
-        if len(ids) != 2:
-            raise ValueError(
-                f"merge_datasets merges 2 Datasets at a time. The ids argument contained {len(ids)} dataset indexes"
-            )
-        if any(f1 in self[ids[1]].features for f1 in self[ids[0]].features):
-            raise ValueError(
-                f"Datasets shared common features, cannot merge, common features were {set(self[ids[0]].features).intersection(set(self[ids[1]].features))}"
-            )
-        if common_merge_columns is None:
-            common_merge_columns = list(
-                set.intersection(*map(set, [self[id].df.columns.tolist() for id in ids]))
-            )
-        if len(common_merge_columns) == 0:
-            raise ValueError("No common columns found in dataframes to perform merge")
-        new_df = pd.merge(self[ids[0]].df, self[ids[1]].df, on=common_merge_columns)
-        # Uniquify features, preserving order
-        merged_features = self[ids[0]].features + self[ids[1]].features
-
-        self.datasets.append(
-            Dataset(
-                dataset_name=new_dataset_name,
-                input_file_path_or_df=new_df,
-                metadata={"features": merged_features},
-            )
-        )
-
-    def save(self, output_filename: Union[str, Path], overwrite_existing: bool = False) -> None:
+    def save(
+        self, output_filename: Union[str, Path], overwrite_existing: bool = False
+    ) -> None:
         """Save Phenonaut object and contained Data to a pickle
 
         Writes a gzipped Python pickle file. If no compression, or another
         compressison format is required, then the user should use a custom
         pickle.dump and not rely on this helper function.
 
         Parameters
@@ -1047,15 +1006,17 @@
         overwrite_existing : bool, optional
             If True and the file exists, overwrite it. By default False.
         """
         for ds in self.datasets:
             ds.sha256 = b64encode(ds.sha256.digest()).decode("utf-8")
         output_filename = check_path(output_filename)
         if output_filename.exists() and not overwrite_existing:
-            raise FileExistsError(f"{output_filename} exists, and overwrite_existing was False")
+            raise FileExistsError(
+                f"{output_filename} exists, and overwrite_existing was False"
+            )
         self.last_saved_pickle_filename = output_filename
         with gzip.open(output_filename, "wb") as f:
             pickle.dump(self, f)
         for ds in self.datasets:
             ds.sha256 = sha256(ds.sha256.encode("utf-8"))
 
     def revert(self) -> None:
@@ -1069,15 +1030,17 @@
         ------
         FileNotFoundError
             File not found, Phenonaut object has never been written out.
 
         """
         if hasattr(self, "last_saved_pickle_filename"):
             if not self.last_saved_pickle_filename.exists():
-                raise FileNotFoundError(f"Could not find file {self.last_saved_pickle_filename}")
+                raise FileNotFoundError(
+                    f"Could not find file {self.last_saved_pickle_filename}"
+                )
             with gzip.open(self.last_saved_pickle_filename, "rb") as f:
                 phe = pickle.load(f)
                 for ds in phe.datasets:
                     ds.sha256 = sha256(ds.sha256.encode("utf-8"))
                 self.__dict__ = phe.__dict__
         else:
             raise FileNotFoundError(
@@ -1107,15 +1070,15 @@
         """
         filepath = check_path(filepath, make_parents=False)
         if not filepath.exists():
             raise FileNotFoundError(f"Could not find file {filepath}")
         with gzip.open(filepath, "rb") as f:
             phe = pickle.load(f)
             if isinstance(phe, Dataset):
-                phe=Phenonaut(phe)
+                phe = Phenonaut(phe)
             for ds in phe.datasets:
                 ds.sha256 = sha256(ds.sha256.encode("utf-8"))
             return phe
 
     def get_df_features_perturbation_column(
         self, ds_index=-1, quiet: bool = False
     ) -> tuple[pd.DataFrame, list[str], Union[str, None]]:
@@ -1146,7 +1109,132 @@
         return (
             self[ds_index].df,
             self[ds_index].features,
             self[ds_index]._metadata.get("perturbation_column", None)
             if quiet
             else self[ds_index].perturbation_column,
         )
+
+    def groupby_datasets(
+        self, by: Union[str, List[str]], ds_index=-1, remove_original=True
+    ):
+        """Perform a groupby operation on a dataset
+
+        Akin to performing a groupby operation on a pd.DataFrame, this splits a dataset
+        by column(s), optionally keeping or removing (by default) the original.
+
+        Parameters
+        ----------
+        by : Union[str, list]
+            Columns in the dataset's DataFrames which should be used for grouping
+        ds_index : int, optional
+            Index of the Dataset to be returned. By default -1, which uses the
+            last added Dataset.
+        remove_original : bool, optional
+            If True, then the original split dataset is deleted after splitting
+        """
+        target_ds = self[ds_index]
+        if remove_original:
+            del self[ds_index]
+        self.datasets.extend(target_ds.groupby(by))
+
+    def merge_datasets(
+        self,
+        datasets: Union[List[Dataset], List[int], Literal["all"]] = "all",
+        new_dataset_name: Optional[str] = "Merged Dataset",
+        return_merged: bool = False,
+        remove_merged: Optional[bool] = True,
+    ):
+        """Merge datasets
+
+        After performing a groupby operation on Phenonaut.Dataset objects, a list of
+        datasets may be merged into a single Dataset using this method.
+
+        Parameters
+        ----------
+        datasets : Union[List[Dataset], List[int], List[str]]
+            Datasets which should be groupbed together. May be a list of Datasets, in
+            which case these are merged together and inserted into the Phenonaut object,
+            or a list of integers or dataset names which will be used to look up
+            datasets in the current Phenonaut object.  Mixing of ints and dataset string
+            identifiers is acceptable but mixing of any identifier and Datasets is not
+            supported. If 'all', then all datasets in the Phenonaut object are merged.
+            By default 'all'
+        return_merged: bool
+            If True the merged dataset is returned by this function. If False, then the
+            new merged dataset is added to the current Phenonaut object.  By default
+            False
+        remove_merged : bool
+            If True and return_merged is False causing the new object to be merged into
+            the Phenonaut object, then source datasets which are in the current object
+            (addressed by index or int in the datasets list) are removed from the
+            Phenonaut object. By default True
+        """
+
+        def _check_features_match(ds_list):
+            first_set = ds_list[0].features
+            if all([d.features == first_set for d in ds_list[1:]]):
+                return True
+            return False
+
+        if isinstance(datasets, str):
+            if datasets == "all":
+                datasets = list(range(len(self.datasets)))
+            else:
+                raise ValueError(
+                    f"'{datasets}' is not a supported value for datasets, try 'all' to merge all, or include datasets, dataset names, or dataset"
+                )
+
+        if len(datasets) == 1:
+            raise ValueError(
+                "Cannot merge when there is only 1 dataset included in the merge"
+            )
+
+        # Check no mix of Datasets and dataset identifiers (int/str)
+        if any([isinstance(d, Dataset) for d in datasets]):
+            if not all([isinstance(d, Dataset) for d in datasets]):
+                raise ValueError(
+                    f"Cannot mix datasets with identifiers, datasets had the types: {[type(d) for d in datasets]}"
+                )
+            # All datasets at this point
+            if not _check_features_match(datasets):
+                raise ValueError(
+                    "Datasets did not have the same features, could not ungroup"
+                )
+            new_ds = datasets[0].copy()
+            new_ds.df = pd.concat([d.df for d in datasets])
+            new_ds.features = (
+                new_ds.features,
+                f"Performed merge_datasets, {return_merged=}, {remove_merged=}",
+            )
+            new_ds.name = new_dataset_name
+            if return_merged:
+                return new_ds
+            else:
+                self.datasets.append(new_ds)
+        else:
+            # All identifiers
+
+            if not _check_features_match([self[d] for d in datasets]):
+                raise ValueError(
+                    "Datasets did not have the same features, could not ungroup"
+                )
+            new_ds = self[datasets[0]].copy()
+            new_ds.df = pd.concat([self[d].df for d in datasets])
+            new_ds.features = (
+                new_ds.features,
+                f"Performed merge_datasets, {return_merged=}, {remove_merged=}",
+            )
+            new_ds.name = new_dataset_name
+            if return_merged:
+                return new_ds
+            else:
+                if remove_merged:
+                    for d in reversed(datasets):
+                        if isinstance(d, int):
+                            del self[d]
+                        else:
+                            del self[self.get_dataset_index_from_name(d)]
+                self.datasets.append(new_ds)
+
+    def __repr__(self):
+        return f"Phenonaut object (name = {self.name}), {len(self.datasets)} datasets, dataset names = {[d.name for d in self.datasets]})"
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/default_predictors/classifiers.py` & `phenonaut-2.0.3/src/phenonaut/predict/default_predictors/classifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+from mvlearn.semi_supervised import CTClassifier
+from sklearn.discriminant_analysis import QuadraticDiscriminantAnalysis
+from sklearn.ensemble import AdaBoostClassifier, RandomForestClassifier
+from sklearn.gaussian_process import GaussianProcessClassifier
 from sklearn.naive_bayes import GaussianNB
-from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
 from sklearn.neighbors import KNeighborsClassifier
+from sklearn.neural_network import MLPClassifier
 from sklearn.svm import SVC
-from sklearn.gaussian_process import GaussianProcessClassifier
 from sklearn.tree import DecisionTreeClassifier
-from sklearn.neural_network import MLPClassifier
-from sklearn.discriminant_analysis import QuadraticDiscriminantAnalysis
-from mvlearn.semi_supervised import CTClassifier
+
 from phenonaut.predict.predictor_dataclasses import (
-    PhenonautPredictor,
-    HyperparameterInt,
-    HyperparameterFloat,
     HyperparameterCategorical,
+    HyperparameterFloat,
+    HyperparameterInt,
     HyperparameterLog,
+    PhenonautPredictor,
 )
 
 default_classifiers = [
     PhenonautPredictor("Naive Bayes", GaussianNB),
     PhenonautPredictor(
         "Random Forest",
         RandomForestClassifier,
         [
             HyperparameterCategorical("max_depth", (5, 10, 20, None)),
             HyperparameterInt("n_estimators", 50, 200),
-            HyperparameterCategorical("max_features", (None, "auto", "log2")),
+            HyperparameterCategorical("max_features", (None, "sqrt", "log2")),
         ],
         constructor_kwargs={"n_jobs": -1},
     ),
     PhenonautPredictor(
         "KNN",
         KNeighborsClassifier,
         HyperparameterInt("n_neighbors", 2, 10),
@@ -56,36 +57,35 @@
             HyperparameterCategorical("gamma", ("scale", "auto")),
         ],
         dataset_size_cutoff=1000,
     ),
     PhenonautPredictor(
         "Gaussian Process",
         GaussianProcessClassifier,
-        constructor_kwargs={
-            "copy_X_train": False,
-            "n_jobs": -1,
-        },
+        constructor_kwargs={"copy_X_train": False, "n_jobs": -1},
         embed_in_results=False,
     ),
     PhenonautPredictor(
         "Decision Tree",
         DecisionTreeClassifier,
         [
             HyperparameterCategorical("criterion", ("gini", "entropy")),
             HyperparameterCategorical("max_depth", (None, 5, 10, 15, 20)),
-            HyperparameterCategorical("max_features", (None, "auto", "log2")),
+            HyperparameterCategorical("max_features", (None, "sqrt", "log2")),
         ],
     ),
     PhenonautPredictor(
         "SciKit NeuralNet",
         MLPClassifier,
         [
             HyperparameterLog("alpha", 0.00001, 0.001),
             HyperparameterCategorical("solver", ["adam", "sgd"]),
             HyperparameterCategorical("max_iter", [1000]),
             HyperparameterCategorical("learning_rate", ["constant", "adaptive"]),
         ],
     ),
     PhenonautPredictor("AdaBoost", AdaBoostClassifier),
     PhenonautPredictor("QDA", QuadraticDiscriminantAnalysis),
-    PhenonautPredictor("mvlearn CTClassifier (GNB,GNB)", CTClassifier, num_views=2, max_classes=2),
+    PhenonautPredictor(
+        "mvlearn CTClassifier (GNB,GNB)", CTClassifier, num_views=2, max_classes=2
+    ),
 ]
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/default_predictors/multiregressors.py` & `phenonaut-2.0.3/src/phenonaut/predict/default_predictors/multiregressors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+from sklearn.dummy import DummyRegressor
 from sklearn.ensemble import GradientBoostingRegressor
-from sklearn.multioutput import MultiOutputRegressor
 from sklearn.linear_model import LinearRegression
-from sklearn.dummy import DummyRegressor
-from phenonaut.predict.default_predictors.pytorch_models import MultiRegressorNN, DAVE
+from sklearn.multioutput import MultiOutputRegressor
+
+from phenonaut.predict.default_predictors.pytorch_models import (
+    DAVE,
+    MultiRegressorNN,
+)
 from phenonaut.predict.predictor_dataclasses import (
-    PhenonautPredictor,
-    HyperparameterInt,
-    HyperparameterFloat,
     HyperparameterCategorical,
+    HyperparameterFloat,
+    HyperparameterInt,
     HyperparameterLog,
+    PhenonautPredictor,
 )
 
 default_multiregressors = [
-    PhenonautPredictor("DummyRegressor-Average", (MultiOutputRegressor, DummyRegressor)),
     PhenonautPredictor(
-        "MultiOutputRegressor-LinearRegression", (MultiOutputRegressor, LinearRegression)
+        "DummyRegressor-Average", (MultiOutputRegressor, DummyRegressor)
+    ),
+    PhenonautPredictor(
+        "MultiOutputRegressor-LinearRegression",
+        (MultiOutputRegressor, LinearRegression),
     ),
     PhenonautPredictor(
         "MultiOutputRegressor-GradientBoosting",
         (MultiOutputRegressor, GradientBoostingRegressor),
         [
             HyperparameterFloat("learning_rate", 0.05, 0.2),
             HyperparameterInt("n_estimators", 1, 200),
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/default_predictors/pytorch_models/dave.py` & `phenonaut-2.0.3/src/phenonaut/predict/default_predictors/pytorch_models/dave.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+from pathlib import Path
 from typing import Optional, Union
+
+import numpy as np
 import torch
 import torch.utils.data
 from torch import nn, optim
 from torch.nn import functional as F
-from pathlib import Path
-import numpy as np
 
 
 class _DAVE_model(nn.Module):
     def _topol_to_inout_tuples(
         self, input: np.ndarray
     ) -> tuple[tuple[int, ...], tuple[int, int], tuple[tuple[int, ...]]]:
         """DAVE topology to view encoder sizes tuple list, embeding tuple, and decoder tuple list
@@ -37,39 +38,44 @@
             element 1 = 2 member tuple giving embedding space input and output sizes
             element 2 = List of decoder node input output tuples
         """
         encoding = [(input[0], input[1])]
         for i in range(2, len(input) - 1):
             encoding.append((encoding[-1][1], input[i]))
         embedding = (input[-2], input[-1])
-        decoding = [(embedding[1], encoding[-1][1])] + list((t[1], t[0]) for t in encoding[::-1])
+        decoding = [(embedding[1], encoding[-1][1])] + list(
+            (t[1], t[0]) for t in encoding[::-1]
+        )
         return (encoding, embedding, decoding)
 
     def _assign_layers(self, topology: tuple[tuple[int, ...], tuple[int, ...]]):
-
         self.encoder1 = nn.ModuleList()
         self.encoder2 = nn.ModuleList()
         self.decoder1 = nn.ModuleList()
         self.decoder2 = nn.ModuleList()
 
         # Set up network nodes for view 1 - also do embedding here
-        encoder_dims, embedding_dims, decoder_dims = self._topol_to_inout_tuples(topology[0])
+        encoder_dims, embedding_dims, decoder_dims = self._topol_to_inout_tuples(
+            topology[0]
+        )
         for dims in encoder_dims:
             self.encoder1.append(nn.Linear(*dims))
             self.encoder1.append(nn.ReLU())
         self.latent1 = nn.Linear(*embedding_dims)
         self.latent2 = nn.Linear(*embedding_dims)
         for dims in decoder_dims[:-1]:
             self.decoder1.append(nn.Linear(*dims))
             self.decoder1.append(nn.ReLU())
         self.decoder1.append(nn.Linear(*decoder_dims[-1]))
         self.decoder1.append(nn.Sigmoid())
 
         # Set up network nodes for view 2 - embedding already initialised above
-        encoder_dims, embedding_dims, decoder_dims = self._topol_to_inout_tuples(topology[1])
+        encoder_dims, embedding_dims, decoder_dims = self._topol_to_inout_tuples(
+            topology[1]
+        )
         for dims in encoder_dims:
             self.encoder2.append(nn.Linear(*dims))
             self.encoder2.append(nn.ReLU())
         for dims in decoder_dims[:-1]:
             self.decoder2.append(nn.Linear(*dims))
             self.decoder2.append(nn.ReLU())
         self.decoder2.append(nn.Linear(*decoder_dims[-1]))
@@ -82,16 +88,20 @@
         n_hidden: Union[int, tuple[int, int], list[int, int]] = (3, 3),
         topology: tuple[tuple[int, ...], tuple[int, ...]] = None,
     ):
         super().__init__()
         if isinstance(n_hidden, int):
             n_hidden = (n_hidden, n_hidden)
         if topology is None:
-            view_1 = np.linspace(view_sizes[0], embedding_size, n_hidden[0] + 2, dtype=int)
-            view_2 = np.linspace(view_sizes[1], embedding_size, n_hidden[1] + 2, dtype=int)
+            view_1 = np.linspace(
+                view_sizes[0], embedding_size, n_hidden[0] + 2, dtype=int
+            )
+            view_2 = np.linspace(
+                view_sizes[1], embedding_size, n_hidden[1] + 2, dtype=int
+            )
             # Num inputs to latent space must be the same for each view.
             if view_1[-2] != view_2[-2]:
                 if len(view_1) < 3 or len(view_2) < 3:
                     raise ValueError(
                         "Node sizes leading into embedding space were not the same, and with no hidden layers, "
                         "the sizes could not be averaged to give view 1 and view 2 pre-embedding layer the same number of inputs"
                     )
@@ -182,15 +192,18 @@
         # https://arxiv.org/abs/1312.6114
         # 0.5 * sum(1 + log(sigma^2) - mu^2 - sigma^2)
         kldA = -0.5 * torch.sum(1 + logvarA - muA.pow(2) - logvarA.exp())
         kldB = -0.5 * torch.sum(1 + logvarB - muB.pow(2) - logvarB.exp())
         return bceA + bceB + kldA + kldB
 
     def fit(self, X, y):
-        if self.model.topology[0][0] != X.shape[1] or self.model.topology[1][0] != y.shape[1]:
+        if (
+            self.model.topology[0][0] != X.shape[1]
+            or self.model.topology[1][0] != y.shape[1]
+        ):
             self.model = _DAVE_model(
                 view_sizes=(X.shape[1], y.shape[1]), n_hidden=self.num_hidden_layers
             ).to(self.device)
         print(
             f"Constructed DAVE model on {self.device}, {self.batch_size=}, {self.learning_rate=}, {self.epochs=}, {self.num_hidden_layers=}"
         )
         y = torch.tensor(y.astype(np.float32))
@@ -211,20 +224,26 @@
                 # get the inputs; data is a list of [inputs, labels]
                 X_train, y_train = data
                 X_train = X_train.to(self.device)
                 y_train = y_train.to(self.device)
 
                 # zero the parameter gradients
                 optimizer.zero_grad()
-                reconA, reconB, muA, muB, logvarA, logvarB = self.model(X_train, y_train)
+                reconA, reconB, muA, muB, logvarA, logvarB = self.model(
+                    X_train, y_train
+                )
                 loss = self.loss_function(
                     reconA, reconB, X_train, y_train, muA, muB, logvarA, logvarB
                 )
                 loss.backward()
                 epoch_loss += loss.item()
                 optimizer.step()
 
     def predict(self, X):
         self.model.eval()
         with torch.no_grad():
             data = torch.tensor(X.astype(np.float32)).to(self.device)
-            return self.model.decode_view2(self.model.encode_view1(data)[0]).to("cpu").numpy()
+            return (
+                self.model.decode_view2(self.model.encode_view1(data)[0])
+                .to("cpu")
+                .numpy()
+            )
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/default_predictors/pytorch_models/multiregressor_nn.py` & `phenonaut-2.0.3/src/phenonaut/predict/default_predictors/pytorch_models/multiregressor_nn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+from pathlib import Path
 from typing import Optional, Union
+
+import numpy as np
 import torch
 import torch.utils.data
 from torch import nn, optim
 from torch.nn import functional as F
-from pathlib import Path
-import numpy as np
 
 
 class _MRegressorNN(nn.Module):
     def __init__(self, network_shape):
         super().__init__()
         self.layers = nn.ModuleList()
         for nodes_i in range(len(network_shape) - 1):
-            self.layers.append(nn.Linear(network_shape[nodes_i], network_shape[nodes_i + 1]))
+            self.layers.append(
+                nn.Linear(network_shape[nodes_i], network_shape[nodes_i + 1])
+            )
             self.layers.append(nn.ReLU())
         self.layers.append(nn.Linear(network_shape[-2], network_shape[-1]))
         self.layers.append(nn.Sigmoid())
 
     def forward(self, x):
         for layer in self.layers[:-1]:
             x = layer(x)
@@ -29,67 +32,61 @@
 class MultiRegressorNN:
     def __init__(
         self,
         batch_size=128,
         learning_rate=1e-3,
         epochs=100,
         num_hidden_layers=1,
-        hidden_layer_sizes: Optional[list[int]] = None,
+        hidden_layer_sizes: list[int] | None = None,
         use_optimizer: str = "ADAM",
-        seed: Optional[int] = None,
+        seed: int | None = None,
     ):
         if seed is not None:
             torch.manual_seed(seed)
         self.batch_size = batch_size
         self.learning_rate = learning_rate
         self.epochs = epochs
         self.num_hidden_layers = num_hidden_layers
         self.use_optimizer = use_optimizer
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.hidden_layer_sizes = hidden_layer_sizes
         if self.hidden_layer_sizes is None:
-            self.network_shape = np.linspace(100, 100, num=self.num_hidden_layers + 2, dtype=int)
-        else:
-            self.network_shape = np.array(
-                [
-                    100,
-                ]
-                + self.hidden_layer_sizes
-                + [100]
+            self.network_shape = np.linspace(
+                100, 100, num=self.num_hidden_layers + 2, dtype=int
             )
+        else:
+            self.network_shape = np.array([100] + self.hidden_layer_sizes + [100])
         self.model = _MRegressorNN(self.network_shape).to(self.device)
 
     def fit(self, X, y):
         if self.network_shape[0] != X.shape[1] or self.network_shape[-1] != y.shape[1]:
             del self.model
             if self.hidden_layer_sizes is None:
                 self.network_shape = np.linspace(
                     X.shape[1], y.shape[1], num=self.num_hidden_layers + 2, dtype=int
                 )
             else:
                 self.network_shape = np.array(
-                    [
-                        X.shape[1],
-                    ]
-                    + self.hidden_layer_sizes
-                    + [y.shape[1]]
+                    [X.shape[1]] + self.hidden_layer_sizes + [y.shape[1]]
                 )
             self.model = _MRegressorNN(self.network_shape).to(self.device)
         y = torch.tensor(y.astype(np.float32))
         X = torch.tensor(X.astype(np.float32))
         train_tensor = torch.utils.data.TensorDataset(X, y)
         train_loader = torch.utils.data.DataLoader(
             dataset=train_tensor, batch_size=self.batch_size, shuffle=True
         )
 
         optimizer = None
         if self.use_optimizer == "ADAM":
             optimizer = optim.Adam(self.model.parameters(), lr=self.learning_rate)
         elif self.use_optimizer == "SGD":
-            optimizer = optim.SGD(self.model.parameters(), lr=self.learning_rate, momentum=0.9)
+            optimizer = optim.SGD(
+                self.model.parameters(), lr=self.learning_rate, momentum=0.9
+            )
         else:
             raise ValueError(
                 f"Valid options for use_optimizer argument are 'ADAM' or 'SGD', use_optimizer was {self.use_optimizer}"
             )
         criterion = nn.MSELoss()
         self.model.train()
         for epoch in range(self.epochs):  # loop over the dataset multiple times
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/default_predictors/regressors.py` & `phenonaut-2.0.3/src/phenonaut/predict/default_predictors/regressors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from sklearn.ensemble import RandomForestRegressor, AdaBoostRegressor, GradientBoostingRegressor
-from sklearn.tree import DecisionTreeRegressor
-from sklearn.svm import SVR
+from sklearn.ensemble import (
+    AdaBoostRegressor,
+    GradientBoostingRegressor,
+    RandomForestRegressor,
+)
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.neighbors import KNeighborsRegressor
 from sklearn.neural_network import MLPRegressor
+from sklearn.svm import SVR
+from sklearn.tree import DecisionTreeRegressor
+
 from phenonaut.predict.predictor_dataclasses import (
-    PhenonautPredictor,
-    HyperparameterInt,
-    HyperparameterFloat,
     HyperparameterCategorical,
+    HyperparameterFloat,
+    HyperparameterInt,
     HyperparameterLog,
+    PhenonautPredictor,
 )
 
 default_regressors = [
     PhenonautPredictor(
         "Random Forest",
         RandomForestRegressor,
         [
             HyperparameterCategorical("max_depth", [5, 10, 20, None]),
             HyperparameterInt("n_estimators", 50, 200),
-            HyperparameterCategorical("max_features", [None, "auto", "log2"]),
+            HyperparameterCategorical("max_features", (None, "sqrt", "log2")),
         ],
         constructor_kwargs={"n_jobs": -1},
     ),
     PhenonautPredictor(
         "Linear SVR",
         SVR,
         [
@@ -43,15 +48,17 @@
             HyperparameterCategorical("kernel", ["rbf"]),
             HyperparameterLog("C", 0.001, 10),
             HyperparameterCategorical("gamma", ["scale", "auto"]),
         ],
         dataset_size_cutoff=1000,
     ),
     PhenonautPredictor(
-        "AdaBoost Regressor", AdaBoostRegressor, HyperparameterInt("n_estimators", 50, 200)
+        "AdaBoost Regressor",
+        AdaBoostRegressor,
+        HyperparameterInt("n_estimators", 50, 200),
     ),
     PhenonautPredictor("Gradient Boosting Regressor", GradientBoostingRegressor),
     PhenonautPredictor("Decision Tree Regressor", DecisionTreeRegressor),
     PhenonautPredictor(
         "Gaussian Process Regressor",
         GaussianProcessRegressor,
         constructor_kwargs={"copy_X_train": False},
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/optuna_functions.py` & `phenonaut-2.0.3/src/phenonaut/predict/optuna_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import base64
+import gzip
 from copy import deepcopy
-from sklearn.model_selection import KFold
-from phenonaut.predict.predictor_dataclasses import PhenonautPredictionMetric, PhenonautPredictor
-import numpy as np
-import optuna
-from typing import Optional, Union
+from pathlib import Path
 from pickle import dumps as pickle_dumps
 from pickle import loads as pickle_loads
 from timeit import default_timer
-import base64
-import gzip
-from pathlib import Path
-import phenonaut
+from typing import Optional, Union
 
+import numpy as np
+import optuna
+from sklearn.model_selection import KFold
+
+import phenonaut
 from phenonaut.predict.predict_utils import PredictionType
+from phenonaut.predict.predictor_dataclasses import (
+    PhenonautPredictionMetric,
+    PhenonautPredictor,
+)
 
 
 def predictor_to_str(ob: PhenonautPredictor) -> str:
     """Encode a PhenonautPredictor (or any serialisable object) to str
 
     First serialise the object using pickle.dumps, compress using gzip and
     return the base64 string representation.  Works with any serialisable
@@ -66,15 +70,15 @@
     predictor: PhenonautPredictor,
     metric: PhenonautPredictionMetric,
     n_optuna_trials: int,
     phe_name: str,
     dataset_combination: list[str],
     optuna_db_path: Union[Path, str],
     n_splits: int = 5,
-    seed: Optional[int] = None,
+    random_state: Optional[Union[int, np.random.Generator]] = None,
     optuna_db_protocol: str = "sqlite:///",
     target_dataset_name: Optional[str] = None,
 ):
     """Run Optuna-led hyperparameter optimisation on predictor and data
 
     Parameters
     ----------
@@ -100,37 +104,43 @@
         Name of the Phenonaut object from which the data comes
     dataset_combination : list[str]
         Combination views of datasets to be used
     optuna_db_path : Union[Path, str]
         Output file path for Optuna sqlite3 database file
     n_splits : int, optional
         Number of splits to be used in cross fold validation, by default 5
-    seed : Optional[int], optional
+    random_state : Optional[Union[int, np.random.Generator]], optional
         Seed for use by random number generator, allow deterministing repeats.
         If None, then do no pre-seed the generator. By default None
     optuna_db_protocol : _type_, optional
         Protocol for optuna to use to access storage. By default "sqlite:///"
     target_dataset_name : Optional[str], optional
         If predicting a view, then the target Dataset may be given a name,
         by default None.
     """
 
     # First, we make a deepcopy of predictor, as the type is mutable, and we will be changing it in
     # this function, adding a member variable to obtain the trained predictor back from the
     # augmented optuna objective function.
     predictor = deepcopy(predictor)
+
+    if isinstance(random_state, np.random.Generator):
+        random_state = random_state.integers(int(1e9))
+
     # If predictor has max_optuna_trials set lower than max_optuna trials supplied by the function arg,
     # then take the lower. If not set, then we can use all trials denoted by n_optuna_trials argument.
     if predictor.max_optuna_trials is None:
         n_optuna_trials_for_predictor = n_optuna_trials
     else:
-        n_optuna_trials_for_predictor = min(predictor.max_optuna_trials, n_optuna_trials)
+        n_optuna_trials_for_predictor = min(
+            predictor.max_optuna_trials, n_optuna_trials
+        )
 
     for fold_index, (train_indexes, validation_indexes) in enumerate(
-        KFold(n_splits=n_splits, shuffle=True, random_state=seed).split(
+        KFold(n_splits=n_splits, shuffle=True, random_state=random_state).split(
             X[0] if isinstance(X, list) else X
         )
     ):
         if isinstance(X, list):
             X_train = [X[i][train_indexes] for i in range(len(X))]
             X_val = [X[i][validation_indexes] for i in range(len(X))]
         else:
@@ -167,31 +177,27 @@
 
         # It is a new study, set the user attributes for ease of analysis
         if len(optuna_study.trials) == 0:
             optuna_study.set_user_attr("phe_obj_name", phe_name)
             optuna_study.set_user_attr("predictor_name", predictor.name)
             optuna_study.set_user_attr("dataset", ":".join(dataset_combination))
             optuna_study.set_user_attr("prediction_type", prediction_type.name)
-            if prediction_type == PredictionType.view and target_dataset_name is not None:
+            if (
+                prediction_type == PredictionType.view
+                and target_dataset_name is not None
+            ):
                 optuna_study.set_user_attr("predicting_view", target_dataset_name)
             optuna_study.set_user_attr("metric_name", metric.name)
             optuna_study.set_user_attr("lower_is_better", metric.lower_is_better)
             optuna_study.set_user_attr("merge_folds", False)
             optuna_study.set_user_attr("fold_index", fold_index + 1)
         start_time = default_timer()
         optuna_study.optimize(
             lambda trial: _optuna_augmented_objective(
-                trial,
-                optuna_study,
-                X_train,
-                X_val,
-                y_train,
-                y_val,
-                predictor,
-                metric,
+                trial, optuna_study, X_train, X_val, y_train, y_val, predictor, metric
             ),
             n_trials=n_optuna_trials_for_predictor,
         )
         optuna_study.set_user_attr("time_taken", default_timer() - start_time)
         test_score = metric(y_test, predictor._best_predictor_instance.predict(X_test))
         optuna_study.set_user_attr("test_score", test_score)
 
@@ -234,15 +240,15 @@
     """
     optuna_dict = {}
     if predictor.optuna is None:
         optuna_dict = {}
     else:
         optuna_dict = {
             hyperparameter.name: getattr(trial, hyperparameter.optuna_func)(
-                hyperparameter.name, *hyperparameter.parameters
+                hyperparameter.name, *hyperparameter.parameters, **hyperparameter.kwargs
             )
             for hyperparameter in predictor.optuna
         }
 
     if predictor.conditional_hyperparameter_generator is not None:
         optuna_dict.update(
             predictor.conditional_hyperparameter_generator(
@@ -254,15 +260,17 @@
             )
         )
     if isinstance(predictor.predictor, tuple):
         predictor_instance = predictor.predictor[0](
             predictor.predictor[1](**optuna_dict, **predictor.constructor_kwargs)
         )
     else:
-        predictor_instance = predictor.predictor(**optuna_dict, **predictor.constructor_kwargs)
+        predictor_instance = predictor.predictor(
+            **optuna_dict, **predictor.constructor_kwargs
+        )
     predictor_instance.fit(X_train, y_train)
     score = metric(y_val, predictor_instance.predict(X_val))
 
     # If not yet set (because its a new study with 0 trials and was initialised to None, then set it to the current score)
     if "best_trained_model_score" not in optuna_study.user_attrs:
         optuna_study.set_user_attr("best_trained_model_score", score)
     if not hasattr(predictor, "_best_predictor_instance"):
@@ -288,36 +296,36 @@
     predictor: PhenonautPredictor,
     metric: PhenonautPredictionMetric,
     n_optuna_trials: int,
     phe_name: str,
     dataset_combination: list[str],
     optuna_db_path: Union[Path, str],
     n_splits: int = 5,
-    seed: Optional[int] = None,
+    random_state: Optional[int] = None,
     optuna_db_protocol: str = "sqlite:///",
     target_dataset_name: Optional[str] = None,
 ):
     # First, we make a deepcopy of predictor, as the type is mutable, and we will be changing it in
     # this function, adding a member variable to obtain the trained predictor back from the
     # augmented optuna objective function.
     predictor = deepcopy(predictor)
     # If predictor has max_optuna_trials set lower than max_optuna trials supplied by the function arg,
     # then take the lower. If not set, then we can use all trials denoted by n_optuna_trials argument.
     if predictor.max_optuna_trials is None:
         n_optuna_trials_for_predictor = n_optuna_trials
     else:
-        n_optuna_trials_for_predictor = min(predictor.max_optuna_trials, n_optuna_trials)
+        n_optuna_trials_for_predictor = min(
+            predictor.max_optuna_trials, n_optuna_trials
+        )
 
     # Name the study- must be unique for predictor/dataset/target predictions
     if prediction_type == PredictionType.view and target_dataset_name is not None:
         optuna_study_name = f"{phe_name};{prediction_type.name};{predictor.name};{dataset_combination};{target_dataset_name};merge_folds"
     else:
-        optuna_study_name = (
-            f"{phe_name};{prediction_type.name};{predictor.name};{dataset_combination};merge_folds"
-        )
+        optuna_study_name = f"{phe_name};{prediction_type.name};{predictor.name};{dataset_combination};merge_folds"
 
     # Load study
     optuna_study = optuna.create_study(
         study_name=optuna_study_name,
         storage=f"{optuna_db_protocol}{optuna_db_path}",
         load_if_exists=True,
         direction="minimize" if metric.lower_is_better else "maximize",
@@ -345,15 +353,22 @@
             optuna_study.set_user_attr("predicting_view", target_dataset_name)
         optuna_study.set_user_attr("metric_name", metric.name)
         optuna_study.set_user_attr("lower_is_better", metric.lower_is_better)
         optuna_study.set_user_attr("merge_folds", True)
     start_time = default_timer()
     optuna_study.optimize(
         lambda trial: _optuna_augmented_objective_merge_folds(
-            trial, optuna_study, X, y, predictor, metric, n_splits, seed=seed
+            trial,
+            optuna_study,
+            X,
+            y,
+            predictor,
+            metric,
+            n_splits,
+            random_state=random_state,
         ),
         n_trials=n_optuna_trials_for_predictor,
     )
     optuna_study.set_user_attr("time_taken", default_timer() - start_time)
     test_score = metric(y_test, predictor._best_predictor_instance.predict(X_test))
     optuna_study.set_user_attr("test_score", test_score)
 
@@ -362,16 +377,18 @@
     trial: optuna.Trial,
     optuna_study: optuna.Study,
     X: Union[list[np.ndarray], np.ndarray],
     y: np.ndarray,
     predictor: PhenonautPredictor,
     metric: PhenonautPredictionMetric,
     n_splits: int = 5,
-    seed=None,
+    random_state=None,
 ):
+    if isinstance(random_state, np.random.Generator):
+        random_state = random_state.integers(int(1e9))
     scores = []
     optuna_dict = {}
     if predictor.optuna is None:
         optuna_dict = {}
     else:
         optuna_dict = {
             hyperparameter.name: getattr(trial, hyperparameter.optuna_func)(
@@ -388,31 +405,33 @@
                 optuna_dict,
                 X.shape[1],
                 y.shape[1] if y.ndim == 2 else 1,
             )
         )
 
     if isinstance(predictor.predictor, tuple):
-        predictor_instance = predictor.predictor[0](predictor.predictor[1](**optuna_dict))
+        predictor_instance = predictor.predictor[0](
+            predictor.predictor[1](**optuna_dict)
+        )
     else:
         predictor_instance = predictor.predictor(**optuna_dict)
 
     # multi view
     if isinstance(X, list):
         for train_indexes, validation_indexes in KFold(
-            n_splits=n_splits, shuffle=True, random_state=seed
+            n_splits=n_splits, shuffle=True, random_state=random_state
         ).split(X[0]):
             mv_X_train = [X[i][train_indexes] for i in range(len(X))]
             mv_X_test = [X[i][validation_indexes] for i in range(len(X))]
             predictor_instance.fit(mv_X_train, y[train_indexes])
             y_pred = predictor_instance.predict(mv_X_test)
             scores.append(metric(y[validation_indexes], y_pred))
     else:
         for train_indexes, validation_indexes in KFold(
-            n_splits=n_splits, shuffle=True, random_state=seed
+            n_splits=n_splits, shuffle=True, random_state=random_state
         ).split(X):
             predictor_instance.fit(X[train_indexes], y[train_indexes])
             y_pred = predictor_instance.predict(X[validation_indexes])
             scores.append(metric(y[validation_indexes], y_pred))
 
     # If not yet set (because its a new study with 0 trials and was initialised to None, then set it to the current score)
     if "best_trained_model_score" not in optuna_study.user_attrs:
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/predict_utils.py` & `phenonaut-2.0.3/src/phenonaut/predict/predict_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+from enum import Enum, auto
+from functools import reduce
 from pathlib import Path
-import pandas as pd
+from typing import Optional, Tuple, Union
+
 import numpy as np
-from functools import reduce
+import pandas as pd
 
 import phenonaut.data
-from typing import Optional, Tuple, Union
 from phenonaut.data import dataset
-
 from phenonaut.data.dataset import Dataset
 from phenonaut.phenonaut import Phenonaut
-from phenonaut.predict.predictor_dataclasses import PhenonautPredictionMetric, PhenonautPredictor
-from enum import Enum, auto
+from phenonaut.predict.predictor_dataclasses import (
+    PhenonautPredictionMetric,
+    PhenonautPredictor,
+)
+
 
 # The PredictionType enum is used in multiple places to denote the prediction task.
 # 'view' is simply multi-y-regression for prediction either different views, or multiple
 # properties at the same time
 class PredictionType(Enum):
     """PredictionType Enum for classification, regression or view prediction.
 
@@ -31,15 +35,18 @@
     classification = auto()
     regression = auto()
     view = auto()
 
 
 def get_y_from_target(
     data: Union[
-        phenonaut.data.Dataset, pd.DataFrame, list[phenonaut.data.Dataset], list[pd.DataFrame]
+        phenonaut.data.Dataset,
+        pd.DataFrame,
+        list[phenonaut.data.Dataset],
+        list[pd.DataFrame],
     ],
     target: Optional[Union[str, pd.Series, np.ndarray, tuple]] = None,
 ) -> Union[list, pd.Series, tuple, np.ndarray]:
     """Get target y from Dataset(s) or DataFrame
 
     Parameters
     ----------
@@ -229,23 +236,27 @@
     """
     import optuna
 
     df_dict_list = []
     if isinstance(optuna_db_file, str):
         optuna_db_file = Path(optuna_db_file)
     if not optuna_db_file.exists():
-        raise FileNotFoundError(f"Could not find optuna database file ({optuna_db_file})")
+        raise FileNotFoundError(
+            f"Could not find optuna database file ({optuna_db_file})"
+        )
     study_names = [
         study.study_name
         for study in optuna.study.get_all_study_summaries(
             storage=f"sqlite:///{optuna_db_file.resolve()}"
         )
     ]
     for study_name in study_names:
-        study = optuna.study.load_study(study_name, storage=f"sqlite:///{optuna_db_file.resolve()}")
+        study = optuna.study.load_study(
+            study_name, storage=f"sqlite:///{optuna_db_file.resolve()}"
+        )
         if get_only_best_per_study:
             # If optuna is interuped with CTRL+C when using an sqlite database, then an sqlite database
             # can have a study, but no trials, resulting in a crash here. The following issue addresses
             # the problem:  https://github.com/optuna/optuna/issues/2101
             try:
                 trial = study.best_trial
             except ValueError:
@@ -256,15 +267,18 @@
             row_dict = {k: v for k, v in study.user_attrs.items()}
             row_dict.update({k: v for k, v in trial.user_attrs.items()})
 
             if "KFoldScores" in row_dict:
                 del row_dict["KFoldScores"]
                 fold_scores = trial.user_attrs["KFoldScores"]
                 row_dict.update(
-                    {f"FoldScore_{i+1}": fold_scores[i] for i in range(len(fold_scores))}
+                    {
+                        f"FoldScore_{i+1}": fold_scores[i]
+                        for i in range(len(fold_scores))
+                    }
                 )
             row_dict.update({"parameters": trial.params})
             df_dict_list.append(row_dict)
 
         else:  # Getting all
             for trial in study.get_trials():
                 row_dict = {
@@ -273,15 +287,18 @@
                     if k not in ["best_trained_model_score", "best_trained_model"]
                 }
                 row_dict.update({k: v for k, v in trial.user_attrs.items()})
                 if "KFoldScores" in row_dict:
                     del row_dict["KFoldScores"]
                     fold_scores = trial.user_attrs["KFoldScores"]
                     row_dict.update(
-                        {f"FoldScore_{i+1}": fold_scores[i] for i in range(len(fold_scores))}
+                        {
+                            f"FoldScore_{i+1}": fold_scores[i]
+                            for i in range(len(fold_scores))
+                        }
                     )
                 row_dict.update({"parameters": trial.params})
                 df_dict_list.append(row_dict)
 
     df = pd.DataFrame(df_dict_list)
     columns_for_the_end = ["test_score", "parameters"]
     df = df[
@@ -317,23 +334,27 @@
     Returns
     -------
     pd.DataFrame
         DataFrame containing information on the best predictor.
     """
     unique_predictors = df["predictor_name"].unique()
     unique_dataset_views = df["dataset"].unique()
-    heatmap_data_array = np.full((len(unique_dataset_views), len(unique_predictors)), np.nan)
+    heatmap_data_array = np.full(
+        (len(unique_dataset_views), len(unique_predictors)), np.nan
+    )
 
     for pred_i in range(len(unique_predictors)):
         for ds_i in range(len(unique_dataset_views)):
             heatmap_data_array[ds_i, pred_i] = df.query(
                 f"predictor_name=='{unique_predictors[pred_i]}' and dataset=='{str(unique_dataset_views[ds_i])}'"
             )[column_containing_values].max()
 
-    return pd.DataFrame(heatmap_data_array, index=unique_dataset_views, columns=unique_predictors)
+    return pd.DataFrame(
+        heatmap_data_array, index=unique_dataset_views, columns=unique_predictors
+    )
 
 
 def get_metric(metric: Union[str, dict, PhenonautPredictionMetric]):
     """Get metric function from various options for metric definition
 
     Helper function which allows specification of metrics with strings
     indicating common names, dictionaries.
@@ -393,15 +414,17 @@
         )
 
     elif isinstance(metric, dict):
         if not all([k in metric for k in ("func", "name", "lower_is_better")]):
             raise KeyError(
                 f"'func', 'name', and 'lower_is_better' should be metric dictionary keys (containing the types Callable, str, bool), but found: {', '.join(metric.keys())}"
             )
-        return PhenonautPredictionMetric(metric["func"], metric["name"], metric["lower_is_better"])
+        return PhenonautPredictionMetric(
+            metric["func"], metric["name"], metric["lower_is_better"]
+        )
     else:
         raise ValueError(
             f"Metric should be a str, PhenonautPredictionMetric, or dict, it was: {type(metric)}"
         )
 
 
 def get_X_y(
@@ -431,17 +454,21 @@
     tuple
         X, y tuple for training of predictor.
     """
     X = None
     y = get_y_from_target(phe[dataset_combination], target=target)
     common_indices = None
     if isinstance(y, (pd.DataFrame, pd.Series)):
-        common_indices = get_common_indexes([phe[dsn].df for dsn in dataset_combination] + [y])
+        common_indices = get_common_indexes(
+            [phe[dsn].df for dsn in dataset_combination] + [y]
+        )
     elif isinstance(y, dataset):
-        common_indices = get_common_indexes([phe[dsn].df for dsn in dataset_combination] + [y.data])
+        common_indices = get_common_indexes(
+            [phe[dsn].df for dsn in dataset_combination] + [y.data]
+        )
     # 1 datasets
     if len(dataset_combination) == 1:
         #  1 view predictor
         if predictor.num_views == 1:
             if prediction_type == PredictionType.view:
                 if common_indices is None:
                     return (phe[dataset_combination[0]].data.values, y.values)
@@ -464,15 +491,17 @@
             return (None, None)
 
     # Multiple datasets - multiview
     else:
         if predictor.num_views == 1:  # Predictor can only do 1 view
             if common_indices is None:
                 return (
-                    np.hstack([phe[ds_name].data.values for ds_name in dataset_combination]),
+                    np.hstack(
+                        [phe[ds_name].data.values for ds_name in dataset_combination]
+                    ),
                     y.values,
                 )
             else:
                 return (
                     np.hstack(
                         [
                             phe[ds_name].data.loc[common_indices, :].values
@@ -481,15 +510,18 @@
                     ),
                     y.loc[common_indices].values,
                 )
         else:  # Predictor is multiview
             if len(dataset_combination) != predictor.num_views:
                 return (None, None)
             if common_indices is None:
-                return ([phe[ds_name].data.values for ds_name in dataset_combination], y.values)
+                return (
+                    [phe[ds_name].data.values for ds_name in dataset_combination],
+                    y.values,
+                )
             else:
                 return (
                     [
                         phe[ds_name].data.loc[common_indices, :].values
                         for ds_name in dataset_combination
                     ],
                     y.loc[common_indices].values,
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/predictor_dataclasses.py` & `phenonaut-2.0.3/src/phenonaut/predict/predictor_dataclasses.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from typing import Any, Iterable, Optional, Type, Union, Callable
+from collections.abc import Callable, Iterable
 from dataclasses import dataclass, field
-from sklearn.base import BaseEstimator
-from sklearn.metrics import accuracy_score
-from sklearn.metrics import mean_absolute_error
 from functools import reduce
+from typing import Any, Optional, Type, Union
+
+from sklearn.base import BaseEstimator
+from sklearn.metrics import accuracy_score, mean_absolute_error
+from dataclasses import field
 
 
 @dataclass
 class OptunaHyperparameter:
     """OptunaHyperparameter base dataclass which is inherited from"""
 
     name: str
@@ -45,34 +47,37 @@
 class HyperparameterInt(OptunaHyperparameterNumber):
     """Optuna hyperparameter dataclass for ints"""
 
     def __post_init__(self):
         self._check_bounds()
         self.optuna_func = "suggest_int"
         self.parameters = (self.lower_bound, self.upper_bound)
+        self.kwargs = {}
 
 
 @dataclass
 class HyperparameterFloat(OptunaHyperparameterNumber):
     """Optuna hyperparameter dataclass for floats"""
 
     def __post_init__(self):
         self._check_bounds()
         self.optuna_func = "suggest_float"
         self.parameters = (self.lower_bound, self.upper_bound)
+        self.kwargs = {}
 
 
 @dataclass
 class HyperparameterLog(OptunaHyperparameterNumber):
     """Optuna hyperparameter dataclass for loguniform distributions of floats"""
 
     def __post_init__(self):
         self._check_bounds()
-        self.optuna_func = "suggest_loguniform"
+        self.optuna_func = "suggest_float"
         self.parameters = (self.lower_bound, self.upper_bound)
+        self.kwargs = {'log': True}
 
 
 @dataclass
 class HyperparameterCategorical(OptunaHyperparameter):
     """Optuna hyperparameter dataclass for categorical lists"""
 
     choices: Union[list, tuple]
@@ -81,14 +86,15 @@
     def __post_init__(self):
         if len(self.choices) == 0:
             raise ValueError(
                 "Choices must be an iterable (usualy list or tuple) with length at least one"
             )
         self.optuna_func = "suggest_categorical"
         self.parameters = (self.choices,)
+        self.kwargs = {}
 
 
 @dataclass
 class PhenonautPredictionMetric:
     """PhenonautPredictionMetric dataclass to hold metric, name and direction."""
 
     func: Callable
@@ -125,12 +131,16 @@
     def __post_init__(self):
         if isinstance(self.optuna, OptunaHyperparameter):
             self.optuna = (self.optuna,)
         if self.optuna is None and self.max_optuna_trials is None:
             self.max_optuna_trials = 1
         if isinstance(self.optuna, Iterable):
             if all(
-                [isinstance(opt_option, HyperparameterCategorical) for opt_option in self.optuna]
+                [
+                    isinstance(opt_option, HyperparameterCategorical)
+                    for opt_option in self.optuna
+                ]
             ):
                 self.max_optuna_trials = reduce(
-                    lambda x, y: x * y, [len(opt_options.parameters) for opt_options in self.optuna]
+                    lambda x, y: x * y,
+                    [len(opt_options.parameters) for opt_options in self.optuna],
                 )
```

### Comparing `phenonaut-1.3.4/phenonaut/predict/profile.py` & `phenonaut-2.0.3/src/phenonaut/predict/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+from collections.abc import Callable
 from copy import deepcopy
 from optparse import Option
-from typing import Callable, Optional, Union
-import pandas as pd
+from pathlib import Path
+from typing import Optional, Union
+
 import numpy as np
-import phenonaut
 import optuna
+import pandas as pd
+
+import phenonaut
+import phenonaut.data
 from phenonaut.data.dataset import Dataset
-from phenonaut.predict.predictor_dataclasses import PhenonautPredictionMetric, PhenonautPredictor
 from phenonaut.predict.predict_utils import (
     PredictionType,
-    get_y_from_target,
-    get_prediction_type_from_y,
-    get_df_from_optuna_db,
     get_best_predictor_dataset_df,
+    get_df_from_optuna_db,
     get_metric,
+    get_prediction_type_from_y,
     get_X_y,
+    get_y_from_target,
+)
+from phenonaut.predict.predictor_dataclasses import (
+    PhenonautPredictionMetric,
+    PhenonautPredictor,
 )
-import phenonaut.data
-from .optuna_functions import run_optuna_opt, run_optuna_opt_merge_folds
-from pathlib import Path
 from phenonaut.utils import check_path
 
+from .optuna_functions import run_optuna_opt, run_optuna_opt_merge_folds
+
 
 def profile(
     phe: phenonaut.Phenonaut,
     output_directory: str,
     dataset_combinations: Optional[Union[None, list[int], list[str]]] = None,
     target: Optional[Union[str, pd.Series, np.ndarray, phenonaut.data.Dataset]] = None,
     predictors: Optional[list[PhenonautPredictor]] = None,
     prediction_type: Optional[Union[str, PredictionType]] = None,
     n_splits: int = 5,
-    seed: Optional[int] = None,
+    random_state: Optional[Union[int, np.random.Generator]] = None,
     optuna_db_path: Optional[Union[Path, str]] = None,
     optuna_db_protocol: str = "sqlite:///",
     n_optuna_trials=20,
     metric: Optional[Union[PhenonautPredictionMetric, str]] = None,
     no_output: bool = False,
     write_pptx: bool = True,
     optuna_merge_folds: bool = False,
     test_set_fraction: float = 0.2,
-    save_models: bool = True,
 ):
     """Profile predictors in their ability to predict a given target.
 
     This predict.profile function operates on a Phenonaut object (optionally
     containing multiple Datasets) and a given or indicated prediction target.
     The data within the prediction target is examined and the prediction type
     determined from classification, regression, and multiregression/view
@@ -103,17 +109,19 @@
     prediction_type : Optional[Union[str, PredictionType]], optional
         The type of prediction task like "classification", "regression" and
         "view", or the proper PredictionType enum. If None, then the prediction
         task is assigned through inspection of the target data types and values
         present.  By default, None.
     n_splits : int, optional
         Number of splits to use in the N-fold cross validation, by default 5.
-    seed : Optional[int], optional
-        Optionally set the seed used for random number generation.
-        By default None.
+    random_state : Union[int, np.random.Generator], optional
+        If an int, then use this to seed a np.random.Generator for reproducibility of
+        random operations (like shuffling etc). If a numpy.random.Generator, then this
+        is used as the source of randomness. Can also be None, in which case a random
+        seed is used. By default, None.
     optuna_db_path : Optional[Union[Path, str]], optional
         Path to Optuna sqlite3 database file. If None, then a default filename
         will be assigned by Phenonaut. By default None.
     optuna_db_protocol : _type_, optional
         Protocol that Optuna should use for accessing its required persistent
         storage. By default "sqlite:///"
     n_optuna_trials : int, optional
@@ -146,20 +154,36 @@
         test_set_fraction controls the size of this split. By default 0.2.
     save_models : bool, optional
         Save the trained models to pickle files for later use. By default False.
 
     """
     output_directory = check_path(output_directory, is_dir=True)
 
+    if isinstance(random_state, int):
+        np_rng = np.random.default_rng(random_state)
+    elif isinstance(random_state, np.random.Generator):
+        np_rng = random_state
+    else:
+        if random_state is None:
+            np_rng = np.random.default_rng(None)
+        else:
+            raise ValueError(
+                f"random_state must be an int, numpy.random.Generator, or None. It was {type(random_state)}"
+            )
+
     # Set up optuna_db_path. Dont do any file checks on it - as a sql
     # database may be specified in combination with the optuna_db_protocol
     # argument.
     if optuna_db_path is None:
         optuna_db_path = output_directory / "optuna_scan.db"
-    if predictors == [] and optuna_db_protocol == "sqlite:///" and not optuna_db_path.exists():
+    if (
+        predictors == []
+        and optuna_db_protocol == "sqlite:///"
+        and not optuna_db_path.exists()
+    ):
         raise ValueError(
             "predictors argument was empty, no optuna_db_path given and no 'optuna_scan.db' was found in the targeted output directory"
         )
 
     if dataset_combinations is None:
         dataset_combinations = phe.get_dataset_combinations()
 
@@ -194,30 +218,34 @@
                 metric = "mse"
     metric = get_metric(metric)
 
     if n_optuna_trials > 0:
         # If not supplied, set the default predictors
         if predictors is None:
             if prediction_type == PredictionType.classification:
-                from phenonaut.predict.default_predictors.classifiers import default_classifiers
+                from phenonaut.predict.default_predictors.classifiers import (
+                    default_classifiers,
+                )
 
                 predictors = default_classifiers
             if prediction_type == PredictionType.regression:
                 from .default_predictors.regressors import default_regressors
 
                 predictors = default_regressors
             if prediction_type == PredictionType.view:
                 from .default_predictors.multiregressors import default_multiregressors
 
                 predictors = default_multiregressors
 
         for dataset_combination in dataset_combinations:
             print(f"Working on datasets: {dataset_combination=}")
             for predictor in predictors:
-                X, y = get_X_y(phe, dataset_combination, target, predictor, prediction_type)
+                X, y = get_X_y(
+                    phe, dataset_combination, target, predictor, prediction_type
+                )
 
                 if X is None or y is None:
                     continue
                 if (
                     prediction_type == PredictionType.classification
                     and predictor.max_classes is not None
                     and predictor.max_classes < len(np.unique(y))
@@ -227,22 +255,25 @@
                     predictor.dataset_size_cutoff is not None
                     and predictor.dataset_size_cutoff < len(y)
                 ):
                     continue
 
                 # Split out a test set, leaving train and validation in X and y
                 shuffled_indexes = np.arange(y.shape[0], dtype=int)
-                np.random.seed(seed)
-                np.random.shuffle(shuffled_indexes)
+                np_rng.shuffle(shuffled_indexes)
 
                 if isinstance(X, list):
                     X_test = [
-                        Xv[shuffled_indexes[: int(y.shape[0] * test_set_fraction)]] for Xv in X
+                        Xv[shuffled_indexes[: int(y.shape[0] * test_set_fraction)]]
+                        for Xv in X
+                    ]
+                    X = [
+                        Xv[shuffled_indexes[int(y.shape[0] * test_set_fraction) :]]
+                        for Xv in X
                     ]
-                    X = [Xv[shuffled_indexes[int(y.shape[0] * test_set_fraction) :]] for Xv in X]
                 else:
                     X_test = X[shuffled_indexes[: int(y.shape[0] * test_set_fraction)]]
                     X = X[shuffled_indexes[int(y.shape[0] * test_set_fraction) :]]
                 y_test = y[shuffled_indexes[: int(y.shape[0] * test_set_fraction)]]
                 y = y[shuffled_indexes[int(y.shape[0] * test_set_fraction) :]]
 
                 if isinstance(target, Dataset):
@@ -260,15 +291,15 @@
                         predictor=predictor,
                         metric=metric,
                         n_optuna_trials=n_optuna_trials,
                         phe_name=phe.name,
                         dataset_combination=dataset_combination,
                         optuna_db_path=optuna_db_path,
                         n_splits=n_splits,
-                        seed=seed,
+                        random_state=random_state,
                         optuna_db_protocol=optuna_db_protocol,
                         target_dataset_name=target_dataset_name,
                     )
                 else:
                     run_optuna_opt(
                         X,
                         X_test,
@@ -278,15 +309,15 @@
                         predictor=predictor,
                         metric=metric,
                         n_optuna_trials=n_optuna_trials,
                         phe_name=phe.name,
                         dataset_combination=dataset_combination,
                         optuna_db_path=optuna_db_path,
                         n_splits=n_splits,
-                        seed=seed,
+                        random_state=random_state,
                         optuna_db_protocol=optuna_db_protocol,
                         target_dataset_name=target_dataset_name,
                     )
 
     if no_output:
         return
 
@@ -359,22 +390,22 @@
                 df_best.query(f"dataset == '{dataset}'")["metric_name"].unique()[0],
             )
 
     else:
         best_with_folds_as_scores = []
         df_best = df_best.reset_index()  # make sure indexes pair with number of rows
         mean_df = (
-            df_best.groupby(["dataset", "predictor_name"])
+            df_best.groupby(["dataset", "predictor_name"])["test_score"]
             .mean()
             .reset_index()[["dataset", "predictor_name", "test_score"]]
             .dropna(axis=0, how="all")
             .dropna(axis=1, how="all")
         )
         sd_df = (
-            df_best.groupby(["dataset", "predictor_name"])
+            df_best.groupby(["dataset", "predictor_name"])["test_score"]
             .std()
             .reset_index()[["dataset", "predictor_name", "test_score"]]
             .dropna(axis=0, how="all")
             .dropna(axis=1, how="all")
         )
 
         # When plotting the best predictors, we want boxplots to contain the fold results.
@@ -438,12 +469,15 @@
             if str(f.stem).endswith("_best")
             else str(f.stem).replace("_all", "").replace("boxplot_", "")
         )
 
         # Sort filenames first by alphabetical, then by length then iterate
         # Unneded: for f in sorted(boxplot_image_filenames, key=lambda x: (len(x.name), x.name)):
         ppt.add_image_slide(
-            "Heatmap", output_directory / "best_predictor_ds_heatmap.png", width=15, height=15
+            "Heatmap",
+            output_directory / "best_predictor_ds_heatmap.png",
+            width=15,
+            height=15,
         )
         for f in boxplot_best_paths:
             ppt.add_image_slide(f"{dfromp(f)}", f)
         ppt.save(output_directory / f"prediction_performance.pptx")
```

### Comparing `phenonaut-1.3.4/phenonaut/transforms/dimensionality_reduction.py` & `phenonaut-2.0.3/src/phenonaut/transforms/dimensionality_reduction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# Copyright © The University of Edinburgh, 2022.
+# Copyright © The University of Edinburgh, 2024.
 # Development has been supported by GSK.
 
-from phenonaut import data
+from collections.abc import Callable
+from pathlib import Path
+from typing import Optional, Union
+
+import numpy as np
+import pandas as pd
+import umap
+from matplotlib import pyplot as plt
 from numpy import isin
 from pandas.errors import DataError
-
-from phenonaut.data import Dataset
-from typing import Callable, Optional, Union
 from sklearn.decomposition import PCA as _SKLearnPCA
-from sklearn.manifold import TSNE as _SKLearn_TSNE
-import umap
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as sklearn_LDA
-import numpy as np
-from matplotlib import pyplot as plt
-from pathlib import Path
-import pandas as pd
+from sklearn.manifold import TSNE as _SKLearn_TSNE
+
+from phenonaut import data
+from phenonaut.data import Dataset
 from phenonaut.phenonaut import Phenonaut
 from phenonaut.transforms.transformer import Transformer
 
 
 class PCA(Transformer):
     """Principal Component Analysis (PCA) dimensionality reduction.
 
@@ -53,15 +55,15 @@
             constructor_kwargs={"n_components": ndims},
         )
         self.ndims = ndims
 
     def __call__(
         self,
         dataset: Union[Dataset, Phenonaut],
-        ndims: int = 2,
+        ndims: Optional[int] = None,
         new_feature_names: Union[list[str], str] = "PC",
         groupby: Optional[Union[str, list[str]]] = None,
         center_on_perturbation_id: Optional[str] = None,
         centering_function: Callable = np.median,
         fit_perturbation_ids: Optional[Union[str, list]] = None,
         fit_query: Optional[str] = None,
         explain_variance_in_features: bool = False,
@@ -70,15 +72,16 @@
 
         Parameters
         ----------
         dataset : Union[Dataset, Phenonaut]
             The Phenonaut dataset or Phenonaut object containing one dataset
             on which to apply PCA.
         ndims : int
-            Number of dimensions to embed the data into, by default 2
+            Number of dimensions to embed the data into. If None, then the value of
+            ndims passed to the constructor is used.
         new_feature_names : Union[list[str], str]
             List of strings containing the names for the new features. Can also
             be just a single string, which then has numerical suffixes attached
             enumerating the number of new features generated. By default "PC"
         groupby : Optional[Union[str, list[str]]], optional
             Often we would like to apply transformations on a plate-by-plate
             basis. This groupby argument allows definition of a string which
@@ -103,14 +106,16 @@
             A pandas style query may be supplied to perform fitting. By default
             None.
         explain_variance_in_features : bool, optional
             If True, then the percentage explained variance of each PCA
             dimension is included in the new PCA descriptor feature name.
             Overrides new_feature_names. By default False.
         """
+        if ndims == None:
+            ndims = self.ndims
         if self.ndims != ndims:
             super().__init__(
                 _SKLearnPCA,
                 new_feature_names=new_feature_names,
                 transformer_name="SciKitPCA",
                 constructor_kwargs={"n_components": ndims},
             )
@@ -135,17 +140,22 @@
                 pca_variance_ratio = self._method.explained_variance_ratio_
 
             explained_var_features = [
                 f"PC{x+1} ({expvariance*100:.2f} % explained variance)"
                 for x, expvariance in zip(range(self.ndims), pca_variance_ratio)
             ]
 
-            column_rename_dict = {k: v for k, v in zip(dataset.features, explained_var_features)}
+            column_rename_dict = {
+                k: v for k, v in zip(dataset.features, explained_var_features)
+            }
             dataset.df.rename(columns=column_rename_dict, inplace=True)
-            dataset.features = explained_var_features, "Added explained variance to features"
+            dataset.features = (
+                explained_var_features,
+                "Added explained variance to features",
+            )
 
     def save_scree_plot(
         self, output_filename: Optional[Union[str, Path]] = None, title="Scree plot"
     ):
         """Produce a Scree plot showing ndims vs explained variance
 
         Parameters
@@ -160,14 +170,17 @@
         ------
         DataError
             PCA must have been fitted before a Scree plot can be made.
         """
         if self._method is None:
             raise DataError("Cant make scree plot, nothing fitted")
         if isinstance(self._method, list):
+            print(
+                "Multiple fitted PCAs found (groupby used?) producing Scree plot for the last"
+            )
             pca_object = self._method[-1]
         else:
             pca_object = self._method
         fig, ax = plt.subplots(1)
         ax.plot(
             range(1, pca_object.explained_variance_ratio_.shape[0] + 1),
             np.cumsum(pca_object.explained_variance_ratio_),
@@ -179,18 +192,18 @@
             pca_object.explained_variance_ratio_,
             label="Explained variance",
             marker="x",
         )
 
         ax.set_xlabel("Feature")
         ax.set_ylabel("Fraction explained variance")
-        ax.set_xlim((0.25, self.pca.explained_variance_ratio_.shape[0]))
+        ax.set_xlim((0.25, pca_object.explained_variance_ratio_.shape[0]))
         ax.set_ylim((0, 1))
         ax.set_title(title)
-        plt.xticks(range(1, self.pca.explained_variance_ratio_.shape[0] + 1))
+        plt.xticks(range(1, pca_object.explained_variance_ratio_.shape[0] + 1))
         plt.tight_layout()
         plt.grid()
         ax.legend()
         if output_filename is None:
             plt.show()
         else:
             if isinstance(output_filename, str):
@@ -217,15 +230,14 @@
         be just a single string, which then has numerical suffixes attached
         enumerating the number of new features generated. By default "TSNE"
     ndims : int, optional
         Number of dimensions to embed the data into, by default 2
     """
 
     def __init__(self, constructor_kwargs={}, new_feature_names="TSNE", ndims: int = 2):
-
         constructor_kwargs["n_components"] = ndims
 
         if ndims > 3:
             constructor_kwargs["method"] = "exact"
         else:
             constructor_kwargs["method"] = "barnes_hut"
 
@@ -323,22 +335,32 @@
         The Phenonaut dataset on which to apply the transformation
     new_feature_names : Union[list[str], str]
         List of strings containing the names for the new features. Can also
         be just a single string, which then has numerical suffixes attached
         enumerating the number of new features generated. By default "UMAP"
     ndims : int, optional
         Number of dimensions to embed the data into, by default 2
+    umap_kwargs : dict
+        Keyword arguments to pass to UMAP-lean constructor. Often the number of
+        neighbors requires changing and this can be achieved here by passing in
+        {'n_neighbors': 50} for example, to run UMAP with 50 neighbors.  Any value of
+        an n_components key within this dictionary will be overwritten by the value of
+        the ndims argument.
     """
 
-    def __init__(self, new_feature_names="UMAP", ndims: int = 2):
+    def __init__(
+        self, new_feature_names="UMAP", ndims: int = 2, umap_kwargs: dict = {}
+    ):
+        self.umap_object_kwargs = {"n_components": ndims}
+        self.umap_object_kwargs.update(umap_kwargs)
         super().__init__(
             umap.UMAP,
             new_feature_names=new_feature_names,
             transformer_name="UMAP",
-            constructor_kwargs={"n_components": ndims},
+            constructor_kwargs=self.umap_object_kwargs,
         )
         self.ndims = ndims
 
     def __call__(
         self,
         dataset: Union[Dataset, Phenonaut],
         ndims: int = 2,
@@ -381,19 +403,20 @@
         centering_function : Callable
             Used with center_on_perturbation, this function is applied to
             all data for matching perturbations. By default, we use the median
             of perturbations. This behavior can be overridden by supplying a
             different function here. By default np.median.
         """
         if self.ndims != ndims:
+            self.umap_object_kwargs.update({"n_components": ndims})
             super().__init__(
                 umap.UMAP,
                 new_feature_names=new_feature_names,
                 transformer_name="UMAP",
-                constructor_kwargs={"n_components": ndims},
+                constructor_kwargs=self.umap_object_kwargs,
             )
             self.ndims = ndims
 
         self.fit_transform(
             dataset,
             groupby=groupby,
             new_feature_names=new_feature_names,
@@ -489,18 +512,15 @@
         X, y = (
             dataset.df.loc[:, dataset.features],
             dataset.df.loc[:, dataset.perturbation_column],
         )
         self.lda.fit(X, y)
 
         dataset.df.loc[:, lda_feature_column_names] = self.lda.transform(X)
-        dataset.features = (
-            lda_feature_column_names,
-            f"Performed LDA, ndims={ndims}",
-        )
+        dataset.features = (lda_feature_column_names, f"Performed LDA, ndims={ndims}")
         if center_on_perturbation_id is not None:
             if isinstance(center_on_perturbation_id, str):
                 if center_by_median:
                     center_on_coords = np.median(
                         dataset.df.query(
                             f"{dataset.perturbation_column} =='{center_on_perturbation_id}'"
                         )[dataset.features],
@@ -520,17 +540,17 @@
             )
             dataset.features = (
                 dataset.features,
                 f"Centered on {center_on_perturbation_id}, {center_by_median=}",
             )
 
         if predict_proba:
-            dataset.df[[f"proba_{c}" for c in self.lda.classes_]] = self.lda.predict_proba(
-                dataset.df[dataset.features]
-            )
+            dataset.df[
+                [f"proba_{c}" for c in self.lda.classes_]
+            ] = self.lda.predict_proba(dataset.df[dataset.features])
             for index, row in dataset.df.iterrows():
                 correct_proba = row[f"proba_{row['Edit']}"]
                 dataset.df.loc[index, "Correct_proba"] = correct_proba
 
             dataset.features = (
                 [f"proba_{c}" for c in self.lda.classes_],
                 "LDA prediction probability",
```

### Comparing `phenonaut-1.3.4/phenonaut/transforms/imputers.py` & `phenonaut-2.0.3/src/phenonaut/transforms/imputers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from .transformer import Transformer
-from typing import Union, Optional
-from sklearn.impute import SimpleImputer as _SKLearnSimpleImputer
-from sklearn.impute import KNNImputer as _SKLearnKNNImputer
-from sklearn.experimental import enable_iterative_imputer # although it looks unused, it must be present to import iterative_imputer into sklearn.impute
-from sklearn.impute import IterativeImputer as _SKLearnIterativeImputer
+from typing import Optional, Union
+
 from sklearn.ensemble import RandomForestRegressor as _SKLearnRandomForestRegressor
+from sklearn.experimental import (  # although it looks unused, it must be present to import iterative_imputer into sklearn.impute
+    enable_iterative_imputer,
+)
+from sklearn.impute import IterativeImputer as _SKLearnIterativeImputer
+from sklearn.impute import KNNImputer as _SKLearnKNNImputer
+from sklearn.impute import SimpleImputer as _SKLearnSimpleImputer
+
+from .transformer import Transformer
 
 
 class SimpleImputer(Transformer):
-    """SciKitLearn SimpleImputer
+    r"""SciKitLearn SimpleImputer
 
     SciKit's SimpleImputer wrapped in a Phenonaut Transformer. Allows passing a
     strategy argument containing 'mean', 'median', 'most_frequent', or 'constant'.
     If constant is passed, then must supply a fill_value argument.
 
     Can be used as follows:
 
@@ -45,15 +49,15 @@
             new_feature_names=new_feature_names,
             transformer_name="SimpleImputer",
             constructor_kwargs={"strategy": strategy, "fill_value": fill_value},
         )
 
 
 class KNNImputer(Transformer):
-    """SciKitLearn KNNImputer
+    r"""SciKitLearn KNNImputer
 
     SciKit's KNNImputer wrapped in a Phenonaut Transformer. Allows passing a
     numer of neighbors to use for imputation.
 
     Can be used as follows:
 
     .. code-block:: python
@@ -76,34 +80,34 @@
         Name of new features. If ending in _, then this is prepended to existing
         features. By default 'KNNImputed\_'.
     """
 
     def __init__(
         self,
         n_neighbors: int = 5,
-        weights : str  = 'uniform',
+        weights: str = "uniform",
         new_feature_names: Union[list[str], str] = "KNNImputed_",
     ):
         super().__init__(
             _SKLearnKNNImputer,
             new_feature_names=new_feature_names,
             transformer_name="KNNImputer",
-            constructor_kwargs={"n_neighbors": n_neighbors, 'weights':weights},
+            constructor_kwargs={"n_neighbors": n_neighbors, "weights": weights},
         )
 
 
 class RFImputer(Transformer):
-    """
+    r"""
     RandomForestImputer
-    
+
     RandomForestImputer inspired by SKLearn documentation here:
     https://scikit-learn.org/stable/auto_examples/impute/plot_iterative_imputer_variants_comparison.html#sphx-glr-auto-examples-impute-plot-iterative-imputer-variants-comparison-py
 
     Can be very computationally expensive, so careful setting of max_iter is advised.
-    
+
     Can be used as follows:
 
     .. code-block:: python
 
         imputer=RFImputer()
         imputer(dataset)
 
@@ -124,23 +128,23 @@
     new_feature_names : Union[list[str], str], optional
         Name of new features. If ending in _, then this is prepended to existing
         features. By default 'RFImputed\_'.
     """
 
     def __init__(
         self,
-        rf_kwargs={'n_jobs':-1},
+        rf_kwargs={"n_jobs": -1},
         max_iter: int = 25,
         tol: float = 1e-3,
         new_feature_names: Union[list[str], str] = "RFImputed_",
     ):
         super().__init__(
             _SKLearnIterativeImputer,
             new_feature_names=new_feature_names,
             transformer_name="RFImputer",
             constructor_kwargs={
                 "random_state": 42,
                 "estimator": _SKLearnRandomForestRegressor(**rf_kwargs),
-                'max_iter': max_iter,
-                'tol': tol,
+                "max_iter": max_iter,
+                "tol": tol,
             },
         )
```

### Comparing `phenonaut-1.3.4/phenonaut/transforms/preparative.py` & `phenonaut-2.0.3/src/phenonaut/transforms/preparative.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
 from typing import Optional, Union
-from phenonaut.data import Dataset
-from phenonaut import Phenonaut
+from scipy.linalg import eigh as _scipy_eigh
+
 import numpy as np
 import pandas as pd
+from typing import List
 from scipy.linalg import svd
+from sklearn.linear_model import LinearRegression as SklearnLinreg
 from sklearn.preprocessing import StandardScaler as SK_StandardScaler
 
-from sklearn.linear_model import LinearRegression as SklearnLinreg
-from phenonaut.transforms.transformer import Transformer
+from phenonaut import Phenonaut
+from phenonaut.data import Dataset
+from phenonaut.transforms.transformer import (
+    Transformer,
+    PheTransformerFitQueryMatchedNoRows,
+)
 
 """This module contains functionality to remove highly correlated features from phenonaut datasets"""
 
 
 class RemoveHighlyCorrelated:
     def __init__(self, verbose: bool = False):
         """RemoveHighlyCorrelated
@@ -104,19 +110,25 @@
             dataset features list, but the columns for these features will be removed
             from the dataframe, by default False
         corr_kwargs : dict
             Keyword arguments which may be passed to the pd.Dataframe.corr function, allowing
             chaniging of the correlation calculation method from pearson to otheres.
         """
         if threshold is not None:
-            self._filter_threshold(ds, threshold, drop_columns=drop_columns, **corr_kwargs)
+            self._filter_threshold(
+                ds, threshold, drop_columns=drop_columns, **corr_kwargs
+            )
         if min_features is not None:
-            self._filter_leaving_n(ds, min_features, drop_columns=drop_columns, **corr_kwargs)
+            self._filter_leaving_n(
+                ds, min_features, drop_columns=drop_columns, **corr_kwargs
+            )
 
-    def _filter_leaving_n(self, ds: Dataset, n: int, drop_columns: bool = False, **corr_kwargs):
+    def _filter_leaving_n(
+        self, ds: Dataset, n: int, drop_columns: bool = False, **corr_kwargs
+    ):
         """Filter the dataset, iteratively removing highest correlated features
 
         Parameters
         ----------
         ds : Dataset
             The dataset to be filtered.
         n : int
@@ -147,15 +159,19 @@
         if drop_columns:
             ds.drop_columns(
                 removed_features,
                 " because columns were old features removed by RemoveHighlyCorrelated",
             )
 
     def _filter_threshold(
-        self, ds: Dataset, threshold: float = 0.9, drop_columns: bool = False, **corr_kwargs
+        self,
+        ds: Dataset,
+        threshold: float = 0.9,
+        drop_columns: bool = False,
+        **corr_kwargs,
     ):
         """Filter dataset by feature correlation threshold
 
         Parameters
         ----------
         ds : Dataset
             The dataset to be filtered
@@ -207,15 +223,17 @@
         Parameters:
         ----------
         verbose : bool, optional
             If True, then details of the removed features are printed.
         """
         self.verbose = verbose
 
-    def __call__(self, ds, vif_cutoff: float = 5.0, min_features=2, drop_columns: bool = False):
+    def __call__(
+        self, ds, vif_cutoff: float = 5.0, min_features=2, drop_columns: bool = False
+    ):
         """Run the variance inflation factor filter, the same as calling the filter method.
 
         Parameters
         ----------
         ds : Dataset
             The phenonaut dataset to be operated on
         vif_cutoff : float, optional
@@ -255,15 +273,17 @@
         vif_scores = {}
         for held_out_feat in use_features:
             X = ds.df[[feat for feat in use_features if feat != held_out_feat]].values
             y = ds.df[held_out_feat].values
             vif_scores[held_out_feat] = 1 / (1 - SklearnLinreg().fit(X, y).score(X, y))
         return vif_scores
 
-    def filter(self, ds, vif_cutoff: float = 5.0, min_features=2, drop_columns: bool = False):
+    def filter(
+        self, ds, vif_cutoff: float = 5.0, min_features=2, drop_columns: bool = False
+    ):
         """Run the variance inflation factor filter
 
         Parameters
         ----------
         ds : Dataset
             The phenonaut dataset to be operated on
         vif_cutoff : float, optional
@@ -398,15 +418,21 @@
             dataset features list, but the columns for these features will be removed
             from the dataframe, by default False
         corr_kwargs : dict
             Keyword arguments which may be passed to the pd.Dataframe.corr function, allowing
             chaniging of the correlation calculation method from pearson to otheres.
         """
         rhc = RemoveHighlyCorrelated(self.verbose)
-        rhc(ds, threshold=None, min_features=n_before_vif, drop_columns=drop_columns, **corr_kwargs)
+        rhc(
+            ds,
+            threshold=None,
+            min_features=n_before_vif,
+            drop_columns=drop_columns,
+            **corr_kwargs,
+        )
         vif = VIF(self.verbose)
         vif(ds, drop_columns=drop_columns, min_features=min_features)
 
 
 class _ZCA:
     """
     Private class used by ZCA, implementing fit, transform and
@@ -449,19 +475,23 @@
     new_feature_names : Union[list[str], str]
         List of strings containing the names for the new features. Can also
         be just a single string, which then has numerical suffixes attached
         enumerating the number of new features generated. By default "ZCA"
     """
 
     def __init__(self, new_feature_names: Union[list[str], str] = "ZCA_"):
-        super().__init__(_ZCA, new_feature_names=new_feature_names, transformer_name="ZCA")
+        super().__init__(
+            _ZCA, new_feature_names=new_feature_names, transformer_name="ZCA"
+        )
 
 
 class __RobustMAD__:
-    def __init__(self, mad_scale: Union[str, float] = "normal", epsilon: Optional[float] = None):
+    def __init__(
+        self, mad_scale: Union[str, float] = "normal", epsilon: Optional[float] = None
+    ):
         """RobustMAD
 
         Robust scaling, as used popularly in pycytominer
 
         https://github.com/cytomining/pycytominer/blob/master/pycytominer/operations/transform.py
 
         Perform robust normalization using median and mad
@@ -504,15 +534,17 @@
         -------
         RobustMAD
             Returns a reference to itself as an object.
         """
         from scipy.stats import median_abs_deviation
 
         self._median = np.median(data, axis=0)
-        self._mad = median_abs_deviation(data, nan_policy="omit", scale=self._mad_scale, axis=0)
+        self._mad = median_abs_deviation(
+            data, nan_policy="omit", scale=self._mad_scale, axis=0
+        )
         return self
 
     def transform(self, dataset: np.ndarray):
         return (dataset - self._median) / (self._mad + self._epsilon)
 
 
 class RobustMAD(Transformer):
```

### Comparing `phenonaut-1.3.4/phenonaut/transforms/supervised_transformer.py` & `phenonaut-2.0.3/src/phenonaut/transforms/supervised_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from phenonaut.data.dataset import Dataset
-from typing import Union, List
 from inspect import isclass
+from typing import List, Optional, Union
+
 import numpy as np
 import pandas as pd
 
+from phenonaut.data.dataset import Dataset
+
 
 class SupervisedTransformer:
     method = None
     method_kwargs = {}
     has_fit = False
     has_transform = False
     has_fit_transform = False
     new_feature_names = None
     is_callable = False
     callable_args = {}
 
-    def __init__(self, method, new_feature_names=None, callable_args: dict = {}, **kwargs):
-
+    def __init__(
+        self, method, new_feature_names=None, callable_args: dict = {}, **kwargs
+    ):
         # Here we need to handle a method being put in, a class, and a class instance.
 
         if isclass(method):
             method = method(**kwargs)
         if hasattr(method, "fit"):
             self.has_fit = True
         if hasattr(method, "transform"):
@@ -34,27 +37,21 @@
             self.is_callable = True
             self.method_kwargs = kwargs
             self.callable_args = callable_args
         self.method = method
         self.new_feature_names = new_feature_names
 
     def _fit_df(
-        self,
-        X: Union[pd.DataFrame, np.array],
-        y: Union[pd.DataFrame, np.array],
+        self, X: Union[pd.DataFrame, np.array], y: Union[pd.DataFrame, np.array]
     ):
         if not self.has_fit:
             raise TypeError(f"Supplied method {self.method} has no fit function")
         self.method.fit(X, y)
 
-    def _transform_df(
-        self,
-        df: pd.DataFrame,
-    ) -> np.ndarray:
-
+    def _transform_df(self, df: pd.DataFrame) -> np.ndarray:
         if self.is_callable:
             transformed_data = self.method(df, **self.callable_args)
             if isinstance(transformed_data, pd.DataFrame):
                 return transformed_data.values
             return transformed_data
 
         if not self.has_transform:
@@ -63,18 +60,17 @@
         if isinstance(transformed_data, pd.DataFrame):
             return transformed_data.values
         return transformed_data
 
     def fit(
         self,
         data: Union[Dataset, pd.DataFrame],
-        y_or_ycolumnlabel: Union[str, pd.Series, np.array] = None,
-        fit_perturbation_ids: Union[str, list] = None,
+        y_or_ycolumnlabel: Optional[Union[str, pd.Series, np.array]] = None,
+        fit_perturbation_ids: Optional[Union[str, list]] = None,
     ):
-
         # Dataframe
         if isinstance(data, pd.DataFrame):
             if isinstance(y_or_ycolumnlabel, str):
                 if y_or_ycolumnlabel in data.columns:
                     X = data[list(data.columns).remove(y_or_ycolumnlabel)]
                     y = data[y_or_ycolumnlabel]
                     self._fit_df(X, y)
@@ -86,34 +82,37 @@
                     f"fit requires a pd.DataFrame, or a Dataset class, received {type(data)}"
                 )
             if fit_perturbation_ids is None:
                 fit_perturbation_ids = list(data.get_unique_perturbations())
             if isinstance(y_or_ycolumnlabel, str):
                 self._fit_df(
                     data.df.loc[
-                        data.df.query(f"{data.perturbation_column} == @fit_perturbation_ids").index,
+                        data.df.query(
+                            f"{data.perturbation_column} == @fit_perturbation_ids"
+                        ).index,
                         data.features,
                     ],
                     data.df.loc[y_or_ycolumnlabel],
                 )
             else:
                 self._fit_df(
                     data.df.loc[
-                        data.df.query(f"{data.perturbation_column} == @fit_perturbation_ids").index,
+                        data.df.query(
+                            f"{data.perturbation_column} == @fit_perturbation_ids"
+                        ).index,
                         data.features,
                     ],
                     y_or_ycolumnlabel,
                 )
 
     def transform(
         self,
         data: Union[Dataset, pd.DataFrame],
-        new_feature_names: List = None,
+        new_feature_names: Optional[List[str]] = None,
     ):
-
         # Do appropriate calls for DataFrame or Dataset to get transformed_data
         # which will be a np.array
         transformed_data = None
         if isinstance(data, pd.DataFrame):
             transformed_data = self.transform_df(data.df)
         else:
             if not isinstance(data, Dataset):
@@ -126,38 +125,34 @@
         # new_feature_names (argument to this function)
         # self.new_feature_names
         # generated from self.method.__name__ with -n after, where x is the column number/feature count.
         if new_feature_names is None:
             new_feature_names = self.new_feature_names
         if new_feature_names is None:
             new_feature_names = [
-                f"{self.method.__name__}-{n+1}" for n in range(transformed_data.shape[1])
+                f"{self.method.__name__}-{n+1}"
+                for n in range(transformed_data.shape[1])
             ]
         data.df[new_feature_names] = transformed_data
         data.features = (new_feature_names, f"{self.method}")
 
-    def _fit_transform_df(
-        self,
-        df: pd.DataFrame,
-    ) -> np.ndarray:
-
+    def _fit_transform_df(self, df: pd.DataFrame) -> np.ndarray:
         if not self.has_fit_transform:
-            raise TypeError(f"Supplied method {self.method} has no fit_transform function")
+            raise TypeError(
+                f"Supplied method {self.method} has no fit_transform function"
+            )
 
         transformed_data = self.method.fit_transform(df)
         if isinstance(transformed_data, pd.DataFrame):
             return transformed_data.values
         return transformed_data
 
     def fit_transform(
-        self,
-        data: Union[Dataset, pd.DataFrame],
-        new_feature_names: List = None,
+        self, data: Union[Dataset, pd.DataFrame], new_feature_names: list = None
     ):
-
         # Do appropriate calls for DataFrame or Dataset to get transformed_data
         # which will be a np.array
         transformed_data = None
         if isinstance(data, pd.DataFrame):
             transformed_data = self._fit_transform_df(data.df)
         else:
             if not isinstance(data, Dataset):
@@ -170,11 +165,12 @@
         # new_feature_names (argument to this function)
         # self.new_feature_names
         # generated from self.method.__name__ with -n after, where x is the column number/feature count.
         if new_feature_names is None:
             new_feature_names = self.new_feature_names
         if new_feature_names is None:
             new_feature_names = [
-                f"{self.method.__name__}-{n+1}" for n in range(transformed_data.shape[1])
+                f"{self.method.__name__}-{n+1}"
+                for n in range(transformed_data.shape[1])
             ]
         data.df[new_feature_names] = transformed_data
         data.features = (new_feature_names, f"{self.method}")
```

### Comparing `phenonaut-1.3.4/phenonaut/transforms/transformer.py` & `phenonaut-2.0.3/src/phenonaut/transforms/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from multiprocessing.sharedctypes import Value
-from sklearn import decomposition
-from phenonaut import data
-from phenonaut.data.dataset import Dataset
-from typing import Callable, Iterable, Optional, Type, Union, List
-from inspect import isclass
+from collections.abc import Callable, Iterable
 from copy import deepcopy
-from numpy import array
+from inspect import isclass
+from multiprocessing.sharedctypes import Value
+from typing import List, Optional, Type, Union
+
 import numpy as np
 import pandas as pd
+from numpy import array
+from sklearn import decomposition
 
+from phenonaut import data
+from phenonaut.data.dataset import Dataset
 from phenonaut.phenonaut import Phenonaut
 
 
+class PheTransformerFitQueryMatchedNoRows(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+
+
 class Transformer:
-    """Generic transformer to turn methods/objects into Phenonaut transforms
+    r"""Generic transformer to turn methods/objects into Phenonaut transforms
 
     This generic transformer class may be used to wrap functions which perform
     a simple transform (like np.log2), or even more complex objects, like PCA,
     t-SNE and StandardScaler from scikit (which provide their own fit/transform/
     fit_transform functions).
 
     This way, a Phenonaut transformer may be constructed with applies the given
@@ -153,15 +160,17 @@
         # Here we need to handle a method being put in, a class, and a class instance.
         if isclass(method):
             method = method(**constructor_kwargs)
         self._method = method
 
         self._has_fit = True if hasattr(self._method, "fit") else False
         self._has_transform = True if hasattr(self._method, "transform") else False
-        self._has_fit_transform = True if hasattr(self._method, "fit_transform") else False
+        self._has_fit_transform = (
+            True if hasattr(self._method, "fit_transform") else False
+        )
         self._is_callable = True if hasattr(self._method, "__call__") else False
 
     def fit(
         self,
         dataset: Union[Dataset, Phenonaut],
         groupby: Optional[Union[str, list[str]]] = None,
         fit_perturbation_ids: Union[str, list] = None,
@@ -215,29 +224,38 @@
             fit_perturbation_ids = list(fit_perturbation_ids)
             fit_query = f"{dataset.perturbation_column} == @fit_perturbation_ids"
 
         if groupby is None:
             if fit_query is None:
                 self._method.fit(dataset.data, **fit_kwargs)
             else:
-                self._method.fit(dataset.df.query(fit_query)[dataset.features], **fit_kwargs)
+                query_res = dataset.df.query(fit_query)
+                if len(query_res) == 0:
+                    raise PheTransformerFitQueryMatchedNoRows(
+                        f"Nothing to fit to, '{fit_query}' returned an empty DataFrame"
+                    )
+                self._method.fit(query_res[dataset.features], **fit_kwargs)
         else:
             self._original_features = dataset.features
             self._grouped_data = dataset.df.groupby(groupby)
             self._dataframes = [gdf for _, gdf in self._grouped_data]
             self._method = []
             for df in self._dataframes:
                 if isclass(self._original_method):
-                    self._method.append(self._original_method(**self._constructor_kwargs))
+                    self._method.append(
+                        self._original_method(**self._constructor_kwargs)
+                    )
                 else:
                     self._method.append(deepcopy(self._orignal_method))
                 if fit_query is None:
                     self._method[-1].fit(df[self._original_features], **fit_kwargs)
                 else:
-                    self._method[-1].fit(df.query(fit_query)[self._original_features], **fit_kwargs)
+                    self._method[-1].fit(
+                        df.query(fit_query)[self._original_features], **fit_kwargs
+                    )
         self._fit_has_been_called = True
         return self
 
     def transform(
         self,
         dataset: Union[Dataset, Phenonaut],
         new_feature_names: Optional[Union[list[str], str]] = None,
@@ -285,17 +303,23 @@
             all data for matching perturbations. By default, we use the median
             of perturbations. This behavior can be overridden by supplying a
             different function here. By default np.median.
 
         """
         if not self._has_transform:
             if self._is_callable:
-                self.__call__(dataset, new_feature_names=new_feature_names, method_name=method_name)
+                self.__call__(
+                    dataset,
+                    new_feature_names=new_feature_names,
+                    method_name=method_name,
+                )
             else:
-                raise ValueError("No transform method found, and transform is also not callable.")
+                raise ValueError(
+                    "No transform method found, and transform is also not callable."
+                )
         if transform_kwargs is None:
             transform_kwargs = self._transform_kwargs
         if not isinstance(dataset, (Phenonaut, Dataset)):
             raise TypeError(
                 "Supplied data must be of type phenonaut.Dataset, or a Phenonaut object, "
                 "in which case behavior is as if .ds was called to return the dataset with"
                 f" the highest index (last added), found type was {type(dataset)}"
@@ -305,31 +329,40 @@
 
         if isinstance(self._method, list):
             if len(self._method) == 0 or len(self._method) != len(self._dataframes):
                 raise ValueError(
                     f"groupby appears to have failed, there are {len(self._method)} transformers, and {len(self._dataframes)} groups"
                 )
 
-            for df_index, (fitted_object, df) in enumerate(zip(self._method, self._dataframes)):
+            for df_index, (fitted_object, df) in enumerate(
+                zip(self._method, self._dataframes)
+            ):
                 transformed_data_array = np.array(
-                    fitted_object.transform(df[self._original_features], **transform_kwargs)
+                    fitted_object.transform(
+                        df[self._original_features], **transform_kwargs
+                    )
                 )
-                method_name, new_feature_names = self._get_method_name_and_feature_names(
+                (
+                    method_name,
+                    new_feature_names,
+                ) = self._get_method_name_and_feature_names(
                     transformed_data_array.shape[1],
                     method_name,
                     dataset.features,
                     new_feature_names,
                     dataset.df.columns.values.tolist(),
                 )
 
                 transformed_df = pd.concat(
                     [
                         df,
                         pd.DataFrame(
-                            data=transformed_data_array, columns=new_feature_names, index=df.index
+                            data=transformed_data_array,
+                            columns=new_feature_names,
+                            index=df.index,
                         ),
                     ],
                     axis=1,
                 )
 
                 self._dataframes[df_index] = self._center_df(
                     dataset,
@@ -382,27 +415,34 @@
 
         dataset.features = (
             new_feature_names,
             f"Applied {method_name}, {self._constructor_kwargs=}, {self._fit_kwargs=}, {self._transform_kwargs=}, {self._fit_transform_kwargs=}, {self._callable_kwargs=}, centered on {center_on_perturbation_id}, {centering_function}",
         )
 
     def _center_df(
-        self, dataset, df, center_on_perturbation_id, new_feature_names, centering_function
+        self,
+        dataset,
+        df,
+        center_on_perturbation_id,
+        new_feature_names,
+        centering_function,
     ):
         if center_on_perturbation_id is not None:
             if isinstance(center_on_perturbation_id, str):
                 center_on_coords = centering_function(
-                    df.query(f"{dataset.perturbation_column} =='{center_on_perturbation_id}'")[
-                        new_feature_names
-                    ],
+                    df.query(
+                        f"{dataset.perturbation_column} =='{center_on_perturbation_id}'"
+                    )[new_feature_names],
                     axis=0,
                 )
             else:
                 center_on_coords = center_on_perturbation_id
-            df.loc[:, new_feature_names] = df.loc[:, new_feature_names] - center_on_coords
+            df.loc[:, new_feature_names] = (
+                df.loc[:, new_feature_names] - center_on_coords
+            )
         return df
 
     def fit_transform(
         self,
         dataset: Union[Dataset, Phenonaut],
         groupby: Optional[Union[str, list[str]]] = None,
         fit_perturbation_ids: Union[str, list] = None,
@@ -514,20 +554,25 @@
                     f"fit_perturbation_ids and fit_query cannot be used when the transformation has a native fit_transform method.  Call fit, then transform on the transformer"
                 )
             if groupby is None:
                 # Below we check if fit_transform_kwargs has anythin in it. This is not needed
                 # for scikit and similar, but the UMAP package thinks that a y argument of length 0
                 # if being passed if anything is there, so we work around it.
                 if fit_transform_kwargs is None or fit_transform_kwargs == {}:
-                    transformed_data_array = np.array(self._method.fit_transform(dataset.data))
+                    transformed_data_array = np.array(
+                        self._method.fit_transform(dataset.data)
+                    )
                 else:
                     transformed_data_array = np.array(
                         self._method.fit_transform(dataset.data, **fit_transform_kwargs)
                     )
-                method_name, new_feature_names = self._get_method_name_and_feature_names(
+                (
+                    method_name,
+                    new_feature_names,
+                ) = self._get_method_name_and_feature_names(
                     transformed_data_array.shape[1],
                     method_name,
                     dataset.features,
                     new_feature_names,
                     dataset.df.columns.values.tolist(),
                 )
                 transformed_df = pd.concat(
@@ -552,22 +597,29 @@
             else:  # Groupby is used
                 self._original_features = dataset.features
                 self._grouped_data = dataset.df.groupby(groupby)
                 self._dataframes = [gdf for _, gdf in self._grouped_data]
                 self._method = []
                 for df_index, df in enumerate(self._dataframes):
                     if isclass(self._original_method):
-                        self._method.append(self._original_method(**self._constructor_kwargs))
+                        self._method.append(
+                            self._original_method(**self._constructor_kwargs)
+                        )
                     else:
                         self._method.append(deepcopy(self._orignal_method))
                     transformed_data_array = np.array(
-                        self._method[-1].fit_transform(df[dataset.features], **fit_transform_kwargs)
+                        self._method[-1].fit_transform(
+                            df[dataset.features], **fit_transform_kwargs
+                        )
                     )
 
-                    method_name, new_feature_names = self._get_method_name_and_feature_names(
+                    (
+                        method_name,
+                        new_feature_names,
+                    ) = self._get_method_name_and_feature_names(
                         transformed_data_array.shape[1],
                         method_name,
                         dataset.features,
                         new_feature_names,
                         dataset.df.columns.values.tolist(),
                     )
 
@@ -658,15 +710,16 @@
         if existing_column_names is not None:
             f_repeat_counter = 1
             if set(new_features).intersection(set(existing_column_names)):
                 new_features = [f"{f}_{f_repeat_counter}" for f in new_features]
             while set(new_features).intersection(set(existing_column_names)):
                 f_repeat_counter += 1
                 new_features = [
-                    f"{'_'.join(f.split('_')[:-1])}_{f_repeat_counter}" for f in new_features
+                    f"{'_'.join(f.split('_')[:-1])}_{f_repeat_counter}"
+                    for f in new_features
                 ]
         return method_name, new_features
 
     def __call__(
         self,
         dataset: Union[Dataset, Phenonaut, np.ndarray],
         groupby: Optional[Union[str, list[str]]] = None,
@@ -768,15 +821,17 @@
                 transformed_data_array.shape[1],
                 method_name,
                 dataset.features,
                 new_feature_names,
                 dataset.df.columns.values.tolist(),
             )
             transformed_df = pd.DataFrame(
-                data=transformed_data_array, columns=new_feature_names, index=dataset.df.index
+                data=transformed_data_array,
+                columns=new_feature_names,
+                index=dataset.df.index,
             )
             dataset.df = pd.concat([dataset.df, transformed_df], axis=1)
             dataset.features = (
                 new_feature_names,
                 f"Applied callable {method_name}, {self._callable_kwargs=}",
             )
             return
```

### Comparing `phenonaut-1.3.4/phenonaut/utils.py` & `phenonaut-2.0.3/src/phenonaut/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
-from typing import Union
-from pathlib import Path
 import json
+from pathlib import Path
+from typing import Union
+
 import yaml
 
 
 def check_path(
     p: Union[Path, str],
     is_dir: bool = False,
     make_parents: bool = True,
```

### Comparing `phenonaut-1.3.4/phenonaut/workflow.py` & `phenonaut-2.0.3/src/phenonaut/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright © The University of Edinburgh, 2022.
 # Development has been supported by GSK.
 
+import re
 from pathlib import Path
-import phenonaut
-from pandas.errors import DataError
 from typing import Union
-import re
+
+from pandas.errors import DataError
+
+import phenonaut
 from phenonaut.transforms.preparative import RemoveHighlyCorrelated
 from phenonaut.utils import load_dict
 
 
 class Workflow:
     """Phenonaut Workflows allow operation through simple YAML workflows.
 
@@ -130,15 +132,17 @@
                     )
                 command = next(iter(task))
                 arguments = task[command]
                 print(f"Performing : {command}")
                 try:
                     getattr(self, command)(arguments)
                 except AttributeError as error:
-                    raise AttributeError(f"{command} not implemented in Phenonaut Workflow")
+                    raise AttributeError(
+                        f"{command} not implemented in Phenonaut Workflow"
+                    )
 
     def load(self, arguments: dict):
         """Workflow function: load a dataset (CSV or PakcagedDataset)
 
         Workflow runnable function allowing loading of dataset from CSV or a
         PackagedDataset. As with all workflow runnable functions, this is
         designed to be called from a worflow.
@@ -210,15 +214,18 @@
                     metadata["sep"] = "\t"
             if file.endswith(".h5"):
                 if "key" not in arguments:
                     raise KeyError(
                         "Workflow load called on an h5 file, without supplying a key argument"
                     )
                 self.phe.load_dataset(
-                    "Workflow loaded dataset", file, metadata=metadata, h5_key=arguments["key"]
+                    "Workflow loaded dataset",
+                    file,
+                    metadata=metadata,
+                    h5_key=arguments["key"],
                 )
             self.phe.load_dataset("Workflow loaded dataset", file, metadata=metadata)
             return
         if "dataset" in arguments:
             packaged_dataset_name = metadata["dataset"]
             working_dir = arguments.get("working_dir", None)
             if packaged_dataset_name == "TCGA":
@@ -242,15 +249,17 @@
                 self.phe = phenonaut.Phenonaut(Iris_2_views(working_dir))
                 return
             if packaged_dataset_name == "BreastCancer":
                 from phenonaut.packaged_datasets import BreastCancer
 
                 self.phe = phenonaut.Phenonaut(BreastCancer(working_dir))
                 return
-            raise KeyError("Name of packaged dataset not found or accessible within a workflow")
+            raise KeyError(
+                "Name of packaged dataset not found or accessible within a workflow"
+            )
         raise KeyError("Did not find file or dataset argument for load command")
 
     def filter_rows(self, arguments: dict):
         """Workflow function: Filter rows
 
         Designed to be called from a workflow, filter_rows alows keeping of only
         rows with a certain value in a certain column. Takes as arguments a
@@ -432,15 +441,17 @@
                 value to be found in the column defined previously.
             output_column_label:
                 Output from the scalar projection will have the form: on_target_<output_column_label> and off_target_<output_column_label>
                 if this is missing, then it is set to target_perturbation_column_value
 
         """
         if "output_column_label" not in arguments:
-            arguments["output_column_label"] = arguments["target_perturbation_column_value"]
+            arguments["output_column_label"] = arguments[
+                "target_perturbation_column_value"
+            ]
         phenonaut.metrics.scalar_projection(
             self.phe[arguments.get("target_dataset", -1)], **arguments
         )
 
     def euclidean_distance(self, arguments: dict):
         """Workflow function: Add a column for the euclidean distance to a target perturbation.
 
@@ -459,15 +470,17 @@
             target_perturbation_column_value:
                 value to be found in the column defined previously.
             output_column_label:
                 Output column for the measurement. If this is missing, then it is set to target_perturbation_column_value.
 
         """
         if "output_column_label" not in arguments:
-            arguments["output_column_label"] = arguments["target_perturbation_column_value"]
+            arguments["output_column_label"] = arguments[
+                "target_perturbation_column_value"
+            ]
         target_perturbation_column_name = arguments["target_perturbation_column_name"]
         target_perturbation_column_value = arguments["target_perturbation_column_value"]
         output_column_label = arguments["output_column_label"]
         ds = self.phe[arguments.get("target_dataset", -1)]
         ds.df[output_column_label] = phenonaut.metrics.euclidean(
             ds.data,
             ds.df.query(
@@ -493,15 +506,17 @@
             target_perturbation_column_value:
                 value to be found in the column defined previously.
             output_column_label:
                 Output column for the measurement. If this is missing, then it is set to target_perturbation_column_value.
 
         """
         if "output_column_label" not in arguments:
-            arguments["output_column_label"] = arguments["target_perturbation_column_value"]
+            arguments["output_column_label"] = arguments[
+                "target_perturbation_column_value"
+            ]
         target_perturbation_column_name = arguments["target_perturbation_column_name"]
         target_perturbation_column_value = arguments["target_perturbation_column_value"]
         output_column_label = arguments["output_column_label"]
         ds = self.phe[arguments.get("target_dataset", -1)]
         ds.df[output_column_label] = phenonaut.metrics.mahalanobis(
             ds.data,
             ds.df.query(
@@ -527,15 +542,17 @@
             target_perturbation_column_value:
                 value to be found in the column defined previously.
             output_column_label:
                 Output column for the measurement. If this is missing, then it is set to target_perturbation_column_value.
 
         """
         if "output_column_label" not in arguments:
-            arguments["output_column_label"] = arguments["target_perturbation_column_value"]
+            arguments["output_column_label"] = arguments[
+                "target_perturbation_column_value"
+            ]
         target_perturbation_column_name = arguments["target_perturbation_column_name"]
         target_perturbation_column_value = arguments["target_perturbation_column_value"]
         output_column_label = arguments["output_column_label"]
         ds = self.phe[arguments.get("target_dataset", -1)]
         ds.df[output_column_label] = phenonaut.metrics.manhattan(
             ds.data,
             ds.df.query(
@@ -559,15 +576,17 @@
             target_perturbation_column_value:
                 value to be found in the column defined previously.
             output_column_label:
                 Output column for the measurement. If this is missing, then it is set to target_perturbation_column_value.
 
         """
         if "output_column_label" not in arguments:
-            arguments["output_column_label"] = arguments["target_perturbation_column_value"]
+            arguments["output_column_label"] = arguments[
+                "target_perturbation_column_value"
+            ]
         target_perturbation_column_name = arguments["target_perturbation_column_name"]
         target_perturbation_column_value = arguments["target_perturbation_column_value"]
         output_column_label = arguments["output_column_label"]
         ds = self.phe[arguments.get("target_dataset", -1)]
         ds.df[output_column_label] = phenonaut.metrics.manhattan(
             ds.data,
             ds.df.query(
@@ -746,15 +765,17 @@
         """
 
         query_column = arguments.pop("query_column", None)
         if query_column is None:
             message = f"if_blank_also_blank needs a 'query_column' argument"
             raise KeyError(message)
         if arguments.pop("regex_query", False):
-            query_column = list(filter(re.compile(query_column).match, self.phe.df.columns.values))
+            query_column = list(
+                filter(re.compile(query_column).match, self.phe.df.columns.values)
+            )
             if len(query_column) == 1:
                 query_column = query_column[0]
             else:
                 message = "Multiple columns matched query_column using the regex"
                 raise IndexError(message)
 
         target_columns = []
@@ -767,15 +788,17 @@
         if len(target_columns) == 0:
             message = "No target columns found for if_blank_also_blank, use target_column keys"
             raise KeyError(message)
 
         if arguments.pop("regex_targets", False):
             expanded_target_columns = []
             for pattern in target_columns:
-                for match in list(filter(re.compile(pattern).match, self.phe.df.columns.values)):
+                for match in list(
+                    filter(re.compile(pattern).match, self.phe.df.columns.values)
+                ):
                     if match not in expanded_target_columns:
                         expanded_target_columns.append(match)
             target_columns = expanded_target_columns
 
         print(f"{target_columns=}  {query_column}")
         self.phe.df.loc[self.phe.df[query_column].isnull(), target_columns] = ""
 
@@ -930,15 +953,17 @@
             column:
                 str type giving the new column name which will be set to mark
                 perturbations.
 
         """
         if "column" not in arguments:
             raise KeyError("Must supply a 'column' key in arguments dictionary")
-        self.phe[arguments.get("target_dataset", -1)].perturbation_column = arguments["column"]
+        self.phe[arguments.get("target_dataset", -1)].perturbation_column = arguments[
+            "column"
+        ]
 
     def VIF_filter_features(self, arguments: dict):
         """Workflow function: Perform VIF feature filter
 
         Designed to be called from a workflow, performs variance inflation
         factor (VIF) filtering on a dataset, removing features which are not
         detrimental to capturing variance.
```

### Comparing `phenonaut-1.3.4/test/test_dataset.py` & `phenonaut-2.0.3/test/test_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright © The University of Edinburgh, 2022.
+# Copyright © The University of Edinburgh, 2024.
 # Development has been supported by GSK.
 
-import phenonaut
-from phenonaut.data.dataset import Dataset
 import numpy as np
 import pandas as pd
+
+import phenonaut
+from phenonaut.data.dataset import Dataset
 from phenonaut.phenonaut import Phenonaut
 
 
 def test_get_features_and_non_features(dataset_iris):
     features = dataset_iris.features
     print(features)
     non_features = dataset_iris.get_non_feature_columns()
-    assert sorted(
-        features + non_features) == sorted(dataset_iris.df.columns.values)
+    assert sorted(features + non_features) == sorted(dataset_iris.df.columns.values)
 
 
 def test_new_aggregated_dataset(small_2_plate_df):
     """Here we test a df as follows:
     ROW	COLUMN	BARCODE	feat_1	feat_2	feat_3	filename	FOV
     1	1	    Plate1	1.2	    1.2	    1.3	    fileA.png	1
     1	1	    Plate1	1.3	    1.4	    1.5	    FileB.png	2
@@ -29,15 +29,15 @@
     As there are multiple fields of view, we merge on common ROW, COLUMN and BARCODE fields.
     Merging uses np.mean, but may be any callable which returns a sing value
 
     """
     phe = phenonaut.Phenonaut(small_2_plate_df)
 
     new_ds = phe.ds.new_aggregated_dataset(["ROW", "COLUMN", "BARCODE"])
-    assert set(new_ds.features) == set(["feat_1", "feat_2", "feat_3"])
+    assert set(new_ds.features) == {"feat_1", "feat_2", "feat_3"}
     assert abs(new_ds.df["feat_1"][0] - 1.25) < 1e-6
     assert np.abs(new_ds.df["feat_1"][1] - 5.70) < 1e-6
     assert np.abs(new_ds.df["feat_1"][2] - 0.15) < 1e-6
     assert np.abs(new_ds.df["feat_2"][0] - 1.3) < 1e-6
     assert np.abs(new_ds.df["feat_2"][1] - 5.6) < 1e-6
     assert np.abs(new_ds.df["feat_2"][2] - 0.2) < 1e-6
     assert np.abs(new_ds.df["feat_3"][0] - 1.4) < 1e-6
@@ -61,25 +61,23 @@
     with tempfile.NamedTemporaryFile(mode="w") as tmp:
         tmp.write(
             "row, column, feature1, feature2, derived_feature3, feature10, feature003\n1,1,1,2,3,4,5\n2,1,6,7,8,9,10"
         )
         tmp.flush()
         phe = Phenonaut()
         phe.load_dataset(tmp.name, tmp.name, {"features_prefix": "feat"})
-        assert phe.ds.features == ["feature1",
-                                   "feature2", "feature003", "feature10"]
+        assert phe.ds.features == ["feature1", "feature2", "feature003", "feature10"]
 
     with tempfile.NamedTemporaryFile(mode="w") as tmp:
         tmp.write(
             "sepal length (cm),sepal width (cm),petal length (cm),petal width (cm),target\n5.4,3.4,1.7,0.2,0\n7.2,3.0,5.8,1.6,2\n6.4,2.8,5.6,2.1,2\n4.8,3.1,1.60.2,0\n5.6,2.5,3.9,1.1,1"
         )
         tmp.flush()
         phe = Phenonaut()
-        phe.load_dataset(tmp.name, tmp.name, {
-                         "features_regex": ".*(width|length).*"})
+        phe.load_dataset(tmp.name, tmp.name, {"features_regex": ".*(width|length).*"})
         assert phe.ds.features == [
             "petal length (cm)",
             "petal width (cm)",
             "sepal length (cm)",
             "sepal width (cm)",
         ]
 
@@ -92,53 +90,88 @@
 
 def test_remove_features_with_outliers(dataset_iris):
     dataset_iris.remove_features_with_outliers(7.5)
     assert len(dataset_iris.features) == 3
 
 
 def test_remove_low_variance_features(dataset_iris):
-    dataset_iris.remove_low_variance_features(
-        freq_cutoff=0.5, unique_cutoff=0.2)
+    dataset_iris.remove_low_variance_features(freq_cutoff=0.5, unique_cutoff=0.2)
     assert dataset_iris.features == ["petal length (cm)", "sepal length (cm)"]
 
 
 def test_remove_blocklist_features(dataset_iris):
-    dataset_iris.remove_blocklist_features(
-        ["petal length (cm)", "sepal length (cm)"])
+    dataset_iris.remove_blocklist_features(["petal length (cm)", "sepal length (cm)"])
     assert dataset_iris.features == ["petal width (cm)", "sepal width (cm)"]
 
-    dataset_iris.rename_column("petal width (cm)", "RobustMAD_Nuclei_Correlation_Manders_AGP_DNA")
+    dataset_iris.rename_column(
+        "petal width (cm)", "RobustMAD_Nuclei_Correlation_Manders_AGP_DNA"
+    )
 
     dataset_iris.remove_blocklist_features("CellProfiler")
     assert "RobustMAD_Nuclei_Correlation_Manders_AGP_DNA" not in dataset_iris.df.columns
     assert dataset_iris.features == ["sepal width (cm)"]
 
 
 def test_drop_nans_with_cutoff(nan_inf_dataset):
-
     nan_inf_dataset.drop_nans_with_cutoff(nan_cutoff=0.4)
-    assert (list(nan_inf_dataset.df.columns) == ['A', 'B', 'C', 'D', 'F'])
-    assert (list(nan_inf_dataset.df.index) == [0, 1, 2, 5])
-    assert (nan_inf_dataset.df.equals(pd.DataFrame({'A': {0: 1, 1: 2, 2: 3, 5: 6},
-                                                    'B': {0: 6, 1: 5, 2: 4, 5: 1},
-                                                    'C': {0: 1.0, 1: 2.0, 2: 3.0, 5: 4.0},
-                                                    'D': {0: np.inf, 1: 1.0, 2: 2.0, 5: np.nan},
-                                                    'F': {0: 'g1', 1: 'g1', 2: 'g1', 5: 'g2'}})))
+    assert list(nan_inf_dataset.df.columns) == ["A", "B", "C", "D", "F"]
+    assert list(nan_inf_dataset.df.index) == [0, 1, 2, 5]
+    assert nan_inf_dataset.df.equals(
+        pd.DataFrame(
+            {
+                "A": {0: 1, 1: 2, 2: 3, 5: 6},
+                "B": {0: 6, 1: 5, 2: 4, 5: 1},
+                "C": {0: 1.0, 1: 2.0, 2: 3.0, 5: 4.0},
+                "D": {0: np.inf, 1: 1.0, 2: 2.0, 5: np.nan},
+                "F": {0: "g1", 1: "g1", 2: "g1", 5: "g2"},
+            }
+        )
+    )
 
 
 def test_impute_nans(nan_inf_dataset):
+    nan_inf_dataset.impute_nans(groupby_col=None, impute_fn="median")
 
-    nan_inf_dataset.impute_nans(groupby_col=None, impute_fn='median')
-
-    assert (nan_inf_dataset.df.equals(pd.DataFrame({'A': {0: 1, 1: 2, 2: 3, 3: 4, 4: 5, 5: 6},
-                                                    'B': {0: 6, 1: 5, 2: 4, 3: 3, 4: 2, 5: 1},
-                                                    'C': {0: 1.0, 1: 2.0, 2: 3.0, 3: 2.5, 4: 2.5, 5: 4.0},
-                                                    'D': {0: 2.5, 1: 1.0, 2: 2.0, 3: 3.0, 4: 4.0, 5: 2.5},
-                                                    'E': {0: 5.0, 1: 5.5, 2: 5.5, 3: 5.5, 4: 5.5, 5: 6.0},
-                                                    'F': {0: 'g1', 1: 'g1', 2: 'g1', 3: 'g2', 4: 'g2', 5: 'g2'}})))
-
+    assert nan_inf_dataset.df.equals(
+        pd.DataFrame(
+            {
+                "A": {0: 1, 1: 2, 2: 3, 3: 4, 4: 5, 5: 6},
+                "B": {0: 6, 1: 5, 2: 4, 3: 3, 4: 2, 5: 1},
+                "C": {0: 1.0, 1: 2.0, 2: 3.0, 3: 2.5, 4: 2.5, 5: 4.0},
+                "D": {0: 2.5, 1: 1.0, 2: 2.0, 3: 3.0, 4: 4.0, 5: 2.5},
+                "E": {0: 5.0, 1: 5.5, 2: 5.5, 3: 5.5, 4: 5.5, 5: 6.0},
+                "F": {0: "g1", 1: "g1", 2: "g1", 3: "g2", 4: "g2", 5: "g2"},
+            }
+        )
+    )
 
 
 def test_subtract_from_datasets(small_2_plate_ds):
-    ds=small_2_plate_ds
+    ds = small_2_plate_ds
     ds.subtract_median(query_or_perturbation_name="FOV==1", groupby="BARCODE")
-    assert np.abs(np.sum(ds.df['feat_1'] - np.array([0.55,0.65,-0.55,-0.45,0.00,1.00])))<1e-6
+    assert (
+        np.abs(
+            np.sum(ds.df["feat_1"] - np.array([0.55, 0.65, -0.55, -0.45, 0.00, 1.00]))
+        )
+        < 1e-6
+    )
+
+
+def test_dataset_groupby(small_2_plate_df):
+    """Test split of a Dataset comprising the data below, by filename and FOV
+    ROW	COLUMN	BARCODE	feat_1	feat_2	feat_3	filename	FOV
+    1	1	    Plate1	1.2	    1.2	    1.3	    fileA.png	1
+    1	1	    Plate1	1.3	    1.4	    1.5	    FileB.png	2
+    1	1	    Plate2	5.2	    5.1	    5	    FileC.png	1
+    1	1	    Plate2	6.2	    6.1	    6.8	    FileD.png	2
+    1	2	    Plate1	0.1	    0.2	    0.3	    fileE.png	1
+    1	2	    Plate1	0.2	    0.2	    0.38    FileF.png	2
+
+    """
+    phe = phenonaut.Phenonaut(
+        small_2_plate_df, metadata={"features_prefix": "feat_"}
+    )
+    new_ds = phe.ds.new_aggregated_dataset(["ROW", "COLUMN", "BARCODE"])
+    split_ds = phe.ds.groupby(["FOV", "filename"])
+    assert len(split_ds) == 6
+    assert split_ds[0].df.FOV.unique()[0] == 1
+    assert split_ds[-1].df.FOV.unique()[0] == 2
```

### Comparing `phenonaut-1.3.4/test/test_phenonaut_obj.py` & `phenonaut-2.0.3/test/test_phenonaut_obj.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright © The University of Edinburgh, 2022.
+# Copyright © The University of Edinburgh, 2024.
 # Development has been supported by GSK.
 
-from curses import meta
-import pytest
-import phenonaut
-from phenonaut.data.dataset import Dataset
-import pandas as pd
-import numpy as np
 import tempfile
+from curses import meta
 from io import StringIO
 
+import numpy as np
+import pandas as pd
+import pytest
 
+import phenonaut
+from phenonaut.data.dataset import Dataset
 from phenonaut.phenonaut import Phenonaut
 
 
 def test_possible_dataset_combinations(phenonaut_object_iris_4_views):
     all_possible_views = phenonaut_object_iris_4_views.get_dataset_combinations()
     assert all_possible_views == (
         ("Iris_view1",),
@@ -32,15 +32,17 @@
         ("Iris_view1", "Iris_view3", "Iris_view4"),
         ("Iris_view2", "Iris_view3", "Iris_view4"),
         ("Iris_view1", "Iris_view2", "Iris_view3", "Iris_view4"),
     )
 
 
 def test_possible_dataset_combinations_indexes(phenonaut_object_iris_4_views):
-    all_possible_views = phenonaut_object_iris_4_views.get_dataset_combinations(return_indexes=True)
+    all_possible_views = phenonaut_object_iris_4_views.get_dataset_combinations(
+        return_indexes=True
+    )
     assert all_possible_views == (
         (0,),
         (1,),
         (2,),
         (3,),
         (0, 1),
         (0, 2),
@@ -67,28 +69,28 @@
     another_df = pd.DataFrame({"id2": [9, 8, 7], "A2": [1, 2, 3], "B": [4, 5, 6]})
     ph0 = phenonaut.Phenonaut(df, metadata={"features": ["B"]}, dataframe_name="Bob")
     assert ph0.ds.features == ["B"]
     assert ph0.ds.name == "Bob"
     ph0 = phenonaut.Phenonaut(df, metadata={"features_prefix": ["B"]})
     assert ph0.ds.features == ["B"]
     ph0 = phenonaut.Phenonaut(df, metadata={"features_prefix": ""})
-    assert set(ph0.ds.features) == set(["B", "A", "id"])
+    assert set(ph0.ds.features) == {"B", "A", "id"}
     ph0 = phenonaut.Phenonaut([df, another_df], metadata={"features_prefix": ""})
-    assert set(ph0.datasets[0].features) == set(["B", "A", "id"])
-    assert set(ph0.datasets[1].features) == set(["B", "A2", "id2"])
+    assert set(ph0.datasets[0].features) == {"B", "A", "id"}
+    assert set(ph0.datasets[1].features) == {"B", "A2", "id2"}
     ph0 = phenonaut.Phenonaut([df, another_df], metadata={"features": ["B"]})
-    assert set(ph0.datasets[0].features) == set(["B"])
-    assert set(ph0.datasets[1].features) == set(["B"])
+    assert set(ph0.datasets[0].features) == {"B"}
+    assert set(ph0.datasets[1].features) == {"B"}
     ph0 = phenonaut.Phenonaut(
         [df, another_df],
         metadata=[{"features": ["B"]}, {"features_prefix": ""}],
         dataframe_name=["Bob", "Robert"],
     )
-    assert set(ph0.datasets[0].features) == set(["B"])
-    assert set(ph0.datasets[1].features) == set(["A2", "B", "id2"])
+    assert set(ph0.datasets[0].features) == {"B"}
+    assert set(ph0.datasets[1].features) == {"A2", "B", "id2"}
     assert ph0.datasets[0].name == "Bob"
     assert ph0.datasets[-1].name == "Robert"
 
 
 def test_aggregate_dataset_in_ph0_obj():
     """Here we test a df as follows:
     ROW	COLUMN	BARCODE	feat_1	feat_2	feat_3	filename	FOV
@@ -123,15 +125,15 @@
             "FOV": [1, 2, 1, 2, 1, 2],
         }
     )
 
     phe = phenonaut.Phenonaut(df, metadata={"features_prefix": "feat_"})
     phe.aggregate_dataset(["ROW", "COLUMN", "BARCODE"])
     assert len(phe.datasets) == 2
-    assert set(phe.ds.features) == set(["feat_1", "feat_2", "feat_3"])
+    assert set(phe.ds.features) == {"feat_1", "feat_2", "feat_3"}
     assert abs(phe.ds.df["feat_1"][0] - 1.25 < 0.00001)
     assert np.abs(phe.ds.df["feat_1"][1] - 5.70 < 0.00001)
     assert np.abs(phe.ds.df["feat_1"][2] - 0.15 < 0.00001)
     assert np.abs(phe.ds.df["feat_2"][0] - 1.3 < 0.00001)
     assert np.abs(phe.ds.df["feat_2"][1] - 5.6 < 0.00001)
     assert np.abs(phe.ds.df["feat_2"][2] - 0.2 < 0.00001)
     assert np.abs(phe.ds.df["feat_3"][0] - 1.4 < 0.00001)
@@ -182,15 +184,15 @@
     phe.aggregate_dataset(
         ["ROW", "COLUMN", "BARCODE"],
         datasets=[0, 1],
         new_names_or_prefix=["M1", "M2"],
         inplace=True,
     )
     assert len(phe.datasets) == 2
-    assert set(phe.ds.features) == set(["feat_1", "feat_2", "feat_3"])
+    assert set(phe.ds.features) == {"feat_1", "feat_2", "feat_3"}
     assert abs(phe.ds.df["feat_1"][0] - 1.25 < 0.00001)
     assert np.abs(phe.ds.df["feat_1"][1] - 5.70 < 0.00001)
     assert np.abs(phe.ds.df["feat_1"][2] - 0.15 < 0.00001)
     assert np.abs(phe.ds.df["feat_2"][0] - 1.3 < 0.00001)
     assert np.abs(phe.ds.df["feat_2"][1] - 5.6 < 0.00001)
     assert np.abs(phe.ds.df["feat_2"][2] - 0.2 < 0.00001)
     assert np.abs(phe.ds.df["feat_3"][0] - 1.4 < 0.00001)
@@ -207,15 +209,14 @@
     del phe["Iris"]
     assert len(phe.datasets) == 1
     assert phe.datasets[0].name == "test_ds"
 
 
 def test_phe_save_load_and_revert(dataset_iris):
     tmp_file = tempfile.NamedTemporaryFile(delete=True)
-    print(tmp_file.file)
 
     try:
         phe = Phenonaut(dataset_iris)
         # Save, using overwrite_existing=True, as NamedTemporaryFile makes the
         # file, Phenonaut would then throw a warning saying it exists.
         phe.save(tmp_file.name, overwrite_existing=True)
 
@@ -232,37 +233,39 @@
     phe.clone_dataset("Iris", "Iris2")
     phe.clone_dataset("Iris", "Iris2", overwrite_existing=True)
     phe.clone_dataset("Iris", "Iris3", overwrite_existing=True)
     phe.clone_dataset("Iris", "Iris4", overwrite_existing=False)
     assert phe.keys() == ["Iris", "Iris2", "Iris3", "Iris4"]
 
 
-def test_readin_transformations():
-    df = pd.read_csv(
-        StringIO(
-            """"idx","Var1","Var2","value"
-        
-        "1","ENSG00000225972","A1_CPD1_PLATE1",4.0185
-        "2","ENSG00000225630","A1_CPD1_PLATE1",1.1539
-        "3","ENSG00000225972","A2_CPD2_PLATE1",10.6661
-        "4","ENSG00000225630","A2_CPD2_PLATE1",1.6130
-        "5","ENSG00000225972","A3_CPD3_PLATE1",0.1234
-        "6","ENSG00000225630","A3_CPD3_PLATE1",9.8436
-        "7","ENSG00000225972","A4_Pos_ctrl_PLATE1",0.1234
-        "8","ENSG00000225630","A4_Pos_ctrl_PLATE1",9.8436"""
-        )
-    ).reset_index()
-    phe = Phenonaut(
-        df,
-        "Test_df",
-        metadata={
-            "transforms": [
-                ("replace_str", ("Var2", "Pos_", "Pos-")),
-                ("split_column", ("Var2", "_", ["Well", "CpdID", "PlateID"])),
-                ("pivot", ("Var1", "value")),
-                #'transpose',
-                # (pivot_table(values = 'value', index=["WellName"], columns = 'Var1')
-            ],
-            "features_prefix": "ENSG",
-        },
+def test_splitting_dataset_in_ph0_obj(small_2_plate_df):
+    """Test the splitting of datasets using groupby"""
+    phe = phenonaut.Phenonaut(
+        small_2_plate_df, metadata={"features_prefix": "feat_"}
+    )
+    assert len(phe.datasets) == 1
+    phe.groupby_datasets(["FOV", "filename"])
+    assert len(phe.datasets) == 6
+
+    phe = phenonaut.Phenonaut(
+        small_2_plate_df, metadata={"features_prefix": "feat_"}
     )
-    print(phe.df)
+    assert len(phe.datasets) == 1
+    phe.groupby_datasets(["FOV", "filename"], remove_original=False)
+    assert len(phe.datasets) == 7
+
+
+def test_merge_datasets(small_2_plate_df):
+    """Test merging of datasets split using the groupby method"""
+    phe = phenonaut.Phenonaut(
+        small_2_plate_df, metadata={"features_prefix": "feat_"}
+    )
+    split_ds = phe.ds.groupby(["FOV", "filename"])
+    phe.merge_datasets(split_ds)
+    assert len(phe.ds.df) == len(small_2_plate_df)
+    del phe[-1]
+    merged_ds = phe.merge_datasets(split_ds, return_merged=True)
+    assert len(merged_ds.df) == len(small_2_plate_df)
+    phe.datasets.extend(split_ds)
+    del phe[0]
+    phe.merge_datasets(list(range(0, len(split_ds))))
+    assert len(phe.datasets) == 1
```

### Comparing `phenonaut-1.3.4/test/test_prediction.py` & `phenonaut-2.0.3/test/test_prediction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-# Copyright © The University of Edinburgh, 2022.
+# Copyright © The University of Edinburgh, 2024.
 # Development has been supported by GSK.
 
 import shutil
-import pandas as pd
+import tempfile
+from pathlib import Path
+
 import numpy as np
+import pandas as pd
+
 from phenonaut.output.heatmap import write_heatmap_from_df
 from phenonaut.phenonaut import Phenonaut
-from pathlib import Path
-import tempfile
 
 
 def test_get_y_from_iris_dataset(dataset_iris):
     from phenonaut.predict.predict_utils import get_y_from_target
 
     assert get_y_from_target(dataset_iris).shape == (150,)
```

### Comparing `phenonaut-1.3.4/test/test_preparation.py` & `phenonaut-2.0.3/test/test_preparation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,105 @@
-# Copyright © The University of Edinburgh, 2022.
+# Copyright © The University of Edinburgh, 2024.
 # Development has been supported by GSK.
 
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+import pytest
+
 from phenonaut import Phenonaut
 from phenonaut.data import Dataset
-import numpy as np
 from phenonaut.transforms.preparative import (
     VIF,
-    RemoveHighlyCorrelated,
     RemoveHighestCorrelatedThenVIF,
+    RemoveHighlyCorrelated,
 )
-import pandas as pd
-import pytest
-from pathlib import Path
 
 
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
 def test_VIF(sklearn_regression_df):
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
     vif = VIF()
     vif.filter(phe.ds, vif_cutoff=2, min_features=50)
     assert len(phe.ds.features) == 52
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
     vif = VIF()
     vif(phe.ds, vif_cutoff=2, min_features=60)
     assert len(phe.ds.features) == 79
 
 
 def test_RemoveHighlyCorrelated(sklearn_regression_df):
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
     rhc = RemoveHighlyCorrelated()
     rhc(phe.ds, threshold=0.3)
     assert len(phe.ds.features) == 95
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
     rhc = RemoveHighlyCorrelated()
     rhc(phe.ds, threshold=0.4, min_features=97)
     assert len(phe.ds.features) == 97
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
     rhc = RemoveHighlyCorrelated()
     rhc(phe.ds, threshold=None, min_features=5)
     assert len(phe.ds.features) == 5
 
 
 def test_RemoveHighestCorrelatedThenVIF(sklearn_regression_df):
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
     rhcvif = RemoveHighestCorrelatedThenVIF()
     rhcvif(phe.ds, n_before_vif=95, vif_cutoff=5.0)
     assert len(phe.ds.features) == 78
 
+
 def test_SimpleImputer(sklearn_regression_df):
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
-    df=phe.ds.df
-    df.loc[1, phe.ds.features]=np.nan
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
+    df = phe.ds.df
+    df.loc[1, phe.ds.features] = np.nan
     print(phe.df[phe.ds.features].head())
     from phenonaut.transforms.imputers import SimpleImputer
-    imputer=SimpleImputer()
+
+    imputer = SimpleImputer()
     imputer(phe)
     assert not phe.ds.data.isnull().values.any()
 
 
 def test_KNNImputer(sklearn_regression_df):
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
-    df=phe.ds.df
-    df.loc[1, phe.ds.features]=np.nan
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
+    df = phe.ds.df
+    df.loc[1, phe.ds.features] = np.nan
     print(phe.df[phe.ds.features].head())
     from phenonaut.transforms.imputers import KNNImputer
-    imputer=KNNImputer()
+
+    imputer = KNNImputer()
     imputer(phe)
     assert not phe.ds.data.isnull().values.any()
 
+
 def test_RFImputer(sklearn_regression_df):
-    phe = Phenonaut(sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"})
-    df=phe.ds.df
-    df.loc[1, phe.ds.features]=np.nan
+    phe = Phenonaut(
+        sklearn_regression_df, "PheSmallDS", metadata={"features_prefix": "feat_"}
+    )
+    df = phe.ds.df
+    df.loc[1, phe.ds.features] = np.nan
     print(phe.df[phe.ds.features].head())
     from phenonaut.transforms.imputers import RFImputer
-    imputer=RFImputer(max_iter=3)
+
+    imputer = RFImputer(max_iter=3)
     imputer(phe)
     print(phe.df[phe.ds.features].head())
-    assert not phe.ds.data.isnull().values.any()
+    assert not phe.ds.data.isnull().values.any()
```

### Comparing `phenonaut-1.3.4/test/test_transformations.py` & `phenonaut-2.0.3/test/test_transformations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright © The University of Edinburgh, 2023.
+# Copyright © The University of Edinburgh, 2024.
 # Development has been supported by GSK.
-import phenonaut
 import pandas as pd
+import numpy as np
+import phenonaut
 import phenonaut.transforms
 
 
 def test_transforms_standardscaler(small_2_plate_df):
     phe = phenonaut.Phenonaut(small_2_plate_df)
     stdscaler = phenonaut.transforms.StandardScaler()
     stdscaler(phe.ds)
@@ -16,15 +17,16 @@
 
 
 def test_transforms_pca(small_2_plate_df):
     phe = phenonaut.Phenonaut(small_2_plate_df)
     t_pca = phenonaut.transforms.PCA()
     t_pca(phe.ds)
     assert (
-        phe.df["PC_2"] - pd.Series([0.033607, -0.005505, 0.342870, -0.276157, -0.037338, -0.057477])
+        phe.df["PC_2"]
+        - pd.Series([0.033607, -0.005505, 0.342870, -0.276157, -0.037338, -0.057477])
     ).abs().mean() < 1e-6
 
 
 def test_transforms_zca(small_2_plate_df):
     phe = phenonaut.Phenonaut(small_2_plate_df)
     t_zca = phenonaut.transforms.ZCA()
     t_zca(phe.ds)
@@ -49,15 +51,16 @@
     t_umap = phenonaut.transforms.UMAP()
     t_umap(phe.ds)
     assert len(phe.ds.features) == 2
 
 
 def test_transforms_custom_callable_square(small_2_plate_df):
     phe = phenonaut.Phenonaut(small_2_plate_df)
-    from numpy import square, all as np_all
+    from numpy import all as np_all
+    from numpy import square
 
     f1_series = phe.ds.data.values[:, 0]
     t_square = phenonaut.transforms.Transformer(square)
     t_square(phe.ds)
     assert np_all(f1_series * f1_series == phe.ds.data.values[:, 0])
 
 
@@ -81,7 +84,8 @@
     phe = phenonaut.Phenonaut(small_2_plate_df)
     log2_t = phenonaut.transforms.Log2()
     log2_t(phe.ds)
     assert (
         phe.df["log2_feat_3"]
         - pd.Series([0.378512, 0.584963, 2.321928, 2.765535, -1.736966, -1.395929])
     ).abs().sum() < 2e-6
+
```

