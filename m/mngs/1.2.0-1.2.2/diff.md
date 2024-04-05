# Comparing `tmp/mngs-1.2.0.tar.gz` & `tmp/mngs-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mngs-1.2.0.tar", last modified: Thu Apr  4 08:47:32 2024, max compression
+gzip compressed data, was "mngs-1.2.2.tar", last modified: Fri Apr  5 06:24:19 2024, max compression
```

## Comparing `mngs-1.2.0.tar` & `mngs-1.2.2.tar`

### file list

```diff
@@ -1,193 +1,215 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.896993 mngs-1.2.0/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)    35149 2024-02-03 10:31:02.000000 mngs-1.2.0/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.2.0/MANIFEST.in
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1793 2024-04-04 08:47:32.896993 mngs-1.2.0/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      295 2024-02-03 10:31:02.000000 mngs-1.2.0/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-04 08:47:32.896993 mngs-1.2.0/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.0/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.876993 mngs-1.2.0/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.878993 mngs-1.2.0/src/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      482 2024-04-04 08:47:16.000000 mngs-1.2.0/src/mngs/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.879993 mngs-1.2.0/src/mngs/dsp/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.2.0/src/mngs/dsp/PARAMS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      300 2024-04-04 08:41:51.000000 mngs-1.2.0/src/mngs/dsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3783 2024-04-03 02:08:42.000000 mngs-1.2.0/src/mngs/dsp/_demo_sig.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      338 2024-04-02 12:33:00.000000 mngs-1.2.0/src/mngs/dsp/_ensure_3d.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1455 2024-04-03 21:02:11.000000 mngs-1.2.0/src/mngs/dsp/_hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.2.0/src/mngs/dsp/_mne.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1710 2024-04-04 08:07:31.000000 mngs-1.2.0/src/mngs/dsp/_psd.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1749 2024-04-04 02:34:34.000000 mngs-1.2.0/src/mngs/dsp/_transform.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2848 2024-04-03 20:26:59.000000 mngs-1.2.0/src/mngs/dsp/_wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2791 2024-04-02 11:21:03.000000 mngs-1.2.0/src/mngs/dsp/add_noise.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1232 2024-04-04 02:23:09.000000 mngs-1.2.0/src/mngs/dsp/filt.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.2.0/src/mngs/dsp/ref.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.881993 mngs-1.2.0/src/mngs/general/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1065 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/TimeStamper.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1494 2024-04-02 10:35:31.000000 mngs-1.2.0/src/mngs/general/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2146 2024-03-11 03:28:22.000000 mngs-1.2.0/src/mngs/general/_close.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8880 2024-04-04 02:22:41.000000 mngs-1.2.0/src/mngs/general/_converters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.2.0/src/mngs/general/_norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/_shell.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3822 2024-03-25 01:12:15.000000 mngs-1.2.0/src/mngs/general/_start.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/_xml2dict.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/cuda_collect_env.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2144 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/debug.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/email.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/latex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.2.0/src/mngs/general/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/mat2py.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22093 2024-04-01 10:51:59.000000 mngs-1.2.0/src/mngs/general/misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/pandas.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.0/src/mngs/general/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3941 2024-02-17 20:51:51.000000 mngs-1.2.0/src/mngs/general/repro.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.0/src/mngs/general/save.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/general/torch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.881993 mngs-1.2.0/src/mngs/gists/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/gists/_SigMacro_processFigure_S.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/gists/_SigMacro_toBlue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/gists/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.882993 mngs-1.2.0/src/mngs/io/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-02-04 02:18:33.000000 mngs-1.2.0/src/mngs/io/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.2.0/src/mngs/io/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.0/src/mngs/io/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.0/src/mngs/io/save.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.882993 mngs-1.2.0/src/mngs/linalg/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/linalg/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/linalg/_misc.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.883993 mngs-1.2.0/src/mngs/ml/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/ClassificationReporter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/ClassifierServer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.2.0/src/mngs/ml/EarlyStopping.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/LearningCurveLogger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/__Classifiers.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.2.0/src/mngs/ml/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.883993 mngs-1.2.0/src/mngs/ml/act/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/act/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/act/_define.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.884993 mngs-1.2.0/src/mngs/ml/clustering/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.2.0/src/mngs/ml/clustering/_UMAP.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.2.0/src/mngs/ml/clustering/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.2.0/src/mngs/ml/clustering/_umap.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.884993 mngs-1.2.0/src/mngs/ml/layer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/layer/_Pass.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/layer/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/layer/_switch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.885993 mngs-1.2.0/src/mngs/ml/loss/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/loss/MultiTaskLoss.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/loss/_L1L2Losses.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/loss/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.885993 mngs-1.2.0/src/mngs/ml/metrics/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.2.0/src/mngs/ml/metrics/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.2.0/src/mngs/ml/metrics/_bACC.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.885993 mngs-1.2.0/src/mngs/ml/optim/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.885993 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.886993 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/optim/_get_set.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.887993 mngs-1.2.0/src/mngs/ml/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.2.0/src/mngs/ml/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.2.0/src/mngs/ml/plt/_conf_mat.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.2.0/src/mngs/ml/plt/_learning_curve.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.2.0/src/mngs/ml/plt/_optuna_study.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.888993 mngs-1.2.0/src/mngs/ml/plt/aucs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/plt/aucs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/plt/aucs/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/plt/aucs/pre_rec_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/plt/aucs/roc_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/silhoute_score_block.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.888993 mngs-1.2.0/src/mngs/ml/sk/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.2.0/src/mngs/ml/sk/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.2.0/src/mngs/ml/sk/_clf.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.2.0/src/mngs/ml/sk/_to_sktime.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.889993 mngs-1.2.0/src/mngs/ml/utils/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_DefaultDataset.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.2.0/src/mngs/ml/utils/_LabelEncoder.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.2.0/src/mngs/ml/utils/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.2.0/src/mngs/ml/utils/_check_params.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_format_samples_for_sktime.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.2.0/src/mngs/ml/utils/_merge_labels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_sliding_window_data_augmentation.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_under_sample.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/ml/utils/_verify_n_gpus.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.890993 mngs-1.2.0/src/mngs/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/mngs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/mngs/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.891993 mngs-1.2.0/src/mngs/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.0/src/mngs/nn/_AxiswiseDropout.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_BNet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_BNet_Res.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3998 2024-04-02 14:06:31.000000 mngs-1.2.0/src/mngs/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.0/src/mngs/nn/_GaussianFilter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-02 12:48:08.000000 mngs-1.2.0/src/mngs/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_MNet_1000.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.0/src/mngs/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_ResNet1D.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_SpatialAttention.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.0/src/mngs/nn/_Spectrogram.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/nn/_SwapChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.0/src/mngs/nn/_TransposeLayer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9428 2024-04-02 09:35:04.000000 mngs-1.2.0/src/mngs/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      838 2024-04-02 13:16:20.000000 mngs-1.2.0/src/mngs/nn/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.891993 mngs-1.2.0/src/mngs/os/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.2.0/src/mngs/os/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1342 2024-03-02 10:35:45.000000 mngs-1.2.0/src/mngs/os/_mv.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.892993 mngs-1.2.0/src/mngs/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.2.0/src/mngs/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_add_hue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_annotated_heatmap.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5710 2024-03-07 15:07:44.000000 mngs-1.2.0/src/mngs/plt/_configure_mpl.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_draw_a_cube.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_get_RGBA_from_colormap.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_mk_colorbar.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/_mk_patches.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9875 2024-02-04 02:05:41.000000 mngs-1.2.0/src/mngs/plt/_subplots.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.2.0/src/mngs/plt/_tpl.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.893993 mngs-1.2.0/src/mngs/plt/ax/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      436 2024-03-07 12:38:36.000000 mngs-1.2.0/src/mngs/plt/ax/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_circular_hist.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_extend.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_fill_between.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.2.0/src/mngs/plt/ax/_hide_spines.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_map_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_panel.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_sci_note.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      395 2024-03-29 22:04:00.000000 mngs-1.2.0/src/mngs/plt/ax/_set_n_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.2.0/src/mngs/plt/ax/_set_pos.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/ax/_set_size.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/colors.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/plt/get_mpl_color.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.894993 mngs-1.2.0/src/mngs/resource/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/resource/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/resource/get.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/resource/limit_RAM.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.895993 mngs-1.2.0/src/mngs/stats/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.2.0/src/mngs/stats/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_bonferroni_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_brunner_munzel_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_calc_partial_corr.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_corr_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_fdr_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.2.0/src/mngs/stats/_general.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_multicompair.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_nocorrelation_test.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_smirnov_grubbs.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.2.0/src/mngs/stats/_to_asterisks.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.895993 mngs-1.2.0/src/mngs/torch/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.2.0/src/mngs/torch/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.2.0/src/mngs/torch/_apply_to.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-04 08:47:32.895993 mngs-1.2.0/src/mngs.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1793 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4901 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      375 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-04 08:47:32.000000 mngs-1.2.0/src/mngs.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.371817 mngs-1.2.2/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)    35149 2024-02-03 10:31:02.000000 mngs-1.2.2/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.2.2/MANIFEST.in
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1793 2024-04-05 06:24:19.371817 mngs-1.2.2/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      295 2024-02-03 10:31:02.000000 mngs-1.2.2/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-05 06:24:19.375817 mngs-1.2.2/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.2/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.357818 mngs-1.2.2/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.359818 mngs-1.2.2/src/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      482 2024-04-05 06:24:14.000000 mngs-1.2.2/src/mngs/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.360818 mngs-1.2.2/src/mngs/dsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.2.2/src/mngs/dsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      365 2024-04-05 01:14:27.000000 mngs-1.2.2/src/mngs/dsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5064 2024-04-05 05:01:38.000000 mngs-1.2.2/src/mngs/dsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1455 2024-04-03 21:02:11.000000 mngs-1.2.2/src/mngs/dsp/_hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      539 2024-04-05 01:14:09.000000 mngs-1.2.2/src/mngs/dsp/_misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.2.2/src/mngs/dsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1710 2024-04-04 08:07:31.000000 mngs-1.2.2/src/mngs/dsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1672 2024-04-04 21:38:57.000000 mngs-1.2.2/src/mngs/dsp/_resample.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1749 2024-04-04 02:34:34.000000 mngs-1.2.2/src/mngs/dsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2848 2024-04-03 20:26:59.000000 mngs-1.2.2/src/mngs/dsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2755 2024-04-05 03:19:19.000000 mngs-1.2.2/src/mngs/dsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5938 2024-04-05 06:19:44.000000 mngs-1.2.2/src/mngs/dsp/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1909 2024-04-04 10:07:16.000000 mngs-1.2.2/src/mngs/dsp/filt.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.361817 mngs-1.2.2/src/mngs/dsp/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.2/src/mngs/dsp/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7079 2024-04-05 02:45:12.000000 mngs-1.2.2/src/mngs/dsp/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.2/src/mngs/dsp/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-02 12:48:08.000000 mngs-1.2.2/src/mngs/dsp/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.2/src/mngs/dsp/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.2/src/mngs/dsp/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.2/src/mngs/dsp/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9524 2024-04-05 01:09:23.000000 mngs-1.2.2/src/mngs/dsp/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      838 2024-04-02 13:16:20.000000 mngs-1.2.2/src/mngs/dsp/nn/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      471 2024-04-05 01:15:43.000000 mngs-1.2.2/src/mngs/dsp/norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.2.2/src/mngs/dsp/ref.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.363818 mngs-1.2.2/src/mngs/general/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1065 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/TimeStamper.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1478 2024-04-04 11:51:21.000000 mngs-1.2.2/src/mngs/general/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2146 2024-03-11 03:28:22.000000 mngs-1.2.2/src/mngs/general/_close.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8880 2024-04-04 02:22:41.000000 mngs-1.2.2/src/mngs/general/_converters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.2.2/src/mngs/general/_norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/_shell.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3822 2024-03-25 01:12:15.000000 mngs-1.2.2/src/mngs/general/_start.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/_xml2dict.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/cuda_collect_env.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2144 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/debug.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/email.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/latex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.2.2/src/mngs/general/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/mat2py.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22093 2024-04-01 10:51:59.000000 mngs-1.2.2/src/mngs/general/misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/pandas.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.2/src/mngs/general/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3941 2024-02-17 20:51:51.000000 mngs-1.2.2/src/mngs/general/repro.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.2/src/mngs/general/save.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/torch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.363818 mngs-1.2.2/src/mngs/gists/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/gists/_SigMacro_processFigure_S.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/gists/_SigMacro_toBlue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/gists/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.363818 mngs-1.2.2/src/mngs/io/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-02-04 02:18:33.000000 mngs-1.2.2/src/mngs/io/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.2.2/src/mngs/io/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.2/src/mngs/io/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.2/src/mngs/io/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.363818 mngs-1.2.2/src/mngs/linalg/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/linalg/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/linalg/_misc.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.364817 mngs-1.2.2/src/mngs/ml/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/ClassificationReporter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/ClassifierServer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.2.2/src/mngs/ml/EarlyStopping.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/LearningCurveLogger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/__Classifiers.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.2.2/src/mngs/ml/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.364817 mngs-1.2.2/src/mngs/ml/act/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/act/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/act/_define.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.364817 mngs-1.2.2/src/mngs/ml/clustering/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.2.2/src/mngs/ml/clustering/_UMAP.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.2.2/src/mngs/ml/clustering/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.2.2/src/mngs/ml/clustering/_umap.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.364817 mngs-1.2.2/src/mngs/ml/layer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/layer/_Pass.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/layer/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/layer/_switch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/loss/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/loss/MultiTaskLoss.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/loss/_L1L2Losses.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/loss/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/metrics/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.2.2/src/mngs/ml/metrics/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.2.2/src/mngs/ml/metrics/_bACC.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/optim/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/_get_set.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.2.2/src/mngs/ml/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.2.2/src/mngs/ml/plt/_conf_mat.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.2.2/src/mngs/ml/plt/_learning_curve.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.2.2/src/mngs/ml/plt/_optuna_study.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.366817 mngs-1.2.2/src/mngs/ml/plt/aucs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/plt/aucs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/plt/aucs/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/plt/aucs/pre_rec_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/plt/aucs/roc_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/silhoute_score_block.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.366817 mngs-1.2.2/src/mngs/ml/sk/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.2.2/src/mngs/ml/sk/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.2.2/src/mngs/ml/sk/_clf.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.2.2/src/mngs/ml/sk/_to_sktime.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.367817 mngs-1.2.2/src/mngs/ml/utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_DefaultDataset.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.2.2/src/mngs/ml/utils/_LabelEncoder.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.2.2/src/mngs/ml/utils/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.2.2/src/mngs/ml/utils/_check_params.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_format_samples_for_sktime.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.2.2/src/mngs/ml/utils/_merge_labels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_sliding_window_data_augmentation.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_under_sample.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_verify_n_gpus.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.367817 mngs-1.2.2/src/mngs/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/mngs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/mngs/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.368817 mngs-1.2.2/src/mngs/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.2/src/mngs/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7079 2024-04-05 02:45:12.000000 mngs-1.2.2/src/mngs/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.2/src/mngs/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-02 12:48:08.000000 mngs-1.2.2/src/mngs/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.2/src/mngs/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.2/src/mngs/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.2/src/mngs/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9524 2024-04-05 01:09:23.000000 mngs-1.2.2/src/mngs/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      838 2024-04-02 13:16:20.000000 mngs-1.2.2/src/mngs/nn/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.368817 mngs-1.2.2/src/mngs/os/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.2.2/src/mngs/os/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1342 2024-03-02 10:35:45.000000 mngs-1.2.2/src/mngs/os/_mv.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.369817 mngs-1.2.2/src/mngs/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.2.2/src/mngs/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_add_hue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_annotated_heatmap.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5827 2024-04-05 06:07:27.000000 mngs-1.2.2/src/mngs/plt/_configure_mpl.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_draw_a_cube.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_get_RGBA_from_colormap.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_mk_colorbar.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_mk_patches.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9875 2024-02-04 02:05:41.000000 mngs-1.2.2/src/mngs/plt/_subplots.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.2.2/src/mngs/plt/_tpl.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.369817 mngs-1.2.2/src/mngs/plt/ax/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      436 2024-03-07 12:38:36.000000 mngs-1.2.2/src/mngs/plt/ax/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_circular_hist.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_extend.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_fill_between.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.2.2/src/mngs/plt/ax/_hide_spines.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_map_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_panel.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_sci_note.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      389 2024-04-05 02:48:46.000000 mngs-1.2.2/src/mngs/plt/ax/_set_n_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.2.2/src/mngs/plt/ax/_set_pos.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_set_size.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/colors.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/get_mpl_color.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.370817 mngs-1.2.2/src/mngs/resource/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/resource/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/resource/get.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/resource/limit_RAM.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.370817 mngs-1.2.2/src/mngs/stats/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.2.2/src/mngs/stats/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_bonferroni_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_brunner_munzel_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_calc_partial_corr.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_corr_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_fdr_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.2.2/src/mngs/stats/_general.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_multicompair.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_nocorrelation_test.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_smirnov_grubbs.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_to_asterisks.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.371817 mngs-1.2.2/src/mngs/torch/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.2.2/src/mngs/torch/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.2.2/src/mngs/torch/_apply_to.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.371817 mngs-1.2.2/src/mngs.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1793 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5535 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      375 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/top_level.txt
```

### Comparing `mngs-1.2.0/LICENSE` & `mngs-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/PKG-INFO` & `mngs-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mngs
-Version: 1.2.0
+Version: 1.2.2
 Summary: For lazy python users (monogusa people in Japanse), especially in ML/DSP fields
 Home-page: https://github.com/ywatanabe1989/mngs
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: GPL3.0
 Keywords: utils,utilities,python,machine learning
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mngs-1.2.0/setup.py` & `mngs-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/dsp/PARAMS.py` & `mngs-1.2.2/src/mngs/dsp/PARAMS.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/dsp/_demo_sig.py` & `mngs-1.2.2/src/mngs/dsp/_demo_sig.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-03 13:08:41 (ywatanabe)"
+# Time-stamp: "2024-04-05 16:01:37 (ywatanabe)"
 
 import random
