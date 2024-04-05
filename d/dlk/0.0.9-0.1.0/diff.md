# Comparing `tmp/dlk-0.0.9.tar.gz` & `tmp/dlk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlk-0.0.9.tar", last modified: Wed Mar 23 18:09:00 2022, max compression
+gzip compressed data, was "dlk-0.1.0.tar", last modified: Fri Apr  5 12:02:09 2024, max compression
```

## Comparing `dlk-0.0.9.tar` & `dlk-0.1.0.tar`

### file list

```diff
@@ -1,383 +1,194 @@
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.262345 dlk-0.0.9/
--rw-r--r--   0 sun       (1000) sun       (1000)      351 2021-12-23 12:39:24.000000 dlk-0.0.9/.gitignore
--rw-r--r--   0 sun       (1000) sun       (1000)      753 2021-12-23 14:24:24.000000 dlk-0.0.9/.readthedocs.yaml
--rw-r--r--   0 sun       (1000) sun       (1000)    11382 2021-12-17 16:45:41.000000 dlk-0.0.9/LICENSE
--rw-r--r--   0 sun       (1000) sun       (1000)     1827 2022-03-23 18:09:00.262345 dlk-0.0.9/PKG-INFO
--rw-r--r--   0 sun       (1000) sun       (1000)     1516 2021-12-23 15:27:28.000000 dlk-0.0.9/README.md
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.061312 dlk-0.0.9/dlk/
--rw-r--r--   0 sun       (1000) sun       (1000)      617 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/__init__.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.041365 dlk-0.0.9/dlk/configures/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.039370 dlk-0.0.9/dlk/configures/core/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.074277 dlk-0.0.9/dlk/configures/core/callbacks/
--rw-r--r--   0 sun       (1000) sun       (1000)      858 2021-12-17 18:19:33.000000 dlk-0.0.9/dlk/configures/core/callbacks/checkpoint.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      187 2021-12-17 18:19:16.000000 dlk-0.0.9/dlk/configures/core/callbacks/checkpoint@train_loss.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      214 2021-12-17 18:19:02.000000 dlk-0.0.9/dlk/configures/core/callbacks/checkpoint@val_loss.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      560 2021-12-17 18:30:29.000000 dlk-0.0.9/dlk/configures/core/callbacks/early_stop.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      260 2021-12-17 18:33:03.000000 dlk-0.0.9/dlk/configures/core/callbacks/lr_monitor.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      122 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/callbacks/progressbar.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      610 2021-12-17 18:37:22.000000 dlk-0.0.9/dlk/configures/core/callbacks/weight_average.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.079264 dlk-0.0.9/dlk/configures/core/imodels/
--rw-r--r--   0 sun       (1000) sun       (1000)      263 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/imodels/basic.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      358 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@seq_lab#crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      309 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@seq_lab.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      309 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@span_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      309 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      513 2021-12-20 14:37:30.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@txt_log_reg.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      513 2021-12-20 14:37:40.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@txt_reg.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.081258 dlk-0.0.9/dlk/configures/core/initmethods/
--rw-r--r--   0 sun       (1000) sun       (1000)       50 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/initmethods/default.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)       75 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/initmethods/range_norm.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)       78 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/initmethods/range_uniform.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.039370 dlk-0.0.9/dlk/configures/core/layers/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.084251 dlk-0.0.9/dlk/configures/core/layers/decoders/
--rw-r--r--   0 sun       (1000) sun       (1000)      526 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/decoders/biaffine.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      132 2021-12-19 09:24:47.000000 dlk-0.0.9/dlk/configures/core/layers/decoders/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      473 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/decoders/linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      680 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/decoders/linear_crf.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.088240 dlk-0.0.9/dlk/configures/core/layers/embeddings/
--rw-r--r--   0 sun       (1000) sun       (1000)     2666 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/combine_word_char_cnn.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      103 2021-12-17 18:45:52.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      601 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/pretrained_transformers.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      643 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/pretrained_transformers@gather.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      240 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/random.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      779 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/static.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1282 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/static_char_cnn.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.090235 dlk-0.0.9/dlk/configures/core/layers/encoders/
--rw-r--r--   0 sun       (1000) sun       (1000)      132 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/layers/encoders/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      444 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/encoders/linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      478 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/encoders/lstm.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.093226 dlk-0.0.9/dlk/configures/core/losses/
--rw-r--r--   0 sun       (1000) sun       (1000)      441 2021-12-20 13:50:20.000000 dlk-0.0.9/dlk/configures/core/losses/bce.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      469 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/losses/cross_entropy.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      597 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/losses/cross_entropy@cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      286 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/losses/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      413 2021-12-18 21:32:23.000000 dlk-0.0.9/dlk/configures/core/losses/mse.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.100208 dlk-0.0.9/dlk/configures/core/models/
--rw-r--r--   0 sun       (1000) sun       (1000)     3457 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_cnn_crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2139 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2190 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1277 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1226 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1461 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_lstm_crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1186 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@span_cls#pretrained_transformer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2145 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@txt_cls#lstm_linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1143 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@txt_cls#pretrained_transformers.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.105194 dlk-0.0.9/dlk/configures/core/modules/
--rw-r--r--   0 sun       (1000) sun       (1000)      168 2021-12-20 14:27:27.000000 dlk-0.0.9/dlk/configures/core/modules/bert.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      215 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/modules/biaffine.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      200 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/modules/conv1d.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      158 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/modules/crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      175 2021-12-20 14:27:31.000000 dlk-0.0.9/dlk/configures/core/modules/distil_bert.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      177 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/modules/linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      315 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/modules/lstm.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      171 2021-12-20 14:27:35.000000 dlk-0.0.9/dlk/configures/core/modules/roberta.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.107189 dlk-0.0.9/dlk/configures/core/optimizers/
--rw-r--r--   0 sun       (1000) sun       (1000)      798 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/core/optimizers/adamw.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      538 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/core/optimizers/adamw@bias_nodecay.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      816 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/core/optimizers/sgd.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.110181 dlk-0.0.9/dlk/configures/core/schedulers/
--rw-r--r--   0 sun       (1000) sun       (1000)       77 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/constant.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      116 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/constant_warmup.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      175 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/cosine_warmup.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      150 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/linear_warmup.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      172 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/rec_decay.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.040368 dlk-0.0.9/dlk/configures/data/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.115167 dlk-0.0.9/dlk/configures/data/datamodules/
--rw-r--r--   0 sun       (1000) sun       (1000)      883 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      914 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab#with_char.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      960 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab#wordmask.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      881 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      967 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@span_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      842 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      810 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@txt_reg.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.118159 dlk-0.0.9/dlk/configures/data/postprocessors/
--rw-r--r--   0 sun       (1000) sun       (1000)       28 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/postprocessors/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1651 2022-01-08 15:40:43.000000 dlk-0.0.9/dlk/configures/data/postprocessors/seq_lab.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1458 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/postprocessors/span_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      866 2021-12-23 13:03:12.000000 dlk-0.0.9/dlk/configures/data/postprocessors/txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      769 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/data/postprocessors/txt_reg.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.125141 dlk-0.0.9/dlk/configures/data/processors/
--rw-r--r--   0 sun       (1000) sun       (1000)     5707 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#norm_static.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     7108 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#norm_static_word_char.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     3944 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     5112 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#static.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     3413 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@span_cls#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     3365 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_cls#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     4468 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2690 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_match#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1628 2021-12-31 16:56:37.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_match_reg#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2058 2021-12-31 16:56:37.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_reg#pretrained.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.137109 dlk-0.0.9/dlk/configures/data/subprocessors/
--rw-r--r--   0 sun       (1000) sun       (1000)      838 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@seq_lab.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      889 2022-03-23 18:07:30.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      986 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_cls_pair.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      890 2022-03-23 18:07:43.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_reg.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      987 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_reg_pair.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      796 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/char_gather.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2876 2021-12-31 16:56:37.000000 dlk-0.0.9/dlk/configures/data/subprocessors/fast_tokenizer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2777 2021-12-20 15:46:38.000000 dlk-0.0.9/dlk/configures/data/subprocessors/fast_tokenizer@pair.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      164 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/load.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      119 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/save.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1376 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/configures/data/subprocessors/seq_lab_firstpiece_relabel.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1229 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/configures/data/subprocessors/seq_lab_relabel.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1245 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/configures/data/subprocessors/span_cls_relabel.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      759 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token2charid.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      690 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token2id.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      639 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token_embedding.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      878 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token_gather.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      920 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token_norm.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.138106 dlk-0.0.9/dlk/configures/managers/
--rw-r--r--   0 sun       (1000) sun       (1000)     2123 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/managers/lightning.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2785 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/managers/lightning@advance.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.139104 dlk-0.0.9/dlk/configures/tasks/
--rw-r--r--   0 sun       (1000) sun       (1000)      441 2021-12-18 17:41:20.000000 dlk-0.0.9/dlk/configures/tasks/test_base.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1915 2021-12-18 17:41:14.000000 dlk-0.0.9/dlk/configures/tasks/test_base_search.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.141098 dlk-0.0.9/dlk/core/
--rw-r--r--   0 sun       (1000) sun       (1000)     1334 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     9951 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/base_module.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.144090 dlk-0.0.9/dlk/core/callbacks/
--rw-r--r--   0 sun       (1000) sun       (1000)     1447 2021-12-21 17:45:09.000000 dlk-0.0.9/dlk/core/callbacks/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3243 2021-12-23 14:42:18.000000 dlk-0.0.9/dlk/core/callbacks/checkpoint.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2780 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/callbacks/early_stop.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2011 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/callbacks/lr_monitor.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2746 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/callbacks/weight_average.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.146084 dlk-0.0.9/dlk/core/imodels/
--rw-r--r--   0 sun       (1000) sun       (1000)     3493 2021-12-23 12:36:26.000000 dlk-0.0.9/dlk/core/imodels/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)    13363 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/imodels/basic.py
--rw-r--r--   0 sun       (1000) sun       (1000)      672 2021-12-21 17:45:18.000000 dlk-0.0.9/dlk/core/imodels/distill.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.149077 dlk-0.0.9/dlk/core/initmethods/
--rw-r--r--   0 sun       (1000) sun       (1000)     1500 2021-12-21 17:45:19.000000 dlk-0.0.9/dlk/core/initmethods/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5290 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/initmethods/default.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2413 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/initmethods/range_norm.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2837 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/initmethods/range_uniform.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.149077 dlk-0.0.9/dlk/core/layers/
--rw-r--r--   0 sun       (1000) sun       (1000)      838 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/layers/__init__.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.153066 dlk-0.0.9/dlk/core/layers/decoders/
--rw-r--r--   0 sun       (1000) sun       (1000)     1459 2021-12-21 17:45:21.000000 dlk-0.0.9/dlk/core/layers/decoders/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3901 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/core/layers/decoders/biaffine.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1577 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/decoders/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3205 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/decoders/linear.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5390 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/decoders/linear_crf.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.157055 dlk-0.0.9/dlk/core/layers/embeddings/
--rw-r--r--   0 sun       (1000) sun       (1000)     1900 2021-12-21 17:45:23.000000 dlk-0.0.9/dlk/core/layers/embeddings/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     7628 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/combine_word_char_cnn.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1645 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6148 2021-12-22 18:53:49.000000 dlk-0.0.9/dlk/core/layers/embeddings/pretrained_transformers.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3412 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/random.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4532 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/static.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6084 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/static_char_cnn.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.160048 dlk-0.0.9/dlk/core/layers/encoders/
--rw-r--r--   0 sun       (1000) sun       (1000)     1415 2021-12-21 17:45:26.000000 dlk-0.0.9/dlk/core/layers/encoders/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1617 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/layers/encoders/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3149 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/layers/encoders/linear.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3293 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/layers/encoders/lstm.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.164037 dlk-0.0.9/dlk/core/losses/
--rw-r--r--   0 sun       (1000) sun       (1000)     1415 2021-12-21 17:45:28.000000 dlk-0.0.9/dlk/core/losses/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5002 2021-12-22 18:58:35.000000 dlk-0.0.9/dlk/core/losses/bce.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5572 2021-12-22 18:58:35.000000 dlk-0.0.9/dlk/core/losses/cross_entropy.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4061 2021-12-22 19:06:58.000000 dlk-0.0.9/dlk/core/losses/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5004 2021-12-22 18:58:33.000000 dlk-0.0.9/dlk/core/losses/mse.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4068 2021-12-22 18:58:48.000000 dlk-0.0.9/dlk/core/losses/multi_loss.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.165034 dlk-0.0.9/dlk/core/models/
--rw-r--r--   0 sun       (1000) sun       (1000)     1419 2021-12-21 17:45:31.000000 dlk-0.0.9/dlk/core/models/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     9621 2022-03-23 13:52:15.000000 dlk-0.0.9/dlk/core/models/basic.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.172016 dlk-0.0.9/dlk/core/modules/
--rw-r--r--   0 sun       (1000) sun       (1000)     3230 2022-03-23 13:52:15.000000 dlk-0.0.9/dlk/core/modules/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5854 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/modules/bert.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3423 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/core/modules/biaffine.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2719 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/modules/conv1d.py
--rw-r--r--   0 sun       (1000) sun       (1000)    10299 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/core/modules/crf.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5450 2021-12-23 12:36:26.000000 dlk-0.0.9/dlk/core/modules/distil_bert.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2765 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/modules/linear.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3533 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/modules/logits_gather.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3463 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/modules/lstm.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5885 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/modules/roberta.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.174010 dlk-0.0.9/dlk/core/optimizers/
--rw-r--r--   0 sun       (1000) sun       (1000)     4066 2021-12-22 18:28:20.000000 dlk-0.0.9/dlk/core/optimizers/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2869 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/optimizers/adamw.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2918 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/optimizers/sgd.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.177999 dlk-0.0.9/dlk/core/schedulers/
--rw-r--r--   0 sun       (1000) sun       (1000)     1881 2021-12-22 18:28:20.000000 dlk-0.0.9/dlk/core/schedulers/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1903 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/constant.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2388 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/constant_warmup.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3047 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/cosine_warmup.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3025 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/linear_warmup.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2617 2021-12-21 17:45:41.000000 dlk-0.0.9/dlk/core/schedulers/multi_group_schedule.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2966 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/rec_decay.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.178997 dlk-0.0.9/dlk/data/
--rw-r--r--   0 sun       (1000) sun       (1000)      931 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/__init__.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.180992 dlk-0.0.9/dlk/data/datamodules/
--rw-r--r--   0 sun       (1000) sun       (1000)     5164 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/data/datamodules/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     8952 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/datamodules/basic.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1889 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/data/datamodules/readme.md
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.185978 dlk-0.0.9/dlk/data/postprocessors/
--rw-r--r--   0 sun       (1000) sun       (1000)     9461 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1619 2021-12-21 17:45:43.000000 dlk-0.0.9/dlk/data/postprocessors/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)    34482 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/seq_lab.py
--rw-r--r--   0 sun       (1000) sun       (1000)    18650 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/span_cls.py
--rw-r--r--   0 sun       (1000) sun       (1000)    11011 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/txt_cls.py
--rw-r--r--   0 sun       (1000) sun       (1000)     8979 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/txt_reg.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.187973 dlk-0.0.9/dlk/data/processors/
--rw-r--r--   0 sun       (1000) sun       (1000)     1976 2021-12-22 18:40:25.000000 dlk-0.0.9/dlk/data/processors/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     7983 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/processors/basic.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6747 2021-12-23 12:36:26.000000 dlk-0.0.9/dlk/data/processors/readme.md
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.196949 dlk-0.0.9/dlk/data/subprocessors/
--rw-r--r--   0 sun       (1000) sun       (1000)     2159 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/subprocessors/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5377 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/subprocessors/basic_data_loader.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5309 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/subprocessors/char_gather.py
--rw-r--r--   0 sun       (1000) sun       (1000)    12655 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/subprocessors/fast_tokenizer.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3118 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/subprocessors/load.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3913 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/subprocessors/save.py
--rw-r--r--   0 sun       (1000) sun       (1000)    12051 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/data/subprocessors/seq_lab_firstpiece_relable.py
--rw-r--r--   0 sun       (1000) sun       (1000)    10420 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/data/subprocessors/seq_lab_relabel.py
--rw-r--r--   0 sun       (1000) sun       (1000)    10159 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/data/subprocessors/span_cls_relabel.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5041 2021-12-22 18:51:42.000000 dlk-0.0.9/dlk/data/subprocessors/token2charid.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4209 2021-12-22 18:51:42.000000 dlk-0.0.9/dlk/data/subprocessors/token2id.py
--rw-r--r--   0 sun       (1000) sun       (1000)     7709 2021-12-22 18:51:42.000000 dlk-0.0.9/dlk/data/subprocessors/token_embedding.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6887 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/data/subprocessors/token_gather.py
--rw-r--r--   0 sun       (1000) sun       (1000)     8670 2021-12-31 16:56:37.000000 dlk-0.0.9/dlk/data/subprocessors/token_norm.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3580 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/dlk.drawio
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.198943 dlk-0.0.9/dlk/managers/
--rw-r--r--   0 sun       (1000) sun       (1000)     1446 2021-12-21 17:45:54.000000 dlk-0.0.9/dlk/managers/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)    11092 2022-03-22 14:40:41.000000 dlk-0.0.9/dlk/managers/lightning.py
--rw-r--r--   0 sun       (1000) sun       (1000)      635 2021-12-21 17:45:55.000000 dlk-0.0.9/dlk/online.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6631 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/predict.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1865 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6593 2021-12-18 21:28:01.000000 dlk-0.0.9/dlk/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)     6974 2021-12-31 14:50:29.000000 dlk-0.0.9/dlk/train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.204928 dlk-0.0.9/dlk/utils/
--rw-r--r--   0 sun       (1000) sun       (1000)      596 2021-12-21 17:45:57.000000 dlk-0.0.9/dlk/utils/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     7812 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/utils/config.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1400 2021-12-22 18:45:49.000000 dlk-0.0.9/dlk/utils/get_root.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4263 2021-12-22 18:45:49.000000 dlk-0.0.9/dlk/utils/logger.py
--rw-r--r--   0 sun       (1000) sun       (1000)    29807 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/utils/parser.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3012 2022-01-08 09:28:18.000000 dlk-0.0.9/dlk/utils/quick_search.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2197 2021-12-22 18:45:49.000000 dlk-0.0.9/dlk/utils/register.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3195 2022-01-08 15:40:43.000000 dlk-0.0.9/dlk/utils/tokenizer_util.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6500 2021-12-22 18:45:49.000000 dlk-0.0.9/dlk/utils/vocab.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.070288 dlk-0.0.9/dlk.egg-info/
--rw-r--r--   0 sun       (1000) sun       (1000)     1827 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/PKG-INFO
--rw-r--r--   0 sun       (1000) sun       (1000)    12263 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/SOURCES.txt
--rw-r--r--   0 sun       (1000) sun       (1000)        1 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/dependency_links.txt
--rw-r--r--   0 sun       (1000) sun       (1000)      328 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/requires.txt
--rw-r--r--   0 sun       (1000) sun       (1000)        4 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/top_level.txt
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.207919 dlk-0.0.9/docs/
--rw-r--r--   0 sun       (1000) sun       (1000)      638 2021-12-23 13:05:09.000000 dlk-0.0.9/docs/Makefile
--rw-r--r--   0 sun       (1000) sun       (1000)      799 2021-12-23 13:05:09.000000 dlk-0.0.9/docs/make.bat
--rw-r--r--   0 sun       (1000) sun       (1000)     3686 2021-12-23 12:36:26.000000 dlk-0.0.9/docs/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)       74 2021-12-23 13:47:14.000000 dlk-0.0.9/docs/requirements.txt
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.224446 dlk-0.0.9/docs/source/
--rw-r--r--   0 sun       (1000) sun       (1000)     6593 2021-12-18 21:28:01.000000 dlk-0.0.9/docs/source/appointment.md
--rw-r--r--   0 sun       (1000) sun       (1000)     2830 2021-12-23 14:08:37.000000 dlk-0.0.9/docs/source/conf.py
--rw-r--r--   0 sun       (1000) sun       (1000)      922 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.callbacks.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      510 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.imodels.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      756 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.initmethods.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      784 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.layers.decoders.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1493 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.layers.embeddings.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      764 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.layers.encoders.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      310 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.layers.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      991 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.losses.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      343 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.models.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1480 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.modules.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      525 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.optimizers.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      566 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1343 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.schedulers.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      373 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.datamodules.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      952 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.postprocessors.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      367 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.processors.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      303 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     2975 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.subprocessors.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      337 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.managers.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      743 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1326 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.utils.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      769 2021-12-23 13:08:24.000000 dlk-0.0.9/docs/source/index.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1516 2021-12-23 15:27:28.000000 dlk-0.0.9/docs/source/introduction.md
--rw-r--r--   0 sun       (1000) sun       (1000)     6747 2021-12-23 12:36:26.000000 dlk-0.0.9/docs/source/process_progress.md
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.048346 dlk-0.0.9/examples/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.046352 dlk-0.0.9/examples/sequence_labeling/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.226441 dlk-0.0.9/examples/sequence_labeling/conll2003/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.228435 dlk-0.0.9/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/
--rw-r--r--   0 sun       (1000) sun       (1000)     5357 2022-01-08 15:40:43.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1594 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/prepro.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.230430 dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/
--rw-r--r--   0 sun       (1000) sun       (1000)     4679 2022-03-23 13:51:46.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2113 2021-12-18 07:18:07.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/pre_prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1151 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1669 2021-12-31 17:11:38.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)      391 2021-12-13 15:15:43.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)      922 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.232425 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/
--rw-r--r--   0 sun       (1000) sun       (1000)     2708 2021-12-22 15:37:11.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3491 2021-12-22 15:37:11.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/cls_bio2json.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2728 2021-12-22 15:37:11.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/cls_json2bio.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1172 2021-12-22 15:37:11.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/get_vocab.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.047349 dlk-0.0.9/examples/text_cls/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.234419 dlk-0.0.9/examples/text_cls/sst2/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.236414 dlk-0.0.9/examples/text_cls/sst2/distil_bert/
--rw-r--r--   0 sun       (1000) sun       (1000)     2467 2022-03-23 13:51:46.000000 dlk-0.0.9/examples/text_cls/sst2/distil_bert/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      622 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/text_cls/sst2/distil_bert/prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1527 2021-12-21 17:48:43.000000 dlk-0.0.9/examples/text_cls/sst2/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)       59 2021-12-18 16:17:29.000000 dlk-0.0.9/examples/text_cls/sst2/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:43.000000 dlk-0.0.9/examples/text_cls/sst2/train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.047349 dlk-0.0.9/examples/text_match/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.238409 dlk-0.0.9/examples/text_match/snli/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.239406 dlk-0.0.9/examples/text_match/snli/distil_bert/
--rw-r--r--   0 sun       (1000) sun       (1000)     2636 2022-03-23 13:51:46.000000 dlk-0.0.9/examples/text_match/snli/distil_bert/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      796 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/text_match/snli/distil_bert/prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1718 2021-12-31 14:50:29.000000 dlk-0.0.9/examples/text_match/snli/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)       63 2021-12-18 15:35:09.000000 dlk-0.0.9/examples/text_match/snli/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:45.000000 dlk-0.0.9/examples/text_match/snli/train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.048346 dlk-0.0.9/examples/text_reg/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.241401 dlk-0.0.9/examples/text_reg/sst2/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.242398 dlk-0.0.9/examples/text_reg/sst2/distil_bert/
--rw-r--r--   0 sun       (1000) sun       (1000)     2497 2022-03-23 13:51:46.000000 dlk-0.0.9/examples/text_reg/sst2/distil_bert/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      622 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/text_reg/sst2/distil_bert/prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1482 2021-12-21 17:48:46.000000 dlk-0.0.9/examples/text_reg/sst2/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)       67 2021-12-20 12:35:51.000000 dlk-0.0.9/examples/text_reg/sst2/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:46.000000 dlk-0.0.9/examples/text_reg/sst2/train.py
--rw-r--r--   0 sun       (1000) sun       (1000)      430 2022-01-12 12:59:43.000000 dlk-0.0.9/requirements-f.txt
--rw-r--r--   0 sun       (1000) sun       (1000)      329 2022-01-12 12:59:43.000000 dlk-0.0.9/requirements.txt
--rw-r--r--   0 sun       (1000) sun       (1000)       38 2022-03-23 18:09:00.262345 dlk-0.0.9/setup.cfg
--rw-r--r--   0 sun       (1000) sun       (1000)     1712 2021-12-23 14:10:36.000000 dlk-0.0.9/setup.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2112 2022-03-23 13:51:46.000000 dlk-0.0.9/test_predict.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1218 2021-12-21 17:48:14.000000 dlk-0.0.9/test_process.py
--rw-r--r--   0 sun       (1000) sun       (1000)      871 2021-12-21 17:48:16.000000 dlk-0.0.9/test_train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.243395 dlk-0.0.9/tests/
--rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-09-16 13:28:15.000000 dlk-0.0.9/tests/__init__.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.246387 dlk-0.0.9/tests/parser/
--rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-11-01 16:26:30.000000 dlk-0.0.9/tests/parser/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2168 2021-11-07 08:29:13.000000 dlk-0.0.9/tests/parser/test_base.json
--rw-r--r--   0 sun       (1000) sun       (1000)     2173 2021-12-17 16:45:41.000000 dlk-0.0.9/tests/parser/test_base.py
--rw-r--r--   0 sun       (1000) sun       (1000)      515 2021-12-16 13:42:00.000000 dlk-0.0.9/tests/parser/test_base_inp.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2057 2021-11-02 22:00:17.000000 dlk-0.0.9/tests/parser/test_base_out.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.251374 dlk-0.0.9/tests/processors/
--rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-10-28 17:13:32.000000 dlk-0.0.9/tests/processors/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)    40746 2021-10-11 11:48:46.000000 dlk-0.0.9/tests/processors/bpe_token.json
--rw-r--r--   0 sun       (1000) sun       (1000)     4888 2021-12-16 13:42:00.000000 dlk-0.0.9/tests/processors/process.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1947 2021-12-17 16:45:41.000000 dlk-0.0.9/tests/processors/test_wordpiece_tokenizer.py
--rw-r--r--   0 sun       (1000) sun       (1000)    18702 2021-10-11 11:48:46.000000 dlk-0.0.9/tests/processors/uni_token.json
--rw-r--r--   0 sun       (1000) sun       (1000)    23944 2021-10-11 11:48:46.000000 dlk-0.0.9/tests/processors/wp_token.json
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.251374 dlk-0.0.9/tests/test_test/
--rw-r--r--   0 sun       (1000) sun       (1000)    14948 2021-12-16 13:42:00.000000 dlk-0.0.9/tests/test_test/lightning.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.253368 dlk-0.0.9/tests/test_test/trace/
--rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-10-31 15:02:48.000000 dlk-0.0.9/tests/test_test/trace/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3249 2021-12-17 16:45:41.000000 dlk-0.0.9/tests/test_test/trace/dict_trace.py
--rw-r--r--   0 sun       (1000) sun       (1000)      605 2021-12-16 13:42:00.000000 dlk-0.0.9/tests/test_test/trace/simple_trace.py
--rw-r--r--   0 sun       (1000) sun       (1000)      304 2021-12-17 16:45:41.000000 dlk-0.0.9/tests/test_vocab.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.254366 dlk-0.0.9/tools/
--rw-r--r--   0 sun       (1000) sun       (1000)     1936 2021-12-22 19:11:14.000000 dlk-0.0.9/tools/conf.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.257358 dlk-0.0.9/tools/convert_tokenizer/
--rw-r--r--   0 sun       (1000) sun       (1000)      151 2021-12-22 15:37:11.000000 dlk-0.0.9/tools/convert_tokenizer/convert.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2063 2021-12-22 15:37:11.000000 dlk-0.0.9/tools/convert_tokenizer/convert.py
--rw-r--r--   0 sun       (1000) sun       (1000)      230 2021-12-31 16:56:37.000000 dlk-0.0.9/tools/convert_tokenizer/vocab2tokenizer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     6274 2021-12-21 17:47:44.000000 dlk-0.0.9/tools/convert_tokenizer/vocab2tokenizer.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.258355 dlk-0.0.9/tools/tokenize/
--rw-r--r--   0 sun       (1000) sun       (1000)     1882 2021-12-16 13:42:00.000000 dlk-0.0.9/tools/tokenize/tokenizer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2406 2021-12-21 17:47:45.000000 dlk-0.0.9/tools/tokenize/tokenizer.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.260350 dlk-0.0.9/tools/train_tokenizer/
--rw-r--r--   0 sun       (1000) sun       (1000)      606 2021-12-16 13:42:00.000000 dlk-0.0.9/tools/train_tokenizer/train_tokenizer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     5276 2021-12-21 17:47:46.000000 dlk-0.0.9/tools/train_tokenizer/train_tokenizer.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1160 2021-12-21 17:47:47.000000 dlk-0.0.9/tools/view_config.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.261347 dlk-0.0.9/tools/word2vec/
--rw-r--r--   0 sun       (1000) sun       (1000)     1861 2021-12-31 16:56:37.000000 dlk-0.0.9/tools/word2vec/word2vec.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     6096 2021-12-31 16:56:37.000000 dlk-0.0.9/tools/word2vec/word2vec.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.982678 dlk-0.1.0/
+-rw-rw-r--   0 sun       (1000) sun       (1000)    11382 2022-04-04 17:23:38.000000 dlk-0.1.0/LICENSE
+-rw-r--r--   0 sun       (1000) sun       (1000)     8739 2024-04-05 12:02:09.982678 dlk-0.1.0/PKG-INFO
+-rw-rw-r--   0 sun       (1000) sun       (1000)     7731 2024-04-05 11:45:18.000000 dlk-0.1.0/README.md
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      874 2024-03-30 19:44:10.000000 dlk-0.1.0/dlk/__init__.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk/adv_method/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      969 2024-03-22 11:51:53.000000 dlk-0.1.0/dlk/adv_method/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3688 2024-03-22 11:48:39.000000 dlk-0.1.0/dlk/adv_method/fgm.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     5073 2024-02-20 14:48:13.000000 dlk-0.1.0/dlk/adv_method/free_lb.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4899 2024-02-20 14:48:14.000000 dlk-0.1.0/dlk/adv_method/pgd.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk/callback/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      412 2024-03-22 11:48:37.000000 dlk-0.1.0/dlk/callback/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4535 2024-03-22 11:52:19.000000 dlk-0.1.0/dlk/callback/checkpoint.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2602 2024-03-22 11:52:20.000000 dlk-0.1.0/dlk/callback/early_stop.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1775 2024-03-22 11:52:20.000000 dlk-0.1.0/dlk/callback/lr_monitor.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     6191 2024-03-22 11:52:20.000000 dlk-0.1.0/dlk/callback/progress_bar.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2521 2024-03-22 11:52:20.000000 dlk-0.1.0/dlk/callback/weight_average.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk/data/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      329 2024-03-22 11:48:37.000000 dlk-0.1.0/dlk/data/__init__.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk/data/data_collate/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      411 2024-03-22 11:48:26.000000 dlk-0.1.0/dlk/data/data_collate/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4980 2024-03-25 17:41:37.000000 dlk-0.1.0/dlk/data/data_collate/default.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk/data/datamodule/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1834 2024-03-22 11:48:26.000000 dlk-0.1.0/dlk/data/datamodule/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     5795 2024-04-05 08:58:41.000000 dlk-0.1.0/dlk/data/datamodule/default.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk/data/dataset/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      396 2024-03-22 11:48:27.000000 dlk-0.1.0/dlk/data/dataset/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3185 2024-03-22 11:48:27.000000 dlk-0.1.0/dlk/data/dataset/default.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk/data/postprocessor/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     9737 2024-03-22 11:48:11.000000 dlk-0.1.0/dlk/data/postprocessor/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     8545 2024-04-03 17:59:22.000000 dlk-0.1.0/dlk/data/postprocessor/generate_post.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1142 2024-03-22 11:48:27.000000 dlk-0.1.0/dlk/data/postprocessor/identity.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4380 2024-04-03 18:01:42.000000 dlk-0.1.0/dlk/data/postprocessor/img_cls.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    33682 2024-03-02 14:58:54.000000 dlk-0.1.0/dlk/data/postprocessor/seq_lab.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    16845 2024-03-28 14:55:14.000000 dlk-0.1.0/dlk/data/postprocessor/span_cls.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    32824 2024-03-28 14:55:37.000000 dlk-0.1.0/dlk/data/postprocessor/span_relation.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     9866 2024-04-02 16:26:25.000000 dlk-0.1.0/dlk/data/postprocessor/txt_cls.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     8540 2024-04-04 17:51:48.000000 dlk-0.1.0/dlk/data/postprocessor/txt_reg.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/data/processor/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      391 2024-03-22 11:48:34.000000 dlk-0.1.0/dlk/data/processor/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     9825 2024-04-05 09:23:23.000000 dlk-0.1.0/dlk/data/processor/default.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/data/subprocessor/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2653 2024-03-22 11:48:34.000000 dlk-0.1.0/dlk/data/subprocessor/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4410 2024-03-22 11:48:34.000000 dlk-0.1.0/dlk/data/subprocessor/char_gather.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    15288 2024-03-22 11:48:35.000000 dlk-0.1.0/dlk/data/subprocessor/fast_tokenizer.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4027 2024-03-25 17:01:39.000000 dlk-0.1.0/dlk/data/subprocessor/image_process.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4503 2024-03-22 11:54:45.000000 dlk-0.1.0/dlk/data/subprocessor/piece_rerank_relabel.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    12452 2024-03-22 11:54:46.000000 dlk-0.1.0/dlk/data/subprocessor/seq_lab_firstpiece_relabel.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     9801 2024-03-22 11:54:46.000000 dlk-0.1.0/dlk/data/subprocessor/seq_lab_relabel.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    12394 2024-03-02 17:53:33.000000 dlk-0.1.0/dlk/data/subprocessor/span_cls_relabel.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    10954 2024-03-02 17:53:49.000000 dlk-0.1.0/dlk/data/subprocessor/span_relation_relabel.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4138 2024-03-02 16:18:28.000000 dlk-0.1.0/dlk/data/subprocessor/token2charid.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4715 2024-02-22 12:48:17.000000 dlk-0.1.0/dlk/data/subprocessor/token2id.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     7856 2024-02-20 14:49:18.000000 dlk-0.1.0/dlk/data/subprocessor/token_embedding.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     6057 2024-03-02 12:41:48.000000 dlk-0.1.0/dlk/data/subprocessor/token_gather.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     7106 2024-02-20 14:49:22.000000 dlk-0.1.0/dlk/data/subprocessor/token_norm.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     6637 2024-04-04 18:34:42.000000 dlk-0.1.0/dlk/demo.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/display/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1876 2024-04-02 14:58:02.000000 dlk-0.1.0/dlk/display/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1711 2024-04-03 17:57:21.000000 dlk-0.1.0/dlk/display/img_caption.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1809 2024-04-02 14:58:50.000000 dlk-0.1.0/dlk/display/img_cls.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2444 2024-04-02 14:59:10.000000 dlk-0.1.0/dlk/display/relation_extract.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2418 2024-04-02 14:59:24.000000 dlk-0.1.0/dlk/display/seq_lab.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1995 2024-04-02 14:59:34.000000 dlk-0.1.0/dlk/display/summary.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4618 2024-04-02 17:04:52.000000 dlk-0.1.0/dlk/display/txt_cls.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3187 2024-04-02 15:00:07.000000 dlk-0.1.0/dlk/display/txt_reg.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/imodel/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      379 2024-03-22 11:48:25.000000 dlk-0.1.0/dlk/imodel/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    16212 2024-04-03 19:31:36.000000 dlk-0.1.0/dlk/imodel/default.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/initmethod/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      371 2024-03-22 11:48:24.000000 dlk-0.1.0/dlk/initmethod/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4031 2024-03-22 11:48:24.000000 dlk-0.1.0/dlk/initmethod/default.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1933 2024-03-22 11:48:24.000000 dlk-0.1.0/dlk/initmethod/range_norm.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2285 2024-03-22 11:48:25.000000 dlk-0.1.0/dlk/initmethod/range_uniform.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/nn/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      244 2024-03-22 11:48:22.000000 dlk-0.1.0/dlk/nn/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    11726 2024-04-04 18:53:20.000000 dlk-0.1.0/dlk/nn/base_module.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/nn/layer/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      288 2024-03-31 09:49:58.000000 dlk-0.1.0/dlk/nn/layer/__init__.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/nn/layer/decoder/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      842 2024-03-28 14:56:50.000000 dlk-0.1.0/dlk/nn/layer/decoder/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1919 2024-03-22 11:48:16.000000 dlk-0.1.0/dlk/nn/layer/decoder/biaffine.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1929 2024-03-22 11:48:16.000000 dlk-0.1.0/dlk/nn/layer/decoder/linear.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4796 2024-03-22 11:48:16.000000 dlk-0.1.0/dlk/nn/layer/decoder/linear_crf.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1930 2024-03-22 11:48:16.000000 dlk-0.1.0/dlk/nn/layer/decoder/multi_decoder.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/nn/layer/embedding/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1219 2024-03-28 14:56:38.000000 dlk-0.1.0/dlk/nn/layer/embedding/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3696 2024-03-22 11:48:17.000000 dlk-0.1.0/dlk/nn/layer/embedding/bert_like.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4226 2024-03-22 11:48:17.000000 dlk-0.1.0/dlk/nn/layer/embedding/combine_word_char_cnn.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3166 2024-03-22 11:48:17.000000 dlk-0.1.0/dlk/nn/layer/embedding/random.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2170 2024-04-04 18:52:42.000000 dlk-0.1.0/dlk/nn/layer/embedding/static.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4550 2024-03-22 11:48:18.000000 dlk-0.1.0/dlk/nn/layer/embedding/static_char_cnn.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2303 2024-03-31 09:27:39.000000 dlk-0.1.0/dlk/nn/layer/embedding/vit_embedding.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/nn/layer/encoder/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      796 2024-03-28 14:56:23.000000 dlk-0.1.0/dlk/nn/layer/encoder/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4524 2024-04-01 16:42:38.000000 dlk-0.1.0/dlk/nn/layer/encoder/bart_encoder.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1970 2024-03-22 11:48:18.000000 dlk-0.1.0/dlk/nn/layer/encoder/linear.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2126 2024-03-22 11:48:18.000000 dlk-0.1.0/dlk/nn/layer/encoder/lstm.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.974678 dlk-0.1.0/dlk/nn/layer/token_gen_decoder/
+-rw-r--r--   0 sun       (1000) sun       (1000)      872 2024-03-31 09:49:42.000000 dlk-0.1.0/dlk/nn/layer/token_gen_decoder/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4002 2024-03-31 13:36:44.000000 dlk-0.1.0/dlk/nn/layer/token_gen_decoder/bart_decoder.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/nn/loss/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3476 2024-04-03 20:58:37.000000 dlk-0.1.0/dlk/nn/loss/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1802 2024-03-22 11:57:18.000000 dlk-0.1.0/dlk/nn/loss/bce.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3040 2024-03-02 12:38:22.000000 dlk-0.1.0/dlk/nn/loss/cross_entropy.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3304 2024-03-22 11:57:20.000000 dlk-0.1.0/dlk/nn/loss/focal_loss.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1918 2024-03-22 11:57:24.000000 dlk-0.1.0/dlk/nn/loss/identity.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1917 2024-03-22 11:57:39.000000 dlk-0.1.0/dlk/nn/loss/mse.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3563 2024-03-22 11:57:46.000000 dlk-0.1.0/dlk/nn/loss/multi_loss.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/nn/model/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      313 2024-03-22 11:48:20.000000 dlk-0.1.0/dlk/nn/model/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     5153 2024-03-22 11:48:20.000000 dlk-0.1.0/dlk/nn/model/basic.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     8658 2024-03-31 15:31:06.000000 dlk-0.1.0/dlk/nn/model/token_enc_dec.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/nn/module/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2607 2024-03-28 14:57:14.000000 dlk-0.1.0/dlk/nn/module/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     5443 2024-03-22 11:48:20.000000 dlk-0.1.0/dlk/nn/module/bert.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3658 2024-03-22 11:48:21.000000 dlk-0.1.0/dlk/nn/module/bert_like.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4825 2024-03-22 16:50:08.000000 dlk-0.1.0/dlk/nn/module/biaffine.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3815 2024-03-22 16:53:57.000000 dlk-0.1.0/dlk/nn/module/bilinear.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2236 2024-03-22 11:58:22.000000 dlk-0.1.0/dlk/nn/module/conv1d.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     9794 2024-03-22 11:58:27.000000 dlk-0.1.0/dlk/nn/module/crf.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     5040 2024-03-22 11:58:36.000000 dlk-0.1.0/dlk/nn/module/distil_bert.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2051 2024-03-22 11:58:38.000000 dlk-0.1.0/dlk/nn/module/linear.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2323 2024-03-22 11:58:40.000000 dlk-0.1.0/dlk/nn/module/logits_gather.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2749 2024-03-22 11:58:41.000000 dlk-0.1.0/dlk/nn/module/lstm.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5745 2024-03-28 15:53:43.000000 dlk-0.1.0/dlk/nn/module/module_bart_decoder.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4511 2024-03-22 17:59:20.000000 dlk-0.1.0/dlk/nn/module/module_bart_encoder.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2884 2024-03-31 08:40:48.000000 dlk-0.1.0/dlk/nn/module/module_vit.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     5218 2024-03-22 11:58:43.000000 dlk-0.1.0/dlk/nn/module/roberta.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    33690 2024-03-31 15:29:25.000000 dlk-0.1.0/dlk/nn/token_gen_base.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/nn/utils/
+-rw-r--r--   0 sun       (1000) sun       (1000)        0 2024-03-22 16:47:36.000000 dlk-0.1.0/dlk/nn/utils/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3701 2024-03-22 16:48:33.000000 dlk-0.1.0/dlk/nn/utils/rope.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1387 2024-03-21 17:39:12.000000 dlk-0.1.0/dlk/online.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/optimizer/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4760 2024-03-22 11:48:15.000000 dlk-0.1.0/dlk/optimizer/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1230 2024-03-22 11:48:15.000000 dlk-0.1.0/dlk/optimizer/adamw.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     6575 2024-03-22 11:48:15.000000 dlk-0.1.0/dlk/optimizer/adan.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1288 2024-03-22 11:48:16.000000 dlk-0.1.0/dlk/optimizer/sgd.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     5917 2024-04-04 15:16:30.000000 dlk-0.1.0/dlk/predict.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2463 2024-04-05 11:41:56.000000 dlk-0.1.0/dlk/preprocess.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/scheduler/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3395 2024-04-03 20:57:31.000000 dlk-0.1.0/dlk/scheduler/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1115 2024-03-22 11:59:07.000000 dlk-0.1.0/dlk/scheduler/constant.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1475 2024-03-22 11:59:10.000000 dlk-0.1.0/dlk/scheduler/constant_warmup.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2022 2024-03-22 11:59:12.000000 dlk-0.1.0/dlk/scheduler/cosine_restart.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2707 2024-03-22 11:59:15.000000 dlk-0.1.0/dlk/scheduler/cosine_warmup.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1865 2024-03-22 11:59:17.000000 dlk-0.1.0/dlk/scheduler/linear_warmup.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1982 2024-03-22 11:59:19.000000 dlk-0.1.0/dlk/scheduler/multi_group_schedule.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1692 2024-03-22 11:59:23.000000 dlk-0.1.0/dlk/scheduler/rec_decay.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1833 2024-04-04 18:41:29.000000 dlk-0.1.0/dlk/server.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/token_sample/
+-rw-r--r--   0 sun       (1000) sun       (1000)     3784 2024-03-31 10:41:58.000000 dlk-0.1.0/dlk/token_sample/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2195 2024-03-22 11:48:12.000000 dlk-0.1.0/dlk/token_sample/beam_search.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3301 2024-03-22 11:59:33.000000 dlk-0.1.0/dlk/token_sample/diverse_beam_search.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3253 2024-03-22 11:59:35.000000 dlk-0.1.0/dlk/token_sample/diverse_siblings_search.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2215 2024-03-22 11:59:37.000000 dlk-0.1.0/dlk/token_sample/length_constrained_beam_search.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    14119 2024-03-22 11:59:38.000000 dlk-0.1.0/dlk/token_sample/lexically_constrained_beam_search.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2991 2024-03-22 11:59:40.000000 dlk-0.1.0/dlk/token_sample/prefix_constrained_beam_search.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5494 2024-03-22 11:59:43.000000 dlk-0.1.0/dlk/token_sample/sampling.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     9275 2024-04-03 19:15:33.000000 dlk-0.1.0/dlk/train.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/trainer/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      362 2024-03-22 11:48:13.000000 dlk-0.1.0/dlk/trainer/__init__.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    12144 2024-04-03 20:59:48.000000 dlk-0.1.0/dlk/trainer/lightning_trainer.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.978678 dlk-0.1.0/dlk/utils/
+-rw-rw-r--   0 sun       (1000) sun       (1000)      163 2024-03-22 11:48:23.000000 dlk-0.1.0/dlk/utils/__init__.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.982678 dlk-0.1.0/dlk/utils/display/
+-rw-r--r--   0 sun       (1000) sun       (1000)      163 2024-03-22 12:02:50.000000 dlk-0.1.0/dlk/utils/display/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      976 2024-03-22 12:03:20.000000 dlk-0.1.0/dlk/utils/display/annotation.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     5897 2024-03-22 12:03:30.000000 dlk-0.1.0/dlk/utils/display/ner.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    24196 2024-03-22 12:03:29.000000 dlk-0.1.0/dlk/utils/display/origin.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    22722 2024-03-22 12:03:46.000000 dlk-0.1.0/dlk/utils/display/relation_extraction.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2473 2024-03-22 12:03:57.000000 dlk-0.1.0/dlk/utils/display/style_utils.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)      982 2024-03-22 11:48:23.000000 dlk-0.1.0/dlk/utils/get_root.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      647 2024-03-22 12:00:19.000000 dlk-0.1.0/dlk/utils/import_module.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2221 2024-03-22 12:00:21.000000 dlk-0.1.0/dlk/utils/io.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2553 2024-03-22 12:00:23.000000 dlk-0.1.0/dlk/utils/logger.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2994 2024-03-31 08:48:43.000000 dlk-0.1.0/dlk/utils/ngram_repeat_block.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     2320 2024-03-22 12:00:29.000000 dlk-0.1.0/dlk/utils/register.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)    16508 2024-03-31 08:48:40.000000 dlk-0.1.0/dlk/utils/token_generation_constraints.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     3719 2024-03-22 11:48:23.000000 dlk-0.1.0/dlk/utils/tokenizer_util.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)     6792 2024-03-22 12:00:36.000000 dlk-0.1.0/dlk/utils/vocab.py
+-rw-rw-r--   0 sun       (1000) sun       (1000)       22 2024-04-05 12:02:09.000000 dlk-0.1.0/dlk/version.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.970678 dlk-0.1.0/dlk.egg-info/
+-rw-r--r--   0 sun       (1000) sun       (1000)     8739 2024-04-05 12:02:09.000000 dlk-0.1.0/dlk.egg-info/PKG-INFO
+-rw-rw-r--   0 sun       (1000) sun       (1000)     4677 2024-04-05 12:02:09.000000 dlk-0.1.0/dlk.egg-info/SOURCES.txt
+-rw-rw-r--   0 sun       (1000) sun       (1000)        1 2024-04-05 12:02:09.000000 dlk-0.1.0/dlk.egg-info/dependency_links.txt
+-rw-rw-r--   0 sun       (1000) sun       (1000)      387 2024-04-05 12:02:09.000000 dlk-0.1.0/dlk.egg-info/requires.txt
+-rw-rw-r--   0 sun       (1000) sun       (1000)        4 2024-04-05 12:02:09.000000 dlk-0.1.0/dlk.egg-info/top_level.txt
+-rw-rw-r--   0 sun       (1000) sun       (1000)       38 2024-04-05 12:02:09.982678 dlk-0.1.0/setup.cfg
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1713 2024-03-24 16:43:54.000000 dlk-0.1.0/setup.py
+drwxrwxr-x   0 sun       (1000) sun       (1000)        0 2024-04-05 12:02:09.982678 dlk-0.1.0/tests/
+-rw-rw-r--   0 sun       (1000) sun       (1000)     1799 2022-06-04 08:30:44.000000 dlk-0.1.0/tests/test_vocab.py
```

### Comparing `dlk-0.0.9/LICENSE` & `dlk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dlk-0.0.9/dlk/core/callbacks/lr_monitor.py` & `dlk-0.1.0/dlk/callback/lr_monitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
 from typing import Dict