+import warnings
 
 import mne
 import numpy as np
 from mne import Epochs, compute_covariance, find_events, make_ad_hoc_cov
 from mne.datasets import sample
 from mne.simulation import (
     add_ecg,
@@ -18,80 +19,113 @@
 from ripple_detection.simulate import simulate_LFP, simulate_time
 from scipy.signal import chirp
 
 
 def demo_sig(
     batch_size=8,
     n_chs=19,
-    t_sec=3,
+    t_sec=4,
     fs=512,
-    freqs_hz="random",
-    type="periodic",
+    freqs_hz=None,
+    sig_type="periodic",
+    verbose=False,
 ):
-    tt = np.linspace(0, t_sec, int(t_sec * fs))
-    if type == "meg":
+
+    assert sig_type in [
+        "uniform",
+        "gauss",
+        "periodic",
+        "chirp",
+        "ripple",
+        "meg",
+    ]
+    tt = np.linspace(0, t_sec, int(t_sec * fs), endpoint=False)
+
+    if sig_type == "uniform":
+        return (
+            np.random.uniform(
+                low=-0.5, high=0.5, size=(batch_size, n_chs, len(tt))
+            ),
+            tt,
+            fs,
+        )
+
+    if sig_type == "gauss":
+        return np.random.randn(batch_size, n_chs, len(tt)), tt, fs
+
+    elif sig_type == "meg":
         return (
             _demo_sig_meg(
-                batch_size=batch_size, n_chs=n_chs, t_sec=t_sec, fs=fs
-            ).astype(np.float32),
+                batch_size=batch_size,
+                n_chs=n_chs,
+                t_sec=t_sec,
+                fs=fs,
+                verbose=verbose,
+            ).astype(np.float32)[..., : len(tt)],
             tt,
             fs,
         )
 
     else:
         fn_1d = {
             "periodic": _demo_sig_periodic_1d,
             "chirp": _demo_sig_chirp_1d,
             "ripple": _demo_sig_ripple_1d,
-        }.get(type)
+        }.get(sig_type)
 
         return (
             (
                 np.array(
                     [
                         fn_1d(
                             t_sec=t_sec,
                             fs=fs,
                             freqs_hz=freqs_hz,
+                            verbose=verbose,
                         )
                         for _ in range(int(batch_size * n_chs))
                     ]
                 )
                 .reshape(batch_size, n_chs, -1)
-                .astype(np.float32)
+                .astype(np.float32)[..., : len(tt)]
             ),
             tt,
             fs,
         )
 
 
-def _demo_sig_meg(batch_size=8, n_chs=19, t_sec=10, fs=512, **kwargs):
+def _demo_sig_meg(
+    batch_size=8, n_chs=19, t_sec=10, fs=512, verbose=False, **kwargs
+):
     data_path = sample.data_path()
     meg_path = data_path / "MEG" / "sample"
     raw_fname = meg_path / "sample_audvis_raw.fif"
     fwd_fname = meg_path / "sample_audvis-meg-eeg-oct-6-fwd.fif"
 
     # Load real data as the template
-    raw = mne.io.read_raw_fif(raw_fname)
-    raw.set_eeg_reference(projection=True)
+    raw = mne.io.read_raw_fif(raw_fname, verbose=verbose)
+    raw = raw.crop(tmax=t_sec, verbose=verbose)
+    raw = raw.resample(fs, verbose=verbose)
+    raw.set_eeg_reference(projection=True, verbose=verbose)
+
+    return raw.get_data(
+        picks=raw.ch_names[: batch_size * n_chs], verbose=verbose
+    ).reshape(batch_size, n_chs, -1)
 
-    raw = raw.resample(fs)
-    raw = raw.crop(tmax=t_sec)
 
-    return raw.get_data(picks=raw.ch_names[: batch_size * n_chs]).reshape(
-        batch_size, n_chs, -1
-    )
-
-
-def _demo_sig_periodic_1d(t_sec=10, fs=512, freqs_hz="random", **kwargs):
+def _demo_sig_periodic_1d(
+    t_sec=10, fs=512, freqs_hz=None, verbose=False, **kwargs
+):
     """Returns a demo signal with the shape (t_sec*fs,)."""
 