-from . import callback_register, callback_config_register
-from pytorch_lightning.callbacks import LearningRateMonitor
-
 
-@callback_config_register('lr_monitor')
-class LearningRateMonitorCallbackConfig(object):
-    """Config for LearningRateMonitorCallback
-
-    Config Example:
-        >>> {
-        >>>     "_name": "lr_monitor",
-        >>>     "config": {
-        >>>         "logging_interval": null, // set to None to log at individual interval according to the interval key of each scheduler. other value : step, epoch
-        >>>         "log_momentum": true, // log momentum or not
-        >>>     }
-        >>> }
-    """
-    def __init__(self, config: Dict):
-        config = config['config']
-        self.logging_interval = config["logging_interval"]
-        self.log_momentum = config["log_momentum"]
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+from lightning.pytorch.callbacks import LearningRateMonitor
+
+from dlk.utils.register import register
+
+
+@cregister("callback", "lr_monitor")
+class LearningRateMonitorCallbackConfig(Base):
+    """callback for monitor the learning rate of the optimizer"""
+
+    logging_interval = StrField(
+        value=None,
+        options=["step", "epoch", None],
+        help="""set to ``'epoch'`` or ``'step'`` to log ``lr`` of all optimizers at the same interval, set to ``None`` to log at individual interval according to the ``interval`` key of each scheduler. Defaults to ``None``.""",
+    )
+    log_momentum = BoolField(
+        value=False,
+        help="option to also log the momentum values of the optimizer, if the optimizer has the ``momentum`` or ``betas`` attribute. Defaults to ``False``.",
+    )
 
 
-@callback_register('lr_monitor')
+@register("callback", "lr_monitor")
 class LearningRateMonitorCallback(object):
-    """Monitor the learning rate
-    """
+    """Monitor the learning rate"""
 
     def __init__(self, config: LearningRateMonitorCallbackConfig):
         super().__init__()
-        self.config = config
+        self.config = config._to_dict(only_para=True)
 
-    def __call__(self, rt_config: Dict)->LearningRateMonitor:
+    def __call__(self, rt_config: Dict) -> LearningRateMonitor:
         """return LearningRateMonitor object
 
         Args:
             rt_config: runtime config, include save_dir, and the checkpoint path name
 
-        Returns: 
+        Returns:
             LearningRateMonitor object
 
         """
-        return LearningRateMonitor(**self.config.__dict__)
+        return LearningRateMonitor(**self.config)
```

### Comparing `dlk-0.0.9/dlk/core/initmethods/default.py` & `dlk-0.1.0/dlk/initmethod/default.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-import torch.nn as nn
-from . import initmethod_register, initmethod_config_register
+import logging
 from typing import Dict, List
-from dlk.utils.logger import Logger
-from dlk.utils.config import BaseConfig
+
 import numpy as np
 import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
 
-logger = Logger.get_logger()
+logger = logging.getLogger(__name__)
 
 
-@initmethod_config_register('default')
-class DefaultInitConfig(BaseConfig):
-    """Config for RangeNormInit
-
-    Config Example:
-        >>> {
-        >>>     "_name": "default",
-        >>>     "config": {
-        >>>     }
-        >>> }
+@cregister("initmethod", "default")
+class DefaultInitConfig:
     """
-    def __init__(self, config):
-        super(DefaultInitConfig, self).__init__(config)
-        self.post_check(config['config'])
+    The default init method for the modules
+    """
+
+    pass
+
 
-@initmethod_register('default')
+@register("initmethod", "default")
 class DefaultInit(object):
-    """default method for init the modules
-    """
+    """default method for init the modules"""
 
     def __init__(self, config: DefaultInitConfig):
         super().__init__()
 
     def __call__(self, module):
         """Initialize the weights"""
         if isinstance(module, nn.Linear):
             # use the default kaiming init method
             torch.nn.init.xavier_uniform_(module.weight)
             if module.bias is not None:
                 module.bias.data.zero_()
         elif isinstance(module, nn.Embedding):
             torch.nn.init.xavier_uniform_(module.weight)
         elif isinstance(module, nn.LayerNorm):
-            module.bias.data.zero_()
-            module.weight.data.fill_(1.0)
+            # use the default init
+            # weight are initialized to 1, bias to 0
+            module.reset_parameters()
         elif isinstance(module, nn.Conv1d):
             torch.nn.init.kaiming_uniform_(module.weight)
         elif isinstance(module, nn.Conv2d):
             torch.nn.init.kaiming_uniform_(module.weight)
         elif isinstance(module, nn.Conv3d):
             torch.nn.init.kaiming_uniform_(module.weight)
         elif isinstance(module, nn.LSTM):
@@ -75,56 +75,39 @@
         else:
             logger.info(f"{module} is not initialization.")
 
     def init_lstm(self, lstm):
         """
         Initialize lstm
         """
-        # nn.init.xavier_uniform_(lstm.weight_hh_l0)
-        # nn.init.xavier_uniform_(lstm.weight_hh_l0_reverse)
-        # nn.init.xavier_uniform_(lstm.weight_ih_l0)
-        # nn.init.xavier_uniform_(lstm.weight_ih_l0_reverse)
-        # lstm.bias_hh_l0.data.fill_(0)
-        # lstm.bias_hh_l0_reverse.data.fill_(0)
-        # lstm.bias_ih_l0.data.fill_(0)
-        # lstm.bias_ih_l0_reverse.data.fill_(0)
-        # # Init forget gates to 1
-        # for names in lstm._all_weights:
-            # for name in filter(lambda n: 'bias' in n, names):
-                # bias = getattr(lstm, name)
-                # n = bias.size(0)
-                # start, end = n // 4, n // 2
-                # bias.data[start:end].fill_(1.)
-
-        # Another init method
         for ind in range(0, lstm.num_layers):
-            weight = eval('lstm.weight_ih_l' + str(ind))
+            weight = eval("lstm.weight_ih_l" + str(ind))
             bias = np.sqrt(6.0 / (weight.size(0) / 4 + weight.size(1)))
             nn.init.uniform_(weight, -bias, bias)
-            weight = eval('lstm.weight_hh_l' + str(ind))
+            weight = eval("lstm.weight_hh_l" + str(ind))
             bias = np.sqrt(6.0 / (weight.size(0) / 4 + weight.size(1)))
             nn.init.uniform_(weight, -bias, bias)
         if lstm.bidirectional:
             for ind in range(0, lstm.num_layers):
-                weight = eval('lstm.weight_ih_l' + str(ind) + '_reverse')
+                weight = eval("lstm.weight_ih_l" + str(ind) + "_reverse")
                 bias = np.sqrt(6.0 / (weight.size(0) / 4 + weight.size(1)))
                 nn.init.uniform_(weight, -bias, bias)
-                weight = eval('lstm.weight_hh_l' + str(ind) + '_reverse')
+                weight = eval("lstm.weight_hh_l" + str(ind) + "_reverse")
                 bias = np.sqrt(6.0 / (weight.size(0) / 4 + weight.size(1)))
                 nn.init.uniform_(weight, -bias, bias)
 
         if lstm.bias:
             for ind in range(0, lstm.num_layers):
-                weight = eval('lstm.bias_ih_l' + str(ind))
+                weight = eval("lstm.bias_ih_l" + str(ind))
                 weight.data.zero_()
-                weight.data[lstm.hidden_size: 2 * lstm.hidden_size] = 1
-                weight = eval('lstm.bias_hh_l' + str(ind))
+                weight.data[lstm.hidden_size : 2 * lstm.hidden_size] = 1
+                weight = eval("lstm.bias_hh_l" + str(ind))
                 weight.data.zero_()
-                weight.data[lstm.hidden_size: 2 * lstm.hidden_size] = 1
+                weight.data[lstm.hidden_size : 2 * lstm.hidden_size] = 1
             if lstm.bidirectional:
                 for ind in range(0, lstm.num_layers):
-                    weight = eval('lstm.bias_ih_l' + str(ind) + '_reverse')
+                    weight = eval("lstm.bias_ih_l" + str(ind) + "_reverse")
                     weight.data.zero_()
-                    weight.data[lstm.hidden_size: 2 * lstm.hidden_size] = 1
-                    weight = eval('lstm.bias_hh_l' + str(ind) + '_reverse')
+                    weight.data[lstm.hidden_size : 2 * lstm.hidden_size] = 1
+                    weight = eval("lstm.bias_hh_l" + str(ind) + "_reverse")
                     weight.data.zero_()
-                    weight.data[lstm.hidden_size: 2 * lstm.hidden_size] = 1
+                    weight.data[lstm.hidden_size : 2 * lstm.hidden_size] = 1
```

### Comparing `dlk-0.0.9/dlk/core/initmethods/range_norm.py` & `dlk-0.1.0/dlk/initmethod/range_norm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-import torch.nn as nn
-from dlk.utils.config import BaseConfig
-from . import initmethod_register, initmethod_config_register
 from typing import Dict, List
-import torch
+
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
 
 
-@initmethod_config_register('range_norm')
-class RangeNormInitConfig(BaseConfig):
-    """Config for RangeNormInit
-
-    Config Example:
-        >>> {
-        >>>     "_name": "range_norm",
-        >>>     "config": {
-        >>>         "range": 0.1,
-        >>>     }
-        >>> }
+@cregister("initmethod", "range_norm")
+class RangeNormInitConfig:
     """
-    def __init__(self, config):
-        super(RangeNormInitConfig, self).__init__(config)
-        self.range = config.get("range", 0.1)
-        self.post_check(config['config'], used=['range'])
+    init the parameters by the normal distribution with the given std
+    """
+
+    std = FloatField(
+        value=0.1,
+        minimum=0.0,
+        help="the std of the normal distribution init method",
+    )
+
 
-@initmethod_register('range_norm')
+@register("initmethod", "range_norm")
 class RangeNormInit(object):
-    """default for transformers init method
-    """
+    """default for transformers init method"""
 
     def __init__(self, config: RangeNormInitConfig):
         super().__init__()
-        self.range = config.range
-
+        self.std = config.std
 
     def __call__(self, module):
         """Initialize the weights"""
         if isinstance(module, nn.Linear):
-            module.weight.data.normal_(mean=0.0, std=self.range)
+            module.weight.data.normal_(mean=0.0, std=self.std)
             if module.bias is not None:
                 module.bias.data.zero_()
         elif isinstance(module, nn.Embedding):
-            module.weight.data.normal_(mean=0.0, std=self.range)
+            module.weight.data.normal_(mean=0.0, std=self.std)
             if module.padding_idx is not None:
                 module.weight.data[module.padding_idx].zero_()
         elif isinstance(module, nn.LayerNorm):
-            module.bias.data.zero_()
-            module.weight.data.fill_(1.0)
+            # use the default init
+            # weight are initialized to 1, bias to 0
+            module.reset_parameters()
         elif isinstance(module, nn.Conv1d):
-            module.weight.data.normal_(mean=0.0, std=self.range)
+            module.weight.data.normal_(mean=0.0, std=self.std)
         elif isinstance(module, nn.Conv2d):
-            module.weight.data.normal_(mean=0.0, std=self.range)
+            module.weight.data.normal_(mean=0.0, std=self.std)
         elif isinstance(module, nn.Conv3d):
-            module.weight.data.normal_(mean=0.0, std=self.range)
+            module.weight.data.normal_(mean=0.0, std=self.std)
```

### Comparing `dlk-0.0.9/dlk/core/initmethods/range_uniform.py` & `dlk-0.1.0/dlk/initmethod/range_uniform.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,76 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-import torch.nn as nn
-from dlk.utils.config import BaseConfig
-from . import initmethod_register, initmethod_config_register
 from typing import Dict, List
+
 import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
 
 
-@initmethod_config_register('range_uniform')
-class RangeUniformInitConfig(BaseConfig):
-    """Config for RangeNormInit
-
-    Config Example:
-        >>> {
-        >>>     "_name": "range_uniform",
-        >>>     "config": {
-        >>>         "range": 0.1,
-        >>>     }
-        >>> }
+@cregister("initmethod", "range_uniform")
+class RangeUniformInitConfig:
+
+    """
+    init the parameters by the uniform distribution with the given range
     """
-    def __init__(self, config):
-        super(RangeUniformInitConfig, self).__init__(config)
-        range = config.get("range", 0.1)
-        if isinstance(range, list):
-            assert len(range) == 2
-            self.range_from = range[0]
-            self.range_to = range[1]
-        else:
-            assert isinstance(range, float)
-            self.range_from = -abs(range)
-            self.range_to = abs(range)
-        self.post_check(config['config'], used='range')
 
-@initmethod_register('range_uniform')
+    range_from = FloatField(value=-0.1, help="the lower bound of the init value")
+    range_to = FloatField(value=0.1, help="the upper bound of the init value")
+
+
+@register("initmethod", "range_uniform")
 class RangeUniformInit(object):
-    """for transformers
-    """
+    """for transformers"""
 
     def __init__(self, config: RangeUniformInitConfig):
         super().__init__()
         self.config = config
 
     def __call__(self, module):
         """Initialize the weights"""
         if isinstance(module, nn.Linear):
-            module.weight.data.uniform_(from_=self.config.range_from, to=self.config.range_to)
+            module.weight.data.uniform_(
+                from_=self.config.range_from, to=self.config.range_to
+            )
             if module.bias is not None:
                 module.bias.data.zero_()
         elif isinstance(module, nn.Embedding):
-            module.weight.data.uniform_(from_=self.config.range_from, to=self.config.range_to)
+            module.weight.data.uniform_(
+                from_=self.config.range_from, to=self.config.range_to
+            )
             if module.padding_idx is not None:
                 module.weight.data[module.padding_idx].zero_()
         elif isinstance(module, nn.LayerNorm):
-            module.bias.data.zero_()
-            module.weight.data.fill_(1.0)
+            # use the default init,
+            # weight are initialized to 1, bias to 0
+            module.reset_parameters()
         elif isinstance(module, nn.Conv1d):
-            module.weight.data.uniform_(from_=self.config.range_from, to=self.config.range_to)
+            module.weight.data.uniform_(
+                from_=self.config.range_from, to=self.config.range_to
+            )
         elif isinstance(module, nn.Conv2d):
-            module.weight.data.uniform_(from_=self.config.range_from, to=self.config.range_to)
+            module.weight.data.uniform_(
+                from_=self.config.range_from, to=self.config.range_to
+            )
         elif isinstance(module, nn.Conv3d):
-            module.weight.data.uniform_(from_=self.config.range_from, to=self.config.range_to)
+            module.weight.data.uniform_(
+                from_=self.config.range_from, to=self.config.range_to
+            )
```

### Comparing `dlk-0.0.9/dlk/core/layers/decoders/biaffine.py` & `dlk-0.1.0/dlk/nn/loss/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,113 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import torch
-from typing import Dict, List, Set, Callable
-from dlk.core.base_module import SimpleModule, BaseModuleConfig
-from . import decoder_register, decoder_config_register
-from dlk.core.modules import module_config_register, module_register
-import torch.nn as nn
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-@decoder_config_register("biaffine")
-class BiAffineConfig(BaseModuleConfig):
-    """Config for BiAffine 
-
-    Config Example:
-        >>> {
-        >>>     "module": {
-        >>>         "_base": "biaffine",
-        >>>     },
-        >>>     "config": {
-        >>>         "input_size": "*@*",
-        >>>         "hidden_size": 0, //default equals to input_size
-        >>>         "output_size": "*@*",
-        >>>         "dropout": 0.0,
-        >>>         "output_map": {},
-        >>>         "input_map": {}, // required_key: provide_key
-        >>>     },
-        >>>     "_link":{
-        >>>         "config.input_size": ["module.config.hidden_size"],
-        >>>         "config.output_size": ["module.config.output_size"],
-        >>>     },
-        >>>     "_name": "biaffine",
-        >>> }
-    """
-    def __init__(self, config: Dict):
-        super(BiAffineConfig, self).__init__(config)
-        self.biaffine_config = config["module"]
-        config = config['config']
-        self.input_size = config['input_size']
-        self.hidden_size = config['hidden_size']
-        if not self.hidden_size:
-            self.hidden_size = self.input_size
-            self.biaffine_config['input_size'] = self.hidden_size
-        self.dropout = config['dropout']
-        self.post_check(config, used=[
-            "input_size",
-            "output_size",
-            "pool",
-            "dropout",
-        ])
-
-
-@decoder_register("biaffine")
-class BiAffine(SimpleModule):
-    """biaffine a x A x b
-    """
-    def __init__(self, config: BiAffineConfig):
-        super(BiAffine, self).__init__(config)
-        self._provide_keys = {'logits'}
-        self._required_keys = {'embedding'}
-        self._provided_keys = set()
+import importlib
+import os
+from typing import Dict
 
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    dataclass,
+)
+
+from dlk.utils.import_module import import_module_dir
+
+
+@dataclass
+class BaseLossConfig(Base):
+    """the base loss config"""
+
+    schedule = ListField(value=[1], help="the schedule of the loss, works with scale")
+    scale = ListField(value=[1], help="the scale of the loss for every schedule stage")
+    pred_truth_pair = DictField(
+        value={},
+        suggestions=[{"logits": "label_ids"}],
+        help="""
+        it's a dict of [predit_logits, truth_target] pair.
+        If you have more than one pair,
+        you should use the `multi_loss` module and provide this module as the submodule.
+        """,
+    )
+    reduction = StrField(
+        value="mean",
+        options=["mean", "sum", "none"],
+        help="the reduction method, support 'mean', 'sum', 'none'",
+    )
+
+    class LogMap:
+        loss = StrField(value="loss", help="the output loss name")
+
+    log_map = NestField(value=LogMap, help="the output loss name")
+
+
+class BaseLoss(nn.Module):
+    def __init__(self, config: BaseLossConfig):
+        super(BaseLoss, self).__init__()
         self.config = config
-        self.linear_a = nn.Linear(config.input_size, config.hidden_size)
-        self.linear_b = nn.Linear(config.input_size, config.hidden_size)
-        self.dropout = nn.Dropout(p=config.dropout)
-        self.active = nn.LeakyReLU() # TODO: why GELU get loss nan?
+        if len(self.config.pred_truth_pair) == 1:
+            self.pred_name = list(self.config.pred_truth_pair.keys())[0]
+            self.truth_name = self.config.pred_truth_pair[self.pred_name]
+        else:
+            assert len(self.config.pred_truth_pair) < 1
 
-        self.biaffine = module_register.get('biaffine')(module_config_register.get('biaffine')(config.biaffine_config))
+    def update_config(self, rt_config: Dict):
+        """callback for imodel to update the total steps and epochs
 
-    def init_weight(self, method: Callable):
-        """init the weight of submodules by 'method'
+        when init the loss module, the total step and epoch is not known, when all data ready, the imodel update the value for loss module
 
         Args:
-            method: init method
+            rt_config: { "total_steps": self.num_training_steps, "total_epochs": self.num_training_epochs}
 
-        Returns: 
+        Returns:
             None
 
         """
-        self.biaffine.init_weight(method)
+        self.current_stage = 0
+        self.config.schedule = [
+            rt_config["total_steps"] * i for i in self.config.schedule
+        ]
 
-    def forward(self, inputs: Dict[str, torch.Tensor])->Dict[str, torch.Tensor]:
-        """
+    def _calc(self, result, inputs, rt_config, scale):
+        """calc the loss the predict is from result, the ground truth is from inputs
 
         Args:
-            inputs: one mini-batch inputs
+            result: the model predict dict
+            inputs: the all inputs for model
+            rt_config: provide the current training status
+                >>> {
+                >>>     "current_step": self.global_step,
+                >>>     "current_epoch": self.current_epoch,
+                >>>     "total_steps": self.num_training_steps,
+                >>>     "total_epochs": self.num_training_epochs
+                >>> }
+            scale: the scale rate for the loss
 
-        Returns: 
-            one mini-batch outputs
+        Returns:
+            loss
 
         """
-        embedding = inputs[self.get_input_name('embedding')]
-        input_a = self.dropout(self.active(self.linear_a(embedding)))
-        input_b = self.dropout(self.active(self.linear_b(embedding)))
-        inputs[self.get_output_name("logits")] = self.biaffine(input_a, input_b)
-        if self._logits_gather.layer_map:
-            inputs.update(self._logits_gather([inputs[self.get_output_name('logits')]]))
-        return inputs
+        raise NotImplementedError
+
+    def forward(self, result, inputs, rt_config):
+        """same as self.calc"""
+        if rt_config["current_step"] > self.config.schedule[self.current_stage]:
+            self.current_stage += 1
+        scale = self.config.scale[self.current_stage]
+        return self._calc(result, inputs, rt_config, scale)
+
+
+loss_dir = os.path.dirname(__file__)
+import_module_dir(loss_dir, "dlk.nn.loss")
```

### Comparing `dlk-0.0.9/dlk/core/layers/decoders/linear_crf.py` & `dlk-0.1.0/dlk/nn/layer/decoder/linear_crf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,164 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
+
+from typing import Callable, Dict, List, Set
 
 import torch
-from typing import Dict, List, Set, Callable
-from dlk.core.base_module import BaseModule, BaseModuleConfig
-from . import decoder_register, decoder_config_register
-from dlk.core.modules import module_config_register, module_register
-import copy
-
-@decoder_config_register("linear_crf")
-class LinearCRFConfig(BaseModuleConfig):
-    """Config for LinearCRF 
-
-    Config Example:
-        >>> {
-        >>>     "module@linear": {
-        >>>         "_base": "linear",
-        >>>     },
-        >>>     "module@crf": {
-        >>>         "_base": "crf",
-        >>>     },
-        >>>     "config": {
-        >>>         "input_size": "*@*",  // the linear input_size
-        >>>         "output_size": "*@*", // the linear output_size
-        >>>         "reduction": "mean", // crf reduction method
-        >>>         "output_map": {}, //provide_key: output_key
-        >>>         "input_map": {} // required_key: provide_key
-        >>>     },
-        >>>     "_link":{
-        >>>         "config.input_size": ["module@linear.config.input_size"],
-        >>>         "config.output_size": ["module@linear.config.output_size", "module@crf.config.output_size"],
-        >>>         "config.reduction": ["module@crf.config.reduction"],
-        >>>     }
-        >>>     "_name": "linear_crf",
-        >>> }
-    """
-    def __init__(self, config: Dict):
-        super(LinearCRFConfig, self).__init__(config)
-        self.linear_config = config["module@linear"]
-        self.crf_config = config["module@crf"]
-        self.post_check(config['config'], used=['input_size', 'output_size', 'reduction'])
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.nn.base_module import BaseModule
+from dlk.utils.register import register
+
+
+@cregister("decoder", "linear_crf")
+class DecoderLinearCRFConfig(Base):
+    """the linear_crf decoder module"""
+
+    input_size = IntField(value=MISSING, minimum=1, help="the input size")
+    output_size = IntField(value=MISSING, minimum=1, help="the output size")
+    reduction = StrField(
+        value="mean",
+        options=["none", "sum", "mean", "token_mean"],
+        help="the reduction method",
+    )
+
+    class InputMap:
+        embedding = StrField(value="embedding", help="the embedding")
+        label_ids = StrField(value="label_ids", help="the label ids")
+        attention_mask = StrField(value="attention_mask", help="the attention mask")
+
+    input_map = NestField(value=InputMap, help="the input map of the linear_crf module")
+
+    class OutputMap:
+        predict_seq_label = StrField(
+            value="predict_seq_label", help="the predict seq label"
+        )
+        loss = StrField(value="loss", help="the loss")
+
+    output_map = NestField(
+        value=OutputMap, help="the output map of the linear_crf module"
+    )
+
+    submodule = SubModule(
+        {
+            "module@linear": {
+                "input_size": "@$$.input_size @lambda x: x",
+                "output_size": "@$$.output_size @lambda x: x",
+            },
+            "module@crf": {
+                "reduction": "@$$.reduction @lambda x: x",
+                "output_size": "@$$.output_size @lambda x: x",
+            },
+        }
+    )
 
 
-@decoder_register("linear_crf")
-class LinearCRF(BaseModule):
+@register("decoder", "linear_crf")
+class DecoderLinearCRF(BaseModule):
     """use torch.nn.Linear get the emission probability and fit to CRF"""
-    def __init__(self, config: LinearCRFConfig):
-        super(LinearCRF, self).__init__(config)
-        self._provide_keys = {'logits', "predict_seq_label"}
-        self._required_keys = {'embedding', 'label_ids', 'attention_mask'}
 
+    def __init__(self, config: DecoderLinearCRFConfig):
+        super(DecoderLinearCRF, self).__init__(config)
+
+        self.linear = register.get("module", "linear")(config["@module@linear"])
+        self.crf = register.get("module", "crf")(config["@module@crf"])
         self.config = config
-        self.linear = module_register.get('linear')(module_config_register.get('linear')(config.linear_config))
-        self.crf = module_register.get('crf')(module_config_register.get('crf')(config.crf_config))
 
     def init_weight(self, method: Callable):
         """init the weight of submodules by 'method'
 
         Args:
             method: init method
 
-        Returns: 
+        Returns:
             None
 
         """
         self.linear.init_weight(method)
         self.crf.init_weight(method)
 
-    def forward(self, inputs: Dict[str, torch.Tensor])->Dict[str, torch.Tensor]:
+    def forward(self, inputs: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """do predict, only get the predict labels
 
         Args:
             inputs: one mini-batch inputs
 
-        Returns: 
+        Returns:
             one mini-batch outputs
 
         """
         return self.predict_step(inputs)
 
-    def predict_step(self, inputs: Dict[str, torch.Tensor])->Dict[str, torch.Tensor]:
+    def predict_step(self, inputs: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """do predict, only get the predict labels
 
         Args:
             inputs: one mini-batch inputs
 
-        Returns: 
+        Returns:
             one mini-batch outputs
 
         """
-        logits = self.linear(inputs[self.get_input_name('embedding')])
-        if self._logits_gather.layer_map:
-            inputs.update(self._logits_gather([logits]))
-        inputs[self.get_output_name("predict_seq_label")] = self.crf(logits, inputs[self.get_input_name('attention_mask')])
+        logits = self.linear(inputs[self.config.input_map.embedding])
+        inputs[self.config.output_map.predict_seq_label] = self.crf(
+            logits, inputs[self.config.input_map.attention_mask]
+        )
         return inputs
 
-    def training_step(self, inputs: Dict[str, torch.Tensor])->Dict[str, torch.Tensor]:
+    def training_step(self, inputs: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """do training step, get the crf loss
 
         Args:
             inputs: one mini-batch inputs
 
-        Returns: 
+        Returns:
             one mini-batch outputs
 
         """
-        logits = self.linear(inputs[self.get_input_name('embedding')])
-        loss = self.crf.training_step(logits, inputs[self.get_input_name('label_ids')], inputs[self.get_input_name('attention_mask')])
-        if self._logits_gather.layer_map:
-            inputs.update(self._logits_gather([logits]))
-        inputs[self.get_output_name('loss')] = loss
+        logits = self.linear(inputs[self.config.input_map.embedding])
+        loss = self.crf.training_step(
+            logits,
+            inputs[self.config.input_map.label_ids],
+            inputs[self.config.input_map.attention_mask],
+        )
+        inputs[self.config.output_map.loss] = loss
         return inputs
 
-    def validation_step(self, inputs: Dict[str, torch.Tensor])->Dict[str, torch.Tensor]:
+    def validation_step(
+        self, inputs: Dict[str, torch.Tensor]
+    ) -> Dict[str, torch.Tensor]:
         """do validation step, get the crf loss and the predict labels
 
         Args:
             inputs: one mini-batch inputs
 