-    if freqs_hz == "random":
+    if freqs_hz is None:
         n_freqs = random.randint(1, 5)
         freqs_hz = np.random.permutation(np.arange(fs))[:n_freqs]
+        if verbose:
+            print(f"freqs_hz was randomly determined as {freqs_hz}")
 
     n = int(t_sec * fs)
     t = np.linspace(0, t_sec, n, endpoint=False)
 
     summed = np.array(
         [
             np.random.rand()
@@ -99,21 +133,25 @@
             for f_hz in freqs_hz
         ]
     ).sum(axis=0)
     return summed
 
 
 def _demo_sig_chirp_1d(
-    t_sec=10, fs=512, low_hz="random", high_hz="random", **kwargs
+    t_sec=10, fs=512, low_hz=None, high_hz=None, verbose=False, **kwargs
 ):
-    if low_hz == "random":
+    if low_hz is None:
         low_hz = random.randint(1, 20)
+        if verbose:
+            warnings.warn(f"low_hz was randomly determined as {low_hz}.")
 
-    if high_hz == "random":
+    if high_hz is None:
         high_hz = random.randint(100, 1000)
+        if verbose:
+            warnings.warn(f"high_hz was randomly determined as {high_hz}.")
 
     n = int(t_sec * fs)
     t = np.linspace(0, t_sec, n, endpoint=False)
     x = chirp(t, low_hz, t[-1], high_hz)
     x *= 1.0 + 0.5 * np.sin(2.0 * np.pi * 3.0 * t)
     return x
 
@@ -123,21 +161,25 @@
     t = simulate_time(n_samples, fs)
     n_ripples = random.randint(1, 5)
     mid_time = np.random.permutation(t)[:n_ripples]
     return simulate_LFP(t, mid_time, noise_amplitude=1.2, ripple_amplitude=5)
 
 
 if __name__ == "__main__":
-    mm = demo_sig(type="meg")
-    pp = demo_sig(type="periodic")
-    cc = demo_sig(type="chirp")
-    rr = demo_sig(type="ripple")
-
-    fig, axes = mngs.plt.subplots(nrows=4)
-    axes[0].plot(mm[0, 0], label="meg")
-    axes[1].plot(pp[0, 0], label="periodic")
-    axes[2].plot(cc[0, 0], label="chirp")
-    axes[3].plot(rr[0, 0], label="ripple")
+    uu, tt, fs = demo_sig(sig_type="uniform")
+    gg, tt, fs = demo_sig(sig_type="gauss")
+    mm, tt, fs = demo_sig(sig_type="meg")
+    pp, tt, fs = demo_sig(sig_type="periodic")
+    cc, tt, fs = demo_sig(sig_type="chirp")
+    rr, tt, fs = demo_sig(sig_type="ripple")
+
+    fig, axes = mngs.plt.subplots(nrows=6)
+    axes[0].plot(uu[0, 0], label="uniform")
+    axes[1].plot(gg[0, 0], label="gauss")
+    axes[2].plot(mm[0, 0], label="meg")
+    axes[3].plot(pp[0, 0], label="periodic")
+    axes[4].plot(cc[0, 0], label="chirp")
+    axes[5].plot(rr[0, 0], label="ripple")
     for ax in axes:
         ax.legend(loc="upper right")
 
     plt.show()
```

### Comparing `mngs-1.2.0/src/mngs/dsp/_hilbert.py` & `mngs-1.2.2/src/mngs/dsp/_hilbert.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/dsp/_mne.py` & `mngs-1.2.2/src/mngs/dsp/_mne.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/dsp/_psd.py` & `mngs-1.2.2/src/mngs/dsp/_psd.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/dsp/_transform.py` & `mngs-1.2.2/src/mngs/dsp/_transform.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/dsp/_wavelet.py` & `mngs-1.2.2/src/mngs/dsp/_wavelet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/dsp/add_noise.py` & `mngs-1.2.2/src/mngs/dsp/add_noise.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-02 22:21:02 (ywatanabe)"
+# Time-stamp: "2024-04-05 14:19:18 (ywatanabe)"
 
 import mngs
 
 # import numpy as np
 import torch
 from mngs.general import torch_fn
 
@@ -50,28 +50,28 @@
     return x + noise.to(x.device)
 
 
 @torch_fn
 def brown(x, amp=1.0, dim=-1):
     noise = _uniform(x.shape, amp=amp)
     noise = torch.cumsum(noise, dim=dim)
-    noise = mngs.gen.unbias(noise, dim=dim)
-    noise = mngs.gen.to_1_1(noise, amp=amp, dim=dim)
+    noise = mngs.dsp.norm.minmax(noise, amp=amp, dim=dim)
     return x + noise.to(x.device)
 
 
 if __name__ == "__main__":
     import matplotlib.pyplot as plt
 
     plt, CC = mngs.plt.configure_mpl(plt)
 
     t_sec = 1
     fs = 128