-        Returns: 
+        Returns:
             one mini-batch outputs
 
         """
-        logits = self.linear(inputs[self.get_input_name('embedding')])
-        loss = self.crf.training_step(logits, inputs[self.get_input_name('label_ids')], inputs[self.get_input_name('attention_mask')])
-        if self._logits_gather.layer_map:
-            inputs.update(self._logits_gather([logits]))
-        inputs[self.get_output_name('loss')] = loss
-        inputs[self.get_output_name("predict_seq_label")] = self.crf(logits, inputs[self.get_input_name('attention_mask')])
+        logits = self.linear(inputs[self.config.input_map.embedding])
+        loss = self.crf.training_step(
+            logits,
+            inputs[self.config.input_map.label_ids],
+            inputs[self.config.input_map.attention_mask],
+        )
+        inputs[self.config.output_map.loss] = loss
+        inputs[self.config.output_map.predict_seq_label] = self.crf(
+            logits, inputs[self.config.input_map.attention_mask]
+        )
         return inputs
```

### Comparing `dlk-0.0.9/dlk/core/layers/embeddings/random.py` & `dlk-0.1.0/dlk/nn/layer/embedding/random.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,117 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from . import embedding_register, embedding_config_register
-from typing import Dict, List, Set, Callable
-from dlk.core.base_module import SimpleModule, BaseModuleConfig
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
+
 import pickle as pkl
-import torch.nn as nn
-import torch
+from typing import Callable, Dict, List, Set
+
 import numpy as np
+import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
 
+from dlk.nn.base_module import SimpleModule
+from dlk.utils.register import register
 
-@embedding_config_register('random')
-class RandomEmbeddingConfig(BaseModuleConfig):
-    """Config for RandomEmbedding
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "vocab_size": "*@*",
-        >>>         "embedding_dim": "*@*",
-        >>>         "dropout": 0, //dropout rate
-        >>>         "padding_idx": 0, //dropout rate
-        >>>         "output_map": {},
-        >>>         "input_map": {},
-        >>>     },
-        >>>     "_name": "random",
-        >>> }
+
+@cregister("embedding", "random")
+class RandomEmbeddingConfig(Base):
+    """
+    the random embedding module config
     """
-    def __init__(self, config: Dict):
-        super(RandomEmbeddingConfig, self).__init__(config)
-        config = config['config']
-        self.vocab_size = config['vocab_size']
-        self.embedding_dim = config['embedding_dim']
-        self.dropout = config['dropout']
-        self.padding_idx = config['padding_idx']
-        self.post_check(config, used=[
-            "vocab_size",
-            "embedding_dim",
-            "padding_idx",
-            "dropout"
-        ])
 
+    vocab_size = IntField(
+        value=0,
+        minimum=0,
+        help="the vocab size, when the vocab size is 0, it means this class is overload by other Embedding(like Static)",
+    )
+    embedding_dim = IntField(value=MISSING, minimum=1, help="the embedding dim")
+    dropout = FloatField(value=0, minimum=0.0, maximum=1.0, help="dropout rate")
+    padding_idx = IntField(value=0, minimum=0, help="padding index")
+
+    class OutputMap:
+        embedding = StrField(value="embedding", help="the output of embedding name")
+
+    output_map = NestField(
+        value=OutputMap, help="the output map of the random embedding module"
+    )
+
+    class InputMap:
+        input_ids = StrField(value="input_ids", help="the input of input_ids name")
+
+    input_map = NestField(
+        value=InputMap, help="the input map of the random embedding module"
+    )
 
-@embedding_register('random')
+
+@register("embedding", "random")
 class RandomEmbedding(SimpleModule):
-    """ from 'input_ids' generate 'embedding'
-    """
+    """from 'input_ids' generate 'embedding'"""
 
     def __init__(self, config: RandomEmbeddingConfig):
         super().__init__(config)
-        self._provided_keys = set() # provided by privous module, will update by the check_keys_are_provided
-        self._provide_keys = {'embedding'} # provide by this module
-        self._required_keys = {'input_ids'} # required by this module
         self.config = config
         self.dropout = nn.Dropout(float(self.config.dropout))
-        normal =  torch.distributions.Normal(torch.tensor([0.0]), torch.tensor([2.0/self.config.embedding_dim]))
-        self.embedding = nn.Embedding.from_pretrained(normal.sample((self.config.vocab_size, self.config.embedding_dim)), padding_idx=self.config.padding_idx)
+        normal = torch.distributions.Normal(
+            torch.tensor([0.0]), torch.tensor([2.0 / self.config.embedding_dim])
+        )
+        if self.config.vocab_size:
+            self.embedding = nn.Embedding.from_pretrained(
+                normal.sample(
+                    (self.config.vocab_size, self.config.embedding_dim)
+                ).squeeze_(-1),
+                padding_idx=self.config.padding_idx,
+            )
 
     def init_weight(self, method: Callable):
         """init the weight of submodules by 'method'
 
         Args:
             method: init method
 
-        Returns: 
+        Returns:
             None
 
         """
         self.embedding.apply(method)
 
-    def forward(self, inputs: Dict[str, torch.Tensor])->Dict[str, torch.Tensor]:
+    def share_embedding(self, embedding):
+        """link the embedding.embedding to self.embedding
+
+        Args:
+            embedding: source embedding
+
+        Returns:
+            None
+
+        """
+        self.embedding = embedding.embedding
+
+    def forward(self, inputs: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """get the random embedding
 
         Args:
             inputs: one mini-batch inputs
 
-        Returns: 
+        Returns:
             one mini-batch outputs
 
         """
-        inputs[self.get_output_name('embedding')] = self.dropout(self.embedding(inputs[self.get_input_name('input_ids')]))
-        if self._logits_gather.layer_map:
-            inputs.update(self._logits_gather([inputs[self.get_output_name('embedding')]]))
-
+        inputs[self.config.output_map.embedding] = self.dropout(
+            self.embedding(inputs[self.config.input_map.input_ids])
+        )
         return inputs
```

### Comparing `dlk-0.0.9/dlk/core/losses/identity.py` & `dlk-0.1.0/dlk/nn/loss/focal_loss.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,120 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
+import logging
 from typing import Dict
-import torch.nn as nn
-from . import loss_register, loss_config_register
-from dlk.core.base_module import BaseModuleConfig
-import torch.nn as nn
-
 
-@loss_config_register("identity")
-class IdentityLossConfig(BaseModuleConfig):
-    """Config for IdentityLoss
-
-    Config Example:
-        >>> {
-        >>>     config: {
-        >>>         "schedule": [1],
-        >>>         "scale": [1], # scale the loss for every schedule
-        >>>         // "schedule": [0.3, 1.0], # can be a list or str
-        >>>         // "scale": "[0.5, 1]",
-        >>>         "loss": "loss", // the real loss from result['loss']
-        >>>     },
-        >>>     _name: "identity",
-        >>> }
-    """
-    def __init__(self, config: Dict):
-        super(IdentityLossConfig, self).__init__(config)
-        config = config['config']
-
-        self.scale = config['scale']
-        self.schedule = config['schedule']
-        self.loss = config['loss']
-
-        if isinstance(self.scale, str):
-            self.scale = eval(self.scale)
-        if isinstance(self.schedule, str):
-            self.schedule = eval(self.schedule)
-
-        if not isinstance(self.scale, list):
-            assert isinstance(float(self.scale), float)
-            self.scale = [self.scale]
-        if not isinstance(self.schedule, list):
-            assert isinstance(float(self.schedule), float)
-            self.schedule = [self.schedule]
-        assert len(self.schedule) == len(self.scale)
-        assert self.schedule[-1] - 1 < 0.00001
-        self.post_check(config, used=[
-            "loss",
-            "schedule",
-            "scale",
-        ])
-
-@loss_register("identity")
-class IdentityLoss(object):
-    """gather the loss and return when the loss is calc previor module like crf
-    """
-    def __init__(self, config: IdentityLossConfig):
-        super(IdentityLoss, self).__init__()
-        self.config = config
-
-    def update_config(self, rt_config):
-        """callback for imodel to update the total steps and epochs
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
+
+from . import BaseLoss, BaseLossConfig
+
+logger = logging.getLogger(__name__)
+
+
+@cregister("loss", "focal_loss")
+class FocalLossConfig(BaseLossConfig):
+    """the focal_loss loss config"""
+
+    weight = ListField(
+        value=None,
+        additions=[None],
+        help="the list of weights of every class",
+    )
+    ignore_index = IntField(value=-100, help="the ignore index")
+    gamma = FloatField(value=1.0, help="the gamma of focal loss")
+
+
+@register("loss", "focal_loss")
+class FocalLoss(BaseLoss):
+    """for multi class classification"""
+
+    def __init__(self, config: FocalLossConfig):
+        super(FocalLoss, self).__init__(config)
+        self.config: FocalLossConfig
+        if self.config.weight:
+            self.weight = torch.tensor(self.config.weight, dtype=torch.float)
+        else:
+            self.weight = None
 
-        when init the loss module, the total step and epoch is not known, when all data ready, the imodel update the value for loss module
+    def focal_loss(self, pred, target):
+        """calc focal loss
 
         Args:
-            rt_config: { "total_steps": self.num_training_steps, "total_epochs": self.num_training_epochs}
+            pred: NxC for logits
+            target: N for target
 
-        Returns: 
-            None
+        Returns:
+            loss
 
         """
+        # drop the ignore target
+        mask = target != self.config.ignore_index
+        target = target[mask]
+        pred = pred[mask]
+        # [N, 1]
+        target = target.unsqueeze(-1)
+        # [N, C]
+        pt = F.softmax(pred, dim=-1)
+        logpt = F.log_softmax(pred, dim=-1)
+        # [N]
+        pt = pt.gather(1, target).squeeze(-1)
+        logpt = logpt.gather(1, target).squeeze(-1)
+
+        if self.weight is not None:
+            # [N] at[i] = weight[target[i]]
+            at = self.weight.gather(0, target.squeeze(-1))
+            logpt = logpt * at
+
+        loss = -1 * (1 - pt) ** self.config.gamma * logpt
+        if self.config.reduction == "none":
+            return loss
+        if self.config.reduction == "mean":
+            return loss.mean()
+        return loss.sum()
 
-        self.current_stage = 0
-        self.config.schedule = [rt_config['total_steps']*i for i in self.config.schedule]
-
-    def calc(self, result, inputs, rt_config):
+    def _calc(self, result, inputs, rt_config, scale):
         """calc the loss the predict is from result, the ground truth is from inputs
 
         Args:
             result: the model predict dict
             inputs: the all inputs for model
-            rt_config: provide the current training status 
+            rt_config: provide the current training status
                 >>> {
                 >>>     "current_step": self.global_step,
                 >>>     "current_epoch": self.current_epoch,
                 >>>     "total_steps": self.num_training_steps,
                 >>>     "total_epochs": self.num_training_epochs
                 >>> }
+            scale: the scale rate for the loss
 
-        Returns: 
+        Returns:
             loss
 
         """
-        if rt_config['current_step']>self.config.schedule[self.current_stage]:
-            self.current_stage += 1
-        scale = self.config.scale[self.current_stage]
-        loss = result[self.config.loss] * scale
-        return loss
+        pred = result[self.pred_name]
+        target = inputs[self.truth_name]
+        pred = pred.reshape(-1, pred.shape[-1])
+        target = target.reshape(-1)
 
-    def __call__(self, result, inputs, rt_config):
-        """same as self.calc
-        """
-        return self.calc(result, inputs, rt_config)
+        loss = self.focal_loss(pred, target) * scale
+        return loss, {self.config.log_map.loss: loss}
```

### Comparing `dlk-0.0.9/dlk/core/modules/bert.py` & `dlk-0.1.0/dlk/nn/module/roberta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,139 +1,147 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-from transformers.models.bert.modeling_bert import BertModel
-from transformers.models.bert.configuration_bert import BertConfig
 import json
 import os
-import torch.nn as nn
-import torch
-from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
 from typing import Dict
-from . import module_register, module_config_register, Module
-from dlk.utils.config import BaseConfig
 
+import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+from transformers.models.roberta.configuration_roberta import RobertaConfig
+from transformers.models.roberta.modeling_roberta import RobertaModel
+
+from dlk.nn.module.bert import BertWrap, BertWrapConfig
+from dlk.utils.io import open
+from dlk.utils.register import register
+
+from . import Module
+
+
+@cregister("module", "roberta")
+class RobertaWrapConfig(BertWrapConfig):
+    """the Roberta config"""
+
+    pass
+
+
+@register("module", "roberta")
+class RobertaWrap(BertWrap):
+    """Roberta Wrap"""
 
-@module_config_register("bert")
-class BertWrapConfig(BaseConfig):
-    """Config for BertWrap
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "pretrained_model_path": "*@*",
-        >>>         "from_pretrain": true,
-        >>>         "freeze": false,
-        >>>         "dropout": 0.0,
-        >>>     },
-        >>>     "_name": "bert",
-        >>> }
-    """
-
-    def __init__(self, config: Dict):
-        super(BertWrapConfig, self).__init__(config)
-        self.pretrained_model_path = config['config']['pretrained_model_path']
-        self.from_pretrain = config['config']['from_pretrain']
-        self.freeze = config['config']['freeze']
-        self.dropout = config['config']['dropout']
-        if os.path.isdir(self.pretrained_model_path):
-            if os.path.exists(os.path.join(self.pretrained_model_path, 'config.json')):
-                self.bert_config = BertConfig(**json.load(open(os.path.join(self.pretrained_model_path, 'config.json'), 'r')))
+    def __init__(self, config: RobertaWrapConfig):
+        super(RobertaWrap, self).__init__(config)
+        self.config = config
+        if os.path.isdir(self.config.pretrained_model_path):
+            if os.path.exists(
+                os.path.join(self.config.pretrained_model_path, "config.json")
+            ):
+                with open(
+                    os.path.join(self.config.pretrained_model_path, "config.json"), "r"
+                ) as f:
+                    self.bert_config = RobertaConfig(**json.load(f))
             else:
-                raise PermissionError(f"config.json must in the dir {self.pretrained_model_path}")
+                raise PermissionError(
+                    f"config.json must in the dir {self.pretrained_model_path}"
+                )
         else:
-            if os.path.isfile(self.pretrained_model_path):
+            if os.path.isfile(self.config.pretrained_model_path):
                 try:
-                    self.bert_config = BertConfig(**json.load(open(self.pretrained_model_path, 'r')))
+                    with open(self.config.pretrained_model_path, "r") as f:
+                        self.bert_config = RobertaConfig(**json.load(f))
                 except:
-                    raise PermissionError(f"You must provide the pretrained model dir or the config file path.")
-        self.post_check(config['config'], used=['pretrained_model_path', 'from_pretrain', 'freeze', 'dropout'])
-
+                    raise PermissionError(
+                        f"You must provide the pretrained model dir or the config file path."
+                    )
 
-@module_register("bert")
-class BertWrap(Module):
-    """Bert wrap"""
-    def __init__(self, config: BertWrapConfig):
-        super(BertWrap, self).__init__()
-        self.config = config
-
-        self.bert = BertModel(config.bert_config, add_pooling_layer=False)
+        self.roberta = RobertaModel(self.bert_config, add_pooling_layer=False)
         self.dropout = nn.Dropout(float(self.config.dropout))
 
     def init_weight(self, method):
         """init the weight of model by 'bert.init_weight()' or from_pretrain
 
         Args:
             method: init method, no use for pretrained_transformers
 
-        Returns: 
+        Returns:
             None
 
         """
         if self.config.from_pretrain:
             self.from_pretrained()
         else:
-            self.bert.init_weights()
+            self.roberta.init_weights()
 
     def from_pretrained(self):
-        """init the model from pretrained_model_path
-        """
-        self.bert = BertModel.from_pretrained(self.config.pretrained_model_path)
+        """init the model from pretrained_model_path"""
+        self.roberta = RobertaModel.from_pretrained(self.config.pretrained_model_path)
 
-    def forward(self, inputs: Dict):
+    def forward(self, inputs):
         """do forward on a mini batch
 
         Args:
             batch: a mini batch inputs
 
-        Returns: 
+        Returns:
             sequence_output, all_hidden_states, all_self_attentions
 
         """
         if self.config.freeze:
+            self.roberta.eval()
             with torch.no_grad():
-                outputs = self.bert(
-                    input_ids = inputs.get("input_ids", None),
-                    attention_mask = inputs.get("attention_mask", None),
-                    token_type_ids = inputs.get("token_type_ids", None),
-                    position_ids = inputs.get("position_ids", None),
-                    head_mask = inputs.get("head_mask", None),
-                    inputs_embeds = inputs.get("inputs_embeds", None),
-                    encoder_hidden_states = inputs.get("encoder_hidden_states", None),
-                    encoder_attention_mask = inputs.get("encoder_attention_mask", None),
-                    past_key_values = inputs.get("past_key_values", None),
-                    use_cache = None,
-                    output_attentions = True,
-                    output_hidden_states = True,
-                    return_dict = False
+                outputs = self.roberta(
+                    input_ids=inputs.get("input_ids", None),
+                    attention_mask=inputs.get("attention_mask", None),
+                    token_type_ids=inputs.get("token_type_ids", None),
+                    position_ids=inputs.get("position_ids", None),
+                    head_mask=inputs.get("head_mask", None),
+                    inputs_embeds=inputs.get("inputs_embeds", None),
+                    encoder_hidden_states=inputs.get("encoder_hidden_states", None),
+                    encoder_attention_mask=inputs.get("encoder_attention_mask", None),
+                    past_key_values=inputs.get("past_key_values", None),
+                    use_cache=None,
+                    output_attentions=True,
+                    output_hidden_states=True,
+                    return_dict=False,
                 )
         else:
-            outputs = self.bert(
-                input_ids = inputs.get("input_ids", None),
-                attention_mask = inputs.get("attention_mask", None),
-                token_type_ids = inputs.get("token_type_ids", None),
-                position_ids = inputs.get("position_ids", None),
-                head_mask = inputs.get("head_mask", None),
-                inputs_embeds = inputs.get("inputs_embeds", None),
-                encoder_hidden_states = inputs.get("encoder_hidden_states", None),
-                encoder_attention_mask = inputs.get("encoder_attention_mask", None),
-                past_key_values = inputs.get("past_key_values", None),
-                use_cache = None,
-                output_attentions = True,
-                output_hidden_states = True,
-                return_dict = False
+            outputs = self.roberta(
+                input_ids=inputs.get("input_ids", None),
+                attention_mask=inputs.get("attention_mask", None),
+                token_type_ids=inputs.get("token_type_ids", None),
+                position_ids=inputs.get("position_ids", None),
+                head_mask=inputs.get("head_mask", None),
+                inputs_embeds=inputs.get("inputs_embeds", None),
+                encoder_hidden_states=inputs.get("encoder_hidden_states", None),
+                encoder_attention_mask=inputs.get("encoder_attention_mask", None),
+                past_key_values=inputs.get("past_key_values", None),
+                use_cache=None,
+                output_attentions=True,
+                output_hidden_states=True,
+                return_dict=False,
             )
-        assert len(outputs) == 4, f"Please check transformers version, the len(outputs) is 4 in version == 4.12|4.15, or check your config and remove the 'add_cross_attention'"
-        sequence_output, all_hidden_states, all_self_attentions = outputs[0], outputs[2], outputs[3]
+        assert (
+            len(outputs) == 4
+        ), f"Please check transformers version, the len(outputs) is 4 in version == 4.12, or check your config and remove the 'add_cross_attention'"
+        sequence_output, all_hidden_states, all_self_attentions = (
+            outputs[0],
+            outputs[2],
+            outputs[3],
+        )
         sequence_output = self.dropout(sequence_output)
         return sequence_output, all_hidden_states, all_self_attentions
```

### Comparing `dlk-0.0.9/dlk/core/modules/conv1d.py` & `dlk-0.1.0/dlk/nn/module/conv1d.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,80 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
+
+from typing import Collection, Dict, List
 
-import torch.nn as nn
-from dlk.utils.config import BaseConfig
 import torch
-from typing import Dict, List, Collection
-from . import module_register, module_config_register, Module
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.io import open
+from dlk.utils.register import register
+
+from . import Module
+
+
+@cregister("module", "conv1d")
+class Conv1dConfig:
+    """the 1D convolution config"""
+
+    in_channels = IntField(value=MISSING, minimum=0, help="the input channels")
+    out_channels = IntField(value=MISSING, minimum=0, help="the output channels")
+    dropout = FloatField(value=0.0, minimum=0.0, maximum=1.0, help="the dropout rate")
+    kernel_sizes = ListField(value=[3], help="the kernel sizes")
 
-@module_config_register("conv1d")
-class Conv1dConfig(BaseConfig):
-    """Config for Conv1d
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "in_channels": "*@*",
-        >>>         "out_channels": "*@*",
-        >>>         "dropout": 0.0,
-        >>>         "kernel_sizes": [3],
-        >>>     },
-        >>>     "_name": "conv1d",
-        >>> }
-    """
-    def __init__(self, config: Dict):
-        super(Conv1dConfig, self).__init__(config)
-        config = config['config']
-        self.kernel_sizes = config['kernel_sizes']
-        out_channels = config['out_channels']
-        assert all(k % 2 == 1 for k in self.kernel_sizes), 'the kernel sizes must be odd'
-        assert out_channels % len(self.kernel_sizes) == 0, 'out channels must be dividable by kernels'
-        self.in_channels = config['in_channels']
-        self.out_channels = out_channels // len(self.kernel_sizes)
-        self.dropout = config['dropout']
-        self.post_check(config, used=[
-            "in_channels",
-            "out_channels",
-            "dropout",
-            "kernel_sizes",
-        ])
 
-@module_register("conv1d")
+@register("module", "conv1d")
 class Conv1d(Module):
-    """Conv for 1d input
-    """
+    """Conv for 1d input"""
+
     def __init__(self, config: Conv1dConfig):
         super().__init__()
+        self.config = config
+        assert all(
+            k % 2 == 1 for k in self.config.kernel_sizes
+        ), "the kernel sizes must be odd"
+        assert (
+            self.config.out_channels % len(self.config.kernel_sizes) == 0
+        ), "out channels must be dividable by kernels"
+        self.config.out_channels = self.config.out_channels // len(
+            self.config.kernel_sizes
+        )
+
         convs = []
-        for kernel_size in config.kernel_sizes:
-            conv = nn.Conv1d(config.in_channels, config.out_channels, kernel_size,
-                             padding=(kernel_size - 1) // 2)
+        for kernel_size in self.config.kernel_sizes:
+            conv = nn.Conv1d(
+                self.config.in_channels,
+                self.config.out_channels,
+                kernel_size,
+                padding=(kernel_size - 1) // 2,
+            )
             convs.append(nn.Sequential(conv, nn.GELU()))
         self.convs = nn.ModuleList(convs)
-        self.dropout = nn.Dropout(p=float(config.dropout))
+        self.dropout = nn.Dropout(p=float(self.config.dropout))
 
     def forward(self, x: torch.Tensor):
         """do forward on a mini batch
 
         Args:
             batch: a mini batch inputs
 
-        Returns: 
+        Returns:
             conv result the shape is the same as input
 
         """
         return self.dropout(torch.cat([conv(x) for conv in self.convs], dim=-1))
```

### Comparing `dlk-0.0.9/dlk/core/modules/crf.py` & `dlk-0.1.0/dlk/nn/module/crf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,76 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-import torch
-import torch.nn as nn
 from typing import Callable, Dict, List
-from . import module_register, module_config_register, Module
-from dlk.utils.config import BaseConfig
 
-@module_config_register("crf")
-class CRFConfig(BaseConfig):
-    """Config for ConditionalRandomField
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "output_size": 2,
-        >>>         "batch_first": true,
-        >>>         "reduction": "mean", //none|sum|mean|token_mean
-        >>>     },
-        >>>     "_name": "crf",
-        >>> }
-    """
-    def __init__(self, config: Dict):
-        super(CRFConfig, self).__init__(config)
-        config = config['config']
-        self.output_size = config['output_size']
-        if self.output_size <= 0:
-            raise ValueError(f'invalid number of tags: {self.output_size}')
-        self.post_check(config, used=[
-            "output_size",
-            "batch_first",
-            "reduction",
-        ])
+import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
+
+from . import Module
+
+
+@cregister("module", "crf")
+class CRFConfig:
+    """the ConditionalRandomField config"""
+
+    output_size = IntField(value=MISSING, minimum=0, help="the output size")
+    batch_first = BoolField(value=True, help="whether the input is batch first")
+    reduction = StrField(
+        value="mean",
+        options=["none", "sum", "mean", "token_mean"],
+        help="the reduction method",
+    )
 
 
-@module_register("crf")
+@register("module", "crf")
 class ConditionalRandomField(Module):
-    """ CRF, training_step for training, forward for decode。
-    """
+    """CRF, training_step for training, forward for decode。"""
 
     def __init__(self, config: CRFConfig):
         super(ConditionalRandomField, self).__init__()
+        self.config = config
 
-        self.num_tags = config.output_size
+        self.num_tags = self.config.output_size
 
-        self.transitions = nn.parameter.Parameter(torch.randn(self.num_tags, self.num_tags))
+        self.transitions = nn.parameter.Parameter(
+            torch.randn(self.num_tags, self.num_tags)
+        )
         self.start_transitions = nn.parameter.Parameter(torch.randn(self.num_tags))
         self.end_transitions = nn.parameter.Parameter(torch.randn(self.num_tags))
 
     def init_weight(self, method: Callable):
         """init the weight of transitions, start_transitions and end_transitions
 
         Initialize the transition parameters.
         The parameters will be initialized randomly from a uniform distribution
         between -0.1 and 0.1.
 
         Args:
             method: init method, no use
 
-        Returns: 
+        Returns:
             None
 
         """
 
         nn.init.normal_(self.transitions, -1, 0.1)
         nn.init.uniform_(self.start_transitions, -0.1, 0.1)
         nn.init.uniform_(self.end_transitions, -0.1, 0.1)
@@ -83,76 +80,89 @@
 
         The sum of the likelihoods across all possible state sequences.
 
         Args:
             logits: max_len*batch_size*num_tags
             mask: max_len*batch_size
 
-        Returns: 
+        Returns:
             batch_size*every sum
 
         """
         seq_len, batch_size, n_tags = logits.size()
         alpha = logits[0]
         alpha = alpha + self.start_transitions.view(1, -1)
 
         flip_mask = mask.eq(False)
 
         for i in range(1, seq_len):
             emit_score = logits[i].view(batch_size, 1, n_tags)
             trans_score = self.transitions.view(1, n_tags, n_tags)
             tmp = alpha.view(batch_size, n_tags, 1) + emit_score + trans_score
-            alpha = torch.logsumexp(tmp, 1).masked_fill(flip_mask[i].view(batch_size, 1), 0) + \
-                    alpha.masked_fill(mask[i].eq(True).view(batch_size, 1), 0)
+            alpha = torch.logsumexp(tmp, 1).masked_fill(
+                flip_mask[i].view(batch_size, 1), 0
+            ) + alpha.masked_fill(mask[i].eq(True).view(batch_size, 1), 0)
 
         alpha = alpha + self.end_transitions.view(1, -1)
 
         return torch.logsumexp(alpha, 1)
 
-    def _gold_score(self, logits: torch.FloatTensor, tags: torch.LongTensor, mask: torch.ByteTensor):
-        """ Compute the score for the gold path.
+    def _gold_score(
+        self, logits: torch.FloatTensor, tags: torch.LongTensor, mask: torch.ByteTensor
+    ):
+        """Compute the score for the gold path.
 
         Args:
             logits: max_len*batch_size*num_tags
             tags: max_len*batch_size
             mask: max_len*batch_size
 
-        Returns: 
+        Returns:
             batch_size*every_gold_score
 
         """
         seq_len, batch_size, _ = logits.size()
         batch_idx = torch.arange(batch_size, dtype=torch.long, device=logits.device)
         seq_idx = torch.arange(seq_len, dtype=torch.long, device=logits.device)
 
         # trans_socre [L-1, B]
         mask = mask.eq(True)
         flip_mask = mask.eq(False)
-        trans_score = self.transitions[tags[:seq_len - 1], tags[1:]].masked_fill(flip_mask[1:, :], 0)
+        trans_score = self.transitions[tags[: seq_len - 1], tags[1:]].masked_fill(
+            flip_mask[1:, :], 0
+        )
         # emit_score [L, B]
-        emit_score = logits[seq_idx.view(-1, 1), batch_idx.view(1, -1), tags].masked_fill(flip_mask, 0)
+        emit_score = logits[
+            seq_idx.view(-1, 1), batch_idx.view(1, -1), tags
+        ].masked_fill(flip_mask, 0)
         # score [L-1, B]
-        score = trans_score + emit_score[:seq_len - 1, :]
+        score = trans_score + emit_score[: seq_len - 1, :]
         score = score.sum(0) + emit_score[-1].masked_fill(flip_mask[-1], 0)
-        st_scores = self.start_transitions.view(1, -1).repeat(batch_size, 1)[batch_idx, tags[0]]
+        st_scores = self.start_transitions.view(1, -1).repeat(batch_size, 1)[
+            batch_idx, tags[0]
+        ]
         last_idx = mask.long().sum(0) - 1
-        ed_scores = self.end_transitions.view(1, -1).repeat(batch_size, 1)[batch_idx, tags[last_idx, batch_idx]]
+        ed_scores = self.end_transitions.view(1, -1).repeat(batch_size, 1)[
+            batch_idx, tags[last_idx, batch_idx]
+        ]
         score = score + st_scores + ed_scores
         # return [B,]
         return score
 
-    def training_step(self, logits: torch.FloatTensor, tags: torch.LongTensor, mask: torch.LongTensor):
+    def training_step(
+        self, logits: torch.FloatTensor, tags: torch.LongTensor, mask: torch.LongTensor
+    ):
         """training step, calc the loss
 
         Args:
             logits: emissions, batch_size*max_len*num_tags
             tags: batch_size*max_len
             mask: batch_size*max_len, mask==0 means padding
 
-        Returns: 
+        Returns:
             loss
 
         """
         logits = logits.transpose(0, 1)
         tags = tags.transpose(0, 1).long()
         mask = mask.transpose(0, 1).byte()
         all_path_score = self._normalizer_likelihood(logits, mask)
@@ -163,31 +173,32 @@
     def forward(self, logits: torch.FloatTensor, mask: torch.LongTensor):
         """predict step, get the best path
 
         Args:
             logits: emissions, batch_size*max_len*num_tags
             mask: batch_size*max_len, mask==0 means padding
 
-        Returns: 
+        Returns:
             batch*max_len
 
         """
         logits = logits.transpose(0, 1)  # L, B, H
         mask = mask.transpose(0, 1)
         return self._viterbi_decode(logits, mask)
 
-    def _viterbi_decode(self, emissions: torch.FloatTensor,
-                        mask: torch.LongTensor) -> torch.Tensor:
+    def _viterbi_decode(
+        self, emissions: torch.FloatTensor, mask: torch.LongTensor
+    ) -> torch.Tensor:
         """predict step, get the best path
 
         Args:
             logits: emissions, max_len*batch_size*num_tags
             mask: max_len*batch_size, mask==0 means padding
 
-        Returns: 
+        Returns:
             batch*max_len
 
         """
         # emissions: (seq_length, batch_size, num_tags)
         # mask: (seq_length, batch_size)
         assert emissions.dim() == 3 and mask.dim() == 2
         assert emissions.shape[:2] == mask.shape
@@ -249,21 +260,21 @@
             # Find the tag which maximizes the score at the last timestep; this is our best tag
             # for the last timestep
             _, best_last_tag = score[idx].max(dim=0)
             best_tags = [best_last_tag.item()]
 
             # We trace back where the best last tag comes from, append that to our best tag
             # sequence, and trace it back again, and so on
-            for hist in reversed(history[:seq_ends[idx]]):
+            for hist in reversed(history[: seq_ends[idx]]):
                 best_last_tag = hist[idx][best_tags[-1]]
                 best_tags.append(best_last_tag.item())
 
             # Reverse the order because we start from the last timestep
             best_tags.reverse()
             best_tags_list.append(best_tags)
 
         output = torch.jit.annotate(List[List[int]], [])
         for tag_list in best_tags_list:
-            if len(tag_list)<seq_length:
-                tag_list = tag_list + [-1]*(seq_length-len(tag_list))
+            if len(tag_list) < seq_length:
+                tag_list = tag_list + [-1] * (seq_length - len(tag_list))
             output.append(tag_list)
         return torch.tensor(output, dtype=torch.long, device=mask.device)
```

### Comparing `dlk-0.0.9/dlk/core/modules/distil_bert.py` & `dlk-0.1.0/dlk/nn/module/distil_bert.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,133 +1,145 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-from transformers.models.distilbert.modeling_distilbert import DistilBertModel
-from transformers.models.distilbert.configuration_distilbert import DistilBertConfig
 import json
+import logging
 import os
-import torch.nn as nn
+from typing import Dict
+
 import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
 from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
-from typing import Dict
-from dlk.utils.logger import Logger
-from . import module_register, module_config_register, Module
-from dlk.utils.config import BaseConfig
-
-logger = Logger.get_logger()
-
-@module_config_register("distil_bert")
-class DistilBertWrapConfig(BaseConfig):
-    """Config for DistilBertWrap
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "pretrained_model_path": "*@*",
-        >>>         "from_pretrain": true,
-        >>>         "freeze": false,
-        >>>         "dropout": 0.0,
-        >>>     },
-
-        >>>     "_name": "distil_bert",
-        >>> }
-    """
-
-    def __init__(self, config: Dict):
-        super(DistilBertWrapConfig, self).__init__(config)
-        self.pretrained_model_path = config['config']['pretrained_model_path']
-        self.from_pretrain = config['config']['from_pretrain']
-        self.freeze = config['config']['freeze']
-        self.dropout = config['config']['dropout']
-        if os.path.isdir(self.pretrained_model_path):
-            if os.path.exists(os.path.join(self.pretrained_model_path, 'config.json')):
-                self.distil_bert_config = DistilBertConfig(**json.load(open(os.path.join(self.pretrained_model_path, 'config.json'), 'r')))
-            else:
-                raise PermissionError(f"config.json must in the dir {self.pretrained_model_path}")
-        else:
-            if os.path.isfile(self.pretrained_model_path):
-                try:
-                    self.distil_bert_config = DistilBertConfig(**json.load(open(self.pretrained_model_path, 'r')))
-                except:
-                    raise PermissionError(f"You must provide the pretrained model dir or the config file path.")
-        self.post_check(config['config'], used=['pretrained_model_path', 'from_pretrain', 'freeze', 'dropout'])
+from transformers.models.distilbert.configuration_distilbert import DistilBertConfig
+from transformers.models.distilbert.modeling_distilbert import DistilBertModel
+
+from dlk.utils.io import open
+from dlk.utils.register import register
+
+from . import Module
+
+logger = logging.getLogger(__name__)
+
+
+@cregister("module", "distil_bert")
+class DistilBertWrapConfig:
+    """the distil_bert config"""
+
+    pretrained_model_path = StrField(value=MISSING, help="the pretrained model path")
+    from_pretrain = BoolField(value=True, help="whether to load the pretrained model")
+    freeze = BoolField(value=False, help="whether to freeze the model")
+    dropout = FloatField(value=0.0, minimum=0.0, maximum=1.0, help="the dropout rate")
 
 
-@module_register("distil_bert")
+@register("module", "distil_bert")
 class DistilBertWrap(Module):
     """DistillBertWrap"""
+
     def __init__(self, config: DistilBertWrapConfig):
         super(DistilBertWrap, self).__init__()
         self.config = config
+        if os.path.isdir(self.config.pretrained_model_path):
+            if os.path.exists(
+                os.path.join(self.config.pretrained_model_path, "config.json")
+            ):
+                with open(
+                    os.path.join(self.config.pretrained_model_path, "config.json"), "r"
+                ) as f:
+                    self.bert_config = DistilBertConfig(**json.load(f))
+            else:
+                raise PermissionError(
+                    f"config.json must in the dir {self.pretrained_model_path}"
+                )
+        else:
+            if os.path.isfile(self.config.pretrained_model_path):
+                try:
+                    with open(self.config.pretrained_model_path, "r") as f:
+                        self.bert_config = DistilBertConfig(**json.load(f))
+                except:
+                    raise PermissionError(
+                        f"You must provide the pretrained model dir or the config file path."
+                    )
 
-        self.distil_bert = DistilBertModel(config.distil_bert_config)
+        self.distil_bert = DistilBertModel(self.bert_config)
         self.dropout = nn.Dropout(float(self.config.dropout))
 
     def init_weight(self, method):
         """init the weight of model by 'bert.init_weight()' or from_pretrain
 
         Args:
             method: init method, no use for pretrained_transformers
 
-        Returns: 
+        Returns:
             None
 
         """
         if self.config.from_pretrain:
             self.from_pretrained()
         else:
-            logger.info(f'Training the distill bert from scratch')
+            logger.info(f"Training the distill bert from scratch")
             self.distil_bert.init_weights()
 
     def from_pretrained(self):
-        """init the model from pretrained_model_path
-        """
-        logger.info(f'Init the distill bert from {self.config.pretrained_model_path}')
-        self.distil_bert = DistilBertModel.from_pretrained(self.config.pretrained_model_path)
+        """init the model from pretrained_model_path"""
+        logger.info(f"Init the distill bert from {self.config.pretrained_model_path}")
+        self.distil_bert = DistilBertModel.from_pretrained(
+            self.config.pretrained_model_path
+        )
 
     def forward(self, inputs):
         """do forward on a mini batch
 
         Args:
             batch: a mini batch inputs
 