-    x = torch.tensor(mngs.dsp.demo_sig(t_sec=t_sec, fs=fs))
-    t = np.linspace(0, t_sec, x.shape[-1])
+    xx, tt, fs = mngs.dsp.demo_sig(t_sec=t_sec, fs=fs)
+
+    # t = np.linspace(0, t_sec, x.shape[-1])
 
     funcs = {
         "orig": lambda x: x,
         "gauss": gauss,
         "white": white,
         "pink": pink,
         "brown": brown,
@@ -80,17 +80,17 @@
     fig, axes = plt.subplots(
         nrows=len(funcs), ncols=2, sharex=True, sharey=True
     )
     count = 0
     for (k, fn), axes_row in zip(funcs.items(), axes):
         for ax in axes_row:
             if count % 2 == 0:
-                ax.plot(t, fn(x)[0, 0], label=k, c="blue")
+                ax.plot(tt, fn(xx)[0, 0], label=k, c="blue")
             else:
-                ax.plot(t, (fn(x) - x)[0, 0], label=f"{k} - orig", c="red")
+                ax.plot(tt, (fn(xx) - xx)[0, 0], label=f"{k} - orig", c="red")
             count += 1
             ax.legend(loc="upper right")
     plt.show()
 
     # fig, axes = plt.subplots(nrows=len(funcs), sharex=True, sharey=True)
     # for (k, fn), ax in zip(funcs.items(), axes):
     #     ax.plot(t, fn(x)[0, 0], label=k, c="blue")
```

### Comparing `mngs-1.2.0/src/mngs/dsp/filt.py` & `mngs-1.2.2/src/mngs/dsp/filt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-04 13:23:08 (ywatanabe)"
+# Time-stamp: "2024-04-04 21:07:15 (ywatanabe)"
 
 
 import mngs
-import scipy.ndimage
-import torch
 from mngs.general import torch_fn
-from mngs.nn import BandPassFilter, GaussianFilter
-
-# @torch_fn
-# def resample(x, src_fs, tgt_fs):
-#     resampler = T.Resample(src_fs, tgt_fs, dtype=x.dtype).to(x.device)
-#     return resampler(x)
+from mngs.nn import BandPassFilter, BandStopFilter, GaussianFilter
 
 
 @torch_fn
 def gauss(x, sigma):
     return GaussianFilter(sigma)(x)
 
 
 @torch_fn
 def bandpass(x, samp_rate, low_hz, high_hz):
     return BandPassFilter(low_hz, high_hz, samp_rate)(x)
 
 
 @torch_fn
 def bandstop(x, samp_rate, low_hz, high_hz):
-    return BandPassFilter(low_hz, high_hz, samp_rate)(x)
+    return BandStopFilter(low_hz, high_hz, samp_rate)(x)
 
 
 def _custom_print(x):
     print(type(x), x.shape)
 
 
 if __name__ == "__main__":
+    import torch
+
     t_sec = 10
     src_fs = 1024
     tgt_fs = 128
     freqs_hz = [30, 60, 100, 200, 1000]
 
-    x = mngs.dsp.demo_sig(
+    xx, tt, fs = mngs.dsp.demo_sig(
         t_sec=t_sec, fs=src_fs, freqs_hz=freqs_hz, type="ripple"
     )
+    tt_resampled = mngs.dsp.resample(tt, src_fs, tgt_fs)
+
+    # Filtering
+    filted_bp = mngs.dsp.filt.bandpass(xx, fs, low_hz=20, high_hz=50)
+    filted_bs = mngs.dsp.filt.bandstop(xx, fs, low_hz=20, high_hz=50)
+    filted_gauss = mngs.dsp.filt.gauss(xx, sigma=3)
+
+    # Plots
+    fig, axes = plt.subplots(nrows=5, ncols=1, sharex=True, sharey=True)
+    i_batch = 0
+    i_ch = 0
+    axes[0].plot(tt, xx[i_batch, i_ch], label="Original")
+    axes[1].plot(tt_resampled, resampled[i_batch, i_ch], label="Resampled")
+    axes[2].plot(tt, filted_bp[i_batch, i_ch], label="Bandpass-filtered")
+    # axes[3].plot(tt, filted_bs[i_batch, i_ch], label="Bandstop-filtered")
+    # axes[4].plot(tt, filted_gauss[i_batch, i_ch], label="Gaussian-filtered")
+    for ax in axes:
+        ax.legend(loc="upper left")
+    plt.show()
 
     mngs.dsp.filt.bandpass(x, src_fs, low_hz=55, high_hz=65)
 
     _custom_print(x)
     for xx in [x, torch.tensor(x)]:
         _custom_print(gauss(xx, 6))
         _custom_print(bandpass(xx, src_fs, low_hz=55, high_hz=65))
```

### Comparing `mngs-1.2.0/src/mngs/dsp/ref.py` & `mngs-1.2.2/src/mngs/dsp/ref.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/TimeStamper.py` & `mngs-1.2.2/src/mngs/general/TimeStamper.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/__init__.py` & `mngs-1.2.2/src/mngs/general/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     numpy_fn,
     squeeze_if,
     to_numpy,
     to_torch,
     torch_fn,
     unsqueeze_if,
 )
-from ._norm import to_1_1, to_z, unbias
+from ._norm import to_z
 from ._shell import run_shellcommand, run_shellscript
 from ._start import start
 from .cuda_collect_env import main as cuda_collect_env
 from .debug import *
 from .email import notify, send_gmail
 from .latex import add_hat_in_the_latex_style, to_the_latex_style
 from .mat2py import *
```

### Comparing `mngs-1.2.0/src/mngs/general/_close.py` & `mngs-1.2.2/src/mngs/general/_close.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/_converters.py` & `mngs-1.2.2/src/mngs/general/_converters.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/_norm.py` & `mngs-1.2.2/src/mngs/general/_norm.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/_shell.py` & `mngs-1.2.2/src/mngs/general/_shell.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/_start.py` & `mngs-1.2.2/src/mngs/general/_start.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/_xml2dict.py` & `mngs-1.2.2/src/mngs/general/_xml2dict.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/cuda_collect_env.py` & `mngs-1.2.2/src/mngs/general/cuda_collect_env.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/debug.py` & `mngs-1.2.2/src/mngs/general/debug.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/email.py` & `mngs-1.2.2/src/mngs/general/email.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/load.py` & `mngs-1.2.2/src/mngs/general/load.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/mat2py.py` & `mngs-1.2.2/src/mngs/general/mat2py.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/misc.py` & `mngs-1.2.2/src/mngs/general/misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/pandas.py` & `mngs-1.2.2/src/mngs/general/pandas.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/path.py` & `mngs-1.2.2/src/mngs/general/path.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/repro.py` & `mngs-1.2.2/src/mngs/general/repro.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/save.py` & `mngs-1.2.2/src/mngs/general/save.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/general/torch.py` & `mngs-1.2.2/src/mngs/general/torch.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/gists/_SigMacro_processFigure_S.py` & `mngs-1.2.2/src/mngs/gists/_SigMacro_processFigure_S.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/gists/_SigMacro_toBlue.py` & `mngs-1.2.2/src/mngs/gists/_SigMacro_toBlue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/io/load.py` & `mngs-1.2.2/src/mngs/io/load.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/io/path.py` & `mngs-1.2.2/src/mngs/io/path.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/io/save.py` & `mngs-1.2.2/src/mngs/io/save.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/linalg/_misc.py` & `mngs-1.2.2/src/mngs/linalg/_misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/ClassificationReporter.py` & `mngs-1.2.2/src/mngs/ml/ClassificationReporter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/ClassifierServer.py` & `mngs-1.2.2/src/mngs/ml/ClassifierServer.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/EarlyStopping.py` & `mngs-1.2.2/src/mngs/ml/EarlyStopping.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/LearningCurveLogger.py` & `mngs-1.2.2/src/mngs/ml/LearningCurveLogger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/__Classifiers.py` & `mngs-1.2.2/src/mngs/ml/__Classifiers.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/clustering/_UMAP.py` & `mngs-1.2.2/src/mngs/ml/clustering/_UMAP.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/clustering/_umap.py` & `mngs-1.2.2/src/mngs/ml/clustering/_umap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/loss/MultiTaskLoss.py` & `mngs-1.2.2/src/mngs/ml/loss/MultiTaskLoss.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/loss/_L1L2Losses.py` & `mngs-1.2.2/src/mngs/ml/loss/_L1L2Losses.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/metrics/_bACC.py` & `mngs-1.2.2/src/mngs/ml/metrics/_bACC.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py` & `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py` & `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py` & `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py` & `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py` & `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/optim/_get_set.py` & `mngs-1.2.2/src/mngs/ml/optim/_get_set.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/plt/_conf_mat.py` & `mngs-1.2.2/src/mngs/ml/plt/_conf_mat.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/plt/_learning_curve.py` & `mngs-1.2.2/src/mngs/ml/plt/_learning_curve.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/plt/_optuna_study.py` & `mngs-1.2.2/src/mngs/ml/plt/_optuna_study.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/plt/aucs/example.py` & `mngs-1.2.2/src/mngs/ml/plt/aucs/example.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/plt/aucs/pre_rec_auc.py` & `mngs-1.2.2/src/mngs/ml/plt/aucs/pre_rec_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/plt/aucs/roc_auc.py` & `mngs-1.2.2/src/mngs/ml/plt/aucs/roc_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/silhoute_score_block.py` & `mngs-1.2.2/src/mngs/ml/silhoute_score_block.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/sk/_clf.py` & `mngs-1.2.2/src/mngs/ml/sk/_clf.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/sk/_to_sktime.py` & `mngs-1.2.2/src/mngs/ml/sk/_to_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/utils/_DefaultDataset.py` & `mngs-1.2.2/src/mngs/ml/utils/_DefaultDataset.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/utils/_LabelEncoder.py` & `mngs-1.2.2/src/mngs/ml/utils/_LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/utils/_check_params.py` & `mngs-1.2.2/src/mngs/ml/utils/_check_params.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/utils/_format_samples_for_sktime.py` & `mngs-1.2.2/src/mngs/ml/utils/_format_samples_for_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/utils/_merge_labels.py` & `mngs-1.2.2/src/mngs/ml/utils/_merge_labels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/ml/utils/_under_sample.py` & `mngs-1.2.2/src/mngs/ml/utils/_under_sample.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/mngs/setup.py` & `mngs-1.2.2/src/mngs/mngs/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_AxiswiseDropout.py` & `mngs-1.2.2/src/mngs/dsp/nn/_AxiswiseDropout.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_BNet.py` & `mngs-1.2.2/src/mngs/dsp/nn/_BNet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_BNet_Res.py` & `mngs-1.2.2/src/mngs/dsp/nn/_BNet_Res.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_ChannelGainChanger.py` & `mngs-1.2.2/src/mngs/dsp/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_DropoutChannels.py` & `mngs-1.2.2/src/mngs/dsp/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_FreqGainChanger.py` & `mngs-1.2.2/src/mngs/dsp/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_GaussianFilter.py` & `mngs-1.2.2/src/mngs/dsp/nn/_GaussianFilter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_Hilbert.py` & `mngs-1.2.2/src/mngs/dsp/nn/_Hilbert.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_MNet_1000.py` & `mngs-1.2.2/src/mngs/dsp/nn/_MNet_1000.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_PSD.py` & `mngs-1.2.2/src/mngs/dsp/nn/_PSD.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_ResNet1D.py` & `mngs-1.2.2/src/mngs/dsp/nn/_ResNet1D.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_SpatialAttention.py` & `mngs-1.2.2/src/mngs/dsp/nn/_SpatialAttention.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_Spectrogram.py` & `mngs-1.2.2/src/mngs/dsp/nn/_Spectrogram.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_SwapChannels.py` & `mngs-1.2.2/src/mngs/dsp/nn/_SwapChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/nn/_Wavelet.py` & `mngs-1.2.2/src/mngs/dsp/nn/_Wavelet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-02 20:35:03 (ywatanabe)"
+# Time-stamp: "2024-04-05 12:09:22 (ywatanabe)"
 
 
 import mngs
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
@@ -192,14 +192,18 @@
             filtered_x_real.pow(2) + filtered_x_imag.pow(2)
         )
 
         filtered_x = filtered_x.view(
             x.shape[0], x.shape[1], kernel_batched.shape[0], -1
         )
 
+        filtered_x = filtered_x[..., :seq_len]
+
+        assert filtered_x.shape[-1] == seq_len
+
         if self.out_scale == "log":
             return torch.log(filtered_x + 1e-5)
         else:
             return filtered_x
 
     def init_kernel(self, samp_rate, kernel_size=None, freq_scale="log"):
         device = self.dummy.device
```

### Comparing `mngs-1.2.0/src/mngs/nn/__init__.py` & `mngs-1.2.2/src/mngs/dsp/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/os/_mv.py` & `mngs-1.2.2/src/mngs/os/_mv.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/_add_hue.py` & `mngs-1.2.2/src/mngs/plt/_add_hue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/_annotated_heatmap.py` & `mngs-1.2.2/src/mngs/plt/_annotated_heatmap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/_configure_mpl.py` & `mngs-1.2.2/src/mngs/plt/_configure_mpl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-03-08 02:07:41 (ywatanabe)"
+# Time-stamp: "2024-04-05 17:07:26 (ywatanabe)"
 
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 
 
 def rgba_to_hex(rgba):
@@ -34,18 +34,21 @@
     font_size_base=8,
     font_size_title=8,
     font_size_axis_label=8,
     font_size_tick_label=7,
     font_size_legend=6,
     # Hide spines
     hide_top_right_spines=True,
+    # line
+    line_width=0.1,
     # Color transparency
     alpha=0.75,
     # Whether to print configurations or not
-    show=True,
+    verbose=False,
+    **kwargs,
 ):
     """
     Configures Matplotlib and Seaborn settings for publication-quality plots.
     For axis control, refer to the mngs.plt.ax module.
 
     Example:
         plt, cc = configure_mpl(plt)
@@ -89,15 +92,15 @@
 
         hide_top_right_spines (bool, optional):
             If True, hides the top and right spines of the plot. Defaults to True.
 
         alpha (float, optional):
             Color transparency. Defaults to 0.75.
 
-        show (bool, optional):
+        verbose (bool, optional):
             If True, prints the configuration settings. Defaults to True.
 
     Returns:
         dict: A dictionary of the custom colors used in the configuration.
     """
 
     COLORS_RGBA = {
@@ -141,18 +144,20 @@
             # Legend
             "legend.fontsize": font_size_legend,
             # Top and Right Axes
             "axes.spines.top": not hide_top_right_spines,
             "axes.spines.right": not hide_top_right_spines,
             # Custom color cycle
             "axes.prop_cycle": plt.cycler(color=COLORS_RGBA_NORM.values()),
+            # Line
+            "lines.linewidth": line_width,
         }
     )
 