-        Returns: 
+        Returns:
             sequence_output, all_hidden_states, all_self_attentions
 
         """
         if self.config.freeze:
             self.distil_bert.eval()
             with torch.no_grad():
                 outputs = self.distil_bert(
-                    input_ids = inputs.get("input_ids", None),
-                    attention_mask = inputs.get("attention_mask", None),
-                    head_mask = inputs.get("head_mask", None),
-                    inputs_embeds = inputs.get("inputs_embeds", None),
-                    output_attentions = True,
-                    output_hidden_states = True,
-                    return_dict = False
+                    input_ids=inputs.get("input_ids", None),
+                    attention_mask=inputs.get("attention_mask", None),
+                    head_mask=inputs.get("head_mask", None),
+                    inputs_embeds=inputs.get("inputs_embeds", None),
+                    output_attentions=True,
+                    output_hidden_states=True,
+                    return_dict=False,
                 )
         else:
             outputs = self.distil_bert(
-                input_ids = inputs.get("input_ids", None),
-                attention_mask = inputs.get("attention_mask", None),
-                head_mask = inputs.get("head_mask", None),
-                inputs_embeds = inputs.get("inputs_embeds", None),
-                output_attentions = True,
-                output_hidden_states = True,
-                return_dict = False
+                input_ids=inputs.get("input_ids", None),
+                attention_mask=inputs.get("attention_mask", None),
+                head_mask=inputs.get("head_mask", None),
+                inputs_embeds=inputs.get("inputs_embeds", None),
+                output_attentions=True,
+                output_hidden_states=True,
+                return_dict=False,
             )
-        assert len(outputs) == 3, f"Please check transformers version, the len(outputs) is 3 for version == 4.12, and this version the output logistic of distil_bert is not as the same as bert and roberta."
-        sequence_output, all_hidden_states, all_self_attentions = outputs[0], outputs[1], outputs[2]
+        assert (
+            len(outputs) == 3
+        ), f"Please check transformers version, the len(outputs) is 3 for version == 4.12, and this version the output logistic of distil_bert is not as the same as bert and roberta."
+        sequence_output, all_hidden_states, all_self_attentions = (
+            outputs[0],
+            outputs[1],
+            outputs[2],
+        )
         sequence_output = self.dropout(sequence_output)
         return sequence_output, all_hidden_states, all_self_attentions
```

### Comparing `dlk-0.0.9/dlk/core/modules/linear.py` & `dlk-0.1.0/dlk/nn/module/linear.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,77 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-import torch.nn as nn
-import torch
 from typing import Dict, List
-from . import module_register, module_config_register, Module
-from dlk.utils.config import BaseConfig
+
+import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
+
+from . import Module
 
 
-@module_config_register("linear")
-class LinearConfig(BaseConfig):
-    """Config for Linear
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "input_size": 256,
-        >>>         "output_size": 2,
-        >>>         "dropout": 0.0, //the module output no need dropout
-        >>>         "bias": true, // use bias or not in linear , if set to false, all the bias will be set to 0
-        >>>         "pool": null, // pooling output or not
-        >>>     },
-        >>>     "_name": "linear",
-        >>> }
+@cregister("module", "linear")
+class LinearConfig:
     """
-    def __init__(self, config: Dict):
-        super(LinearConfig, self).__init__(config)
-        config = config['config']
-        self.input_size = config['input_size']
-        self.output_size = config['output_size']
-        self.dropout = float(config['dropout'])
-        self.bias = config['bias']
-        self.pool = config['pool']
-        self.post_check(config, used=[
-            "input_size",
-            "output_size",
-            "dropout",
-            "bias",
-            "pool",
-        ])
+    The Linear module config
+    """
+
+    input_size = IntField(value=MISSING, minimum=0, help="the input size")
+    output_size = IntField(value=MISSING, minimum=0, help="the output size")
+    dropout = FloatField(value=0.0, minimum=0.0, maximum=1.0, help="the dropout rate")
+    bias = BoolField(value=True, help="whether to use bias")
+    pool = StrField(
+        value=None,
+        options=["first", None],
+        help="the pooling method, currently only implement `first`",
+    )
 
 
-@module_register("linear")
+@register("module", "linear")
 class Linear(Module):
     """wrap for nn.Linear"""
+
     def __init__(self, config: LinearConfig):
         super(Linear, self).__init__()
-        self.linear = nn.Linear(in_features=config.input_size, out_features=config.output_size, )
-        self.dropout = nn.Dropout(p=float(config.dropout))
         self.config = config
+        self.linear = nn.Linear(
+            in_features=self.config.input_size, out_features=self.config.output_size
+        )
+        self.dropout = nn.Dropout(p=float(self.config.dropout))
 
-    def forward(self, input: torch.Tensor)->torch.Tensor:
+    def forward(self, input: torch.Tensor) -> torch.Tensor:
         """do forward on a mini batch
 
         Args:
             batch: a mini batch inputs
 
-        Returns: 
+        Returns:
             project result the shape is the same as input(no poll), otherwise depend on poll method
 
         """
         output = self.dropout(self.linear(input))
         if not self.config.pool:
             return output
-        elif self.config.pool == 'first':
+        elif self.config.pool == "first":
             return output[:, 0]
         else:
-            raise PermissionError(f"Currenttly we have not support the pool method '{self.config.pool}' in linear.")
+            raise PermissionError(
+                f"Currenttly we have not support the pool method '{self.config.pool}' in linear."
+            )
```

### Comparing `dlk-0.0.9/dlk/core/modules/lstm.py` & `dlk-0.1.0/dlk/nn/module/lstm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
+
+from typing import Dict
 
-import torch.nn as nn
 import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
 from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
-from typing import Dict
-from dlk.utils.config import BaseConfig
-from . import module_register, module_config_register, Module
-from dlk.utils.logger import Logger
-
-logger = Logger.get_logger()
-
-@module_config_register("lstm")
-class LSTMConfig(BaseConfig):
-    """Config for def 
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "bidirectional": true,
-        >>>         "output_size": 200, //the output is 2*hidden_size if use
-        >>>         "input_size": 200,
-        >>>         "num_layers": 1,
-        >>>         "dropout": 0.1, // dropout between layers
-        >>>         "dropout_last": true, //dropout the last layer output or not
-        >>>     },
-        >>>     "_name": "lstm",
-        >>> }
-    """
-
-    def __init__(self, config: Dict):
-        super(LSTMConfig, self).__init__(config)
-        config = config['config']
-        self.num_layers = config['num_layers']
-        self.bidirectional= config['bidirectional']
-        self.input_size = config['input_size']
-        self.output_size = config['output_size']
-        self.hidden_size = self.output_size
-        if self.bidirectional:
-            assert self.output_size % 2 == 0
-            self.hidden_size = self.output_size // 2
-        self.dropout = config['dropout']
-        self.dropout_last = config['dropout_last']
-        self.post_check(config, used=[
-            "bidirectional",
-            "output_size",
-            "input_size",
-            "num_layers",
-            "dropout",
-            "dropout_last",
-        ])
 
+from dlk.utils.register import register
 
-@module_register("lstm")
+from . import Module
+
+
+@cregister("module", "lstm")
+class LSTMConfig:
+    """the lstm config"""
+
+    bidirectional = BoolField(value=True, help="whether to use bidirectional lstm")
+    input_size = IntField(value=MISSING, minimum=0, help="the input size")
+    output_size = IntField(value=MISSING, minimum=0, help="the output size")
+    num_layers = IntField(value=1, minimum=1, help="the number of layers")
+    dropout = FloatField(value=0.0, minimum=0.0, maximum=1.0, help="the dropout rate")
+    dropout_last = BoolField(
+        value=True, help="whether to dropout the last layer output"
+    )
+
+
+@register("module", "lstm")
 class LSTM(Module):
     "A wrap for nn.LSTM"
+
     def __init__(self, config: LSTMConfig):
         super(LSTM, self).__init__()
+        self.config = config
 
-        if config.num_layers <= 1:
+        if self.config.num_layers <= 1:
             inlstm_dropout = 0
         else:
-            inlstm_dropout = config.dropout
-        self.lstm = nn.LSTM(input_size=config.input_size, hidden_size=config.hidden_size, num_layers=config.num_layers, batch_first=True, bidirectional=config.bidirectional, dropout=inlstm_dropout)
-        self.dropout_last = nn.Dropout(p=float(config.dropout) if config.dropout_last else 0)
+            inlstm_dropout = self.config.dropout
+
+        hidden_size = self.config.output_size
+        if self.config.bidirectional:
+            assert self.config.output_size % 2 == 0
+            hidden_size = self.config.output_size // 2
+
+        self.lstm = nn.LSTM(
+            input_size=self.config.input_size,
+            hidden_size=hidden_size,
+            num_layers=self.config.num_layers,
+            batch_first=True,
+            bidirectional=self.config.bidirectional,
+            dropout=inlstm_dropout,
+        )
+        self.dropout_last = nn.Dropout(
+            p=float(self.config.dropout) if self.config.dropout_last else 0
+        )
 
-    def forward(self, input: torch.Tensor, mask: torch.Tensor)->torch.Tensor:
+    def forward(self, input: torch.Tensor, mask: torch.Tensor) -> torch.Tensor:
         """do forward on a mini batch
 
         Args:
             batch: a mini batch inputs
 
-        Returns: 
+        Returns:
             lstm output the shape is the same as input
 
         """
         max_seq_len = input.size(1)
         seq_lens = mask.sum(1).cpu()
-        pack_seq_rep = pack_padded_sequence(input=input, lengths=seq_lens, batch_first=True, enforce_sorted=False)
+        pack_seq_rep = pack_padded_sequence(
+            input=input, lengths=seq_lens, batch_first=True, enforce_sorted=False
+        )
         pack_seq_rep = self.lstm(pack_seq_rep)[0]
-        output, _ = pad_packed_sequence(sequence=pack_seq_rep, batch_first=True, total_length=max_seq_len)
+        output, _ = pad_packed_sequence(
+            sequence=pack_seq_rep, batch_first=True, total_length=max_seq_len
+        )
 
         return self.dropout_last(output)
```

### Comparing `dlk-0.0.9/dlk/core/modules/roberta.py` & `dlk-0.1.0/dlk/nn/module/bert.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,139 +1,149 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-from transformers.models.roberta.modeling_roberta import RobertaModel
-from transformers.models.roberta.configuration_roberta import RobertaConfig
 import json
-import torch
 import os
-import torch.nn as nn
 from typing import Dict
-from dlk.utils.config import BaseConfig
-from . import module_register, module_config_register, Module
 
+import torch
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
+from transformers.models.bert.configuration_bert import BertConfig
+from transformers.models.bert.modeling_bert import BertModel
+
+from dlk.utils.io import open
+from dlk.utils.register import register
+
+from . import Module
+
+
+@cregister("module", "bert")
+class BertWrapConfig:
+    """the BERT config"""
+
+    pretrained_model_path = StrField(value=MISSING, help="the pretrained model path")
+    from_pretrain = BoolField(value=True, help="whether to load the pretrained model")
+    freeze = BoolField(value=False, help="whether to freeze the model")
+    dropout = FloatField(value=0.0, minimum=0.0, maximum=1.0, help="the dropout rate")
+
+
+@register("module", "bert")
+class BertWrap(Module):
+    """Bert wrap"""
 
-@module_config_register("roberta")
-class RobertaWrapConfig(BaseConfig):
-    """Config for RobertaWrap
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "pretrained_model_path": "*@*",
-        >>>         "from_pretrain": true
-        >>>         "freeze": false,
-        >>>         "dropout": 0.0,
-        >>>     },
-        >>>     "_name": "roberta",
-        >>> }
-    """
-
-    def __init__(self, config: Dict):
-        super(RobertaWrapConfig, self).__init__(config)
-        self.pretrained_model_path = config['config']['pretrained_model_path']
-        self.from_pretrain = config['config']['from_pretrain']
-        self.freeze = config['config']['freeze']
-        self.dropout = config['config']['dropout']
-        if os.path.isdir(self.pretrained_model_path):
-            if os.path.exists(os.path.join(self.pretrained_model_path, 'config.json')):
-                self.roberta_config = RobertaConfig(**json.load(open(os.path.join(self.pretrained_model_path, 'config.json'), 'r')))
+    def __init__(self, config: BertWrapConfig):
+        super(BertWrap, self).__init__()
+        self.config = config
+        if os.path.isdir(self.config.pretrained_model_path):
+            if os.path.exists(
+                os.path.join(self.config.pretrained_model_path, "config.json")
+            ):
+                with open(
+                    os.path.join(self.config.pretrained_model_path, "config.json"), "r"
+                ) as f:
+                    self.bert_config = BertConfig(**json.load(f))
             else:
-                raise PermissionError(f"config.json must in the dir {self.pretrained_model_path}")
+                raise PermissionError(
+                    f"config.json must in the dir {self.pretrained_model_path}"
+                )
         else:
-            if os.path.isfile(self.pretrained_model_path):
+            if os.path.isfile(self.config.pretrained_model_path):
                 try:
-                    self.reberta_config = RobertaConfig(**json.load(open(self.pretrained_model_path, 'r')))
+                    with open(self.config.pretrained_model_path, "r") as f:
+                        self.bert_config = BertConfig(**json.load(f))
                 except:
-                    raise PermissionError(f"You must provide the pretrained model dir or the config file path.")
-        self.post_check(config['config'], used=['pretrained_model_path', 'from_pretrain', 'freeze', 'dropout'])
-
+                    raise PermissionError(
+                        f"You must provide the pretrained model dir or the config file path."
+                    )
 
-@module_register("roberta")
-class RobertaWrap(Module):
-    """Roberta Wrap"""
-    def __init__(self, config: RobertaWrapConfig):
-        super(RobertaWrap, self).__init__()
-        self.config = config
-
-        self.roberta = RobertaModel(config.roberta_config, add_pooling_layer=False)
+        self.bert = BertModel(self.bert_config, add_pooling_layer=True)
         self.dropout = nn.Dropout(float(self.config.dropout))
 
     def init_weight(self, method):
         """init the weight of model by 'bert.init_weight()' or from_pretrain
 
         Args:
             method: init method, no use for pretrained_transformers
 
-        Returns: 
+        Returns:
             None
 
         """
         if self.config.from_pretrain:
             self.from_pretrained()
         else:
-            self.roberta.init_weights()
+            self.bert.init_weights()
 
     def from_pretrained(self):
-        """init the model from pretrained_model_path
-        """
-        self.roberta = RobertaModel.from_pretrained(self.config.pretrained_model_path)
+        """init the model from pretrained_model_path"""
+        self.bert = BertModel.from_pretrained(self.config.pretrained_model_path)
 
-    def forward(self, inputs):
+    def forward(self, inputs: Dict):
         """do forward on a mini batch
 
         Args:
             batch: a mini batch inputs
 
-        Returns: 
+        Returns:
             sequence_output, all_hidden_states, all_self_attentions
 
         """
         if self.config.freeze:
-            self.roberta.eval()
             with torch.no_grad():
-                outputs = self.roberta(
-                    input_ids = inputs.get("input_ids", None),
-                    attention_mask = inputs.get("attention_mask", None),
-                    token_type_ids = inputs.get("token_type_ids", None),
-                    position_ids = inputs.get("position_ids", None),
-                    head_mask = inputs.get("head_mask", None),
-                    inputs_embeds = inputs.get("inputs_embeds", None),
-                    encoder_hidden_states = inputs.get("encoder_hidden_states", None),
-                    encoder_attention_mask = inputs.get("encoder_attention_mask", None),
-                    past_key_values = inputs.get("past_key_values", None),
-                    use_cache = None,
-                    output_attentions = True,
-                    output_hidden_states = True,
-                    return_dict = False
+                outputs = self.bert(
+                    input_ids=inputs.get("input_ids", None),
+                    attention_mask=inputs.get("attention_mask", None),
+                    token_type_ids=inputs.get("token_type_ids", None),
+                    position_ids=inputs.get("position_ids", None),
+                    head_mask=inputs.get("head_mask", None),
+                    inputs_embeds=inputs.get("inputs_embeds", None),
+                    encoder_hidden_states=inputs.get("encoder_hidden_states", None),
+                    encoder_attention_mask=inputs.get("encoder_attention_mask", None),
+                    past_key_values=inputs.get("past_key_values", None),
+                    use_cache=None,
+                    output_attentions=True,
+                    output_hidden_states=True,
+                    return_dict=False,
                 )
         else:
-            outputs = self.roberta(
-                input_ids = inputs.get("input_ids", None),
-                attention_mask = inputs.get("attention_mask", None),
-                token_type_ids = inputs.get("token_type_ids", None),
-                position_ids = inputs.get("position_ids", None),
-                head_mask = inputs.get("head_mask", None),
-                inputs_embeds = inputs.get("inputs_embeds", None),
-                encoder_hidden_states = inputs.get("encoder_hidden_states", None),
-                encoder_attention_mask = inputs.get("encoder_attention_mask", None),
-                past_key_values = inputs.get("past_key_values", None),
-                use_cache = None,
-                output_attentions = True,
-                output_hidden_states = True,
-                return_dict = False
+            outputs = self.bert(
+                input_ids=inputs.get("input_ids", None),
+                attention_mask=inputs.get("attention_mask", None),
+                token_type_ids=inputs.get("token_type_ids", None),
+                position_ids=inputs.get("position_ids", None),
+                head_mask=inputs.get("head_mask", None),
+                inputs_embeds=inputs.get("inputs_embeds", None),
+                encoder_hidden_states=inputs.get("encoder_hidden_states", None),
+                encoder_attention_mask=inputs.get("encoder_attention_mask", None),
+                past_key_values=inputs.get("past_key_values", None),
+                use_cache=None,
+                output_attentions=True,
+                output_hidden_states=True,
+                return_dict=False,
             )
-        assert len(outputs) == 4, f"Please check transformers version, the len(outputs) is 4 in version == 4.12, or check your config and remove the 'add_cross_attention'"
-        sequence_output, all_hidden_states, all_self_attentions = outputs[0], outputs[2], outputs[3]
+        assert (
+            len(outputs) == 4
+        ), f"Please check transformers version, the len(outputs) is 4 in version == 4.12|4.15, or check your config and remove the 'add_cross_attention'"
+        sequence_output, all_hidden_states, all_self_attentions = (
+            outputs[0],
+            outputs[2],
+            outputs[3],
+        )
         sequence_output = self.dropout(sequence_output)
         return sequence_output, all_hidden_states, all_self_attentions
```

### Comparing `dlk-0.0.9/dlk/core/optimizers/__init__.py` & `dlk-0.1.0/dlk/optimizer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,148 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-"""optimizers"""
-import importlib
+import logging
 import os
-from typing import Callable, Dict, Tuple, Any
-from dlk.utils.register import Register
-import torch.optim as optim
-from dlk.utils.logger import Logger
-import torch
 import re
+from typing import Any, Callable, Dict, Tuple, Type
 
-
-logger = Logger.get_logger()
-optimizer_config_register = Register("Optimizer config register.")
-optimizer_register = Register("Optimizer register.")
+import torch
+import torch.optim as optim
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    dataclass,
+)
+
+from dlk.utils.import_module import import_module_dir
+
+logger = logging.getLogger(__name__)
+
+
+@dataclass
+class BaseOptimizerConfig(Base):
+    """the base optimizer"""
+
+    name = StrField(value="default", help="the name of default group parameters")
+    optimizer_special_groups = DictField(
+        value={},
+        suggestions=[
+            {
+                "order": ["decoder", "bias"],
+                "bias": {
+                    "config": {"weight_decay": 0},
+                    "pattern": ["bias", "LayerNorm.bias", "LayerNorm.weight"],
+                },
+                "decoder": {"config": {"lr": 1e-3}, "pattern": ["decoder"]},
+            }
+        ],
+        help="""the special groups of optimizer, like
+             "order": ['decoder', 'bias'], // the group order, if the para is in decoder & is in bias, set to decoder. The order name is set to the group name
+             "bias": {
+                 "config": { "weight_decay": 0 },
+                 "pattern": ["bias",  "LayerNorm.bias", "LayerNorm.weight"]
+             },
+             "decoder": {
+                 "config": { "lr": 1e-3 },
+                 "pattern": ["decoder"]
+             }""",
+    )
 
 
 class BaseOptimizer(object):
+    def __init__(
+        self,
+        model: torch.nn.Module,
+        config: BaseOptimizerConfig,
+        optimizer: Type[optim.Optimizer],
+    ):
+        super(BaseOptimizer, self).__init__()
+        self.config = config
+        self.model = model
+        self.optimizer = optimizer
 
-    def get_optimizer(self)->optim.Optimizer:
+    def get_optimizer(self) -> optim.Optimizer:
         """return the initialized optimizer
 
-        Returns: 
+        Returns:
             Optimizer
 
         """
-        raise NotADirectoryError
+        return self.init_optimizer(self.optimizer, self.model, self.config)
 
-    def init_optimizer(self, optimizer: optim.Optimizer, model: torch.nn.Module, config: Dict):
+    def init_optimizer(
+        self,
+        optimizer: Type[optim.Optimizer],
+        model: torch.nn.Module,
+        config: BaseOptimizerConfig,
+    ) -> optim.Optimizer:
         """init the optimizer for paras in model, and the group is decided by config
 
         Args:
             optimizer: adamw, sgd, etc.
             model: pytorch model
             config: which decided the para group, lr, etc.
 
-        Returns: 
+        Returns:
             the initialized optimizer
 
         """
-        optimizer_special_groups = config.pop('optimizer_special_groups', {})
+        optimizer_special_groups = config.optimizer_special_groups
         params = []
         all_named_parameters = list(model.named_parameters())
         total_all_named_parameters = len(all_named_parameters)
         logger.info(f"All Named Params Num is {len(all_named_parameters)}")
         has_grouped_params = set()
-        for special_group_name in optimizer_special_groups.get('order', []):
-
-            group_config = optimizer_special_groups[special_group_name]['config']
-            group_patterns = optimizer_special_groups[special_group_name]['pattern']
+        for special_group_name in optimizer_special_groups.get("order", []):
+            group_config = optimizer_special_groups[special_group_name]["config"]
+            group_patterns = optimizer_special_groups[special_group_name]["pattern"]
             # convert to regex
             combine_patterns = []
             for pattern in group_patterns:
                 combine_patterns.append(f"({pattern})")
             cc_patterns = re.compile("|".join(combine_patterns))
             group_param = []
-            for n, p  in all_named_parameters:
+            for n, p in all_named_parameters:
                 # logger.info(f"Param name {n}")
                 if n in has_grouped_params:
                     continue
-                if cc_patterns.search(n): # use regex
+                if cc_patterns.search(n):  # use regex
                     has_grouped_params.add(n)
                     group_param.append(p)
-            group_config['params'] = group_param
-            group_config['name'] = special_group_name
+            group_config["params"] = group_param
+            group_config["name"] = special_group_name
             params.append(group_config)
 
-        reserve_params = [p for n, p in all_named_parameters if not n in has_grouped_params]
-        params.append({"params": reserve_params, "name": config.pop('name')})
+        reserve_params = [
+            p for n, p in all_named_parameters if not n in has_grouped_params
+        ]
+        params.append({"params": reserve_params, "name": config.name})
         logger.info(f"Param Group Nums {len(params)}")
         total_param = 0
         for group in params:
-            total_param = total_param + len(group['params'])
+            total_param = total_param + len(group["params"])
         assert total_param == total_all_named_parameters
+        opt_args = config._to_dict(only_para=True)
+        opt_args.pop("name")
+        opt_args.pop("optimizer_special_groups")
 
-        return optimizer(params=params, **config)
+        return optimizer(params=params, **opt_args)
 
     def __call__(self):
-        """the same as self.get_optimizer()
-        """
+        """the same as self.get_optimizer()"""
         return self.get_optimizer()
 
 
-def import_optimizers(optimizers_dir, namespace):
-    for file in os.listdir(optimizers_dir):
-        path = os.path.join(optimizers_dir, file)
-        if (
-            not file.startswith("_")
-            and not file.startswith(".")
-            and (file.endswith(".py") or os.path.isdir(path))
-        ):
-            optimizer_name = file[: file.find(".py")] if file.endswith(".py") else file
-            importlib.import_module(namespace + "." + optimizer_name)
-
-
-# automatically import any Python files in the optimizers directory
-optimizers_dir = os.path.dirname(__file__)
-import_optimizers(optimizers_dir, "dlk.core.optimizers")
+optimizer_dir = os.path.dirname(__file__)
+import_module_dir(optimizer_dir, "dlk.optimizer")
```

### Comparing `dlk-0.0.9/dlk/core/schedulers/constant_warmup.py` & `dlk-0.1.0/dlk/scheduler/constant_warmup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,55 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
 from typing import Dict
-from dlk.utils.config import BaseConfig
-from . import scheduler_register, scheduler_config_register, BaseScheduler
-from torch.optim.lr_scheduler import LambdaLR
+
 import torch.optim as optim
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+from torch.optim.lr_scheduler import LambdaLR
+
+from dlk.utils.register import register
+
+from . import BaseScheduler, BaseSchedulerConfig
 
 
-@scheduler_config_register("constant_warmup")
-class ConstantWarmupScheduleConfig(BaseConfig):
-    """Config for ConstantWarmupSchedule
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "last_epoch": -1,
-        >>>         "num_warmup_steps": 0,
-        >>>     },
-        >>>     "_name": "constant_warmup",
-        >>> }
-    """
-    def __init__(self, config: Dict):
-        super(ConstantWarmupScheduleConfig, self).__init__(config)
-        config = config['config']
-        self.last_epoch = config["last_epoch"]
-        self.num_warmup_steps = config["num_warmup_steps"]
-        self.post_check(config, used=[
-            "last_epoch",
-            "num_warmup_steps",
-        ])
+@cregister("scheduler", "constant_warmup")
+class ConstantWarmupScheduleConfig(BaseSchedulerConfig):
+    """the constant scheduler begin with a warmup"""
 
 
-@scheduler_register("constant_warmup")
+@register("scheduler", "constant_warmup")
 class ConstantWarmupSchedule(BaseScheduler):
     """ConstantWarmupSchedule"""
-    def __init__(self, optimizer: optim.Optimizer, config: ConstantWarmupScheduleConfig):
-        super(ConstantWarmupSchedule, self).__init__()
-        self.config = config
-        self.optimizer = optimizer
-
-    def get_scheduler(self)->LambdaLR:
-        """return the initialized linear wramup then constant scheduler
-
-        Returns: 
-            Schedule
-
-        """
-        num_warmup_steps = self.config.num_warmup_steps
-        last_epoch = self.config.last_epoch
-
-        def lr_lambda(current_step: int):
-            if current_step < num_warmup_steps:
-                return float(current_step) / float(max(1.0, num_warmup_steps))
-            return 1.0
 
-        return LambdaLR(self.optimizer, lr_lambda, last_epoch=last_epoch)
+    def __init__(
+        self,
+        optimizer: optim.Optimizer,
+        config: ConstantWarmupScheduleConfig,
+        rt_config: Dict,
+    ):
+        super(ConstantWarmupSchedule, self).__init__(optimizer, config, rt_config)
+
+    def step_update(self, current_step: int):
+        if current_step < self.config.num_warmup_steps:
+            return float(current_step) / float(max(1.0, self.config.num_warmup_steps))
+        return 1.0
+
+    def epoch_update(self, current_epoch: int):
+        if current_epoch < self.config.num_warmup_steps:
+            return float(current_epoch) / float(max(1.0, self.config.num_warmup_steps))
+        return 1.0
```

### Comparing `dlk-0.0.9/dlk/core/schedulers/linear_warmup.py` & `dlk-0.1.0/dlk/scheduler/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,112 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
+import os
 from typing import Dict
-from dlk.utils.config import BaseConfig
-from . import scheduler_register, scheduler_config_register, BaseScheduler
+
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    dataclass,
+)
+from torch.optim import Optimizer
 from torch.optim.lr_scheduler import LambdaLR
-from dlk.utils.logger import Logger
-import torch.optim as optim
-logger = Logger.get_logger()
-
-
-@scheduler_config_register("linear_warmup")
-class LinearWarmupScheduleConfig(BaseConfig):
-    """
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "last_epoch": -1,
-        >>>         "num_warmup_steps": 0,
-        >>>         "num_training_steps": -1,
-        >>>     },
-        >>>     "_name": "linear_warmup",
-        >>> }
-    """
-    def __init__(self, config: Dict):
-        super(LinearWarmupScheduleConfig, self).__init__(config)
-        config = config['config']
-        self.last_epoch = config["last_epoch"]
-        self.num_warmup_steps = config["num_warmup_steps"]
-        self.num_training_steps = config["num_training_steps"]
-        self.post_check(config, used=[
-            "last_epoch",
-            "num_warmup_steps",
-            "num_training_steps",
-        ])
-
-
-@scheduler_register("linear_warmup")
-class LinearWarmupSchedule(BaseScheduler):
-    """linear warmup then linear decay"""
-    def __init__(self, optimizer: optim.Optimizer, config: LinearWarmupScheduleConfig):
-        super(LinearWarmupSchedule, self).__init__()
+
+from dlk.utils.import_module import import_module_dir
+
+
+@dataclass
+class BaseSchedulerConfig(Base):
+    """the base scheduler"""
+
+    num_warmup_steps = FloatField(
+        value=0.1,
+        minimum=0.0,
+        help="""
+            only for the scheduler with warmup.
+            for the interval is `step`,
+            the number of warmup steps,
+            it can be float or int, 
+            if it's between 0.0-1.0, means the percentage of total steps,
+            if it's larger than 1, means the number of steps.
+            If the interval is `epoch`,
+            it means the number of warmup epochs
+        """,
+    )
+    last_epoch = IntField(value=-1, minimum=-1, help="the last epoch/step")
+    interval = StrField(
+        value="step", options=["epoch", "step"], help="the interval of scheduler"
+    )
+
+
+class BaseScheduler(object):
+    """interface for Schedule"""
+
+    def __init__(
+        self, optimizer: Optimizer, config: BaseSchedulerConfig, rt_config: Dict
+    ):
+        """update dynamic parameters in self.config based the rt_config
+        Args:
+            rt_config: provide the current training status
+                >>> {
+                >>>     "num_training_steps": self.num_training_steps,
+                >>>     "num_training_epochs": self.num_training_epochs
+                >>> }
+        Returns: None
+        """
+        super(BaseScheduler, self).__init__()
         self.config = config
         self.optimizer = optimizer
+        self.num_training_steps = rt_config["num_training_steps"]
+        self.num_training_epochs = rt_config["num_training_epochs"]
+        if self.config.num_warmup_steps < 1:
+            if self.config.interval == "step":
+                self.config.num_warmup_steps = int(
+                    self.config.num_warmup_steps * self.num_training_steps
+                )
+            else:
+                assert self.config.interval == "epoch"
+                self.config.num_warmup_steps = int(
+                    self.config.num_warmup_steps * self.num_training_epochs
+                )
 
-    def get_scheduler(self)->LambdaLR:
-        """return the initialized linear wramup then linear decay scheduler
+    def get_scheduler(self) -> LambdaLR:
+        """return the initialized scheduler
 
-        Returns: 
+        Returns:
             Schedule
-
         """
-        num_training_steps = self.config.num_training_steps
-        num_warmup_steps = self.config.num_warmup_steps
-        if num_warmup_steps >0 and num_warmup_steps < 1:
-            num_warmup_steps = int(num_warmup_steps * num_training_steps)
-        last_epoch = self.config.last_epoch
-        logger.warning(f"The calculated Total Traning Num is {num_training_steps}, the Num Warmup Steps is {num_warmup_steps}. Please check it carefully.")
-
-        def lr_lambda(current_step: int):
-            if current_step < num_warmup_steps:
-                return float(current_step) / float(max(1, num_warmup_steps))
-            return max(
-                0.0, float(num_training_steps - current_step) / float(max(1, num_training_steps - num_warmup_steps))
+        if self.config.interval == "step":
+            return LambdaLR(
+                self.optimizer, self.step_update, last_epoch=self.config.last_epoch
+            )
+        else:
+            assert self.config.interval == "epoch"
+            return LambdaLR(
+                self.optimizer, self.epoch_update, last_epoch=self.config.last_epoch
             )
 
-        return LambdaLR(self.optimizer, lr_lambda, last_epoch)
+    def step_update(self, current_step: int):
+        raise NotImplementedError
+
+    def epoch_update(self, current_epoch: int):
+        raise NotImplementedError
+
+    def __call__(self):
+        """the same as self.get_scheduler()"""
+        return self.get_scheduler()
+
+
+scheduler_dir = os.path.dirname(__file__)
+import_module_dir(scheduler_dir, "dlk.scheduler")
```

### Comparing `dlk-0.0.9/dlk/core/schedulers/multi_group_schedule.py` & `dlk-0.1.0/dlk/scheduler/multi_group_schedule.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,66 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
 # TODO: WIP Comming soon
 # from typing import Dict
 # import torch.nn as nn
 # from . import scheduler_register, scheduler_config_register, BaseScheduler
 # from torch.optim.lr_scheduler import LambdaLR
 # import torch.optim as optim
 # import copy
 
 # # constant
 
 # # cos warmup
 # # def lr_lambda(current_step):
-    # # if current_step < num_warmup_steps:
-        # # return float(current_step) / float(max(1, num_warmup_steps))
-    # # progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
-    # # return max(0.0, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
+# # if current_step < num_warmup_steps:
+# # return float(current_step) / float(max(1, num_warmup_steps))
+# # progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
+# # return max(0.0, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
 
 
 # # constant warmup
 # # def lr_lambda(current_step: int):
-    # # if current_step < num_warmup_steps:
-        # # return float(current_step) / float(max(1.0, num_warmup_steps))
-    # # return 1.0
+# # if current_step < num_warmup_steps:
+# # return float(current_step) / float(max(1.0, num_warmup_steps))
+# # return 1.0
 
 
 # # linear warmup
 # # def lr_lambda(current_step: int):
-    # # if current_step < num_warmup_steps:
-        # # return float(current_step) / float(max(1, num_warmup_steps))
-    # # return max(
-        # # 0.0, float(num_training_steps - current_step) / float(max(1, num_training_steps - num_warmup_steps))
+# # if current_step < num_warmup_steps:
+# # return float(current_step) / float(max(1, num_warmup_steps))
+# # return max(
+# # 0.0, float(num_training_steps - current_step) / float(max(1, num_training_steps - num_warmup_steps))
 
 
 # @scheduler_config_register("constant")
 # class ConstantScheduleConfig(object):
-    # """
-    # {
-        # config: {
-            # "last_epoch": -1
-        # },
-        # _name: "constant",
-    # }
-    # """
-    # def __init__(self, config: Dict):
-        # super(ConstantScheduleConfig, self).__init__()
-        # config = config['config']
-        # self.last_epoch = config["last_epoch"]
+# """
+# {
+# config: {
+# "last_epoch": -1
+# },
+# _name: "constant",
+# }
+# """
+# def __init__(self, config: Dict):
+# super(ConstantScheduleConfig, self).__init__()
+# config = config['config']
+# self.last_epoch = config["last_epoch"]
 
 
 # @scheduler_register("constant")
 # class ConstantSchedule(BaseScheduler):
-    # def __init__(self, optimizer: optim.Optimizer, config: ConstantScheduleConfig):
-        # super(ConstantSchedule, self).__init__()
-        # self.config = config
-        # self.optimizer = optimizer
-
-    # def get_scheduler(self):
-        # """TODO: Docstring for get_scheduler.
-        # :returns: TODO
-        # """
-        # return LambdaLR(self.optimizer, lambda _: 1, last_epoch=self.config.last_epoch)
+# def __init__(self, optimizer: optim.Optimizer, config: ConstantScheduleConfig):
+# super(ConstantSchedule, self).__init__()
+# self.config = config
+# self.optimizer = optimizer
+
+# def get_scheduler(self):
+# """TODO: Docstring for get_scheduler.
+# :returns: TODO
+# """
+# return LambdaLR(self.optimizer, lambda _: 1, last_epoch=self.config.last_epoch)
```

### Comparing `dlk-0.0.9/dlk/core/schedulers/rec_decay.py` & `dlk-0.1.0/dlk/nn/loss/mse.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,67 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from typing import Dict
-from dlk.utils.config import BaseConfig
-from . import scheduler_register, scheduler_config_register, BaseScheduler
-from torch.optim.lr_scheduler import LambdaLR
-from dlk.utils.logger import Logger
-import torch.optim as optim
-logger = Logger.get_logger()
-
-
-@scheduler_config_register("rec_decay")
-class RecDecayScheduleConfig(BaseConfig):
-    """Config for RecDecaySchedule
-
-    Config Example:
-        >>> {
-        >>>     "config": {
-        >>>         "last_epoch": -1,
-        >>>         "num_training_steps": -1,
-        >>>         "decay": 0.05,
-        >>>         "epoch_training_steps": -1,
-        >>>     },
-        >>>     "_name": "rec_decay",
-        >>> }
-
-    the lr=lr*1/(1+decay)
-    """
-    def __init__(self, config: Dict):
-        super(RecDecayScheduleConfig, self).__init__(config)
-        config = config['config']
-        self.last_epoch = config["last_epoch"]
-        self.epoch_training_steps = config["epoch_training_steps"]
-        self.decay = config["decay"]
-        self.num_training_steps = config["num_training_steps"]
-        self.post_check(config, used=[
-            "last_epoch",
-            "num_training_steps",
-            "decay",
-            "epoch_training_steps",
-        ])
-
-
-@scheduler_register("rec_decay")
-class RecDecaySchedule(BaseScheduler):
-    """lr=lr*1/(1+decay)
-    """
-    def __init__(self, optimizer: optim.Optimizer, config: RecDecayScheduleConfig):
-        super(RecDecaySchedule, self).__init__()
-        self.config = config
-        self.optimizer = optimizer
-
-    def get_scheduler(self):
-        """return the initialized rec_decay scheduler
-
-        lr=lr*1/(1+decay)
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-        Returns: 
-            Schedule
+import torch.nn as nn
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
+
+from . import BaseLoss, BaseLossConfig
+
+
+@cregister("loss", "mse")
+class MSELossConfig(BaseLossConfig):
+    """the MEAN SQUARE ERROR loss(MSE AKA L2 loss)"""
+
+    pass
+
+
+@register("loss", "mse")
+class MSELoss(BaseLoss):
+    """mse loss for regression, distill, etc."""
+
+    def __init__(self, config: MSELossConfig):
+        super(MSELoss, self).__init__(config)
+        self.config: MSELossConfig
+        self.mse = nn.MSELoss(
+            reduction=self.config.reduction
+        )  # we will use masked_select, and apply reduction=batchmean (sum/batch_size)
+
+    def _calc(self, result, inputs, rt_config, scale):
+        """calc the loss the predict is from result, the ground truth is from inputs
+
+        Args:
+            result: the model predict dict
+            inputs: the all inputs for model
+            rt_config: provide the current training status
+                >>> {
+                >>>     "current_step": self.global_step,
+                >>>     "current_epoch": self.current_epoch,
+                >>>     "total_steps": self.num_training_steps,
+                >>>     "total_epochs": self.num_training_epochs
+                >>> }
+            scale: the scale rate for current stage
+        Returns:
+            loss
 
         """
-        num_training_steps = self.config.num_training_steps
-        epoch_training_steps = self.config.epoch_training_steps
-        decay = self.config.decay
-        last_epoch = self.config.last_epoch
-        logger.warning(f"The calculated Total Traning Num is {num_training_steps}, the Epoch training Steps is {epoch_training_steps}. Please check it carefully.")
-
-        def lr_lambda(current_step: int):
-            cur_epoch = (current_step+1)//epoch_training_steps if epoch_training_steps!=0 else 0
-            # return 1/(1+decay*cur_epoch)
-            return 1/((1+decay)**cur_epoch)
-        return LambdaLR(self.optimizer, lr_lambda, last_epoch)
+        pred = result[self.pred_name]
+        target = inputs[self.truth_name]
+        batch_size = target.shape[0]
+        loss = self.mse(pred, target) * scale / batch_size  # batch mean
+        return loss, {self.config.log_map.loss: loss}
```

### Comparing `dlk-0.0.9/dlk/data/postprocessors/__init__.py` & `dlk-0.1.0/dlk/data/postprocessor/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,144 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""postprocessors"""
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
+import abc
 import importlib
+import json
 import os
-from typing import Callable, Dict, Type, List, Union
-from dlk.utils.register import Register
-from dlk.utils.config import BaseConfig
-import torch
-import pandas as pd
-import abc
-
-class IPostProcessorConfig(BaseConfig):
-    """docstring for PostProcessorConfigBase"""
-    def __init__(self, config):
-        super(IPostProcessorConfig, self).__init__(config)
-        self.config = config.get('config', {})
-
-    @property
-    def predict_extend_return(self):
-        """save the extend data in predict
-
-        Returns: 
-            predict_extend_return
-        """
-        return self.config.get('predict_extend_return', {})
-
-    @property
-    def input_map(self):
-        """required the output of model process content name map
+from typing import Callable, Dict, List, Type, TypeVar, Union
 
-        Returns: 
-            input_map
-        """
-        return self.config.get("input_map", {})
-
-    @property
-    def origin_input_map(self):
-        """required the origin data(before pass to datamodule) column name map
+import pandas as pd
+import pyarrow.parquet as pq
+import torch
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    dataclass,
+)
+
+from dlk.utils.import_module import import_module_dir
+
+
+@dataclass
+class BasePostProcessorConfig(Base):
+    """the base postprocessor"""
+
+    meta_dir = StrField(
+        value="data/meta_data",
+        help="the save dir of the meta info",
+    )
+    save_root_path = StrField(
+        value="data",
+        help="the root path of the save data, default relative to the current path",
+    )
+    save_dir = DictField(
+        value={"valid": "valid_output", "test": "test_output"},
+        help="the save path of the data, relative to the save_root_path",
+    )
+    start_save_step = IntField(
+        value=0, minimum=-1, help="the start save step, -1 means the last step"
+    )
+    start_save_epoch = IntField(
+        value=-1, minimum=-1, help="the start save epoch, -1 means the last epoch"
+    )
+    predict_extend_return = DictField(value={}, help="the extend return of predict")
 
-        Returns: 
-            origin_input_map
-        """
-        return self.config.get("origin_input_map", {})
 
+class BasePostProcessor(object):
+    """the base postprocessor"""
 
-class IPostProcessor(metaclass=abc.ABCMeta):
-    """docstring for IPostProcessor"""
+    def __init__(self, config):
+        super(BasePostProcessor, self).__init__()
 
-    def loss_name_map(self, stage)->str:
+    def loss_name_map(self, stage) -> str:
         """get the stage loss name
 
         Args:
             stage: valid, train or test
 
-        Returns: 
+        Returns:
             loss_name
 
         """
         map = {
-            "valid": 'val',
-            'train': 'train',
+            "valid": "val",
+            "train": "train",
             "test": "test",
         }
         return map.get(stage, stage)
 
-    def gather_predict_extend_data(self, input_data: Dict, i: int, predict_extend_return: Dict):
+    def gather_predict_extend_data(
+        self, input_data: Dict, i: int, predict_extend_return: Dict
+    ):
         """gather the data register in `predict_extend_return`
         Args:
             input_data:
                 the model output
             i:
                 the index is i
-            predict_extend_return: 
+            predict_extend_return:
                 the name map which will be reserved
-        Returns: 
+        Returns:
             a dict of data in input_data which is register in predict_extend_return
         """
         result = {}
         for key, name in predict_extend_return.items():
             data = input_data[name][i]
             if torch.is_tensor(data):
                 data = data.detach().tolist()
             result[key] = data
         return result
 
-    def average_loss(self, list_batch_outputs: List[Dict])->float:
+    def average_loss(self, list_batch_outputs: List[Dict]) -> Dict[str, float]:
         """average all the loss of the list_batches
 
         Args:
             list_batch_outputs: a list of outputs
 
-        Returns: 
+        Returns:
             average_loss
 
         """
-        sum_loss = 0
+        loss_names = []
+        average_losses = {}
+        batch_num = len(list_batch_outputs)
+        if not batch_num:
+            return average_losses
+        for key in list_batch_outputs[0]:
+            if key.endswith("_loss") or key == "loss":
+                loss_names.append(key)
+                average_losses[key] = 0
         for batch_output in list_batch_outputs:
-            sum_loss += batch_output.get('loss', 0)
-        return sum_loss / len(list_batch_outputs)
+            for name in loss_names:
+                average_losses[name] = average_losses[name] + batch_output.get(name, 0)
+        average_losses = {
+            key: value / batch_num for key, value in average_losses.items()
+        }
+        return average_losses
 
     @abc.abstractmethod
-    def do_predict(self, stage: str, list_batch_outputs: List[Dict], origin_data: pd.DataFrame, rt_config: Dict)->List:
+    def do_predict(
+        self,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+    ) -> List:
         """Process the model predict to human readable format
 
         Args:
             stage: train/test/etc.
             list_batch_outputs: a list of outputs
             origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
             rt_config:
@@ -125,47 +146,62 @@
                 >>> {
                 >>>     "current_step": self.global_step,
                 >>>     "current_epoch": self.current_epoch,
                 >>>     "total_steps": self.num_training_steps,
                 >>>     "total_epochs": self.num_training_epochs
                 >>> }
 
-        Returns: 
+        Returns:
             all predicts
 
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def do_calc_metrics(self, predicts: List, stage: str, list_batch_outputs: List[Dict], origin_data: pd.DataFrame, rt_config: Dict)->Dict:
+    def do_calc_metrics(
+        self,
+        predicts: List,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+    ) -> Dict:
         """calc the scores use the predicts or list_batch_outputs
 
         Args:
             predicts: list of predicts
             stage: train/test/etc.
             list_batch_outputs: a list of outputs
             origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
             rt_config:
-                >>> 
+                >>>
                 >>> current status
                 >>> {
                 >>>     "current_step": self.global_step,
                 >>>     "current_epoch": self.current_epoch,
                 >>>     "total_steps": self.num_training_steps,
                 >>>     "total_epochs": self.num_training_epochs
                 >>> }
 
-        Returns: 
+        Returns:
             the named scores
 
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def do_save(self, predicts: List, stage: str, list_batch_outputs: List[Dict], origin_data: pd.DataFrame, rt_config: Dict, save_condition: bool=False):
+    def do_save(
+        self,
+        predicts: List,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+        save_condition: bool = False,
+    ):
         """save the predict when save_condition==True
 
         Args:
             predicts: list of predicts
             stage: train/test/etc.
             list_batch_outputs: a list of outputs
             origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
@@ -175,31 +211,38 @@
                 >>>     "current_step": self.global_step,
                 >>>     "current_epoch": self.current_epoch,
                 >>>     "total_steps": self.num_training_steps,
                 >>>     "total_epochs": self.num_training_epochs
                 >>> }
             save_condition: True for save, False for depend on rt_config
 
-        Returns: 
+        Returns:
             None
 
         """
         raise NotImplementedError
 
     @property
-    def without_ground_truth_stage(self)->set:
+    def without_ground_truth_stage(self) -> set:
         """there is not groud truth in the returned stage
 
-        Returns: 
+        Returns:
             without_ground_truth_stage
 
         """
-        return {'predict', 'online'}
+        return {"predict", "online"}
 
-    def process(self, stage: str, list_batch_outputs: List[Dict], origin_data: pd.DataFrame, rt_config: Dict, save_condition: bool=False)->Union[Dict, List]:
+    def process(
+        self,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+        save_condition: bool = False,
+    ) -> Union[Dict, List]:
         """PostProcess entry
 
         Args:
             stage: train/test/etc.
             list_batch_outputs: a list of outputs
             origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
             rt_config:
@@ -208,57 +251,69 @@
                 >>>     "current_step": self.global_step,
                 >>>     "current_epoch": self.current_epoch,
                 >>>     "total_steps": self.num_training_steps,
                 >>>     "total_epochs": self.num_training_epochs
                 >>> }
             save_condition: if save_condition is True, will force save the predict on all stage except online
 
-        Returns: 
+        Returns:
             the log_info(metrics) or the stage is "online" return the predicts
 
         """
         log_info = {}
         if stage not in self.without_ground_truth_stage:
             average_loss = self.average_loss(list_batch_outputs=list_batch_outputs)
-            log_info[f'{self.loss_name_map(stage)}_loss'] = average_loss
+            for name in average_loss:
+                log_info[f"{self.loss_name_map(stage)}_{name}"] = average_loss[name]
         predicts = self.do_predict(stage, list_batch_outputs, origin_data, rt_config)
         if stage not in self.without_ground_truth_stage:
-            log_info.update(self.do_calc_metrics(predicts, stage, list_batch_outputs, origin_data, rt_config))
-        if stage == 'online':
+            log_info.update(
+                self.do_calc_metrics(
+                    predicts, stage, list_batch_outputs, origin_data, rt_config
+                )
+            )
+
+        if stage == "online":
             return predicts
-        if stage == 'predict':
+        if stage == "predict":
             if save_condition:
-                self.do_save(predicts, stage, list_batch_outputs, origin_data, rt_config, save_condition=True)
+                self.do_save(
+                    predicts,
+                    stage,
+                    list_batch_outputs,
+                    origin_data,
+                    rt_config,
+                    save_condition=True,
+                )
             return predicts
         else:
             if save_condition:
-                self.do_save(predicts, stage, list_batch_outputs, origin_data, rt_config, save_condition=True)
+                self.do_save(
+                    predicts,
+                    stage,
+                    list_batch_outputs,
+                    origin_data,
+                    rt_config,
+                    save_condition=True,
+                )
             else:
-                self.do_save(predicts, stage, list_batch_outputs, origin_data, rt_config, save_condition=False)
+                self.do_save(
+                    predicts,
+                    stage,
+                    list_batch_outputs,
+                    origin_data,
+                    rt_config,
+                    save_condition=False,
+                )
             return log_info
 
-    def __call__(self, stage, list_batch_outputs, origin_data, rt_config, save_condition=False):
-        """the same as self.process
-        """
-        return self.process(stage, list_batch_outputs, origin_data, rt_config, save_condition)
-
-
-postprocessor_config_register = Register('PostProcessor config register')
-postprocessor_register = Register("PostProcessor register")
-
-
-def import_postprocessors(postprocessors_dir, namespace):
-    for file in os.listdir(postprocessors_dir):
-        path = os.path.join(postprocessors_dir, file)
-        if (
-            not file.startswith("_")
-            and not file.startswith(".")
-            # and not (file.endswith("subpostprocessors") and os.path.isdir(path))
-            and (file.endswith(".py") or os.path.isdir(path))
-        ):
-            postprocessor_name = file[: file.find(".py")] if file.endswith(".py") else file
-            importlib.import_module(namespace + "." + postprocessor_name)
+    def __call__(
+        self, stage, list_batch_outputs, origin_data, rt_config, save_condition=False
+    ):
+        """the same as self.process"""
+        return self.process(
+            stage, list_batch_outputs, origin_data, rt_config, save_condition
+        )
 
 
-# automatically import any Python files in the models directory
-postprocessors_dir = os.path.dirname(__file__)
-import_postprocessors(postprocessors_dir, "dlk.data.postprocessors")
+postprocessor_dir = os.path.dirname(__file__)
+import_module_dir(postprocessor_dir, "dlk.data.postprocessor")
```

### Comparing `dlk-0.0.9/dlk/data/postprocessors/seq_lab.py` & `dlk-0.1.0/dlk/data/postprocessor/seq_lab.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,204 +1,183 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright cstsunfu.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-import pickle as pkl
 import json
-from typing import Dict, List, Optional, Tuple, Union
+import logging
 import os
+import pickle as pkl
+from typing import Dict, List, Optional, Tuple, Union
+
 import numpy as np
 import pandas as pd
 import torch
-from typing import Dict
-from dlk.data.postprocessors import postprocessor_register, postprocessor_config_register, IPostProcessor, IPostProcessorConfig
-from dlk.utils.logger import Logger
-from dlk.utils.vocab import Vocabulary
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
 from tokenizers import Tokenizer
-import torchmetrics
-logger = Logger.get_logger()
 
+from dlk.data.postprocessor import BasePostProcessor, BasePostProcessorConfig
+from dlk.utils.io import open
+from dlk.utils.register import register
+from dlk.utils.vocab import Vocabulary
 
-@postprocessor_config_register('seq_lab')
-class SeqLabPostProcessorConfig(IPostProcessorConfig):
-    """Config for SeqLabPostProcessor
-
-    Config Example:
-        >>> {
-        >>>     "_name": "seq_lab",
-        >>>     "config": {
-        >>>         "meta": "*@*",
-        >>>         "use_crf": false, //use or not use crf
-        >>>         "word_ready": false, //already gather the subword first token as the word rep or not
-        >>>         "ignore_position": true, // calc the metrics, whether ignore the ground_truth and predict position info.( if set to true, only focus on the entity content not position.)
-        >>>         "ignore_char": " ", // if the entity begin or end with this char, will ignore these char
-        >>>         //"ignore_char": " ()[]-.,:", // if the entity begin or end with this char, will ignore these char
-        >>>         "meta_data": {
-        >>>             "label_vocab": 'label_vocab',
-        >>>             "tokenizer": "tokenizer",
-        >>>         },
-        >>>         "input_map": {
-        >>>             "logits": "logits",
-        >>>             "predict_seq_label": "predict_seq_label",
-        >>>             "_index": "_index",
-        >>>         },
-        >>>         "origin_input_map": {
-        >>>             "uuid": "uuid",
-        >>>             "sentence": "sentence",
-        >>>             "input_ids": "input_ids",
-        >>>             "entities_info": "entities_info",
-        >>>             "offsets": "offsets",
-        >>>             "special_tokens_mask": "special_tokens_mask",
-        >>>             "word_ids": "word_ids",
-        >>>             "label_ids": "label_ids",
-        >>>         },
-        >>>         "save_root_path": ".",  //save data root dir
-        >>>         "save_path": {
-        >>>             "valid": "valid",  // relative dir for valid stage
-        >>>             "test": "test",    // relative dir for test stage
-        >>>         },
-        >>>         "start_save_step": 0,  // -1 means the last
-        >>>         "start_save_epoch": -1,
-        >>>         "aggregation_strategy": "max", // AggregationStrategy item
-        >>>         "ignore_labels": ['O', 'X', 'S', "E"], // Out, Out, Start, End
-        >>>     }
-        >>> }
-    """
-
-    def __init__(self, config: Dict):
-        super(SeqLabPostProcessorConfig, self).__init__(config)
-
-        self.use_crf = self.config['use_crf']
-        self.word_ready = self.config['word_ready']
-        self.aggregation_strategy = self.config['aggregation_strategy']
-        self.ignore_labels = set(self.config['ignore_labels'])
-        self.ignore_char = set(self.config['ignore_char'])
-        self.ignore_position = self.config['ignore_position']
-
-        self.sentence = self.origin_input_map['sentence']
-        self.offsets = self.origin_input_map['offsets']
-        self.entities_info = self.origin_input_map['entities_info']
-        self.uuid = self.origin_input_map['uuid']
-        self.word_ids = self.origin_input_map['word_ids']
-        self.special_tokens_mask = self.origin_input_map['special_tokens_mask']
-        self.input_ids = self.origin_input_map['input_ids']
-        self.label_ids = self.origin_input_map['label_ids']
-
-        self.logits = self.input_map['logits']
-        self.predict_seq_label = self.input_map['predict_seq_label']
-        self._index = self.input_map['_index']
+logger = logging.getLogger(__name__)
 
-        if isinstance(self.config['meta'], str):
-            meta = pkl.load(open(self.config['meta'], 'rb'))
-        else:
-            raise PermissionError("You must provide meta data(vocab & tokenizer) for ner postprocess.")
 
-        vocab_trace_path = []
-        vocab_trace_path_str = self.config['meta_data']['label_vocab']
-        if vocab_trace_path_str and vocab_trace_path_str.strip()!='.':
-            vocab_trace_path = vocab_trace_path_str.split('.')
-        assert vocab_trace_path, "We need vocab and tokenizer all in meta, so you must provide the trace path from meta"
-        self.label_vocab = meta
-        for trace in vocab_trace_path:
-            self.label_vocab = self.label_vocab[trace]
-        self.label_vocab = Vocabulary.load(self.label_vocab)
-
-
-        tokenizer_trace_path = []
-        tokenizer_trace_path_str = self.config['meta_data']['tokenizer']
-        if tokenizer_trace_path_str and tokenizer_trace_path_str.strip()!='.':
-            tokenizer_trace_path = tokenizer_trace_path_str.split('.')
-        assert tokenizer_trace_path, "We need vocab and tokenizer all in meta, so you must provide the trace path from meta"
-        tokenizer_config = meta
-        for trace in tokenizer_trace_path:
-            tokenizer_config = tokenizer_config[trace]
-        self.tokenizer = Tokenizer.from_str(tokenizer_config)
-
-        self.save_path = self.config['save_path']
-        self.save_root_path = self.config['save_root_path']
-        self.start_save_epoch = self.config['start_save_epoch']
-        self.start_save_step = self.config['start_save_step']
-
-        self.post_check(self.config, used=[
-            "meta",
-            "use_crf",
-            "word_ready",
-            "meta_data",
-            "input_map",
-            "origin_input_map",
-            "save_root_path",
-            "save_path",
-            "start_save_step",
-            "start_save_epoch",
-            "aggregation_strategy",
-            "ignore_labels",
-        ])
+@cregister("postprocessor", "seq_lab")
+class SeqLabPostProcessorConfig(BasePostProcessorConfig):
+    """the seq_lab postprocessor"""
+
+    use_crf = BoolField(value=False, help="whether to use crf")
+    word_ready = BoolField(
+        value=False, help="already gathered the first subword index of the word"
+    )
+    ignore_position = BoolField(
+        value=False, help="whether to ignore the position of the entity"
+    )
+    ignore_char = ListField(
+        value=[],
+        suggestions=[[" ", "(", ")", "[", "]", "-", ".", ",", ":", "'", '"']],
+        help="ignore the provided char if these char is prefix or suffix of the entity",
+    )
+    label_vocab = StrField(
+        value=MISSING,
+        help="the label vocab file path of entity, it should be the same as file in the preprocessor",
+    )
+    tokenizer_path = StrField(
+        value=MISSING, help="the tokenizer file path, is not effected by `meta_dir`"
+    )
+
+    class InputMap:
+        logits = StrField(value="logits", help="the output logits")
+        predict_seq_label = StrField(
+            value="predict_seq_label", help="the predict seq label"
+        )
+        index = StrField(value="_index", help="the index of the sample")
+
+    input_map = NestField(
+        value=InputMap,
+        help="the input map of the processor, the key is the name of the processor needed key, the value is the provided data provided key",
+    )
+
+    class OriginInputMap:
+        uuid = StrField(value="uuid", help="the uuid or the id of the sample")
+        sentence = StrField(value="sentence", help="the sentence of the sample")
+        input_ids = StrField(value="input_ids", help="the input ids of the sample")
+        entities_info = StrField(value="entities_info", help="the entities info")
+        offsets = StrField(value="offsets", help="the offsets of the tokens")
+        special_tokens_mask = StrField(
+            value="special_tokens_mask", help="the special tokens mask"
+        )
+        word_ids = StrField(value="word_ids", help="the word ids")
+
+    origin_input_map = NestField(
+        value=OriginInputMap,
+        help="the origin input map of the processor, the key is the name of the processor needed key, the value is the provided data provided key",
+    )
+    aggregation_strategy = StrField(
+        value="max",
+        options=["none", "simple", "first", "average", "max"],
+        help="the aggregation strategy for the same entity",
+    )
+    ignore_labels = ListField(
+        value=["O", "X", "S", "E"],
+        help="the ignore labels, if the entity label in this list, we will ignore this entity",
+    )
 
 
 class AggregationStrategy(object):
     """docstring for AggregationStrategy"""
+
     NONE = "none"
     SIMPLE = "simple"
     FIRST = "first"
     AVERAGE = "average"
     MAX = "max"
 
 
-@postprocessor_register('seq_lab')
-class SeqLabPostProcessor(IPostProcessor):
+@register("postprocessor", "seq_lab")
+class SeqLabPostProcessor(BasePostProcessor):
     """PostProcess for sequence labeling task"""
-    def __init__(self, config:    SeqLabPostProcessorConfig):
-        super(   SeqLabPostProcessor, self).__init__()
+
+    def __init__(self, config: SeqLabPostProcessorConfig):
+        super(SeqLabPostProcessor, self).__init__(config)
+
         self.config = config
-        self.label_vocab = self.config.label_vocab
-        self.tokenizer = self.config.tokenizer
-        self.metric = torchmetrics.Accuracy()
+        self.label_vocab = Vocabulary.load_from_file(
+            os.path.join(self.config.meta_dir, self.config.label_vocab)
+        )
+        with open(self.config.tokenizer_path, "r", encoding="utf-8") as f:
+            tokenizer_str = json.dumps(json.load(f))
+        self.tokenizer = Tokenizer.from_str(tokenizer_str)
 
-    def do_predict(self, stage: str, list_batch_outputs: List[Dict], origin_data: pd.DataFrame, rt_config: Dict)->List:
+    def do_predict(
+        self,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+    ) -> List:
         """Process the model predict to human readable format
 
-        There are three predictor for diffrent seq_lab task dependent on the config.use_crf(the predict is already decoded to ids), and config.word_ready(subword has gathered to firstpiece)
+        There are three predictor for different seq_lab task dependent on the config.use_crf(the predict is already decoded to ids), and config.word_ready(subword has gathered to firstpiece)
 
         Args:
             stage: train/test/etc.
             list_batch_outputs: a list of outputs
             origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
             rt_config:
                 >>> current status
                 >>> {
                 >>>     "current_step": self.global_step,
                 >>>     "current_epoch": self.current_epoch,
                 >>>     "total_steps": self.num_training_steps,
                 >>>     "total_epochs": self.num_training_epochs
                 >>> }
 
-        Returns: 
+        Returns:
             all predicts
 
         """
         predicts = []
         if self.config.use_crf:
-            predicts = self.crf_predict(list_batch_outputs=list_batch_outputs, origin_data=origin_data)
+            predicts = self.crf_predict(
+                list_batch_outputs=list_batch_outputs, origin_data=origin_data
+            )
         elif self.config.word_ready:
-            predicts = self.word_predict(list_batch_outputs=list_batch_outputs, origin_data=origin_data)
+            predicts = self.word_predict(
+                list_batch_outputs=list_batch_outputs, origin_data=origin_data
+            )
         else:
-            predicts = self.predict(list_batch_outputs=list_batch_outputs, origin_data=origin_data)
+            predicts = self.predict(
+                list_batch_outputs=list_batch_outputs, origin_data=origin_data
+            )
         return predicts
 
-    def do_calc_metrics(self, predicts: List, stage: str, list_batch_outputs: List[Dict], origin_data: pd.DataFrame, rt_config: Dict)->Dict:
+    def do_calc_metrics(
+        self,
+        predicts: List,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+    ) -> Dict:
         """calc the scores use the predicts or list_batch_outputs
 
         Args:
             predicts: list of predicts
             stage: train/test/etc.
             list_batch_outputs: a list of outputs
             origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
@@ -207,82 +186,98 @@
                 >>> {
                 >>>     "current_step": self.global_step,
                 >>>     "current_epoch": self.current_epoch,
                 >>>     "total_steps": self.num_training_steps,
                 >>>     "total_epochs": self.num_training_epochs
                 >>> }
 
-        Returns: 
+        Returns:
             the named scores, recall, precision, f1
 
         """
 
-        def _flat_entities_info(entities_info: List[Dict], text: str)->Dict:
+        def _flat_entities_info(entities_info: List[Dict], text: str) -> Dict:
             """gather the same labeled entity to the same list
 
             Args:
-                entities_info: 
+                entities_info:
                     >>> [
                     >>>     {
                     >>>         "start": start1,
                     >>>         "end": end1,
                     >>>         "labels": ["label_1"]
                     >>>     },
                     >>>     {
                     >>>         "start": start2,
                     >>>         "end": end2,
                     >>>         "labels": ["label_2"]
                     >>>     },....
                     >>> ]
                 text: be labeled text
 
-            Returns: 
+            Returns:
                 >>> { "label_1" [text[start1:end1]], "label_2": [text[start_2: end_2]]...}
 
             """
             info = {}
             for item in entities_info:
-                label = item['labels'][0]
+                label = item["labels"][0]
                 if label not in info:
                     info[label] = []
-                start_position, end_position = item['start'], item['end']
+                start_position, end_position = item["start"], item["end"]
                 while start_position < end_position:
                     if text[start_position] in self.config.ignore_char:
                         start_position += 1
                     else:
                         break
                 while start_position < end_position:
-                    if text[end_position-1] in self.config.ignore_char:
+                    if text[end_position - 1] in self.config.ignore_char:
                         end_position -= 1
                     else:
                         break
-                if start_position == end_position: # if the entity after remove ignore char be null, we set it to origin
-                    start_position, end_position = item['start'], item['end']
-                    
+                if (
+                    start_position == end_position
+                ):  # if the entity after remove ignore char be null, we set it to origin
+                    start_position, end_position = item["start"], item["end"]
+
                 if self.config.ignore_position:
-                    info[label].append(text[item['start']: item['end']].strip())
+                    info[label].append(text[item["start"] : item["end"]].strip())
                 else:
                     info[label].append((start_position, end_position))
             return info
 
         all_predicts = []
         all_ground_truths = []
         for predict in predicts:
-            text = predict['sentence']
-            predict_ins = _flat_entities_info(predict['predict_entities_info'], text)
-            ground_truth_ins = _flat_entities_info(predict['entities_info'], text)
+            text = predict["sentence"]
+            predict_ins = _flat_entities_info(predict["predict_entities_info"], text)
+            ground_truth_ins = _flat_entities_info(predict["entities_info"], text)
             all_predicts.append(predict_ins)
             all_ground_truths.append(ground_truth_ins)
 
         precision, recall, f1 = self.calc_score(all_predicts, all_ground_truths)
         real_name = self.loss_name_map(stage)
-        logger.info(f'{real_name}_precision: {precision*100}, {real_name}_recall: {recall*100}, {real_name}_f1: {f1*100}')
-        return {f'{real_name}_precision': precision*100, f'{real_name}_recall': recall*100, f'{real_name}_f1': f1*100}
+        logger.info(
+            f"{real_name}_precision: {precision*100}, {real_name}_recall: {recall*100}, {real_name}_f1: {f1*100}"
+        )
+        return {
+            f"{real_name}_precision": precision * 100,
+            f"{real_name}_recall": recall * 100,
+            f"{real_name}_f1": f1 * 100,
+        }
 
-    def do_save(self, predicts: List, stage: str, list_batch_outputs: List[Dict], origin_data: pd.DataFrame, rt_config: Dict, save_condition: bool=False):
+    def do_save(
+        self,
+        predicts: List,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+        save_condition: bool = False,
+    ):
         """save the predict when save_condition==True
 
         Args:
             predicts: list of predicts
             stage: train/test/etc.
             list_batch_outputs: a list of outputs
             origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
@@ -292,77 +287,82 @@
                 >>>     "current_step": self.global_step,
                 >>>     "current_epoch": self.current_epoch,
                 >>>     "total_steps": self.num_training_steps,
                 >>>     "total_epochs": self.num_training_epochs
                 >>> }
             save_condition: True for save, False for depend on rt_config
 
-        Returns: 
+        Returns:
             None
 
         """
         if self.config.start_save_epoch == -1 or self.config.start_save_step == -1:
-            self.config.start_save_step = rt_config.get('total_steps', 0) - 1
-            self.config.start_save_epoch = rt_config.get('total_epochs', 0) - 1
-        if not save_condition and (rt_config['current_step']>=self.config.start_save_step or rt_config['current_epoch']>=self.config.start_save_epoch):
+            self.config.start_save_step = rt_config.get("total_steps", 0) - 1
+            self.config.start_save_epoch = rt_config.get("total_epochs", 0) - 1
+        if not save_condition and (
+            rt_config["current_step"] >= self.config.start_save_step
+            or rt_config["current_epoch"] >= self.config.start_save_epoch
+        ):
             save_condition = True
         if save_condition:
-            save_path = os.path.join(self.config.save_root_path, self.config.save_path.get(stage, ''))
-            if not os.path.exists(save_path):
-                os.makedirs(save_path, exist_ok=True)
+            save_dir = os.path.join(
+                self.config.save_root_path, self.config.save_dir.get(stage, "")
+            )
             if "current_step" in rt_config:
-                save_file = os.path.join(save_path, f"step_{str(rt_config['current_step'])}_predict.json")
+                save_file = os.path.join(
+                    save_dir, f"step_{str(rt_config['current_step'])}_predict.json"
+                )
             else:
-                save_file = os.path.join(save_path, 'predict.json')
+                save_file = os.path.join(save_dir, "predict.json")
             logger.info(f"Save the {stage} predict data at {save_file}")
-            json.dump(predicts, open(save_file, 'w'), indent=4, ensure_ascii=False)
+            with open(save_file, "w") as f:
+                json.dump(predicts, f, indent=4, ensure_ascii=False)
 
     def calc_score(self, predict_list: List, ground_truth_list: List):
         """use predict_list and ground_truth_list to calc scores
 
         Args:
             predict_list: list of predict
             ground_truth_list: list of ground_truth
 
-        Returns: 
+        Returns:
             precision, recall, f1
 
         """
         category_tp = {}
         category_fp = {}
         category_fn = {}
+
         def _care_div(a, b):
-            """return a/b or 0.0 if b == 0
-            """
-            if b==0:
+            """return a/b or 0.0 if b == 0"""
+            if b == 0:
                 return 0.0
-            return a/b
-
+            return a / b
 
         def _calc_num(_pred: List, _ground_truth: List):
             """calc tp, fn, fp
 
             Args:
                 pred: pred list
                 ground_truth: groud truth list
 
-            Returns: 
+            Returns:
                 tp, fn, fp
 
             """
             num_p = len(_pred)
             num_t = len(_ground_truth)
             truth = 0
             for p in _pred:
                 if p in _ground_truth:
                     truth += 1
-            return truth, num_t-truth, num_p-truth
+            return truth, num_t - truth, num_p - truth
 
         for predict, ground_truth in zip(predict_list, ground_truth_list):
-            keys = set(list(predict.keys())+list(ground_truth.keys()))
+            keys = set(list(predict.keys()) + list(ground_truth.keys()))
             for key in keys:
                 tp, fn, fp = _calc_num(predict.get(key, []), ground_truth.get(key, []))
                 # logger.info(f"{key} tp num {tp}, fn num {fn}, fp num {fp}")
                 category_tp[key] = category_tp.get(key, 0) + tp
                 category_fn[key] = category_fn.get(key, 0) + fn
                 category_fp[key] = category_fp.get(key, 0) + fp
 
@@ -370,305 +370,376 @@
         for key in category_tp:
             if key in self.config.ignore_labels:
                 continue
             tp, fn, fp = category_tp[key], category_fn[key], category_fp[key]
             all_tp += tp
             all_fn += fn
             all_fp += fp
-            precision = _care_div(tp, tp+fp)
-            recall = _care_div(tp, tp+fn)
-            f1 = _care_div(2*precision*recall, precision+recall)
-            logger.info(f"For entity 「{key}」, the precision={precision*100 :.2f}%, the recall={recall*100:.2f}%, f1={f1*100:.2f}%")
-        precision = _care_div(all_tp,all_tp+all_fp)
-        recall = _care_div(all_tp, all_tp+all_fn)
-        f1 = _care_div(2*precision*recall, precision+recall)
+            precision = _care_div(tp, tp + fp)
+            recall = _care_div(tp, tp + fn)
+            f1 = _care_div(2 * precision * recall, precision + recall)
+            logger.info(
+                f"For entity 「{key}」, the precision={precision*100 :.2f}%, the recall={recall*100:.2f}%, f1={f1*100:.2f}%"
+            )
+        precision = _care_div(all_tp, all_tp + all_fp)
+        recall = _care_div(all_tp, all_tp + all_fn)
+        f1 = _care_div(2 * precision * recall, precision + recall)
         return precision, recall, f1
 
-    def get_entity_info(self, sub_tokens_index: List, offset_mapping: List, word_ids: List, label: str)->Dict:
+    def get_entity_info(
+        self, sub_tokens_index: List, offset_mapping: List, word_ids: List, label: str
+    ) -> Dict:
         """gather sub_tokens to get the start and end
 
         Args:
             sub_tokens_index: the entity tokens index list
             offset_mapping: every token offset in text
             word_ids: every token in the index of words
             label: predict label
 
-        Returns: 
+        Returns:
             entity_info
 
         """
-        if (not sub_tokens_index) or (not label) or (label in self.config.ignore_labels):
+        if (
+            (not sub_tokens_index)
+            or (not label)
+            or (label in self.config.ignore_labels)
+        ):
             return {}
         start = offset_mapping[sub_tokens_index[0]][0]
         end = offset_mapping[sub_tokens_index[-1]][1]
-        return {
-            "start": start,
-            "end": end,
-            "labels": [label]
-        }
+        return {"start": start, "end": end, "labels": [label]}
 
-    def _process4predict(self, predict: torch.LongTensor, index: int, origin_data: pd.DataFrame)->Dict:
+    def _process4predict(
+        self, predict: torch.LongTensor, index: int, origin_data: pd.DataFrame
+    ) -> Dict:
         """gather the predict and origin text and ground_truth_entities_info for predict
 
         Args:
             predict: the predict label_ids
             index: the data index in origin_data
             origin_data: the origin pd.DataFrame
 
-        Returns: 
-            >>> one_ins info 
+        Returns:
+            >>> one_ins info
             >>> {
             >>>     "sentence": "...",
             >>>     "uuid": "..",
             >>>     "entities_info": [".."],
             >>>     "predict_entities_info": [".."],
             >>> }
 
         """
         one_ins = {}
         origin_ins = origin_data.iloc[int(index)]
-        one_ins["sentence"] = origin_ins[self.config.sentence]
-        one_ins["uuid"] = origin_ins[self.config.uuid]
-        one_ins["entities_info"] = origin_ins[self.config.entities_info]
+        one_ins["sentence"] = origin_ins[self.config.origin_input_map.sentence]
+        one_ins["uuid"] = origin_ins[self.config.origin_input_map.uuid]
+        one_ins["entities_info"] = origin_ins[
+            self.config.origin_input_map.entities_info
+        ]
 
-        word_ids = origin_ins[self.config.word_ids]
+        word_ids = origin_ins[self.config.origin_input_map.word_ids]
         rel_token_len = len(word_ids)
-        offset_mapping = origin_ins[self.config.offsets][:rel_token_len]
+        offset_mapping = origin_ins[self.config.origin_input_map.offsets][
+            :rel_token_len
+        ]
         predict = list(predict[:rel_token_len])
-        # predict = list(origin_ins['label_ids'][:rel_token_len])
         predict_entities_info = []
-        pre_label = ''
+        pre_label = ""
         sub_tokens_index = []
         for i, label_id in enumerate(predict):
-            if offset_mapping[i] == (0, 0): # added token like [CLS]/<s>/..
+            if offset_mapping[i] == (0, 0):  # added token like [CLS]/<s>/..
                 continue
-            label = self.config.label_vocab[label_id]
-            if label in self.config.ignore_labels \
-                or (label[0]=='B') \
-                or (label.split('-')[-1] != pre_label):   # label == "O" or label=='B' or label.tail != previor_label
-                entity_info = self.get_entity_info(sub_tokens_index, offset_mapping, word_ids, pre_label)
+            label = self.label_vocab[label_id]
+            if (
+                label in self.config.ignore_labels
+                or (label[0] == "B")
+                or (label.split("-")[-1] != pre_label)
+            ):  # label == "O" or label=='B' or label.tail != previor_label
+                entity_info = self.get_entity_info(
+                    sub_tokens_index, offset_mapping, word_ids, pre_label
+                )
                 if entity_info:
                     predict_entities_info.append(entity_info)
-                pre_label = ''
+                pre_label = ""
                 sub_tokens_index = []
             if label not in self.config.ignore_labels:
-                assert len(label.split('-')) == 2
-                pre_label = label.split('-')[-1]
+                assert len(label.split("-")) == 2
+                pre_label = label.split("-")[-1]
                 sub_tokens_index.append(i)
-        entity_info = self.get_entity_info(sub_tokens_index, offset_mapping, word_ids, pre_label)
+        entity_info = self.get_entity_info(
+            sub_tokens_index, offset_mapping, word_ids, pre_label
+        )
         if entity_info:
             predict_entities_info.append(entity_info)
-        one_ins['predict_entities_info'] = predict_entities_info
+        one_ins["predict_entities_info"] = predict_entities_info
         return one_ins
 