-    if show:
+    if verbose:
         print("\n" + "-" * 40)
         print("Matplotlib has been configured as follows:\n")
         print(f"Figure DPI (Display): {dpi_display} DPI")
         print(f"Figure DPI (Save): {dpi_save} DPI")
         print(
             f"Figure Size (Not the Axis Size): "
             f"{fig_size_mm[0] * fig_scale:.1f} x "
```

### Comparing `mngs-1.2.0/src/mngs/plt/_draw_a_cube.py` & `mngs-1.2.2/src/mngs/plt/_draw_a_cube.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/_get_RGBA_from_colormap.py` & `mngs-1.2.2/src/mngs/plt/_get_RGBA_from_colormap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/_mk_colorbar.py` & `mngs-1.2.2/src/mngs/plt/_mk_colorbar.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/_subplots.py` & `mngs-1.2.2/src/mngs/plt/_subplots.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/_tpl.py` & `mngs-1.2.2/src/mngs/plt/_tpl.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/ax/_circular_hist.py` & `mngs-1.2.2/src/mngs/plt/ax/_circular_hist.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/ax/_extend.py` & `mngs-1.2.2/src/mngs/plt/ax/_extend.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/ax/_hide_spines.py` & `mngs-1.2.2/src/mngs/plt/ax/_hide_spines.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/ax/_map_ticks.py` & `mngs-1.2.2/src/mngs/plt/ax/_map_ticks.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/ax/_panel.py` & `mngs-1.2.2/src/mngs/plt/ax/_panel.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/ax/_sci_note.py` & `mngs-1.2.2/src/mngs/plt/ax/_sci_note.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/ax/_set_pos.py` & `mngs-1.2.2/src/mngs/plt/ax/_set_pos.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/colors.py` & `mngs-1.2.2/src/mngs/plt/colors.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/plt/get_mpl_color.py` & `mngs-1.2.2/src/mngs/plt/get_mpl_color.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/resource/get.py` & `mngs-1.2.2/src/mngs/resource/get.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/resource/limit_RAM.py` & `mngs-1.2.2/src/mngs/resource/limit_RAM.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/__init__.py` & `mngs-1.2.2/src/mngs/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/_bonferroni_correction.py` & `mngs-1.2.2/src/mngs/stats/_bonferroni_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/_brunner_munzel_test.py` & `mngs-1.2.2/src/mngs/stats/_brunner_munzel_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/_corr_test.py` & `mngs-1.2.2/src/mngs/stats/_corr_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/_fdr_correction.py` & `mngs-1.2.2/src/mngs/stats/_fdr_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/_general.py` & `mngs-1.2.2/src/mngs/stats/_general.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/_multicompair.py` & `mngs-1.2.2/src/mngs/stats/_multicompair.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/_nocorrelation_test.py` & `mngs-1.2.2/src/mngs/stats/_nocorrelation_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/stats/_smirnov_grubbs.py` & `mngs-1.2.2/src/mngs/stats/_smirnov_grubbs.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs/torch/_apply_to.py` & `mngs-1.2.2/src/mngs/torch/_apply_to.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.0/src/mngs.egg-info/PKG-INFO` & `mngs-1.2.2/src/mngs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mngs
-Version: 1.2.0
+Version: 1.2.2
 Summary: For lazy python users (monogusa people in Japanse), especially in ML/DSP fields
 Home-page: https://github.com/ywatanabe1989/mngs
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: GPL3.0
 Keywords: utils,utilities,python,machine learning
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mngs-1.2.0/src/mngs.egg-info/SOURCES.txt` & `mngs-1.2.2/src/mngs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,44 @@
 src/mngs.egg-info/SOURCES.txt
 src/mngs.egg-info/dependency_links.txt
 src/mngs.egg-info/requires.txt
 src/mngs.egg-info/top_level.txt
 src/mngs/dsp/PARAMS.py
 src/mngs/dsp/__init__.py
 src/mngs/dsp/_demo_sig.py
-src/mngs/dsp/_ensure_3d.py
 src/mngs/dsp/_hilbert.py
+src/mngs/dsp/_misc.py
 src/mngs/dsp/_mne.py
 src/mngs/dsp/_psd.py
+src/mngs/dsp/_resample.py
 src/mngs/dsp/_transform.py
 src/mngs/dsp/_wavelet.py
 src/mngs/dsp/add_noise.py
+src/mngs/dsp/example.py
 src/mngs/dsp/filt.py
+src/mngs/dsp/norm.py
 src/mngs/dsp/ref.py
+src/mngs/dsp/nn/_AxiswiseDropout.py
+src/mngs/dsp/nn/_BNet.py
+src/mngs/dsp/nn/_BNet_Res.py
+src/mngs/dsp/nn/_ChannelGainChanger.py
+src/mngs/dsp/nn/_DropoutChannels.py
+src/mngs/dsp/nn/_Filters.py
+src/mngs/dsp/nn/_FreqGainChanger.py
+src/mngs/dsp/nn/_GaussianFilter.py
+src/mngs/dsp/nn/_Hilbert.py
+src/mngs/dsp/nn/_MNet_1000.py
+src/mngs/dsp/nn/_PSD.py
+src/mngs/dsp/nn/_ResNet1D.py
+src/mngs/dsp/nn/_SpatialAttention.py
+src/mngs/dsp/nn/_Spectrogram.py
+src/mngs/dsp/nn/_SwapChannels.py
+src/mngs/dsp/nn/_TransposeLayer.py
+src/mngs/dsp/nn/_Wavelet.py
+src/mngs/dsp/nn/__init__.py
 src/mngs/general/TimeStamper.py
 src/mngs/general/__init__.py
 src/mngs/general/_close.py
 src/mngs/general/_converters.py
 src/mngs/general/_norm.py
 src/mngs/general/_shell.py
 src/mngs/general/_start.py
```