-    def crf_predict(self, list_batch_outputs: List[Dict], origin_data: pd.DataFrame)->List:
+    def crf_predict(
+        self, list_batch_outputs: List[Dict], origin_data: pd.DataFrame
+    ) -> List:
         """use the crf predict label_ids get predict info
 
         Args:
             list_batch_outputs: the crf predict info
             origin_data: the origin data
 
-        Returns: 
+        Returns:
             all predict instances info
 
         """
-        if self.config.sentence not in origin_data:
-            logger.error(f"{self.config.sentence} not in the origin data")
-            raise PermissionError(f"{self.config.sentence} must be provided")
-        if self.config.uuid not in origin_data:
-            logger.error(f"{self.config.uuid} not in the origin data")
-            raise PermissionError(f"{self.config.uuid} must be provided")
-        if self.config.entities_info not in origin_data:
-            logger.error(f"{self.config.entities_info} not in the origin data")
-            raise PermissionError(f"{self.config.entities_info} must be provided")
+        if self.config.origin_input_map.sentence not in origin_data:
+            logger.error(
+                f"{self.config.origin_input_map.sentence} not in the origin data"
+            )
+            raise PermissionError(
+                f"{self.config.origin_input_map.sentence} must be provided"
+            )
+        if self.config.origin_input_map.uuid not in origin_data:
+            logger.error(f"{self.config.origin_input_map.uuid} not in the origin data")
+            raise PermissionError(
+                f"{self.config.origin_input_map.uuid} must be provided"
+            )
+        if self.config.origin_input_map.entities_info not in origin_data:
+            logger.error(
+                f"{self.config.origin_input_map.entities_info} not in the origin data"
+            )
+            raise PermissionError(
+                f"{self.config.origin_input_map.entities_info} must be provided"
+            )
 
         predicts = []
         for outputs in list_batch_outputs:
-            batch_predict = outputs[self.config.predict_seq_label]
+            batch_predict = outputs[self.config.input_map.predict_seq_label]
             # batch_special_tokens_mask = outputs[self.config.special_tokens_mask]
 
-            indexes = list(outputs[self.config._index])
+            indexes = list(outputs[self.config.input_map.index])
             outputs = []
 
-            for predict, index in zip(batch_predict, indexes):
+            for predict, index in list(zip(batch_predict, indexes)):
                 one_ins = self._process4predict(predict, index, origin_data)
                 predicts.append(one_ins)
         return predicts
 
-    def word_predict(self, list_batch_outputs: List[Dict], origin_data: pd.DataFrame)->List:
+    def word_predict(
+        self, list_batch_outputs: List[Dict], origin_data: pd.DataFrame
+    ) -> List:
         """use the firstpiece or whole word predict label_logits get predict info
 
         Args:
             list_batch_outputs: the predict labels logits info
             origin_data: the origin data
 
-        Returns: 
+        Returns:
             all predict instances info
 
         """
-        if self.config.sentence not in origin_data:
-            logger.error(f"{self.config.sentence} not in the origin data")
-            raise PermissionError(f"{self.config.sentence} must be provided")
-        if self.config.uuid not in origin_data:
-            logger.error(f"{self.config.uuid} not in the origin data")
-            raise PermissionError(f"{self.config.uuid} must be provided")
-        if self.config.entities_info not in origin_data:
-            logger.error(f"{self.config.entities_info} not in the origin data")
-            raise PermissionError(f"{self.config.entities_info} must be provided")
+        if self.config.origin_input_map.sentence not in origin_data:
+            logger.error(
+                f"{self.config.origin_input_map.sentence} not in the origin data"
+            )
+            raise PermissionError(
+                f"{self.config.origin_input_map.sentence} must be provided"
+            )
+        if self.config.origin_input_map.uuid not in origin_data:
+            logger.error(f"{self.config.origin_input_map.uuid} not in the origin data")
+            raise PermissionError(
+                f"{self.config.origin_input_map.uuid} must be provided"
+            )
+        if self.config.origin_input_map.entities_info not in origin_data:
+            logger.error(
+                f"{self.config.origin_input_map.entities_info} not in the origin data"
+            )
+            raise PermissionError(
+                f"{self.config.origin_input_map.entities_info} must be provided"
+            )
 
         predicts = []
         for outputs in list_batch_outputs:
-            batch_logits = outputs[self.config.logits].detach()
-            # batch_special_tokens_mask = outputs[self.config.special_tokens_mask]
+            batch_logits = outputs[self.config.input_map.logits].detach().cpu().numpy()
 
-            indexes = list(outputs[self.config._index])
+            indexes = list(outputs[self.config.input_map.index])
 
             outputs = []
 
-            for logits, index in zip(batch_logits, indexes):
+            for logits, index in list(zip(batch_logits, indexes)):
                 origin_ins = origin_data.iloc[int(index)]
-                word_ids = origin_ins[self.config.word_ids]
+                word_ids = origin_ins[self.config.origin_input_map.word_ids]
 
                 rel_token_len = len(word_ids)
-                logits = logits[:rel_token_len].cpu().numpy()
+                logits = logits[:rel_token_len]
 
                 predict = logits.argmax(-1)
                 one_ins = self._process4predict(predict, index, origin_data)
                 predicts.append(one_ins)
         return predicts
 
-    def predict(self, list_batch_outputs: List[Dict], origin_data: pd.DataFrame)->List:
+    def predict(
+        self, list_batch_outputs: List[Dict], origin_data: pd.DataFrame
+    ) -> List:
         """general predict process (especially for subword)
 
         Args:
             list_batch_outputs: the predict (sub-)labels logits info
             origin_data: the origin data
 
-        Returns: 
+        Returns:
             all predict instances info
 
         """
-        if self.config.sentence not in origin_data:
-            logger.error(f"{self.config.sentence} not in the origin data")
-            raise PermissionError(f"{self.config.sentence} must be provided")
-        if self.config.uuid not in origin_data:
-            logger.error(f"{self.config.uuid} not in the origin data")
-            raise PermissionError(f"{self.config.uuid} must be provided")
-        if self.config.entities_info not in origin_data:
-            logger.error(f"{self.config.entities_info} not in the origin data")
-            raise PermissionError(f"{self.config.entities_info} must be provided")
+        if self.config.origin_input_map.sentence not in origin_data:
+            logger.error(
+                f"{self.config.origin_input_map.sentence} not in the origin data"
+            )
+            raise PermissionError(
+                f"{self.config.origin_input_map.sentence} must be provided"
+            )
+        if self.config.origin_input_map.uuid not in origin_data:
+            logger.error(f"{self.config.origin_input_map.uuid} not in the origin data")
+            raise PermissionError(
+                f"{self.config.origin_input_map.uuid} must be provided"
+            )
+        if self.config.origin_input_map.entities_info not in origin_data:
+            logger.error(
+                f"{self.config.origin_input_map.entities_info} not in the origin data"
+            )
+            raise PermissionError(
+                f"{self.config.origin_input_map.entities_info} must be provided"
+            )
 
         predicts = []
         for outputs in list_batch_outputs:
-            batch_logits = outputs[self.config.logits].detach()
-            # batch_special_tokens_mask = outputs[self.config.special_tokens_mask]
+            batch_logits = outputs[self.config.input_map.logits].detach().cpu().numpy()
 
-            indexes = list(outputs[self.config._index])
+            indexes = list(outputs[self.config.input_map.index])
 
             outputs = []
 
-            for logits, index in zip(batch_logits, indexes):
+            for logits, index in list(zip(batch_logits, indexes)):
                 one_ins = {}
                 origin_ins = origin_data.iloc[int(index)]
 
-                input_ids = origin_ins[self.config.input_ids]
-                one_ins["sentence"] = origin_ins[self.config.sentence]
-                one_ins["uuid"] = origin_ins[self.config.uuid]
-                one_ins["entities_info"] = origin_ins[self.config.entities_info]
+                input_ids = origin_ins[self.config.origin_input_map.input_ids]
+                one_ins["sentence"] = origin_ins[self.config.origin_input_map.sentence]
+                one_ins["uuid"] = origin_ins[self.config.origin_input_map.uuid]
+                one_ins["entities_info"] = origin_ins[
+                    self.config.origin_input_map.entities_info
+                ]
 
                 rel_token_len = len(input_ids)
 
-                special_tokens_mask = np.array(origin_data.iloc[int(index)][self.config.special_tokens_mask][:rel_token_len])
-                offset_mapping = origin_data.iloc[int(index)][self.config.offsets][:rel_token_len]
+                special_tokens_mask = np.array(
+                    origin_data.iloc[int(index)][
+                        self.config.origin_input_map.special_tokens_mask
+                    ][:rel_token_len]
+                )
+                offset_mapping = origin_data.iloc[int(index)][
+                    self.config.origin_input_map.offsets
+                ][:rel_token_len]
 
-                logits = logits[:rel_token_len].cpu().numpy()
+                logits = logits[:rel_token_len]
 
                 entity_idx = logits.argmax(-1)
                 labels = []
                 for i, idx in enumerate(list(entity_idx)):
-                    labels.append(self.config.label_vocab[idx])
+                    labels.append(self.label_vocab[idx])
 
                 maxes = np.max(logits, axis=-1, keepdims=True)
                 shifted_exp = np.exp(logits - maxes)
                 scores = shifted_exp / shifted_exp.sum(axis=-1, keepdims=True)
 
                 pre_entities = self.gather_pre_entities(
-                    one_ins["sentence"], input_ids, scores, offset_mapping, special_tokens_mask)
-                grouped_entities = self.aggregate(pre_entities, self.config.aggregation_strategy)
+                    one_ins["sentence"],
+                    input_ids,
+                    scores,
+                    offset_mapping,
+                    special_tokens_mask,
+                )
+                grouped_entities = self.aggregate(
+                    pre_entities, self.config.aggregation_strategy
+                )
                 # Filter anything that is in self.ignore_labels
                 entities = [
                     entity
                     for entity in grouped_entities
                     if entity.get("entity", None) not in self.config.ignore_labels
-                    and entity.get("entity_group", None) not in self.config.ignore_labels
+                    and entity.get("entity_group", None)
+                    not in self.config.ignore_labels
                 ]
                 predict_entities_info = []
                 for entity in entities:
                     one_predict = {}
-                    one_predict['start'] = entity['start']
-                    one_predict['end'] = entity['end']
-                    one_predict['labels'] = [entity['entity_group']]
+                    one_predict["start"] = entity["start"]
+                    one_predict["end"] = entity["end"]
+                    one_predict["labels"] = [entity["entity_group"]]
                     predict_entities_info.append(one_predict)
-                one_ins['predict_entities_info'] = predict_entities_info
+                one_ins["predict_entities_info"] = predict_entities_info
                 predicts.append(one_ins)
         return predicts
 
-    def aggregate(self, pre_entities: List[dict], aggregation_strategy: AggregationStrategy) -> List[dict]:
-        if aggregation_strategy in {AggregationStrategy.NONE, AggregationStrategy.SIMPLE}:
+    def aggregate(
+        self, pre_entities: List[dict], aggregation_strategy: str
+    ) -> List[dict]:
+        if aggregation_strategy in {
+            AggregationStrategy.NONE,
+            AggregationStrategy.SIMPLE,
+        }:
             entities = []
             for pre_entity in pre_entities:
                 entity_idx = pre_entity["scores"].argmax()
                 score = pre_entity["scores"][entity_idx]
                 entity = {
-                    "entity": self.config.label_vocab[entity_idx],
+                    "entity": self.label_vocab[entity_idx],
                     "score": score,
                     "index": pre_entity["index"],
                     "word": pre_entity["word"],
                     "start": pre_entity["start"],
                     "end": pre_entity["end"],
                 }
                 entities.append(entity)
         else:
             entities = self.aggregate_words(pre_entities, aggregation_strategy)
 
         if aggregation_strategy == AggregationStrategy.NONE:
             return entities
         return self.group_entities(entities)
 
-    def aggregate_word(self, entities: List[dict], aggregation_strategy: AggregationStrategy) -> dict:
-        word = self.tokenizer.decode([self.tokenizer.token_to_id(entity['word']) for entity in entities])
+    def aggregate_word(self, entities: List[dict], aggregation_strategy: str) -> dict:
+        word = self.tokenizer.decode(
+            [self.tokenizer.token_to_id(entity["word"]) for entity in entities]
+        )
         if aggregation_strategy == AggregationStrategy.FIRST:
             scores = entities[0]["scores"]
             idx = scores.argmax()
             score = scores[idx]
-            entity = self.config.label_vocab[idx]
+            entity = self.label_vocab[idx]
         elif aggregation_strategy == AggregationStrategy.MAX:
             max_entity = max(entities, key=lambda entity: entity["scores"].max())
             scores = max_entity["scores"]
             idx = scores.argmax()
             score = scores[idx]
-            entity = self.config.label_vocab[idx]
+            entity = self.label_vocab[idx]
         elif aggregation_strategy == AggregationStrategy.AVERAGE:
             scores = np.stack([entity["scores"] for entity in entities])
             average_scores = np.nanmean(scores, axis=0)
             entity_idx = average_scores.argmax()
-            entity = self.config.label_vocab[entity_idx]
+            entity = self.label_vocab[entity_idx]
             score = average_scores[entity_idx]
         else:
             raise ValueError("Invalid aggregation_strategy")
         new_entity = {
             "entity": entity,
             "score": score,
             "word": word,
             "start": entities[0]["start"],
             "end": entities[-1]["end"],
         }
         return new_entity
 
-
     def group_sub_entities(self, entities: List[dict]) -> dict:
         """Group together the adjacent tokens with the same entity predicted.
 
         Args:
             entities: The entities predicted by the pipeline.
         """
         # Get the first entity in the entity group
@@ -730,36 +801,42 @@
                 entity_group_disagg = [entity]
         if entity_group_disagg:
             # it's the last entity, add it to the entity groups
             entity_groups.append(self.group_sub_entities(entity_group_disagg))
 
         return entity_groups
 
-    def aggregate_words(self, entities: List[dict], aggregation_strategy: AggregationStrategy) -> List[dict]:
+    def aggregate_words(
+        self, entities: List[dict], aggregation_strategy: str
+    ) -> List[dict]:
         """Override tokens from a given word that disagree to force agreement on word boundaries.
 
-        Example: 
+        Example:
             micro|soft| com|pany| B-ENT I-NAME I-ENT I-ENT will be rewritten with first strategy as microsoft|
             company| B-ENT I-ENT
         """
         if aggregation_strategy in {
             AggregationStrategy.NONE,
             AggregationStrategy.SIMPLE,
         }:
-            raise ValueError("NONE and SIMPLE strategies are invalid for word aggregation")
+            raise ValueError(
+                "NONE and SIMPLE strategies are invalid for word aggregation"
+            )
 
         word_entities = []
-        word_group = None
+        word_group = []
         for entity in entities:
-            if word_group is None:
+            if not word_group:
                 word_group = [entity]
             elif entity["is_subword"]:
                 word_group.append(entity)
             else:
-                word_entities.append(self.aggregate_word(word_group, aggregation_strategy))
+                word_entities.append(
+                    self.aggregate_word(word_group, aggregation_strategy)
+                )
                 word_group = [entity]
         # Last item
         word_entities.append(self.aggregate_word(word_group, aggregation_strategy))
         return word_entities
 
     def gather_pre_entities(
         self,
@@ -784,15 +861,19 @@
                 word_ref = sentence[start_ind:end_ind]
                 if getattr(self.tokenizer.model, "continuing_subword_prefix", None):
                     # This is a BPE, word aware tokenizer, there is a correct way
                     # to fuse tokens
                     is_subword = len(word) != len(word_ref)
                 else:
                     # This is a fallback heuristic. This will fail most likely on any kind of text + punctuation mixtures that will be considered "words". Non word aware models cannot do better than this unfortunately.
-                    is_subword = sentence[start_ind - 1 : start_ind] != " " if start_ind > 0 else False
+                    is_subword = (
+                        sentence[start_ind - 1 : start_ind] != " "
+                        if start_ind > 0
+                        else False
+                    )
 
             else:
                 start_ind = None
                 end_ind = None
                 is_subword = False
 
             pre_entity = {
@@ -801,8 +882,7 @@
                 "start": start_ind,
                 "end": end_ind,
                 "index": idx,
                 "is_subword": is_subword,
             }
             pre_entities.append(pre_entity)
         return pre_entities
-
```

### Comparing `dlk-0.0.9/dlk/data/subprocessors/load.py` & `dlk-0.1.0/dlk/preprocess.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,91 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from dlk.utils.config import ConfigTool, BaseConfig
-from dlk.utils.logger import Logger
-from typing import Dict, Callable, Set, List
-from dlk.data.subprocessors import subprocessor_register, subprocessor_config_register, ISubProcessor
-import pickle as pkl
-import os
-
-logger = Logger.get_logger()
-
-@subprocessor_config_register('load')
-class LoadConfig(BaseConfig):
-    """Config for Load
-
-    Config Example:
-        >>> {
-        >>>     "_name": "load",
-        >>>     "config":{
-        >>>         "base_dir": "."
-        >>>         "predict":{
-        >>>             "meta": "./meta.pkl",
-        >>>         },
-        >>>         "online": [
-        >>>             "predict", //base predict
-        >>>             {   // special config, update predict, is this case, the config is null, means use all config from "predict", when this is empty dict, you can only set the value to a str "predict", they will get the same result
-        >>>             }
-        >>>         ]
-        >>>     }
-        >>> },
-    """
-
-    def __init__(self, stage, config):
-        super(LoadConfig, self).__init__(config)
-        self.config = ConfigTool.get_config_by_stage(stage, config)
-        self.base_dir:str = config.get('config').get("base_dir", ".")
-
-
-@subprocessor_register('load')
-class Load(ISubProcessor):
-    """ Loader the $meta, etc. to data
-    """
-
-    def __init__(self, stage: str, config: LoadConfig):
-        super().__init__()
-        self.stage = stage
-        self.config = config.config
-        if not self.config:
-            logger.info(f"Skip 'load' at stage {self.stage}")
-            return
-        self.base_dir = config.base_dir
-
-        self.load_data = {}
-        for key, path in self.config.items():
-            self.load_data[key] = self.load(path)
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-    def load(self, path: str):
-        """load data from path
+import json
+from typing import Any, Dict, Union
 
+import hjson
+import pandas as pd
+import torch
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    Parser,
+    StrField,
+    SubModule,
+    cregister,
+    init_config,
+)
+
+from dlk.utils.io import open
+from dlk.utils.register import register, register_module_name
+
+
+class PreProcessor(object):
+    """Processor"""
+
+    def __init__(self, config: Union[str, dict], stage: str = "train"):
+        super(PreProcessor, self).__init__()
+        config_dict = {}
+        if not isinstance(config, dict):
+            with open(config, "r") as f:
+                config_dict = hjson.load(f, object_pairs_hook=dict)
+        else:
+            config_dict = config
+        prepro_config = self.get_config(config_dict)
+        self.init(prepro_config, stage)
+
+    def init(self, config: Base, stage: str):
+        """init the model and trainer
         Args:
-            path: the path to data
+            config: the preprocess config
+            stage: train/predict/online
 
-        Returns: 
-            loaded data
+        Returns: None
+        """
+        # set processor
+        process_name = register_module_name(config._module_name)
+        processor_ins = register.get("processor", process_name)(
+            config=config, stage=stage
+        )
+        if stage in ["train", "predict"]:
+            self.processor = processor_ins.process
+        else:
+            assert stage == "online", f"stage {stage} is not supported"
+            self.processor = processor_ins.online_process
+
+    def get_config(self, config_dict):
+        """get the predict config
+
+        Args:
+            config: the init config
 
+        Returns:
+            DLKPreProConfig, config_name_str
         """
+        configs = Parser(config_dict).parser_init()
+        assert len(configs) == 1, f"You should not use '_search' for preprocess"
 
-        logger.info(f"Loading file from {os.path.join(self.base_dir, path)}")
-        return pkl.load(open(os.path.join(self.base_dir, path), 'rb'))
+        prepro_config = configs[0]["@processor"]
+        return prepro_config
 
-    def process(self, data: Dict)->Dict:
-        """Load entry
+    def fit(self, data: Union[Dict[str, Any], pd.DataFrame]):
+        """Process the data and return the processed data
 
         Args:
-            data: 
-            >>> {
-            >>>     "data": {"train": ...},
-            >>>     "tokenizer": ..
-            >>> }
+            data: {"train": train DataFrame, 'valid': valid DataFrame} if stage is not online else DataFrame
 
-        Returns: 
-            data + loaded_data
+        Returns:
+            processed data
 
         """
-        for _, meta in self.load_data.items():
-            for key, value in meta.items():
-                data[key] = value
-        return data
+        return self.processor(data)
```

### Comparing `dlk-0.0.9/dlk/data/subprocessors/seq_lab_firstpiece_relable.py` & `dlk-0.1.0/dlk/data/subprocessor/seq_lab_firstpiece_relabel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,167 +1,196 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from dlk.utils.vocab import Vocabulary
-from dlk.utils.config import BaseConfig, ConfigTool
-from typing import Dict, Callable, Set, List
-from dlk.data.subprocessors import subprocessor_register, subprocessor_config_register, ISubProcessor
-from functools import partial
-from dlk.utils.logger import Logger
-import pandas as pd
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-logger = Logger.get_logger()
-
-
-@subprocessor_config_register('seq_lab_firstpiece_relabel')
-class SeqLabFirstPieceRelabelConfig(BaseConfig):
-    """Config for SeqLabFirstPieceRelabel
-
-    Config Example:
-        >>> {
-        >>>     "_name": "seq_lab_firstpiece_relabel",
-        >>>     "config": {
-        >>>         "train":{ //train、predict、online stage config,  using '&' split all stages
-        >>>             "input_map": {  // without necessery, don't change this
-        >>>                 "word_ids": "word_ids",
-        >>>                 "offsets": "offsets",
-        >>>                 "entities_info": "entities_info",
-        >>>             },
-        >>>             "data_set": {                   // for different stage, this processor will process different part of data
-        >>>                 "train": ['train', 'valid', 'test', 'predict'],
-        >>>                 "predict": ['predict'],
-        >>>                 "online": ['online']
-        >>>             },
-        >>>             "output_map": {
-        >>>                 "labels": "labels",
-        >>>                 "gather_index": "gather_index",
-        >>>                 "word_word_ids": "word_ids",
-        >>>                 "word_offsets": "offsets",
-        >>>             },
-        >>>             "drop": "shorter", //'longer'/'shorter'/'none', if entities is overlap, will remove by rule
-        >>>             "start_label": "S",
-        >>>             "end_label": "E",
-        >>>             "clean_droped_entity": true, // after drop entity for training, whether drop the entity for calc metrics, default is true, this only works when the drop != 'none'
-        >>>             "entity_priority": [],
-        >>>             //"entity_priority": ['Product'],
-        >>>             "priority_trigger": 1, // if the overlap entity abs(length_a - length_b)<=priority_trigger, will trigger the entity_priority strategy
-        >>>         }, //3
-        >>>         "predict": "train",
-        >>>         "online": "train",
-        >>>     }
-        >>> }
-    """
-    def __init__(self, stage, config: Dict):
+import logging
+from typing import Callable, Dict, List, Set
 
-        super(SeqLabFirstPieceRelabelConfig, self).__init__(config)
-        self.config = ConfigTool.get_config_by_stage(stage, config)
-        self.data_set = self.config.get('data_set', {}).get(stage, [])
-        if not self.data_set:
-            return
-        self.word_ids = self.config['input_map']['word_ids']
-        self.word_word_ids = self.config['output_map']['word_word_ids']
-        self.word_offsets = self.config['output_map']['word_offsets']
-        self.offsets = self.config['input_map']['offsets']
-        self.entities_info = self.config['input_map']['entities_info']
-        self.clean_droped_entity = self.config['clean_droped_entity']
-        self.drop = self.config['drop']
-        self.start_label = self.config['start_label']
-        self.end_label = self.config['end_label']
-        self.entity_priority = {entity: priority for priority, entity in enumerate(self.config['entity_priority'])}
-        self.priority_trigger = self.config['priority_trigger']
-        self.gather_index = self.config['output_map']['gather_index']
-        self.output_labels = self.config['output_map']['labels']
-        self.post_check(self.config, used=[
-            "drop",
-            "input_map",
-            "data_set",
-            "output_map",
-            "start_label",
-            "end_label",
-            "clean_droped_entity",
-            "entity_priority",
-            "priority_trigger",
-        ])
+import pandas as pd
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.io import open
+from dlk.utils.register import register
+
+from . import BaseSubProcessor, BaseSubProcessorConfig
+
+logger = logging.getLogger(__name__)
+
+
+@cregister("subprocessor", "seq_lab_firstpiece_relabel")
+class SeqLabFirstPieceRelabelConfig(BaseSubProcessorConfig):
+    """the sequence labeling firstpiece relabel subprocessor"""
+
+    train_data_set = ListField(
+        value=["train", "valid", "test"],
+        suggestions=[["train", "valid", "test"]],
+        help="the data set should be processed for train stage",
+    )
+    predict_data_set = ListField(
+        value=["predict"],
+        suggestions=[["predict"]],
+        help="the data set should be processed for predict stage",
+    )
+    online_data_set = ListField(
+        value=["online"],
+        suggestions=[["online"]],
+        help="the data set should be processed for online stage",
+    )
+
+    class InputMap:
+        word_ids = StrField(value="word_ids", help="the word ids")
+        offsets = StrField(value="offsets", help="the offsets")
+        entities_info = StrField(value="entities_info", help="the entities info")
+
+    input_map = NestField(
+        value=InputMap,
+        help="the input map of the processor, the key is the name of the processor needed key, the value is the provided data provided key",
+    )
+
+    class OutputMap:
+        labels = StrField(value="labels", help="the label names")
+        gather_index = StrField(value="gather_index", help="the gather index")
+        word_word_ids = StrField(value="word_ids", help="the word word ids")
+        word_offsets = StrField(value="offsets", help="the word offsets")
+
+    output_map = NestField(
+        value=OutputMap,
+        help="the output map of the processor, the key is the name of the processor provided key, the value is the nexted processor needed key",
+    )
+    drop = StrField(
+        value="shorter",
+        options=["longer", "shorter", "none"],
+        help="the drop strategy for the overlap entities",
+    )
+    start_label = StrField(value="S", help="the start label")
+    end_label = StrField(value="E", help="the end label")
+    clean_droped_entity = BoolField(
+        value=True, help="whether clean the dropped entity for calc metrics"
+    )
+    entity_priority = ListField(
+        value=[],
+        suggestions=[["Product", "Brand"]],
+        help="the entity priority, when conflict, will keep the entity with the highest priority",
+    )
+    priority_trigger = IntField(
+        value=1,
+        help="if the overlap entity abs(length_a - length_b)<=priority_trigger, will trigger the entity_priority strategy",
+    )
 
 
-@subprocessor_register('seq_lab_firstpiece_relabel')
-class SeqLabFirstPieceRelabel(ISubProcessor):
+@register("subprocessor", "seq_lab_firstpiece_relabel")
+class SeqLabFirstPieceRelabel(BaseSubProcessor):
     """Relabel the json data to bio.
 
     And gather the firstpiece subword index to deliver $gather_index; for get the firstpiece index we must use the $word_ids(generator by tokenizer)
     """
 
-    def __init__(self, stage: str, config: SeqLabFirstPieceRelabelConfig):
-        super().__init__()
+    def __init__(
+        self, stage: str, config: SeqLabFirstPieceRelabelConfig, meta_dir: str
+    ):
+        super().__init__(stage, config, meta_dir)
         self.stage = stage
         self.config = config
-        self.data_set = config.data_set
-        if not self.data_set:
-            logger.info(f"Skip 'seq_lab_firstpiece_relabel' at stage {self.stage}")
-            return
+        self.entity_priority = {
+            entity: priority
+            for priority, entity in enumerate(self.config.entity_priority)
+        }
 
-    def process(self, data: Dict)->Dict:
-        """FirstPieceRelabel Entry
+    def process(self, data: pd.DataFrame, deliver_meta: bool) -> pd.DataFrame:
+        """firstpiece relabel the data
 
         Args:
-            data: Dict
-
-        Returns: 
-            relabeled data
+            data: one is like
 
+            >>> {
+            >>>     "uuid": '**-**-**-**'
+            >>>     "sentence": "Mie Merah - Buah Bit",
+            >>>     "offsets": see the offsets in fast_tokenizer
+            >>>     "entities_info": [
+            >>>                 {
+            >>>                     "end": 9,
+            >>>                     "start": 0,
+            >>>                     "labels": [
+            >>>                         "Product"
+            >>>                     ]
+            >>>                 },
+            >>>             ]
+            >>>         },
+            >>>     ],
+            >>> },
+
+            deliver_meta:
+                ignore
+        Returns:
+            relabeld data
         """
 
-        if not self.data_set:
-            return data
-
-        for data_set_name in self.data_set:
-            if data_set_name not in data['data']:
-                logger.info(f'The {data_set_name} not in data. We will skip do seq_lab_firstpiece_relabel on it.')
-                continue
-            data_set = data['data'][data_set_name]
-            data_set[[self.config.output_labels,
-                self.config.gather_index,
-                self.config.word_word_ids,
-                self.config.word_offsets,
-                self.config.entities_info
-            ]] = data_set.parallel_apply(self.relabel, axis=1, result_type="expand")
+        if self.stage in {"predict", "online"}:
+            data[
+                [
+                    self.config.output_map.gather_index,
+                    self.config.output_map.word_word_ids,
+                    self.config.output_map.word_offsets,
+                ]
+            ] = data.apply(self.relabel, axis=1, result_type="expand")
+        else:
+            data[
+                [
+                    self.config.output_map.labels,
+                    self.config.output_map.gather_index,
+                    self.config.output_map.word_word_ids,
+                    self.config.output_map.word_offsets,
+                    self.config.input_map.entities_info,
+                ]
+            ] = data.apply(self.relabel, axis=1, result_type="expand")
         return data
 
-    def find_position_in_offsets(self, position: int, offset_list: List, sub_word_ids: List, start: int, end: int, is_start: bool=False):
+    def find_position_in_offsets(
+        self,
+        position: int,
+        offset_list: List,
+        sub_word_ids: List,
+        start: int,
+        end: int,
+        is_start: bool = False,
+    ):
         """find the sub_word index which the offset_list[index][0]<=position<offset_list[index][1]
 
         Args:
             position: position
             offset_list: list of all tokens offsets
             sub_word_ids: word_ids from tokenizer
             start: start search index
             end: end search index
             is_start: is the position is the start of target token, if the is_start==True and cannot find return -1
 
-        Returns: 
+        Returns:
             the index of the offset which include position
 
         """
-        while start<end:
+        while start < end:
             if sub_word_ids[start] is None:
                 start += 1
-            elif position>=offset_list[start][0] and position<offset_list[start][1]:
+            elif position >= offset_list[start][0] and position < offset_list[start][1]:
                 return start
-            elif position<offset_list[start][0]:
+            elif position < offset_list[start][0]:
                 if start == 1 and offset_list[0] == [0, 0]:
                     return 1
                 if is_start:
                     return -1
                 else:
                     return start - 1
             else:
@@ -170,24 +199,28 @@
 
     def relabel(self, one_ins: pd.Series):
         """make word label, first merge the token_offset to word_offsets then generate word label from  word_offsets
 
         Args:
             one_ins: include sentence, entity_info, offsets
 
-        Returns: 
-            labels(labels for each word not subtoken), gather_index(real token index of labels), word_ids(sub_word_ids, updated to whole word), word_offsets(token_offsets updated to whole word)
-
+        Returns:
+            For train stage:
+                labels(labels for each word not subtoken), gather_index(real token index of labels), word_ids(sub_word_ids, updated to whole word), word_offsets(token_offsets updated to whole word), entities_info
+            For predict / online stage:
+                gather_index(real token index of labels), word_ids(sub_word_ids, updated to whole word), word_offsets(token_offsets updated to whole word)
         """
-        pre_clean_entities_info = one_ins[self.config.entities_info]
-        pre_clean_entities_info.sort(key=lambda x: x['start'])
-        offsets = one_ins[self.config.offsets]
-        sub_word_ids = one_ins[self.config.word_ids]
+        pre_clean_entities_info = one_ins[self.config.input_map.entities_info]
+        pre_clean_entities_info.sort(key=lambda x: x["start"])
+        offsets = one_ins[self.config.input_map.offsets]
+        sub_word_ids = one_ins[self.config.input_map.word_ids]
         if not sub_word_ids:
-            logger.warning(f"entity_info: {pre_clean_entities_info}, offsets: {offsets} ")
+            logger.warning(
+                f"entity_info: {pre_clean_entities_info}, offsets: {offsets} "
+            )
 
         gather_index = []
         pre_word_id = -1
         word_offset = []
         word_offsets = []
         word_ids = []
         for i, (token_offset, word_id) in enumerate(zip(offsets, sub_word_ids)):
@@ -199,76 +232,104 @@
                 word_offset = list(token_offset)
                 pre_word_id = word_id
             else:
                 assert word_offset
                 word_offset[1] = token_offset[1]
         if word_offset:
             word_offsets.append(word_offset)
+        if self.stage in {"predict", "online"}:
+            return gather_index, word_ids, word_offsets
 
         entities_info = []
         pre_end = -1
         pre_length = 0
-        pre_label = ''
+        pre_label = ""
         for entity_info in pre_clean_entities_info:
-            assert len(entity_info['labels']) == 1, f"currently we just support one label for one entity"
-            if entity_info['start']<pre_end: # if overlap will remove one
-                if self.config.drop == 'none':
+            assert (
+                len(entity_info["labels"]) == 1
+            ), f"currently we just support one label for one entity"
+            if entity_info["start"] < pre_end:  # if overlap will remove one
+                if self.config.drop == "none":
                     pass
-                elif abs(entity_info['end'] - entity_info['start'] - pre_length) <= self.config.priority_trigger:
-                    pre_label_order = self.config.entity_priority.get(pre_label, 1e9)
-                    label_order = self.config.entity_priority.get(entity_info['labels'][0], 1e9)
-                    if label_order<pre_label_order:
+                elif (
+                    abs(entity_info["end"] - entity_info["start"] - pre_length)
+                    <= self.config.priority_trigger
+                ):
+                    pre_label_order = self.entity_priority.get(pre_label, 1e9)
+                    label_order = self.entity_priority.get(
+                        entity_info["labels"][0], 1e9
+                    )
+                    if label_order < pre_label_order:
                         entities_info.pop()
                     else:
                         continue
-                elif self.config.drop == 'shorter':
-                    if entity_info['end'] - entity_info['start'] > pre_length:
+                elif self.config.drop == "shorter":
+                    if entity_info["end"] - entity_info["start"] > pre_length:
                         entities_info.pop()
                     else:
                         continue
-                elif self.config.drop =='longer':
-                    if entity_info['end'] - entity_info['start'] < pre_length:
+                elif self.config.drop == "longer":
+                    if entity_info["end"] - entity_info["start"] < pre_length:
                         entities_info.pop()
                     else:
                         continue
                 else:
-                    raise PermissionError(f"The drop method must in 'none'/'shorter'/'longer'")
-                pre_label = entity_info['labels'][0]
+                    raise PermissionError(
+                        f"The drop method must in 'none'/'shorter'/'longer'"
+                    )
+                pre_label = entity_info["labels"][0]
             entities_info.append(entity_info)
-            pre_end = entity_info['end']
-            pre_length = entity_info['end'] - entity_info['start']
+            pre_end = entity_info["end"]
+            pre_length = entity_info["end"] - entity_info["start"]
 
         cur_token_index = 0
         offset_length = len(word_offsets)
         sub_labels = []
         for entity_info in entities_info:
-            start_token_index = self.find_position_in_offsets(entity_info['start'], word_offsets, word_ids, cur_token_index, offset_length, is_start=True)
+            start_token_index = self.find_position_in_offsets(
+                entity_info["start"],
+                word_offsets,
+                word_ids,
+                cur_token_index,
+                offset_length,
+                is_start=True,
+            )
             if start_token_index == -1:
-                logger.warning(f"cannot find the entity_info : {entity_info}, word_offsets: {word_offsets} ")
+                logger.warning(
+                    f"cannot find the entity_info : {entity_info}, word_offsets: {word_offsets} "
+                )
                 continue
-            for _ in range(start_token_index-cur_token_index):
-                sub_labels.append('O')
-            end_token_index = self.find_position_in_offsets(entity_info['end']-1, word_offsets, word_ids, start_token_index, offset_length)
-            assert end_token_index != -1, f"entity_info: {entity_info}, word_offsets: {word_offsets}"
-            sub_labels.append("B-"+entity_info['labels'][0])
-            for _ in range(end_token_index-start_token_index):
-                sub_labels.append("I-"+entity_info['labels'][0])
+            for _ in range(start_token_index - cur_token_index):
+                sub_labels.append("O")
+            end_token_index = self.find_position_in_offsets(
+                entity_info["end"] - 1,
+                word_offsets,
+                word_ids,
+                start_token_index,
+                offset_length,
+            )
+            assert (
+                end_token_index != -1
+            ), f"entity_info: {entity_info}, word_offsets: {word_offsets}"
+            sub_labels.append("B-" + entity_info["labels"][0])
+            for _ in range(end_token_index - start_token_index):
+                sub_labels.append("I-" + entity_info["labels"][0])
             cur_token_index = end_token_index + 1
-        assert cur_token_index<=offset_length
-        for _ in range(offset_length-cur_token_index):
-            sub_labels.append('O')
+        assert cur_token_index <= offset_length
+        for _ in range(offset_length - cur_token_index):
+            sub_labels.append("O")
 
         if word_ids[0] is None:
             sub_labels[0] = self.config.start_label
 
-        if word_ids[offset_length-1] is None:
-            sub_labels[offset_length-1] = self.config.end_label
+        if word_ids[offset_length - 1] is None:
+            sub_labels[offset_length - 1] = self.config.end_label
 
-        if len(sub_labels)!= len(gather_index):
+        if len(sub_labels) != len(gather_index):
             logger.error(f"{len(sub_labels)} vs {len(gather_index)}")
             for i in one_ins:
                 logger.error(f"{i}")
             raise PermissionError
 
         if not self.config.clean_droped_entity:
-            entities_info = one_ins[self.config.entities_info]
+            entities_info = one_ins[self.config.input_map.entities_info]
         return sub_labels, gather_index, word_ids, word_offsets, entities_info
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dlk-0.0.9/dlk/data/subprocessors/seq_lab_relabel.py` & `dlk-0.1.0/dlk/data/subprocessor/span_cls_relabel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,247 +1,337 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright cstsunfu.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-from numpy import result_type
-from dlk.utils.vocab import Vocabulary
-from dlk.utils.config import BaseConfig, ConfigTool
-from typing import Dict, Callable, Set, List
-from dlk.data.subprocessors import subprocessor_register, subprocessor_config_register, ISubProcessor
-from functools import partial
-from dlk.utils.logger import Logger
+import logging
+import os
+from typing import Callable, Dict, List, Set
+
+import numpy as np
 import pandas as pd
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
+from dlk.utils.vocab import Vocabulary
 
-logger = Logger.get_logger()
+from . import BaseSubProcessor, BaseSubProcessorConfig
+
+logger = logging.getLogger(__name__)
 
-@subprocessor_config_register('seq_lab_relabel')
-class SeqLabRelabelConfig(BaseConfig):
-    """Config for SeqLabRelabel
-
-    Config Example:
-        >>> {
-        >>>     "_name": "seq_lab_relabel",
-        >>>     "config": {
-        >>>         "train":{ //train、predict、online stage config,  using '&' split all stages
-        >>>             "input_map": {  // without necessery, don't change this
-        >>>                 "word_ids": "word_ids",
-        >>>                 "offsets": "offsets",
-        >>>                 "entities_info": "entities_info",
-        >>>             },
-        >>>             "data_set": {                   // for different stage, this processor will process different part of data
-        >>>                 "train": ['train', 'valid', 'test'],
-        >>>                 "predict": ['predict'],
-        >>>                 "online": ['online']
-        >>>             },
-        >>>             "output_map": {
-        >>>                 "labels": "labels",
-        >>>             },
-        >>>             "drop": "shorter", //'longer'/'shorter'/'none', if entities is overlap, will remove by rule
-        >>>             "start_label": "S",
-        >>>             "end_label": "E",
-        >>>             "clean_droped_entity": true, // after drop entity for training, whether drop the entity for calc metrics, default is true, this only works when the drop != 'none'
-        >>>             "entity_priority": [],
-        >>>             //"entity_priority": ['Product'],
-        >>>             "priority_trigger": 1, // if the overlap entity abs(length_a - length_b)<=priority_trigger, will trigger the entity_priority strategy
-        >>>         }, //3
-        >>>         "predict": "train",
-        >>>         "online": "train",
-        >>>     }
-        >>> }
-    """
-    def __init__(self, stage, config: Dict):
 
-        super(SeqLabRelabelConfig, self).__init__(config)
-        self.config = ConfigTool.get_config_by_stage(stage, config)
-        self.data_set = self.config.get('data_set', {}).get(stage, [])
-        if not self.data_set:
-            return
-        self.word_ids = self.config['input_map']['word_ids']
-        self.offsets = self.config['input_map']['offsets']
-        self.entities_info = self.config['input_map']['entities_info']
-        self.clean_droped_entity = self.config['clean_droped_entity']
-        self.drop = self.config['drop']
-        self.start_label = self.config['start_label']
-        self.end_label = self.config['end_label']
-        self.output_labels = self.config['output_map']['labels']
-        self.entity_priority = {entity: priority for priority, entity in enumerate(self.config['entity_priority'])}
-        self.priority_trigger = self.config['priority_trigger']
-        self.post_check(self.config, used=[
-            "input_map",
-            "data_set",
-            "drop",
-            "output_map",
-            "start_label",
-            "end_label",
-            "clean_droped_entity",
-            "entity_priority",
-            "priority_trigger",
-        ])
+@cregister("subprocessor", "span_cls_relabel")
+class SpanClsRelabelConfig(BaseSubProcessorConfig):
+    """the span classification relabel subprocessor"""
+
+    train_data_set = ListField(
+        value=["train", "valid", "test"],
+        suggestions=[["train", "valid", "test"]],
+        help="the data set should be processed for train stage",
+    )
+
+    class InputMap:
+        word_ids = StrField(value="word_ids", help="the word ids")
+        offsets = StrField(value="offsets", help="the offsets")
+        entities_info = StrField(value="entities_info", help="the entities info")
+
+    input_map = NestField(
+        value=InputMap,
+        help="the input map of the processor, the key is the name of the processor needed key, the value is the provided data provided key",
+    )
+
+    class OutputMap:
+        label_ids = StrField(value="label_ids", help="the label ids")
+        processed_entities_info = StrField(
+            value="processed_entities_info", help="the processed entities info"
+        )
+
+    output_map = NestField(
+        value=OutputMap,
+        help="the output map of the processor, the key is the name of the processor provided key, the value is the nexted processor needed key",
+    )
+    drop = StrField(
+        value="shorter",
+        options=["longer", "shorter", "none"],
+        help="the drop strategy for the overlap entities",
+    )
+    vocab = StrField(value="label_vocab.json", help="the vocab for the label")
+
+    entity_priority = ListField(
+        value=[],
+        suggestions=[["Product", "Brand"]],
+        help="the entity priority, when conflict, will keep the entity with the highest priority",
+    )
+    priority_trigger = IntField(
+        value=1,
+        help="if the overlap entity abs(length_a - length_b)<=priority_trigger, will trigger the entity_priority strategy",
+    )
+    mask_fill = IntField(value=-100, help="the mask fill for the label")
+    mask_first_sent = BoolField(
+        value=False, help="whether mask the first sentence for anwering"
+    )
+    null_to_zero_index = BoolField(
+        value=False,
+        help="if cannot find the entity, set to point to the first(zero) index token",
+    )
+    strict = BoolField(
+        value=True, help="if strict == True, will drop the invalid sample"
+    )
 
 
-@subprocessor_register('seq_lab_relabel')
-class SeqLabRelabel(ISubProcessor):
+@register("subprocessor", "span_cls_relabel")
+class SpanClsRelabel(BaseSubProcessor):
     """
-    Relabel the json data to bio
+    Relabel the char level entity span to token level and construct matrix
     """
 
-    def __init__(self, stage: str, config: SeqLabRelabelConfig):
-        super().__init__()
+    def __init__(self, stage: str, config: SpanClsRelabelConfig, meta_dir: str):
+        super().__init__(stage, config, meta_dir)
         self.stage = stage
         self.config = config
-        self.data_set = config.data_set
-        if not self.data_set:
-            logger.info(f"Skip 'seq_lab_relabel' at stage {self.stage}")
-            return
+        self.vocab: Vocabulary = None
+        self.entity_priority = {
+            entity: priority
+            for priority, entity in enumerate(self.config.entity_priority)
+        }
+
+    def load_meta(self):
+        self.loaded_meta = True
+        self.vocab = Vocabulary.load_from_file(
+            os.path.join(self.meta_dir, self.config.vocab)
+        )
+        assert (
+            self.vocab.word2idx[self.vocab.unknown] == 0
+        ), f"For span_cls_relabel, 'unknown' must be index 0, and other labels as 1...num_label"
+        assert (
+            not self.vocab.pad
+        ), f"For span_cls_relabel, 'pad' must be index 0, and other labels as 1...num_label"
 
-    def process(self, data: Dict)->Dict:
-        """SeqLabRelabel Entry
+    def process(self, data: pd.DataFrame, deliver_meta: bool) -> pd.DataFrame:
+        """firstpiece relabel the data
 
         Args:
-            data: Dict
-
-        Returns: 
-            
-            relabeled data
+            data: one is like
 
+            >>> {
+            >>>     "uuid": '**-**-**-**'
+            >>>     "sentence": "Mie Merah - Buah Bit",
+            >>>     "offsets": see the offsets in fast_tokenizer
+            >>>     "entities_info": [
+            >>>                 {
+            >>>                     "end": 9,
+            >>>                     "start": 0,
+            >>>                     "labels": [
+            >>>                         "Product"
+            >>>                     ]
+            >>>                 },
+            >>>             ]
+            >>>         },
+            >>>     ],
+            >>> },
+
+            deliver_meta:
+                ignore
+        Returns:
+            relabeld data
         """
+        if not self.loaded_meta:
+            self.load_meta()
 
-        if not self.data_set:
-            return data
-
-        for data_set_name in self.data_set:
-            if data_set_name not in data['data']:
-                logger.info(f'The {data_set_name} not in data. We will skip do seq_lab_relabel on it.')
-                continue
-            data_set = data['data'][data_set_name]
-            data_set[[self.config.output_labels,
-                self.config.entities_info
-            ]] = data_set.parallel_apply(self.relabel, axis=1, result_type='expand')
+        data[
+            [
+                self.config.output_map.label_ids,
+                self.config.output_map.processed_entities_info,
+            ]
+        ] = data.apply(self.relabel, axis=1, result_type="expand")
+        if self.config.strict:
+            data.dropna(axis=0, inplace=True)
+            data.reset_index(inplace=True)
 
         return data
 
-    def find_position_in_offsets(self, position: int, offset_list: List, sub_word_ids: List, start: int, end: int, is_start: bool=False):
+    def find_position_in_offsets(
+        self,
+        position: int,
+        offset_list: List,
+        sub_word_ids: List,
+        start: int,
+        end: int,
+        is_start: bool = False,
+    ):
         """find the sub_word index which the offset_list[index][0]<=position<offset_list[index][1]
 
         Args:
             position: position
             offset_list: list of all tokens offsets
             sub_word_ids: word_ids from tokenizer
             start: start search index
             end: end search index
             is_start: is the position is the start of target token, if the is_start==True and cannot find return -1
 
-        Returns: 
+        Returns:
             the index of the offset which include position
 
         """
-        while start<end:
+        while start < end:
             if sub_word_ids[start] is None:
                 start += 1
-            elif position>=offset_list[start][0] and position<offset_list[start][1]:
+            elif position >= offset_list[start][0] and position < offset_list[start][1]:
                 return start
-            elif position<offset_list[start][0]:
+            elif position < offset_list[start][0]:
                 if start == 1 and offset_list[0] == [0, 0]:
                     return 1
                 if is_start:
                     return -1
                 else:
                     return start - 1
             else:
                 start += 1
         return -1
 
     def relabel(self, one_ins: pd.Series):
-        """make token label, if use the first piece label please use the 'seq_lab_firstpiece_relabel'
+        """make token label, if use the first piece label please use the 'span_cls_firstpiece_relabel'
 
         Args:
             one_ins: include sentence, entity_info, offsets
 
-        Returns: 
+        Returns:
             labels(labels for each subtoken)
-
+            entities_info
+            processed_entities_info: for relation relabal
         """
-        pre_clean_entities_info = one_ins[self.config.entities_info]
-        pre_clean_entities_info.sort(key=lambda x: x['start'])
-        offsets = one_ins[self.config.offsets]
-        sub_word_ids = one_ins[self.config.word_ids]
-        if not sub_word_ids:
-            logger.warning(f"entity_info: {pre_clean_entities_info}, offsets: {offsets} ")
+        pre_clean_entities_info: List = one_ins[self.config.input_map.entities_info]
+        if self.config.drop != "none":
+            pre_clean_entities_info.sort(key=lambda x: x["start"])
+        offsets: List = one_ins[self.config.input_map.offsets]
+        sub_word_ids: List = one_ins[self.config.input_map.word_ids]
+
+        if self.config.mask_first_sent:
+            first_start = sub_word_ids.index(0)
+            second_start = sub_word_ids[first_start + 1 :].index(0)
+            mask_first_index = first_start + second_start + 2
+        else:
+            mask_first_index = 0  # if there is only one sentence, set to 0
 
         entities_info = []
         pre_end = -1
         pre_length = 0
-        pre_label = ''
+        pre_label = ""
         for entity_info in pre_clean_entities_info:
-            assert len(entity_info['labels']) == 1, f"currently we just support one label for one entity"
-            if entity_info['start']<pre_end: # if overlap will remove one
-                if self.config.drop == 'none':
+            assert (
+                len(entity_info["labels"]) == 1
+            ), f"currently we just support one label for one entity"
+            if entity_info["start"] < pre_end:  # if overlap will remove one
+                if self.config.drop == "none":
                     pass
-                elif abs(entity_info['end'] - entity_info['start'] - pre_length) <= self.config.priority_trigger:
-                    pre_label_order = self.config.entity_priority.get(pre_label, 1e9)
-                    label_order = self.config.entity_priority.get(entity_info['labels'][0], 1e9)
-                    if label_order<pre_label_order:
+                elif (
+                    abs(entity_info["end"] - entity_info["start"] - pre_length)
+                    <= self.config.priority_trigger
+                ):
+                    pre_label_order = self.entity_priority.get(pre_label, 1e9)
+                    label_order = self.entity_priority.get(
+                        entity_info["labels"][0], 1e9
+                    )
+                    if label_order < pre_label_order:
                         entities_info.pop()
                     else:
                         continue
-                elif self.config.drop == 'shorter':
-                    if entity_info['end'] - entity_info['start'] > pre_length:
+                elif self.config.drop == "shorter":
+                    if entity_info["end"] - entity_info["start"] > pre_length:
                         entities_info.pop()
                     else:
                         continue
-                elif self.config.drop =='longer':
-                    if entity_info['end'] - entity_info['start'] < pre_length:
+                elif self.config.drop == "longer":
+                    if entity_info["end"] - entity_info["start"] < pre_length:
                         entities_info.pop()
                     else:
                         continue
                 else:
-                    raise PermissionError(f"The drop method must in 'none'/'shorter'/'longer'")
-                pre_label = entity_info['labels'][0]
+                    raise PermissionError(
+                        f"The drop method must in 'none'/'shorter'/'longer'"
+                    )
+            pre_label = entity_info["labels"][0]
             entities_info.append(entity_info)
-            pre_end = entity_info['end']
-            pre_length = entity_info['end'] - entity_info['start']
+            pre_end = entity_info["end"]
+            pre_length = entity_info["end"] - entity_info["start"]
 
-        cur_token_index = 0
         offset_length = len(offsets)
-        sub_labels = []
-        for entity_info in entities_info:
-            start_token_index = self.find_position_in_offsets(entity_info['start'], offsets, sub_word_ids, cur_token_index, offset_length, is_start=True)
-            if start_token_index == -1:
-                logger.warning(f"cannot find the entity_info : {entity_info}, offsets: {offsets} ")
-                continue
-            for _ in range(start_token_index-cur_token_index):
-                sub_labels.append('O')
-            end_token_index = self.find_position_in_offsets(entity_info['end']-1, offsets, sub_word_ids, start_token_index, offset_length)
-            assert end_token_index != -1, f"entity_info: {entity_info}, offsets: {offsets}"
-            sub_labels.append("B-"+entity_info['labels'][0])
-            for _ in range(end_token_index-start_token_index):
-                sub_labels.append("I-"+entity_info['labels'][0])
-            cur_token_index = end_token_index + 1
-        assert cur_token_index<=offset_length
-        for _ in range(offset_length-cur_token_index):
-            sub_labels.append('O')
 
-        if sub_word_ids[0] is None:
-            sub_labels[0] = self.config.start_label
+        unknown_id = self.vocab.get_index(self.vocab.unknown)
+        mask_matrices = np.full(
+            (offset_length, offset_length), self.config.mask_fill, dtype=np.int8
+        )
+        mask_matrices = np.tril(mask_matrices, k=-1)
+
+        unknown_matrices = np.full(
+            (offset_length, offset_length), unknown_id, dtype=np.int8
+        )
+        unknown_matrices = np.triu(unknown_matrices, k=0)
 
-        if sub_word_ids[offset_length-1] is None:
-            sub_labels[offset_length-1] = self.config.end_label
+        label_matrices = unknown_matrices + mask_matrices
+        if sub_word_ids[0] is None:
+            label_matrices[0, :] = self.config.mask_fill
+        if sub_word_ids[-1] is None:
+            label_matrices[:, -1] = self.config.mask_fill
+
+        if mask_first_index > 0:
+            label_matrices[:mask_first_index, :] = self.config.mask_fill
+            label_matrices[:, :mask_first_index] = self.config.mask_fill
+        processed_entities_info = []
+        for entity_info in entities_info:
+            if entity_info["start"] == 0 and entity_info["end"] == 0:
+                start_token_index, end_token_index = 0, 0
+            else:
+                start_token_index = self.find_position_in_offsets(
+                    entity_info["start"],
+                    offsets,
+                    sub_word_ids,
+                    mask_first_index,
+                    offset_length,
+                    is_start=True,
+                )
+                if start_token_index == -1:
+                    if self.config.null_to_zero_index:
+                        start_token_index, end_token_index = 0, 0
+                    else:
+                        if self.config.strict:
+                            logger.warning(
+                                f"cannot find the entity_info : {entity_info}, offsets: {offsets}, we will drop this instance"
+                            )
+                            return None, None
+                        logger.warning(
+                            f"cannot find the entity_info : {entity_info}, offsets: {offsets}"
+                        )
+                        continue
+                else:
+                    end_token_index = self.find_position_in_offsets(
+                        entity_info["end"] - 1,
+                        offsets,
+                        sub_word_ids,
+                        start_token_index,
+                        offset_length,
+                    )
+                    if self.config.null_to_zero_index and end_token_index == -1:
+                        start_token_index, end_token_index = 0, 0
+            assert (
+                end_token_index != -1
+            ), f"entity_info: {entity_info}, offsets: {offsets}"
+            label_id = self.vocab.get_index(entity_info["labels"][0])
+            label_matrices[start_token_index, end_token_index] = label_id
+            entity_info["sub_token_start"] = start_token_index
+            entity_info["sub_token_end"] = end_token_index
+            processed_entities_info.append(entity_info)
 
-        if len(sub_labels)!= offset_length:
-            logger.error(f"{len(sub_labels)} vs {offset_length}")
-            for i in one_ins:
-                logger.error(f"{i}")
-            raise PermissionError
-
-        if not self.config.clean_droped_entity:
-            entities_info = one_ins[self.config.entities_info]
-        return sub_labels, entities_info
+        return label_matrices, processed_entities_info
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dlk-0.0.9/dlk/data/subprocessors/span_cls_relabel.py` & `dlk-0.1.0/dlk/data/subprocessor/seq_lab_relabel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,239 +1,279 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from dlk.utils.vocab import Vocabulary
-from dlk.utils.config import BaseConfig, ConfigTool
-from typing import Dict, Callable, Set, List
-from dlk.data.subprocessors import subprocessor_register, subprocessor_config_register, ISubProcessor
-from functools import partial
-from dlk.utils.logger import Logger
-import numpy as np
-import pandas as pd
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-logger = Logger.get_logger()
-
-@subprocessor_config_register('span_cls_relabel')
-class SpanClsRelabelConfig(BaseConfig):
-    """Config for SpanClsRelabel
-
-    Config Example:
-        >>> {
-        >>>     "_name": "span_cls_relabel",
-        >>>     "config": {
-        >>>         "train":{ //train、predict、online stage config,  using '&' split all stages
-        >>>             "input_map": {  // without necessery, don't change this
-        >>>                 "word_ids": "word_ids",
-        >>>                 "offsets": "offsets",
-        >>>                 "entities_info": "entities_info",
-        >>>             },
-        >>>             "data_set": {                   // for different stage, this processor will process different part of data
-        >>>                 "train": ['train', 'valid', 'test'],
-        >>>                 "predict": ['predict'],
-        >>>                 "online": ['online']
-        >>>             },
-        >>>             "output_map": {
-        >>>                 "label_ids": "label_ids",
-        >>>             },
-        >>>             "drop": "none", //'longer'/'shorter'/'none', if entities is overlap, will remove by rule
-        >>>             "vocab": "label_vocab", // usually provided by the "token_gather" module
-        >>>             "clean_droped_entity": true, // after drop entity for training, whether drop the entity for calc metrics, default is true, this only works when the drop != 'none'
-        >>>             "entity_priority": [],
-        >>>             //"entity_priority": ['Product'],
-        >>>             "priority_trigger": 1, // if the overlap entity abs(length_a - length_b)<=priority_trigger, will trigger the entity_priority strategy
-        >>>         }, //3
-        >>>         "predict": "train",
-        >>>         "online": "train",
-        >>>     }
-        >>> }
-    """
-    def __init__(self, stage, config: Dict):
+import logging
+from typing import Callable, Dict, List, Set
 
-        super(SpanClsRelabelConfig, self).__init__(config)
-        self.config = ConfigTool.get_config_by_stage(stage, config)
-        self.data_set = self.config.get('data_set', {}).get(stage, [])
-        if not self.data_set:
-            return
-        self.word_ids = self.config['input_map']['word_ids']
-        self.offsets = self.config['input_map']['offsets']
-        self.entities_info = self.config['input_map']['entities_info']
-        self.clean_droped_entity = self.config['clean_droped_entity']
-        self.drop = self.config['drop']
-        self.vocab = self.config['vocab']
-        self.output_labels = self.config['output_map']['label_ids']
-        self.entity_priority = {entity: priority for priority, entity in enumerate(self.config['entity_priority'])}
-        self.priority_trigger = self.config['priority_trigger']
-        self.post_check(self.config, used=[
-            "drop",
-            "vocab",
-            "input_map",
-            "data_set",
-            "output_map",
-            "clean_droped_entity",
-            "entity_priority",
-            "priority_trigger",
-        ])
+import pandas as pd
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.utils.register import register
+
+from . import BaseSubProcessor, BaseSubProcessorConfig
+
+logger = logging.getLogger(__name__)
+
+
+@cregister("subprocessor", "seq_lab_relabel")
+class SeqLabRelabelConfig(BaseSubProcessorConfig):
+    """the sequence labeling relabel subprocessor"""
+
+    train_data_set = ListField(
+        value=["train", "valid", "test"],
+        suggestions=[["train", "valid", "test"]],
+        help="the data set should be processed for train stage",
+    )
+
+    class InputMap:
+        word_ids = StrField(value="word_ids", help="the word ids")
+        offsets = StrField(value="offsets", help="the offsets")
+        entities_info = StrField(value="entities_info", help="the entities info")
+
+    input_map = NestField(
+        value=InputMap,
+        help="the input map of the processor, the key is the name of the processor needed key, the value is the provided data provided key",
+    )
+
+    class OutputMap:
+        labels = StrField(value="labels", help="the label names")
+
+    output_map = NestField(
+        value=OutputMap,
+        help="the output map of the processor, the key is the name of the processor provided key, the value is the nexted processor needed key",
+    )
+    drop = StrField(
+        value="shorter",
+        options=["longer", "shorter", "none"],
+        help="the drop strategy for the overlap entities",
+    )
+    start_label = StrField(value="S", help="the start label")
+    end_label = StrField(value="E", help="the end label")
+    clean_droped_entity = BoolField(
+        value=True, help="whether clean the dropped entity for calc metrics"
+    )
+    entity_priority = ListField(
+        value=[],
+        suggestions=[["Product", "Brand"]],
+        help="the entity priority, when conflict, will keep the entity with the highest priority",
+    )
+    priority_trigger = IntField(
+        value=1,
+        help="if the overlap entity abs(length_a - length_b)<=priority_trigger, will trigger the entity_priority strategy",
+    )
 
 
-@subprocessor_register('span_cls_relabel')
-class SpanClsRelabel(ISubProcessor):
+@register("subprocessor", "seq_lab_relabel")
+class SeqLabRelabel(BaseSubProcessor):
     """
     Relabel the json data to bio
     """
 
-    def __init__(self, stage: str, config: SpanClsRelabelConfig):
-        super().__init__()
+    def __init__(self, stage: str, config: SeqLabRelabelConfig, meta_dir: str):
+        super().__init__(stage, config, meta_dir)
         self.stage = stage
         self.config = config
-        self.data_set = config.data_set
-        if not self.data_set:
-            logger.info(f"Skip 'span_cls_relabel' at stage {self.stage}")
-            return
+        self.entity_priority = {
+            entity: priority
+            for priority, entity in enumerate(self.config.entity_priority)
+        }
 
-    def process(self, data: Dict)->Dict:
-        """SpanClsRelabel Entry
+    def process(self, data: pd.DataFrame, deliver_meta: bool) -> pd.DataFrame:
+        """firstpiece relabel the data
 
         Args:
-            data: Dict
-
-        Returns: 
-            
-            relabeled data
+            data: one is like
 
+            >>> {
+            >>>     "uuid": '**-**-**-**'
+            >>>     "sentence": "Mie Merah - Buah Bit",
+            >>>     "offsets": see the offsets in fast_tokenizer
+            >>>     "entities_info": [
+            >>>                 {
+            >>>                     "end": 9,
+            >>>                     "start": 0,
+            >>>                     "labels": [
+            >>>                         "Product"
+            >>>                     ]
+            >>>                 },
+            >>>             ]
+            >>>         },
+            >>>     ],
+            >>> },
+
+            deliver_meta:
+                ignore
+        Returns:
+            relabeld data
         """
-
-        if not self.data_set:
-            return data
-        self.vocab = Vocabulary.load(data[self.config.vocab])
-
-        for data_set_name in self.data_set:
-            if data_set_name not in data['data']:
-                logger.info(f'The {data_set_name} not in data. We will skip do span_cls_relabel on it.')
-                continue
-            data_set = data['data'][data_set_name]
-            data_set[[self.config.output_labels,
-                self.config.entities_info
-            ]] = data_set.parallel_apply(self.relabel, axis=1, result_type='expand')
-
+        data[
+            [self.config.output_map.labels, self.config.input_map.entities_info]
+        ] = data.apply(self.relabel, axis=1, result_type="expand")
         return data
 
-    def find_position_in_offsets(self, position: int, offset_list: List, sub_word_ids: List, start: int, end: int, is_start: bool=False):
+    def find_position_in_offsets(
+        self,
+        position: int,
+        offset_list: List,
+        sub_word_ids: List,
+        start: int,
+        end: int,
+        is_start: bool = False,
+    ):
         """find the sub_word index which the offset_list[index][0]<=position<offset_list[index][1]
 
         Args:
             position: position
             offset_list: list of all tokens offsets
             sub_word_ids: word_ids from tokenizer
             start: start search index
             end: end search index
             is_start: is the position is the start of target token, if the is_start==True and cannot find return -1
 
-        Returns: 
+        Returns:
             the index of the offset which include position
 
         """
-        while start<end:
+        while start < end:
             if sub_word_ids[start] is None:
                 start += 1
-            elif position>=offset_list[start][0] and position<offset_list[start][1]:
+            elif position >= offset_list[start][0] and position < offset_list[start][1]:
                 return start
-            elif position<offset_list[start][0]:
+            elif position < offset_list[start][0]:
                 if start == 1 and offset_list[0] == [0, 0]:
                     return 1
                 if is_start:
                     return -1
                 else:
                     return start - 1
             else:
                 start += 1
         return -1
 
     def relabel(self, one_ins: pd.Series):
-        """make token label, if use the first piece label please use the 'span_cls_firstpiece_relabel'
+        """make token label, if use the first piece label please use the 'seq_lab_firstpiece_relabel'
 
         Args:
             one_ins: include sentence, entity_info, offsets
 
-        Returns: 
+        Returns:
             labels(labels for each subtoken)
 
         """
-        pre_clean_entities_info = one_ins[self.config.entities_info]
-        pre_clean_entities_info.sort(key=lambda x: x['start'])
-        offsets = one_ins[self.config.offsets]
-        sub_word_ids = one_ins[self.config.word_ids]
+        pre_clean_entities_info = one_ins[self.config.input_map.entities_info]
+        pre_clean_entities_info.sort(key=lambda x: x["start"])
+        offsets: List = one_ins[self.config.input_map.offsets]
+        sub_word_ids: List = one_ins[self.config.input_map.word_ids]
         if not sub_word_ids:
-            logger.warning(f"entity_info: {pre_clean_entities_info}, offsets: {offsets} ")
+            logger.warning(
+                f"entity_info: {pre_clean_entities_info}, offsets: {offsets} "
+            )
 
         entities_info = []
         pre_end = -1
         pre_length = 0
-        pre_label = ''
+        pre_label = ""
         for entity_info in pre_clean_entities_info:
-            assert len(entity_info['labels']) == 1, f"currently we just support one label for one entity"
-            if entity_info['start']<pre_end: # if overlap will remove one
-                if self.config.drop == 'none':
+            assert (
+                len(entity_info["labels"]) == 1
+            ), f"currently we just support one label for one entity"
+            if entity_info["start"] < pre_end:  # if overlap will remove one
+                if self.config.drop == "none":
                     pass
-                elif abs(entity_info['end'] - entity_info['start'] - pre_length) <= self.config.priority_trigger:
-                    pre_label_order = self.config.entity_priority.get(pre_label, 1e9)
-                    label_order = self.config.entity_priority.get(entity_info['labels'][0], 1e9)
-                    if label_order<pre_label_order:
+                elif (
+                    abs(entity_info["end"] - entity_info["start"] - pre_length)
+                    <= self.config.priority_trigger
+                ):
+                    pre_label_order = self.entity_priority.get(pre_label, 1e9)
+                    label_order = self.entity_priority.get(
+                        entity_info["labels"][0], 1e9
+                    )
+                    if label_order < pre_label_order:
                         entities_info.pop()
                     else:
                         continue
-                elif self.config.drop == 'shorter':
-                    if entity_info['end'] - entity_info['start'] > pre_length:
+                elif self.config.drop == "shorter":
+                    if entity_info["end"] - entity_info["start"] > pre_length:
                         entities_info.pop()
                     else:
                         continue
-                elif self.config.drop =='longer':
-                    if entity_info['end'] - entity_info['start'] < pre_length:
+                elif self.config.drop == "longer":
+                    if entity_info["end"] - entity_info["start"] < pre_length:
                         entities_info.pop()
                     else:
                         continue
                 else:
-                    raise PermissionError(f"The drop method must in 'none'/'shorter'/'longer'")
-                pre_label = entity_info['labels'][0]
+                    raise PermissionError(
+                        f"The drop method must in 'none'/'shorter'/'longer'"
+                    )
+                pre_label = entity_info["labels"][0]
             entities_info.append(entity_info)
-            pre_end = entity_info['end']
-            pre_length = entity_info['end'] - entity_info['start']
-            
+            pre_end = entity_info["end"]
+            pre_length = entity_info["end"] - entity_info["start"]
+
         cur_token_index = 0
         offset_length = len(offsets)
-
-        unk_id = self.vocab.get_index(self.vocab.unknown)
-        mask_matrices = np.full((offset_length, offset_length), -1)
-        mask_matrices = np.tril(mask_matrices, k=-1)
-
-        unk_matrices = np.full((offset_length, offset_length), unk_id)
-        unk_matrices = np.triu(unk_matrices, k=0)
-
-        label_matrices = unk_matrices + mask_matrices
-        if sub_word_ids[0] is None:
-            label_matrices[0, 0] = -1
-        if sub_word_ids[-1] is None:
-            label_matrices[-1, -1] = -1
-
+        sub_labels = []
         for entity_info in entities_info:
-            start_token_index = self.find_position_in_offsets(entity_info['start'], offsets, sub_word_ids, cur_token_index, offset_length, is_start=True)
+            start_token_index = self.find_position_in_offsets(
+                entity_info["start"],
+                offsets,
+                sub_word_ids,
+                cur_token_index,
+                offset_length,
+                is_start=True,
+            )
             if start_token_index == -1:
-                logger.warning(f"cannot find the entity_info : {entity_info}, offsets: {offsets} ")
+                logger.warning(
+                    f"cannot find the entity_info : {entity_info}, offsets: {offsets} "
+                )
                 continue
-            end_token_index = self.find_position_in_offsets(entity_info['end']-1, offsets, sub_word_ids, start_token_index, offset_length)
-            assert end_token_index != -1, f"entity_info: {entity_info}, offsets: {offsets}"
-            label_id = self.vocab.get_index(entity_info['labels'][0])
-            label_matrices[start_token_index, end_token_index] = label_id
+            for _ in range(start_token_index - cur_token_index):
+                sub_labels.append("O")
+            end_token_index = self.find_position_in_offsets(
+                entity_info["end"] - 1,
+                offsets,
+                sub_word_ids,
+                start_token_index,
+                offset_length,
+            )
+            assert (
+                end_token_index != -1
+            ), f"entity_info: {entity_info}, offsets: {offsets}"
+            sub_labels.append("B-" + entity_info["labels"][0])
+            for _ in range(end_token_index - start_token_index):
+                sub_labels.append("I-" + entity_info["labels"][0])
+            cur_token_index = end_token_index + 1
+        assert cur_token_index <= offset_length
+        for _ in range(offset_length - cur_token_index):
+            sub_labels.append("O")
+
+        if sub_word_ids[0] is None:
+            sub_labels[0] = self.config.start_label
+
+        if sub_word_ids[offset_length - 1] is None:
+            sub_labels[offset_length - 1] = self.config.end_label
+
+        if len(sub_labels) != offset_length:
+            logger.error(f"{len(sub_labels)} vs {offset_length}")
+            for i in one_ins:
+                logger.error(f"{i}")
+            raise PermissionError
 
         if not self.config.clean_droped_entity:
-            entities_info = one_ins[self.config.entities_info]
-        return label_matrices, entities_info
+            entities_info = one_ins[self.config.input_map.entities_info]
+        return sub_labels, entities_info
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dlk-0.0.9/dlk/data/subprocessors/token_norm.py` & `dlk-0.1.0/dlk/data/postprocessor/txt_reg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,217 +1,236 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright cstsunfu.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
+
+import json
+import logging
+import os
+import pickle as pkl
+from typing import Any, Dict, List, Union
 
-from logging import PercentStyle
-from dlk.utils.vocab import Vocabulary
-from dlk.utils.config import BaseConfig, ConfigTool
-from typing import Dict, Callable, Set, List
-from dlk.data.subprocessors import subprocessor_register, subprocessor_config_register, ISubProcessor
-from functools import partial
 import pandas as pd
-from dlk.utils.logger import Logger
-from tokenizers.models import WordLevel
-from tokenizers import Tokenizer
-from tokenizers.pre_tokenizers import WhitespaceSplit
-
-logger = Logger.get_logger()
-
-@subprocessor_config_register('token_norm')
-class TokenNormConfig(BaseConfig):
-    """Config for TokenNorm 
-
-    Config Example:
-        >>> {
-        >>>     "_name": "token_norm",
-        >>>     "config": {
-        >>>         "train":{
-        >>>             "data_set": {                   // for different stage, this processor will process different part of data
-        >>>                 "train": ['train', 'valid', 'test', 'predict'],
-        >>>                 "predict": ['predict'],
-        >>>                 "online": ['online']
-        >>>             },
-        >>>             "zero_digits_replaced": true,
-        >>>             "lowercase": true,
-        >>>             "extend_vocab": "", //when lowercase is true, this upper_case_vocab will collection all tokens the token is not in vocab but it's lowercase is in vocab. this is only for token gather process
-        >>>             "tokenizer": "whitespace_split",  //the path to vocab(if the token in vocab skip norm it), the file is setted to one token per line
-        >>>             "data_pair": {
-        >>>                 "sentence": "norm_sentence"
-        >>>             },
-        >>>         },
-        >>>         "predict": "train",
-        >>>         "online": "train",
-        >>>     }
-        >>> }
-    """
-    def __init__(self, stage, config: Dict):
-
-        super(TokenNormConfig, self).__init__(config)
-        self.config = ConfigTool.get_config_by_stage(stage, config)
-        self.data_set = self.config.get('data_set', {}).get(stage, [])
-        if not self.data_set:
-            return
-        self.data_pair = self.config.pop('data_pair', {})
-        self.zero_digits_replaced = self.config.pop('zero_digits_replaced', True)
-        self.lowercase = self.config.pop('lowercase', True)
-        self.tokenizer = Tokenizer.from_file(self.config['tokenizer'])
-        self.unk = self.tokenizer.model.unk_token
-        self.vocab = self.tokenizer.get_vocab()
-        self.do_extend_vocab = self.config['extend_vocab']
-        self.prefix = self.tokenizer.model.continuing_subword_prefix
-        self.post_check(self.config, used=[
-            "data_set",
-            "zero_digits_replaced",
-            "lowercase",
-            "extend_vocab",
-            "tokenizer",
-            "data_pair",
-        ])
-
-    def tokenize(self, seq):
-        """TODO: Docstring for whitespace_split.
-        :returns: TODO
-        """
-        encode = self.tokenizer.encode(seq)
-        return encode
+import torch
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+
+from dlk.data.postprocessor import BasePostProcessor, BasePostProcessorConfig
+from dlk.utils.io import open
+from dlk.utils.register import register
+from dlk.utils.vocab import Vocabulary
+
+logger = logging.getLogger(__name__)
+
 
+@cregister("postprocessor", "txt_reg")
+class TxtRegPostProcessorConfig(BasePostProcessorConfig):
+    """postprocess for text regression"""
+
+    class InputMap:
+        logits = StrField(value="logits", help="the output logits")
+        value = StrField(value="values", help="the target value of the sample")
+        index = StrField(value="_index", help="the index of the sample")
+
+    input_map = NestField(
+        value=InputMap,
+        help="the input map of the processor, the key is the name of the processor needed key, the value is the provided data provided key",
+    )
+
+    class OriginInputMap:
+        uuid = StrField(value="uuid", help="the uuid or the id of the sample")
+        sentence = StrField(
+            value="sentence", help="the sentence of the sample(for data_type=single)"
+        )
+        sentence_a = StrField(
+            value="sentence_a", help="the sentence_a of the sample(for data_type=pair)"
+        )
+        sentence_b = StrField(
+            value="sentence_b", help="the sentence_b of the sample(for data_type=pair)"
+        )
+
+    origin_input_map = NestField(
+        value=OriginInputMap,
+        help="the origin input map of the processor, the key is the name of the processor needed key, the value is the provided data provided key",
+    )
+    data_type = StrField(
+        value="single", options=["single", "pair"], help="the data type, single or pair"
+    )
+    log_reg = BoolField(value=False, help="whether to return the log reg")
+
+
+@register("postprocessor", "txt_reg")
+class TxtRegPostProcessor(BasePostProcessor):
+    """text regression postprocess"""
 
-@subprocessor_register('token_norm')
-class TokenNorm(ISubProcessor):
-    """
-    This part could merged to fast_tokenizer(it will save some time), but not all process need this part(except some special dataset like conll2003), and will make the fast_tokenizer be heavy.
-
-    Token norm:
-        Love -> love
-        3281 -> 0000
-    """
-
-    def __init__(self, stage: str, config: TokenNormConfig):
-        super().__init__()
-        self.stage = stage
+    def __init__(self, config: TxtRegPostProcessorConfig):
+        super(TxtRegPostProcessor, self).__init__(config)
         self.config = config
-        self.data_set = config.data_set
-        if not self.data_set:
-            logger.info(f"Skip 'token_norm' at stage {self.stage}")
-            return
-        if self.config.do_extend_vocab:
-            self.extend_vocab = set()
-        self._zero_digits_replaced_num = 0
-        self._lower_case_num = 0
-        self._lower_case_zero_digits_replaced_num = 0
 
-    def token_norm(self, token: str)->str:
-        """norm token, the result len(result) == len(token), exp.  12348->00000
+    def do_predict(
+        self,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+    ) -> List:
+        """Process the model predict to human readable format
 
         Args:
-            token: origin token
-
-        Returns: 
-            normed_token
+            stage: train/test/etc.
+            list_batch_outputs: a list of outputs
+            origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
+            rt_config:
+                >>> current status
+                >>> {
+                >>>     "current_step": self.global_step,
+                >>>     "current_epoch": self.current_epoch,
+                >>>     "total_steps": self.num_training_steps,
+                >>>     "total_epochs": self.num_training_epochs
+                >>> }
 
+        Returns:
+            all predicts
         """
-        if token in self.config.vocab:
-            return token
-
-        if self.config.zero_digits_replaced:
-            norm = ''
-            digit_num = 0
-            for c in token:
-                if c.isdigit() or c=='.':
-                    norm += '0'
-                    digit_num += 1
+        results = []
+        for outputs in list_batch_outputs:
+            logits = outputs[self.config.input_map.logits].detach()
+            if self.config.log_reg:
+                logits = torch.sigmoid(logits)
+            assert len(logits.shape) == 2
+            # predict_indexes = list(torch.argmax(logits, 1))
+            indexes = list(outputs[self.config.input_map.index])
+
+            if self.config.input_map.value in outputs:
+                values = outputs[self.config.input_map.value]
+            else:
+                values = [0.0] * len(indexes)
+            for i, (one_logits, index, value) in enumerate(
+                zip(logits, indexes, values)
+            ):
+                one_ins = {}
+                one_origin = origin_data.iloc[int(index)]
+                if self.config.data_type == "single":
+                    sentence = one_origin[self.config.origin_input_map.sentence]
+                    one_ins["sentence"] = sentence
                 else:
-                    norm += c
-            if norm in self.config.vocab or self.config.prefix+norm in self.config.vocab:
-                self._zero_digits_replaced_num += 1
-                return norm
-            elif self.config.do_extend_vocab and digit_num == len(token) and digit_num<20:
-                self.extend_vocab.add(norm)
-
-        if self.config.lowercase:
-            norm = token.lower()
-            if norm in self.config.vocab or self.config.prefix+norm in self.config.vocab:
-                self._lower_case_num += 1
-                if self.config.do_extend_vocab:
-                    self.extend_vocab.add(token)
-                return norm
-
-        if self.config.lowercase and self.config.zero_digits_replaced:
-            norm = ''
-            for c in token.lower():
-                if c.isdigit() or c=='.':
-                    norm += '0'
-                else:
-                    norm += c
-            if norm in self.config.vocab or self.config.prefix+norm in self.config.vocab:
-                self._lower_case_zero_digits_replaced_num += 1
-                return norm
-        return ''
-
-    def seq_norm(self, key:str, one_item: pd.Series)->str:
-        """norm a sentence, the sentence is from one_item[key]
+                    sentence_a = one_origin[self.config.origin_input_map.sentence_a]
+                    one_ins["sentence_a"] = sentence_a
+                    sentence_b = one_origin[self.config.origin_input_map.sentence_b]
+                    one_ins["sentence_b"] = sentence_b
+
+                uuid = one_origin[self.config.origin_input_map.uuid]
+                one_ins["uuid"] = uuid
+                one_ins["values"] = [float(value)]
+                one_ins["predict_values"] = [float(one_logits)]
+                one_ins["predict_extend_return"] = self.gather_predict_extend_data(
+                    outputs, i, self.config.predict_extend_return
+                )
+                results.append(one_ins)
+        return results
+
+    def do_calc_metrics(
+        self,
+        predicts: List,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+    ) -> Dict:
+        """calc the scores use the predicts or list_batch_outputs
 
         Args:
-            key: the name in one_item
-            one_item: a pd.Series which include the key
+            predicts: list of predicts
 
-        Returns: 
-            norm_sentence
+            stage: train/test/etc.
+            list_batch_outputs: a list of outputs
+            origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
+            rt_config:
+                >>> current status
+                >>> {
+                >>>     "current_step": self.global_step,
+                >>>     "current_epoch": self.current_epoch,
+                >>>     "total_steps": self.num_training_steps,
+                >>>     "total_epochs": self.num_training_epochs
+                >>> }
 
-        """
-        seq = one_item[key]
-        norm_seq = [c for c in seq]
-        encode = self.config.tokenize(seq)
-        for i, token in enumerate(encode.tokens):
-            if token == self.config.unk:
-                token_offset = encode.offsets[i]
-                prenorm_token = seq[token_offset[0]: token_offset[1]]
-                norm_token = self.token_norm(prenorm_token)
-                if not norm_token:
-                    continue
-                assert len(norm_token) == token_offset[1] - token_offset[0], f"Prenorm '{prenorm_token}', postnorm: '{norm_token}' and {len(norm_token)}!= {token_offset[1]} - {token_offset[0]}"
-                norm_seq[token_offset[0]: token_offset[1]] = norm_token
-        return ''.join(norm_seq)
+        Returns:
+            the named scores, acc
 
-    def process(self, data: Dict)->Dict:
-        """TokenNorm entry
+        """
+        ses = []
+        for one_ins in predicts:
+            values = one_ins["values"]
+            assert (
+                len(values) == 1
+            ), "We currently is not support multi values in regression postprocess"
+            value = values[0]
+
+            one_predicts = one_ins["predict_values"]
+            predict_value = one_predicts[0]
+            ses.append((predict_value - value) ** 2)
+        real_name = self.loss_name_map(stage)
+        return {f"{real_name}_mse": sum(ses) / len(ses)}
+
+    def do_save(
+        self,
+        predicts: List,
+        stage: str,
+        list_batch_outputs: List[Dict],
+        origin_data: pd.DataFrame,
+        rt_config: Dict,
+        save_condition: bool = False,
+    ):
+        """save the predict when save_condition==True
 
         Args:
-            data: 
-            {
-                "data": {"train": ...},
-                "tokenizer": ..
-            }
+            predicts: list of predicts
+            stage: train/test/etc.
+            list_batch_outputs: a list of outputs
+            origin_data: the origin pd.DataFrame data, there are some data not be able to convert to tensor
+            rt_config:
+                >>> current status
+                >>> {
+                >>>     "current_step": self.global_step,
+                >>>     "current_epoch": self.current_epoch,
+                >>>     "total_steps": self.num_training_steps,
+                >>>     "total_epochs": self.num_training_epochs
+                >>> }
+            save_condition: True for save, False for depend on rt_config
 
-        Returns: 
-            norm data
+        Returns:
+            None
         """
 
-        if not self.data_set:
-            return data
-
-        for data_set_name in self.data_set:
-            if data_set_name not in data['data']:
-                logger.info(f'The {data_set_name} not in data. We will skip do token_norm on it.')
-                continue
-            data_set = data['data'][data_set_name]
-
-            for key, value in self.config.data_pair.items():
-                _seq_norm = partial(self.seq_norm, key)
-                data_set[value] = data_set.apply(_seq_norm, axis=1)
-                # WARNING: if you change the apply to parallel_apply, you should change the _zero_digits_replaced_num, etc. to multiprocess safely(BTW, use parallel_apply in tokenizers==0.10.3 will make the process very slow)
-                # data_set[value] = data_set.apply(_seq_norm, axis=1)
-        logger.info(f"We use zero digits to replace digit token num is {self._zero_digits_replaced_num}, do lowercase token num is {self._lower_case_num}, do both num is {self._lower_case_zero_digits_replaced_num}")
-        if self.config.do_extend_vocab:
-            logger.info(f"We will extend {len(self.extend_vocab)} tokens and deliver to {self.config.do_extend_vocab}")
-            data[self.config.do_extend_vocab] = list(self.extend_vocab)
-        return data
+        if self.config.start_save_epoch == -1 or self.config.start_save_step == -1:
+            self.config.start_save_step = rt_config.get("total_steps", 0) - 1
+            self.config.start_save_epoch = rt_config.get("total_epochs", 0) - 1
+        if not save_condition and (
+            rt_config["current_step"] >= self.config.start_save_step
+            or rt_config["current_epoch"] >= self.config.start_save_epoch
+        ):
+            save_condition = True
+        if save_condition:
+            save_path = os.path.join(
+                self.config.save_root_path, self.config.save_dir.get(stage, "")
+            )
+            if "current_step" in rt_config:
+                save_file = os.path.join(
+                    save_path, f"step_{str(rt_config['current_step'])}_predict.json"
+                )
+            else:
+                save_file = os.path.join(save_path, "predict.json")
+            logger.info(f"Save the {stage} predict data at {save_file}")
+            with open(save_file, "w") as f:
+                json.dump(predicts, f, indent=4, ensure_ascii=False)
```

### Comparing `dlk-0.0.9/dlk/train.py` & `dlk-0.1.0/dlk/predict.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,207 +1,202 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-import hjson
+import copy
+import json
+import logging
 import os
-from typing import Dict, Union, Callable, List, Any
-from dlk.utils.parser import BaseConfigParser
-from dlk.utils.config import ConfigTool
-from dlk.data.datamodules import datamodule_register, datamodule_config_register
-from dlk.managers import manager_register, manager_config_register
-from dlk.core.imodels import imodel_register, imodel_config_register
 import pickle as pkl
 import uuid
-import json
-from dlk.utils.logger import Logger
-import logging
+from typing import Any, Callable, Dict, List, Union
 
-logger = Logger.get_logger()
+import hjson
+import torch
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    Parser,
+    StrField,
+    SubModule,
+    cregister,
+    init_config,
+)
+
+from dlk.train import DLKFitConfig
+from dlk.utils.io import open
+from dlk.utils.register import register, register_module_name
+
+logger = logging.getLogger(__name__)
 
 
-class Train(object):
-    """Trainer
+class Predict(object):
+    """Predict
 
     Config Example:
-        >>> {
-        >>>     "_focus": {
-        >>>     },
-        >>>     "_link": {},
-        >>>     "_search": {},
-        >>>     "config": {
-        >>>         "save_dir": "*@*",  # must be provided
-        >>>         "data_path": "*@*",  # must be provided
-        >>>     },
-        >>>     "task": {
-        >>>         "_name": task_name
-        >>>         ...
-        >>>     }
-        >>> }
     """
 
-    def __init__(self, config: Union[str, Dict], ckpt: str=""):
-        super(Train, self).__init__()
+    def __init__(self, config: Union[str, dict], checkpoint: str):
+        super(Predict, self).__init__()
+        config_dict = {}
+        self.online = False
         if not isinstance(config, dict):
-            config = hjson.load(open(config), object_pairs_hook=dict)
+            with open(config, "r") as f:
+                config_dict = hjson.load(f, object_pairs_hook=dict)
+        else:
+            config_dict = config
+        if isinstance(checkpoint, str):
+            with open(checkpoint, "rb") as f:
+                self.checkpoint = torch.load(f, map_location=torch.device("cpu"))
+        else:
+            self.checkpoint = torch.load(checkpoint, map_location=torch.device("cpu"))
+        dlk_config, name_str = self.get_config(config_dict)
+        self.dlk_config = dlk_config
+        self.init(dlk_config, name_str)
 
-        self.ckpt = ckpt
-        self.focus = config.pop('_focus', {})
-        self.configs = BaseConfigParser(config).parser_with_check()
-        if self.ckpt:
-            assert len(self.configs) == 1, f"Reuse the checkpoint(ckpt is not none), you must provide the (only one) config which generate the checkpoint."
-
-        self.config_names = []
-        for possible_config in self.configs:
-            config_name = []
-            for source, to in self.focus.items():
-                config_point = possible_config
-                trace = source.split('.')
-                for t in trace:
-                    config_point = config_point[t]
-                config_name.append(to+str(config_point))
-            if config_name:
-                self.config_names.append('_'.join(config_name))
-            else:
-                self.config_names.append(possible_config['root']['_name'])
-
-        if len(self.config_names) != len(set(self.config_names)):
-            for config, name in zip(self.configs, self.config_names):
-                logger.info(f"{name}:\n{json.dumps(config, indent=4, ensure_ascii=False)}")
-            raise NameError('The config_names is not unique.')
+    def get_config(self, config_dict):
+        """get the predict config
 
-    def run(self):
-        """run for all configs
-
-        Returns: 
-            None
+        Args:
+            config: the init config
 
+        Returns:
+            DLKFitConfig, config_name_str
         """
-        logger.info(f"You have {len(self.config_names)} training config(s), they all will be run.")
-        for i, (config, name) in enumerate(zip(self.configs, self.config_names)):
-            logger.info(f"Runing the {i}th {name}...")
-            self.run_oneturn(config, name)
+        configs = Parser(config_dict).parser_init()
+        assert len(configs) == 1, f"You should not use '_search' for predict/online"
 
-    def dump_config(self, config: Dict, name: str):
-        """dump the config and change the log file path to config['config']['save_dir']+name
+        fit_config: DLKFitConfig = configs[0]["@fit"]
 
-        Args:
-            config: {"config": {"save_dir": '..'}}
-            name: config name
+        config_name_str = "predict"
+        return fit_config, config_name_str
 
-        Returns: 
-            None
+    def init(self, config, name):
+        """init the model and trainer
+        Args:
+            config: the config
+            name: the name of the config
 
+        Returns: None
         """
-        log_path = os.path.join(config.get('config').get('save_dir'), name)
-        os.makedirs(log_path, exist_ok=True)
-        json.dump({"root":config, "_focus": self.focus}, open(os.path.join(config.get('config').get('save_dir'), name, "config.json"), 'w'), ensure_ascii=False, indent=4)
-        Logger.init_file_logger("log.txt", log_path)
+        # set trainer
+        self.trainer = self.get_trainer(config, name)
+
+        # init imodel and inject the origin test and valid data
+        self.imodel = self.get_imodel(config)
 
-    def run_oneturn(self, config, name):
-        """run this config
+    def predict(self, data=None, save_condition=False):
+        """init the model, datamodule, manager then predict the predict_dataloader
 
         Args:
-            config: {"root": '...'}
-            name: config name
+            data: if provide will not load from data_path
 
-        Returns: 
+        Returns:
             None
 
         """
-
-        config = config['root']
-        # save configure
-        self.dump_config(config, name)
-
-        # get data
-        data = self.get_data(config)
-
         # set datamodule
-        datamodule = self.get_datamodule(config, data)
-
-        # set training manager
-        manager = self.get_manager(config, name)
-
-        # init imodel and inject the origin test and valid data
-        imodel = self.get_imodel(config, data)
-
-        # start training
-        manager.fit(model=imodel, datamodule=datamodule)
-        manager.test(model=imodel, datamodule=datamodule)
+        datamodule, data = self.get_datamodule(
+            self.dlk_config, data, world_size=self.trainer.world_size
+        )
+
+        # start predict
+        with torch.no_grad():
+            predict_result = self.trainer.predict(
+                model=self.imodel, datamodule=datamodule
+            )
+        return self.imodel.postprocessor(
+            stage="predict",
+            list_batch_outputs=predict_result,
+            origin_data=data["predict"],
+            rt_config={},
+            save_condition=save_condition,
+        )
 
     def get_data(self, config):
         """get the data decided by config
 
         Args:
             config: {"config": {"data_path": '..'}}
 
-        Returns: 
+        Returns:
             loaded data
 
         """
-        self.data = pkl.load(open(config['config']['data_path'], 'rb')).get('data', {})
-        return self.data
+        data = {}
+        for data_type in ["predict"]:
+            data_path = os.path.join(config.processed_data_dir, data_type, "0.pkl")
+            if os.path.exists(data_path):
+                with open(data_path, "rb") as f:
+                    data[data_type] = pkl.load(f)
+        return data
 
-    def get_datamodule(self, config, data):
+    def get_datamodule(self, config, data, world_size):
         """get the datamodule decided by config, and fit the data to datamodule
 
         Args:
             config: {"task": {"datamodule": '..'}}
             data: {"train": '..', 'valid': '..', ..}
 
-        Returns: 
+        Returns:
             datamodule
 
         """
-        DataModule, DataModuleConfig = ConfigTool.get_leaf_module(datamodule_register, datamodule_config_register, 'datamodule', config['task']['datamodule'])
-        datamodule = DataModule(DataModuleConfig, data)
-        return datamodule
+        if not data and not self.online:
+            data = self.get_data(config)
+        datamodule_configs = config._get_modules("datamodule")
+        assert len(datamodule_configs) == 1, "Currently only support one datamodule"
+        data_module_config = datamodule_configs[0]
+        data_module_name = register_module_name(data_module_config._module_name)
+        datamodule = register.get("datamodule", data_module_name)(
+            data_module_config, data, {"world_size": world_size}
+        )
+        return datamodule, data
 
-    def get_manager(self, config, name):
-        """get the tranin/predict manager decided by config
+    def get_trainer(self, config: DLKFitConfig, name):
+        """get the train/predict manager decided by config
 
         Args:
-            config: {"task": {"manager": '..'}, "config": {"save_dir"}}
+            config: DLKFitConfig
             name: the predict progress name
 
-        Returns: 
-            manager
+        Returns:
+            trainer
 
         """
-        Manager, ManagerConfig = ConfigTool.get_leaf_module(manager_register, manager_config_register, 'manager', config.get('task').get('manager'))
-        manager = Manager(ManagerConfig, rt_config={"save_dir": config.get('config').get("save_dir"), "name": name})
-        return manager
+        trainer_configs = config._get_modules("trainer")
+        assert len(trainer_configs) == 1, "Currently only support one trainer"
+        trainer_config = trainer_configs[0]
+        trainer_name = register_module_name(trainer_config._module_name)
+        trainer = register.get("trainer", trainer_name)(
+            trainer_config, rt_config={"log_dir": config.log_dir, "name": name}
+        )
+        return trainer
 
-    def get_imodel(self, config, data):
-        """get the imodel decided by config, and inject the origin test and valid data
+    def get_imodel(self, config):
+        """get the imodel decided by config
 
         Args:
-            config: {"task": {"imodel": '..'}}
-            data: {"train": '..', 'valid': '..', ..}
 
-        Returns: 
+        Returns:
             imodel
 
         """
-        IModel, IModelConfig = ConfigTool.get_leaf_module(imodel_register, imodel_config_register, 'imodel', config.get('task').get('imodel'))
-        imodel = IModel(IModelConfig)
-        if self.ckpt:
-            logger.info(f"reuse the checkpoint at {self.ckpt}")
-            imodel.load_from_checkpoint(self.ckpt)
-        if 'valid' in data:
-            imodel._origin_valid_data = data['valid']
-
-        if 'test' in data:
-            imodel._origin_test_data = data['test']
-
+        imodel_configs = config._get_modules("imodel")
+        assert (
+            len(imodel_configs) == 1
+        ), f"Currently only support one imodel, {imodel_configs}"
+        imodel_config = imodel_configs[0]
+        imodel_name = register_module_name(imodel_config._module_name)
+        imodel = register.get("imodel", imodel_name)(imodel_config, checkpoint=True)
+        if self.checkpoint:
+            imodel.load_state_dict(self.checkpoint["state_dict"], strict=True)
+        imodel.eval()
         return imodel
```

### Comparing `dlk-0.0.9/dlk/utils/vocab.py` & `dlk-0.1.0/dlk/utils/vocab.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,232 +1,262 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
+import json
 from collections import Counter
 from typing import Dict, Iterable, List, Union
+
 import pandas as pd
 
+from dlk.utils.io import open
+
 
 class Vocabulary(object):
     """generate vocab from tokens(token or Iterable tokens)
-       you can dumps the object to dict and load from dict
+    you can dumps the object to dict and load from dict
     """
 
-    def __init__(self, do_strip: bool=False, unknown: str='', ignore: str="", pad: str=''):
+    def __init__(
+        self, do_strip: bool = False, unknown: str = "", ignore: str = "", pad: str = ""
+    ):
         self.word2idx = {}
         self.idx2word = {}
         self.do_strip = do_strip
         self.word_num = 0
-        self.word_count = Counter() # reserved
+        self.word_count = Counter()  # reserved
         self.unknown = unknown
         self.ignore = ignore
         self.pad = pad
         if ignore:
-            self.word2idx[ignore] = -1
-            self.idx2word[-1] = ignore
+            self.word2idx[ignore] = -100
+            self.idx2word[-100] = ignore
             self.word_count[ignore] += int(1e10)
         if pad:
             assert self.word_num == 0, f"The pad id must be 0"
             self.word_count[pad] += int(1e10)
             self.word2idx[pad] = self.word_num
             self.idx2word[self.word_num] = pad
             self.word_num += 1
         if unknown:
             self.word_count[unknown] += int(1e10)
             self.word2idx[unknown] = self.word_num
             self.idx2word[self.word_num] = unknown
             self.word_num += 1
 
-    def dumps(self)->Dict:
+    def dumps(self) -> Dict:
         """dumps the object to dict
 
-        Returns: 
+        Returns:
             self.__dict__
 
         """
         return self.__dict__
 
+    def dump(self, path: str):
+        """dump the object to path
+
+        Returns:
+            self.__dict__
+
+        """
+        with open(path, "w", encoding="utf-8") as f:
+            json.dump(self.__dict__, f)
+
     @classmethod
     def load(cls, attr: Dict):
         """load the object from dict
 
         Args:
             attr: self.__dict__
 
-        Returns: 
+        Returns:
+            initialized Vocabulary
+
+        """
+        vocab = cls()
+        vocab.__dict__ = attr
+        return vocab
+
+    @classmethod
+    def load_from_file(cls, path: str):
+        """load the object from path
+
+        Args:
+            path: a json file
+
+        Returns:
             initialized Vocabulary
 
         """
+        with open(path, "r", encoding="utf-8") as f:
+            attr = json.load(f)
         vocab = cls()
         vocab.__dict__ = attr
+        id2word = vocab.idx2word
+        vocab.idx2word = {int(i): id2word[i] for i in id2word}
         return vocab
 
     def __getitem__(self, index: int):
         """get the token by index
 
         Args:
             index: token index
 
-        Returns: 
+        Returns:
             `word` which index is geven, if index is not out of range
 
         Raises:
             KeyError
 
         """
-        try:
-            return self.idx2word[int(index)]
-        except:
-            raise KeyError('Undefined index: {}'.format(index))
+        return self.idx2word[int(index)]
 
     def auto_get_index(self, data: Union[str, List]):
         """get the index of word ∈data from this vocab
 
         Args:
             data: auto detection
 
-        Returns: 
+        Returns:
             type the same as data
 
         """
         if isinstance(data, str):
             return self.get_index(data)
         elif isinstance(data, list):
             return [self.auto_get_index(subdata) for subdata in data]
         else:
             raise ValueError("Don't support the type of {}".format(data))
 
-    def get_index(self, word: str)->int:
+    def get_index(self, word: str) -> int:
         """get the index of word from this vocab
 
         Args:
             word: a single token
 
-        Returns: 
+        Returns:
             index
 
         """
         if self.do_strip:
             word = word.strip()
         try:
             return self.word2idx[word]
         except:
             if self.unknown:
                 return self.word2idx[self.unknown]
             else:
-                raise KeyError('Unkown word: {}'.format(word))
+                raise KeyError("Unkown word: {}".format(word))
 
     def filter_rare(self, min_freq=1, most_common=-1):
         """filter the words which count is to small.
 
         min_freq and most_common can not set all
 
         Args:
             min_freq: minist frequency
             most_common: most common number, -1 means all
 
-        Returns: 
+        Returns:
             None
 
         """
         self.word2idx = {}
         self.idx2word = {}
-        assert min_freq == 1 or most_common==-1, "You should set the min_freq=1 or most_common=-1."
+        assert (
+            min_freq == 1 or most_common == -1
+        ), "You should set the min_freq=1 or most_common=-1."
         if most_common != -1:
             for i, (token, freq) in enumerate(self.word_count.most_common(most_common)):
                 self.word2idx[token] = i
                 self.idx2word[i] = token
         else:
             index = 0
             for token in self.word_count:
-                if self.word_count[token]>=min_freq:
+                if self.word_count[token] >= min_freq:
                     self.word2idx[token] = index
                     self.idx2word[index] = token
                     index += 1
+        return self
 
-    def get_word(self, index: int)->str:
+    def get_word(self, index: int) -> str:
         """get the word by index
 
         Args:
             index: word index
 
-        Returns: 
+        Returns:
             word
 
         """
-        
+
         try:
             return self.idx2word[int(index)]
         except:
             if index == -1:
-                return '[unknown]'
-            raise KeyError('Undefined index: {}'.format(index))
+                return "[unknown]"
+            raise KeyError("Undefined index: {}".format(index))
 
     def add(self, word):
         """add one word to vocab
 
         Args:
             word: single word
 
-        Returns: 
+        Returns:
             self
 
         """
-        
+
         if not self.word_count[word]:
             self.word2idx[word] = self.word_num
             self.idx2word[self.word_num] = word
             self.word_num += 1
         self.word_count[word] += 1
         return self
 
     def auto_update(self, data: Union[str, Iterable]):
         """auto detect data type to update the vocab
 
         Args:
             data:  str| List[str] | Set[str] | List[List[str]]
 
-        Returns: 
+        Returns:
             self
 
         """
         if isinstance(data, str):
             self.add(data)
-        elif isinstance(data, list) or isinstance(data, set) or isinstance(data, pd.Series):
+        elif (
+            isinstance(data, list)
+            or isinstance(data, set)
+            or isinstance(data, pd.Series)
+        ):
             self.add_from_iter(data)
         else:
             raise ValueError("Don't support the type of {}".format(data))
         return self
 
     def __len__(self):
         """get the token num of vocab
-        Returns: 
+        Returns:
             len(self.word2idx)
 
         """
         return len(self.word2idx)
 
     def add_from_iter(self, iterator):
         """add the tokens in iterator to vocab
 
         Args:
             iterator: List[str] | Set[str] | List[List[str]]
 
-        Returns: 
+        Returns:
             self
 
         """
         for word in iterator:
             if isinstance(word, list) or isinstance(word, set):
                 self.add_from_iter(word)
             elif isinstance(word, str):
```

### Comparing `dlk-0.0.9/tools/word2vec/word2vec.py` & `dlk-0.1.0/dlk/callback/progress_bar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,182 +1,170 @@
-# Copyright 2021 cstsunfu. All rights reserved.
+# Copyright the author(s) of DLK.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import multiprocessing
-from gensim.models import Word2Vec
-from gensim.models.callbacks import CallbackAny2Vec
-import hjson
-import time
-import argparse
-import numpy as np
-# Data from https://pytorch.org/text/_modules/torchtext/datasets/language_modeling.html
-from gensim.models.word2vec_inner import MAX_WORDS_IN_BATCH
-import logging
-
-logging.basicConfig(format='%(asctime)s : %(levelname)s : %(message)s', level=logging.WARNING)
-
-
-def any2unicode(text, encoding: str='utf8', errors: str='strict'):
-    """Convert `text` (bytestring in given encoding or unicode) to unicode.
-
-    Args:
-        text : Input text.
-        errors : str, optional
-            Error handling behaviour if `text` is a bytestring.
-        encoding : str, optional
-            Encoding of `text` if it is a bytestring.
-
-    Returns:
-        Unicode version of `text`.
-
-    """
-    if isinstance(text, str):
-        return text
-    return str(text, encoding, errors=errors)
-
-
-class Sentences(object):
-    def __init__(self, file_names, max_sentence_length=MAX_WORDS_IN_BATCH):
-        self.file_names = file_names
-        self.max_sentence_length = max_sentence_length
+# This source code is licensed under the Apache license found in the
+# LICENSE file in the root directory of this source tree.
 
-    def __iter__(self):
-        """read all the lines in the list of self.file_names, and break the sentence by the self.max_sentence_length
-        Returns:
-            Iterable strs
+from typing import Dict, Union
 
+import lightning.pytorch as pl
+from intc import (
+    MISSING,
+    AnyField,
+    Base,
+    BoolField,
+    DictField,
+    FloatField,
+    IntField,
+    ListField,
+    NestField,
+    StrField,
+    SubModule,
+    cregister,
+)
+from lightning.pytorch.callbacks import ProgressBar, RichProgressBar, TQDMProgressBar
+from lightning.pytorch.utilities.rank_zero import rank_zero_warn
+
+from dlk.utils.register import register
+
+
+@cregister("callback", "prograss_bar")
+class ProgressBarCallbackConfig(Base):
+    """callback for the prograss bar"""
+
+    type_bar = StrField(
+        value="tqdm",
+        options=["tqdm", "rich"],
+        help="""the type of the prograss bar, ``tqdm`` or ``rich``. Defaults to ``tqdm``.""",
+    )
+    refresh_rate = IntField(
+        value=1,
+        minimum=0,
+        help="Determines at which rate (in number of batches) the progress bars get updated. Set it to ``0`` to disable the display. Defaults to ``1``.",
+    )
+    leave = BoolField(
+        value=False,
+        help="Leaves the finished progress bar in the terminal at the end of the epoch. Defaults to ``False``.",
+    )
+    theme = StrField(
+        value="default",
+        options=["default"],
+        help="When the `type_bar` is `rich`. Contains styles used to stylize the progress bar. Currently only support `default`.",
+    )
+    process_position = IntField(
+        value=0,
+        help="Set this to a value greater than ``0`` to offset the progress bars by this many lines. This is useful when you have progress bars defined elsewhere and want to show all of them together.",
+    )
+
+
+class NewRichProgressBar(RichProgressBar):
+    """docstring for  ProgressBar"""
+
+    def __init__(self, **config):
+        super(NewRichProgressBar, self).__init__(**config)
+
+    def get_metrics(
+        self, trainer: "pl.Trainer", pl_module: "pl.LightningModule"
+    ) -> Dict[str, Union[int, str, float, Dict[str, float]]]:
+        r"""Combines progress bar metrics collected from the trainer with standard metrics from
+        get_standard_metrics. Implement this to override the items displayed in the progress bar.
+
+        Here is an example of how to override the defaults:
+
+        .. code-block:: python
+
+            def get_metrics(self, trainer, model):
+                # don't show the version number
+                items = super().get_metrics(trainer, model)
+                items.pop("v_num", None)
+                return items
+
+        Return:
+            Dictionary with the items to be displayed in the progress bar.
         """
+        standard_metrics = {}  # NOTE: remove the `v_num` get_standard_metrics(trainer)
+        pbar_metrics = trainer.progress_bar_metrics
+        duplicates = list(standard_metrics.keys() & pbar_metrics.keys())
+        if duplicates:
+            rank_zero_warn(
+                f"The progress bar already tracks a metric with the name(s) '{', '.join(duplicates)}' and"
+                f" `self.log('{duplicates[0]}', ..., prog_bar=True)` will overwrite this value. "
+                " If this is undesired, change the name or override `get_metrics()` in the progress bar callback.",
+            )
+
+        return {**standard_metrics, **pbar_metrics}
+
+
+class NewTQDMProgressBar(TQDMProgressBar):
+    """docstring for  ProgressBar"""
+
+    def __init__(self, **config):
+        super(NewTQDMProgressBar, self).__init__(**config)
+
+    def get_metrics(
+        self, trainer: "pl.Trainer", pl_module: "pl.LightningModule"
+    ) -> Dict[str, Union[int, str, float, Dict[str, float]]]:
+        r"""Combines progress bar metrics collected from the trainer with standard metrics from
+        get_standard_metrics. Implement this to override the items displayed in the progress bar.
+
+        Here is an example of how to override the defaults:
+
+        .. code-block:: python
+
+            def get_metrics(self, trainer, model):
+                # don't show the version number
+                items = super().get_metrics(trainer, model)
+                items.pop("v_num", None)
+                return items
 
-        for fname in self.file_names:
-            print(f"On {fname}")
-            with open(fname, 'r') as fin:
-                for line in fin.readlines():
-                    line = any2unicode(line).split()
-                    i = 0
-                    while i < len(line):
-                        yield line[i: i + self.max_sentence_length]
-                        i += self.max_sentence_length
-
-
-class LossCallback(CallbackAny2Vec):
-    def __init__(self):
-        self.epoch = 1
-        self.losses = []
-        self.cumu_loss = 0.0
-        self.previous_epoch_time = time.time()
-
-    def on_epoch_end(self, model):
-        loss = model.get_latest_training_loss()
-        norms = [np.linalg.norm(v) for v in model.wv.vectors]
-        now = time.time()
-        epoch_seconds = now - self.previous_epoch_time
-        self.previous_epoch_time = now
-        self.cumu_loss += float(loss)
-        print(f"Loss after epoch {self.epoch}: {loss} (cumulative loss so far: {self.cumu_loss}) "+\
-              f"-> epoch took {round(epoch_seconds, 2)} s - vector norms min/avg/max: "+\
-              f"{round(float(min(norms)), 2)}, {round(float(sum(norms)/len(norms)), 2)}, {round(float(max(norms)), 2)}")
-
-        self.epoch += 1
-        self.losses.append(float(loss))
-        # loss will overflow when the loss very large. see https://github.com/RaRe-Technologies/gensim/issues/2735
-        model.running_training_loss = 0.0
-
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--config",
-        type=str,
-        default='./word2vec.hjson',
-        help="The config path.",
-    )
-    parser.add_argument(
-        "--train_files", type=list, default=['train.txt'], help="train tokenizer files."
-    )
-    parser.add_argument(
-        "--embedding_size",
-        type=int,
-        default=128,
-        help=( "vector size")
-    )
-    parser.add_argument(
-        "--min_count",
-        type=int,
-        default=10,
-        help=( "minist word frequence")
-    )
-    parser.add_argument(
-        "--max_vocab_size",
-        type=int,
-        default=300000,
-        help=( "max vocab size")
-    )
-    parser.add_argument(
-        "--workers",
-        type=int,
-        default=0,
-        help=( "0/none means use all cpus")
-    )
-    parser.add_argument(
-        "--window",
-        type=int,
-        default=6,
-        help=( "window size")
-    )
-    parser.add_argument(
-        "--sg",
-        type=bool,
-        default=0,
-        help=( "use skip gram or not. if set to 0 use cbow")
-    )
-    parser.add_argument(
-        "--hs",
-        type=bool,
-        default=0,
-        help=( "If 1, hierarchical softmax will be used for model training.  If 0, and `negative` is non-zero, negative sampling will be used.")
-    )
-    parser.add_argument(
-        "--negative",
-        type=int,
-        default=10,
-        help=( "Anti with hs==1, negative sampling num, num_ns (number of negative samples per positive context word) between [5, 20] is shown to work best for smaller datasets, while num_ns between [2,5] suffices for larger datasets.")
-    )
-    parser.add_argument(
-        "--epochs",
-        type=int,
-        default=10,
-        help=( "training epochs")
-    )
-    parser.add_argument(
-        "--embedding_file",
-        type=str,
-        default='embedding.txt',
-        help=( "embedding file")
-    )
-    args = parser.parse_args()
-    if args.config:
-        config_json = hjson.load(open(args.config), object_pairs_hook=dict)
-        for key, value in config_json.items():
-           setattr(args, key, value)
-    if not args.workers:
-        args.workers = multiprocessing.cpu_count()
-    # print(args)
-
-    print("Start training...")
-    lines = Sentences(args.train_files)
-
-    model = Word2Vec(lines, vector_size=args.embedding_size, hs=args.hs, negative=args.negative, window=args.window, min_count=args.min_count, workers=args.workers, epochs=args.epochs, sg=args.sg, compute_loss=True, max_vocab_size=args.max_vocab_size, callbacks=[LossCallback()])
-    print("Saving embedding...")
-    model.save(args.model_file)
-    model.wv.save_word2vec_format(args.embedding_file, binary=False)
+        Return:
+            Dictionary with the items to be displayed in the progress bar.
+        """
+        standard_metrics = {}  # NOTE: remove the `v_num` get_standard_metrics(trainer)
+        pbar_metrics = trainer.progress_bar_metrics
+        duplicates = list(standard_metrics.keys() & pbar_metrics.keys())
+        if duplicates:
+            rank_zero_warn(
+                f"The progress bar already tracks a metric with the name(s) '{', '.join(duplicates)}' and"
+                f" `self.log('{duplicates[0]}', ..., prog_bar=True)` will overwrite this value. "
+                " If this is undesired, change the name or override `get_metrics()` in the progress bar callback.",
+            )
+
+        return {**standard_metrics, **pbar_metrics}
+
+
+@register("callback", "prograss_bar")
+class RichProgressBarCallback(object):
+    """prograss bar callback for lightning"""
+
+    def __init__(self, config: ProgressBarCallbackConfig):
+        super().__init__()
+        self.config = config
+
+    def __call__(self, rt_config: Dict) -> ProgressBar:
+        """return LearningRateMonitor object
+
+        Args:
+            rt_config: runtime config, include save_dir, and the checkpoint path name
+
+        Returns:
+            RichProgressBar object
+
+        """
+        if self.config.type_bar == "tqdm":
+            return NewTQDMProgressBar(
+                refresh_rate=self.config.refresh_rate,
+                process_position=self.config.process_position,
+            )
+        else:
+            assert self.config.type_bar == "rich"
+            theme = None
+            assert self.config.theme == "default"
+            from lightning.pytorch.callbacks.progress.rich_progress import (
+                RichProgressBarTheme,
+            )
+
+            theme = RichProgressBarTheme()
+            return NewRichProgressBar(
+                refresh_rate=self.config.refresh_rate,
+                leave=self.config.leave,
+                theme=theme,
+            )
```

