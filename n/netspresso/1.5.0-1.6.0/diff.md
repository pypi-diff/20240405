# Comparing `tmp/netspresso-1.5.0.tar.gz` & `tmp/netspresso-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netspresso-1.5.0.tar", last modified: Thu Mar 14 05:11:20 2024, max compression
+gzip compressed data, was "netspresso-1.6.0.tar", last modified: Fri Apr  5 04:43:15 2024, max compression
```

## Comparing `netspresso-1.5.0.tar` & `netspresso-1.6.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.100585 netspresso-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-14 05:11:07.000000 netspresso-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25595 2024-03-14 05:11:20.100585 netspresso-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21157 2024-03-14 05:11:07.000000 netspresso-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.084585 netspresso-1.5.0/netspresso/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/benchmarker/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/benchmarker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/benchmarker/benchmarker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/auth/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/auth/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/auth/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/auth/schemas/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/compressor/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/compressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/compressor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/compressor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/compressor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/compressor/schemas/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/compressor/schemas/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/compressor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/compressor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/compressor/utils/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/configs/config-local.ini
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/configs/config-prod.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/launcher/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/launcher/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso/clients/launcher/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/launcher/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/launcher/schemas/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.092585 netspresso-1.5.0/netspresso/clients/tao/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/tao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/tao/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/tao/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/tao/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/tao/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.092585 netspresso-1.5.0/netspresso/clients/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/utils/requester.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/clients/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.092585 netspresso-1.5.0/netspresso/compressor/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/compressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32100 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/compressor/compressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.092585 netspresso-1.5.0/netspresso/compressor/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/compressor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/compressor/core/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/compressor/core/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.092585 netspresso-1.5.0/netspresso/compressor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/compressor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/compressor/utils/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.092585 netspresso-1.5.0/netspresso/converter/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/converter/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/credit.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/enums/tao/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/tao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/tao/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/tao/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/enums/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/netspresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/tao/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/tao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/tao/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/tao/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/tao/tao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/tao/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/tao/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/tao/utils/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/trainer/augmentations/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/augmentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/trainer/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/optimizers/optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/trainer/registries/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/registries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/registries/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/registries/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/registries/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/registries/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.096585 netspresso-1.5.0/netspresso/trainer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/schedulers/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/trainer/trainer_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.100585 netspresso-1.5.0/netspresso/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/credit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.100585 netspresso-1.5.0/netspresso/utils/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.100585 netspresso-1.5.0/netspresso/utils/metadata/default/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/metadata/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/metadata/default/benchmarker.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/metadata/default/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/metadata/default/compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/metadata/default/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/metadata/default/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/metadata/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20369 2024-03-14 05:11:07.000000 netspresso-1.5.0/netspresso/utils/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 05:11:20.088585 netspresso-1.5.0/netspresso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25595 2024-03-14 05:11:19.000000 netspresso-1.5.0/netspresso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-14 05:11:20.000000 netspresso-1.5.0/netspresso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 05:11:19.000000 netspresso-1.5.0/netspresso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-14 05:11:19.000000 netspresso-1.5.0/netspresso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-14 05:11:19.000000 netspresso-1.5.0/netspresso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-14 05:11:07.000000 netspresso-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 05:11:20.100585 netspresso-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-14 05:11:07.000000 netspresso-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.276750 netspresso-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 04:43:07.000000 netspresso-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-04-05 04:43:15.276750 netspresso-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21251 2024-04-05 04:43:07.000000 netspresso-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/benchmarker/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/benchmarker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/benchmarker/benchmarker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/auth/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/clients/auth/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/auth/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/auth/schemas/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/clients/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/compressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/compressor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/clients/compressor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/compressor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/compressor/schemas/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/compressor/schemas/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/clients/compressor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/compressor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/compressor/utils/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/clients/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/configs/config-local.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/configs/config-prod.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso/clients/launcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/launcher/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.268750 netspresso-1.6.0/netspresso/clients/launcher/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/launcher/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/launcher/schemas/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.268750 netspresso-1.6.0/netspresso/clients/tao/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/tao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/tao/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/tao/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/tao/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/tao/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.268750 netspresso-1.6.0/netspresso/clients/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/utils/requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/clients/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.268750 netspresso-1.6.0/netspresso/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/compressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32139 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/compressor/compressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.268750 netspresso-1.6.0/netspresso/compressor/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/compressor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/compressor/core/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/compressor/core/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.268750 netspresso-1.6.0/netspresso/compressor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/compressor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/compressor/utils/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.268750 netspresso-1.6.0/netspresso/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/converter/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/enums/tao/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/tao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/tao/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/tao/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/enums/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/netspresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/tao/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/tao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/tao/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/tao/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/tao/tao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/tao/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/tao/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/tao/utils/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/trainer/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/augmentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/trainer/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/optimizers/optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/trainer/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/registries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/registries/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/registries/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/registries/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/registries/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/trainer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/schedulers/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/trainer/trainer_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.272750 netspresso-1.6.0/netspresso/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.276750 netspresso-1.6.0/netspresso/utils/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.276750 netspresso-1.6.0/netspresso/utils/metadata/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/metadata/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/metadata/default/benchmarker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/metadata/default/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/metadata/default/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/metadata/default/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/metadata/default/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/metadata/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20369 2024-04-05 04:43:07.000000 netspresso-1.6.0/netspresso/utils/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:43:15.264750 netspresso-1.6.0/netspresso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-04-05 04:43:14.000000 netspresso-1.6.0/netspresso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-05 04:43:15.000000 netspresso-1.6.0/netspresso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:43:14.000000 netspresso-1.6.0/netspresso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-05 04:43:14.000000 netspresso-1.6.0/netspresso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 04:43:14.000000 netspresso-1.6.0/netspresso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-05 04:43:07.000000 netspresso-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:43:15.276750 netspresso-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-05 04:43:07.000000 netspresso-1.6.0/setup.py
```

### Comparing `netspresso-1.5.0/LICENSE` & `netspresso-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/PKG-INFO` & `netspresso-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netspresso
-Version: 1.5.0
+Version: 1.6.0
 Summary: PyNetsPresso
 Home-page: https://github.com/Nota-NetsPresso/PyNetsPresso
 Author: NetsPresso
 Author-email: netspresso@nota.ai
 License: UNKNOWN
 Description: <div align=right>
           <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FNota-NetsPresso%2Fnetspresso-python&count_bg=%2323E7E7E7&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
@@ -371,14 +371,15 @@
           | RASPBERRY_PI_3B_PLUS         |  ✔️  |          |       ✔️        |       |          |
           | RASPBERRY_PI_ZERO_W          |  ✔️  |          |       ✔️        |       |          |
           | RASPBERRY_PI_ZERO_2W         |  ✔️  |          |       ✔️        |       |          |
           | ARM_ETHOS_U_SERIES           |      |          |  ✔️(only INT8)  |       |          |
           | ALIF_ENSEMBLE_E7_DEVKIT_GEN2 |      |          |  ✔️(only INT8)  |       |          |
           | RENESAS_RA8D1                |      |          |  ✔️(only INT8)  |       |          |
           | NXP_iMX93                    |      |          |  ✔️(only INT8)  |       |          |
+          | ARDUINO_NICLA_VISION         |      |          |  ✔️(only INT8)  |       |          |
           | RENESAS_RZ_V2L               |  ✔️  |          |                 |  ✔️   |          |
           | RENESAS_RZ_V2M               |  ✔️  |          |                 |  ✔️   |          |
           | JETSON_NANO                  |  ✔️  |    ✔️    |                 |       |          |
           | JETSON_TX2                   |  ✔️  |    ✔️    |                 |       |          |
           | JETSON_XAVIER                |  ✔️  |    ✔️    |                 |       |          |
           | JETSON_NX                    |  ✔️  |    ✔️    |                 |       |          |
           | JETSON_AGX_ORIN              |  ✔️  |    ✔️    |                 |       |          |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netspresso Version: 1.5.0 Summary: PyNetsPresso
+Metadata-Version: 2.1 Name: netspresso Version: 1.6.0 Summary: PyNetsPresso
 Home-page: https://github.com/Nota-NetsPresso/PyNetsPresso Author: NetsPresso
 Author-email: netspresso@nota.ai License: UNKNOWN Description:
                                    _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
          _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_N_o_t_a_-_N_e_t_s_P_r_e_s_s_o_%_2_F_n_e_t_s_p_r_e_s_s_o_-
 _p_y_t_h_o_n_&_c_o_u_n_t___b_g_=_%_2_3_2_3_E_7_E_7_E_7_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_h_i_t_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
   _[_h_t_t_p_s_:_/_/_n_e_t_s_p_r_e_s_s_o_-_d_o_c_s_-_i_m_g_s_._s_3_._a_p_-_n_o_r_t_h_e_a_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_i_m_g_s_/_b_a_n_n_e_r_/
                            _N_e_t_s_P_r_e_s_s_o_2_._0___b_a_n_n_e_r_._p_n_g_]
@@ -136,30 +136,31 @@
 Framework | ONNX | TENSORRT | TENSORFLOW_LITE | DRPAI | OPENVINO | |:----------
 -------------------|:----:|:--------:|:---------------:|:-----:|:--------:| |
 RASPBERRY_PI_5 | âï¸ | | âï¸ | | | | RASPBERRY_PI_4B | âï¸ | | âï¸
 | | | | RASPBERRY_PI_3B_PLUS | âï¸ | | âï¸ | | | | RASPBERRY_PI_ZERO_W |
 âï¸ | | âï¸ | | | | RASPBERRY_PI_ZERO_2W | âï¸ | | âï¸ | | | |
 ARM_ETHOS_U_SERIES | | | âï¸(only INT8) | | | | ALIF_ENSEMBLE_E7_DEVKIT_GEN2
 | | | âï¸(only INT8) | | | | RENESAS_RA8D1 | | | âï¸(only INT8) | | | |
-NXP_iMX93 | | | âï¸(only INT8) | | | | RENESAS_RZ_V2L | âï¸ | | | âï¸
-| | | RENESAS_RZ_V2M | âï¸ | | | âï¸ | | | JETSON_NANO | âï¸ | âï¸
-| | | | | JETSON_TX2 | âï¸ | âï¸ | | | | | JETSON_XAVIER | âï¸ |
-âï¸ | | | | | JETSON_NX | âï¸ | âï¸ | | | | | JETSON_AGX_ORIN | âï¸
-| âï¸ | | | | | JETSON_ORIN_NANO | âï¸ | âï¸ | | | | | AWS_T4 | âï¸
-| âï¸ | | | | | INTEL_XEON_W_2233 | | | | | âï¸ | ### Software versions
-that support conversions and benchmarks for specific devices Software Versions
-requires only Jetson Device. If you are using a different device, you do not
-need to enter it. | Software Version / Device | JETSON_NANO | JETSON_TX2 |
-JETSON_XAVIER | JETSON_NX | JETSON_AGX_ORIN | JETSON_ORIN_NANO | |:------------
---------------|:-----------:|:----------:|:-------------:|:---------:|:--------
--------:|:----------------:| | JETPACK_4_4_1 | âï¸ | | | | | | | JETPACK_4_6
-| âï¸ | âï¸ | âï¸ | âï¸ | | | | JETPACK_5_0_1 | | | | | âï¸ | |
-| JETPACK_5_0_2 | | | | âï¸ | | | | JETPACK_6_0 | | | | | | âï¸ | The
-code below is an example of using software version. ```python conversion_result
-= converter.convert_model( input_model_path=INPUT_MODEL_PATH,
+NXP_iMX93 | | | âï¸(only INT8) | | | | ARDUINO_NICLA_VISION | | | âï¸
+(only INT8) | | | | RENESAS_RZ_V2L | âï¸ | | | âï¸ | | | RENESAS_RZ_V2M |
+âï¸ | | | âï¸ | | | JETSON_NANO | âï¸ | âï¸ | | | | | JETSON_TX2 |
+âï¸ | âï¸ | | | | | JETSON_XAVIER | âï¸ | âï¸ | | | | | JETSON_NX |
+âï¸ | âï¸ | | | | | JETSON_AGX_ORIN | âï¸ | âï¸ | | | | |
+JETSON_ORIN_NANO | âï¸ | âï¸ | | | | | AWS_T4 | âï¸ | âï¸ | | | | |
+INTEL_XEON_W_2233 | | | | | âï¸ | ### Software versions that support
+conversions and benchmarks for specific devices Software Versions requires only
+Jetson Device. If you are using a different device, you do not need to enter
+it. | Software Version / Device | JETSON_NANO | JETSON_TX2 | JETSON_XAVIER |
+JETSON_NX | JETSON_AGX_ORIN | JETSON_ORIN_NANO | |:--------------------------|:
+-----------:|:----------:|:-------------:|:---------:|:---------------:|:------
+----------:| | JETPACK_4_4_1 | âï¸ | | | | | | | JETPACK_4_6 | âï¸ |
+âï¸ | âï¸ | âï¸ | | | | JETPACK_5_0_1 | | | | | âï¸ | | |
+JETPACK_5_0_2 | | | | âï¸ | | | | JETPACK_6_0 | | | | | | âï¸ | The code
+below is an example of using software version. ```python conversion_result =
+converter.convert_model( input_model_path=INPUT_MODEL_PATH,
 output_dir=OUTPUT_DIR, target_framework=Framework.TENSORRT,
 target_device_name=DeviceName.JETSON_AGX_ORIN,
 target_software_version=SoftwareVersion.JETPACK_5_0_1, ) benchmark_result =
 benchmarker.benchmark_model( input_model_path=CONVERTED_MODEL_PATH,
 target_device_name=DeviceName.JETSON_AGX_ORIN,
 target_software_version=SoftwareVersion.JETPACK_5_0_1, ) ``` ### Hardware type
 that support benchmarks for specific devices Benchmark and compare models with
```

### Comparing `netspresso-1.5.0/README.md` & `netspresso-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,15 @@
   | RASPBERRY_PI_3B_PLUS         |  ✔️  |          |       ✔️        |       |          |
   | RASPBERRY_PI_ZERO_W          |  ✔️  |          |       ✔️        |       |          |
   | RASPBERRY_PI_ZERO_2W         |  ✔️  |          |       ✔️        |       |          |
   | ARM_ETHOS_U_SERIES           |      |          |  ✔️(only INT8)  |       |          |
   | ALIF_ENSEMBLE_E7_DEVKIT_GEN2 |      |          |  ✔️(only INT8)  |       |          |
   | RENESAS_RA8D1                |      |          |  ✔️(only INT8)  |       |          |
   | NXP_iMX93                    |      |          |  ✔️(only INT8)  |       |          |
+  | ARDUINO_NICLA_VISION         |      |          |  ✔️(only INT8)  |       |          |
   | RENESAS_RZ_V2L               |  ✔️  |          |                 |  ✔️   |          |
   | RENESAS_RZ_V2M               |  ✔️  |          |                 |  ✔️   |          |
   | JETSON_NANO                  |  ✔️  |    ✔️    |                 |       |          |
   | JETSON_TX2                   |  ✔️  |    ✔️    |                 |       |          |
   | JETSON_XAVIER                |  ✔️  |    ✔️    |                 |       |          |
   | JETSON_NX                    |  ✔️  |    ✔️    |                 |       |          |
   | JETSON_AGX_ORIN              |  ✔️  |    ✔️    |                 |       |          |
```

#### html2text {}

```diff
@@ -133,30 +133,31 @@
 Framework | ONNX | TENSORRT | TENSORFLOW_LITE | DRPAI | OPENVINO | |:----------
 -------------------|:----:|:--------:|:---------------:|:-----:|:--------:| |
 RASPBERRY_PI_5 | âï¸ | | âï¸ | | | | RASPBERRY_PI_4B | âï¸ | | âï¸
 | | | | RASPBERRY_PI_3B_PLUS | âï¸ | | âï¸ | | | | RASPBERRY_PI_ZERO_W |
 âï¸ | | âï¸ | | | | RASPBERRY_PI_ZERO_2W | âï¸ | | âï¸ | | | |
 ARM_ETHOS_U_SERIES | | | âï¸(only INT8) | | | | ALIF_ENSEMBLE_E7_DEVKIT_GEN2
 | | | âï¸(only INT8) | | | | RENESAS_RA8D1 | | | âï¸(only INT8) | | | |
-NXP_iMX93 | | | âï¸(only INT8) | | | | RENESAS_RZ_V2L | âï¸ | | | âï¸
-| | | RENESAS_RZ_V2M | âï¸ | | | âï¸ | | | JETSON_NANO | âï¸ | âï¸
-| | | | | JETSON_TX2 | âï¸ | âï¸ | | | | | JETSON_XAVIER | âï¸ |
-âï¸ | | | | | JETSON_NX | âï¸ | âï¸ | | | | | JETSON_AGX_ORIN | âï¸
-| âï¸ | | | | | JETSON_ORIN_NANO | âï¸ | âï¸ | | | | | AWS_T4 | âï¸
-| âï¸ | | | | | INTEL_XEON_W_2233 | | | | | âï¸ | ### Software versions
-that support conversions and benchmarks for specific devices Software Versions
-requires only Jetson Device. If you are using a different device, you do not
-need to enter it. | Software Version / Device | JETSON_NANO | JETSON_TX2 |
-JETSON_XAVIER | JETSON_NX | JETSON_AGX_ORIN | JETSON_ORIN_NANO | |:------------
---------------|:-----------:|:----------:|:-------------:|:---------:|:--------
--------:|:----------------:| | JETPACK_4_4_1 | âï¸ | | | | | | | JETPACK_4_6
-| âï¸ | âï¸ | âï¸ | âï¸ | | | | JETPACK_5_0_1 | | | | | âï¸ | |
-| JETPACK_5_0_2 | | | | âï¸ | | | | JETPACK_6_0 | | | | | | âï¸ | The
-code below is an example of using software version. ```python conversion_result
-= converter.convert_model( input_model_path=INPUT_MODEL_PATH,
+NXP_iMX93 | | | âï¸(only INT8) | | | | ARDUINO_NICLA_VISION | | | âï¸
+(only INT8) | | | | RENESAS_RZ_V2L | âï¸ | | | âï¸ | | | RENESAS_RZ_V2M |
+âï¸ | | | âï¸ | | | JETSON_NANO | âï¸ | âï¸ | | | | | JETSON_TX2 |
+âï¸ | âï¸ | | | | | JETSON_XAVIER | âï¸ | âï¸ | | | | | JETSON_NX |
+âï¸ | âï¸ | | | | | JETSON_AGX_ORIN | âï¸ | âï¸ | | | | |
+JETSON_ORIN_NANO | âï¸ | âï¸ | | | | | AWS_T4 | âï¸ | âï¸ | | | | |
+INTEL_XEON_W_2233 | | | | | âï¸ | ### Software versions that support
+conversions and benchmarks for specific devices Software Versions requires only
+Jetson Device. If you are using a different device, you do not need to enter
+it. | Software Version / Device | JETSON_NANO | JETSON_TX2 | JETSON_XAVIER |
+JETSON_NX | JETSON_AGX_ORIN | JETSON_ORIN_NANO | |:--------------------------|:
+-----------:|:----------:|:-------------:|:---------:|:---------------:|:------
+----------:| | JETPACK_4_4_1 | âï¸ | | | | | | | JETPACK_4_6 | âï¸ |
+âï¸ | âï¸ | âï¸ | | | | JETPACK_5_0_1 | | | | | âï¸ | | |
+JETPACK_5_0_2 | | | | âï¸ | | | | JETPACK_6_0 | | | | | | âï¸ | The code
+below is an example of using software version. ```python conversion_result =
+converter.convert_model( input_model_path=INPUT_MODEL_PATH,
 output_dir=OUTPUT_DIR, target_framework=Framework.TENSORRT,
 target_device_name=DeviceName.JETSON_AGX_ORIN,
 target_software_version=SoftwareVersion.JETPACK_5_0_1, ) benchmark_result =
 benchmarker.benchmark_model( input_model_path=CONVERTED_MODEL_PATH,
 target_device_name=DeviceName.JETSON_AGX_ORIN,
 target_software_version=SoftwareVersion.JETPACK_5_0_1, ) ``` ### Hardware type
 that support benchmarks for specific devices Benchmark and compare models with
```

### Comparing `netspresso-1.5.0/netspresso/benchmarker/benchmarker.py` & `netspresso-1.6.0/netspresso/benchmarker/benchmarker.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/auth/main.py` & `netspresso-1.6.0/netspresso/clients/auth/main.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/auth/schemas/auth.py` & `netspresso-1.6.0/netspresso/clients/auth/schemas/auth.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/compressor/main.py` & `netspresso-1.6.0/netspresso/clients/compressor/main.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/compressor/schemas/compression.py` & `netspresso-1.6.0/netspresso/clients/compressor/schemas/compression.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/compressor/schemas/model.py` & `netspresso-1.6.0/netspresso/clients/compressor/schemas/model.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/compressor/utils/validator.py` & `netspresso-1.6.0/netspresso/clients/compressor/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/config.py` & `netspresso-1.6.0/netspresso/clients/config.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/launcher/main.py` & `netspresso-1.6.0/netspresso/clients/launcher/main.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/launcher/schemas/model.py` & `netspresso-1.6.0/netspresso/clients/launcher/schemas/model.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/tao/dataset.py` & `netspresso-1.6.0/netspresso/clients/tao/dataset.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/tao/experiment.py` & `netspresso-1.6.0/netspresso/clients/tao/experiment.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/tao/main.py` & `netspresso-1.6.0/netspresso/clients/tao/main.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/utils/common.py` & `netspresso-1.6.0/netspresso/clients/utils/common.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/utils/requester.py` & `netspresso-1.6.0/netspresso/clients/utils/requester.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/clients/utils/system.py` & `netspresso-1.6.0/netspresso/clients/utils/system.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/compressor/compressor.py` & `netspresso-1.6.0/netspresso/compressor/compressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,18 +356,18 @@
         self.token_handler.validate_token()
 
         try:
             logger.info("Compressing model...")
 
             model_info = self.get_model(compression.original_model_id)
 
+            output_dir = FileHandler.create_unique_folder(folder_path=output_dir)
             default_model_path, extension = FileHandler.get_path_and_extension(
                 folder_path=output_dir, framework=model_info.framework
             )
-            FileHandler.create_unique_folder(folder_path=output_dir)
             metadata = MetadataHandler.init_metadata(folder_path=output_dir, task_type=TaskType.COMPRESS)
 
             current_credit = auth_client.get_credit(
                 self.token_handler.tokens.access_token, verify_ssl=self.token_handler.verify_ssl
             )
             check_credit_balance(
                 user_credit=current_credit,
@@ -505,18 +505,18 @@
         FileHandler.check_input_model_path(input_model_path)
 
         self.token_handler.validate_token()
 
         try:
             logger.info("Compressing recommendation-based model...")
 
+            output_dir = FileHandler.create_unique_folder(folder_path=output_dir)
             default_model_path, extension = FileHandler.get_path_and_extension(
                 folder_path=output_dir, framework=framework
             )
-            FileHandler.create_unique_folder(folder_path=output_dir)
             metadata = MetadataHandler.init_metadata(folder_path=output_dir, task_type=TaskType.COMPRESS)
 
             current_credit = auth_client.get_credit(
                 self.token_handler.tokens.access_token, verify_ssl=self.token_handler.verify_ssl
             )
             check_credit_balance(
                 user_credit=current_credit,
@@ -678,18 +678,18 @@
         FileHandler.check_input_model_path(input_model_path)
 
         self.token_handler.validate_token()
 
         try:
             logger.info("Compressing automatic-based model...")
 
+            output_dir = FileHandler.create_unique_folder(folder_path=output_dir)
             default_model_path, extension = FileHandler.get_path_and_extension(
                 folder_path=output_dir, framework=framework
             )
-            FileHandler.create_unique_folder(folder_path=output_dir)
             metadata = MetadataHandler.init_metadata(folder_path=output_dir, task_type=TaskType.COMPRESS)
 
             current_credit = auth_client.get_credit(
                 self.token_handler.tokens.access_token, verify_ssl=self.token_handler.verify_ssl
             )
             check_credit_balance(
                 user_credit=current_credit,
```

### Comparing `netspresso-1.5.0/netspresso/compressor/core/compression.py` & `netspresso-1.6.0/netspresso/compressor/core/compression.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/compressor/core/model.py` & `netspresso-1.6.0/netspresso/compressor/core/model.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/compressor/utils/onnx.py` & `netspresso-1.6.0/netspresso/compressor/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/converter/converter.py` & `netspresso-1.6.0/netspresso/converter/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,18 @@
         """
 
         FileHandler.check_input_model_path(input_model_path)
 
         self.token_handler.validate_token()
 
         try:
+            output_dir = FileHandler.create_unique_folder(folder_path=output_dir)
             default_model_path, extension = FileHandler.get_path_and_extension(
                 folder_path=output_dir, framework=target_framework
             )
-            FileHandler.create_unique_folder(folder_path=output_dir)
             metadata = MetadataHandler.init_metadata(folder_path=output_dir, task_type=TaskType.CONVERT)
 
             current_credit = auth_client.get_credit(
                 self.token_handler.tokens.access_token, verify_ssl=self.token_handler.verify_ssl
             )
             check_credit_balance(user_credit=current_credit, service_credit=ServiceCredit.MODEL_CONVERT)
             model = launcher_client.upload_model(
```

### Comparing `netspresso-1.5.0/netspresso/enums/__init__.py` & `netspresso-1.6.0/netspresso/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/enums/compression.py` & `netspresso-1.6.0/netspresso/enums/compression.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/enums/device.py` & `netspresso-1.6.0/netspresso/enums/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     JETSON_ORIN_NANO = "Jetson-Orin-Nano"
     AWS_T4 = "AWS-T4"
     INTEL_XEON_W_2233 = "Intel-Xeon"
     ALIF_ENSEMBLE_E7_DEVKIT_GEN2 = "Ensemble-E7-DevKit-Gen2"
     RENESAS_RA8D1 = "Renesas-RA8D1"
     ARM_ETHOS_U_SERIES = "Arm Virtual Hardware Ethos-U Series"
     NXP_iMX93 = "nxp_imx93_ethos_u65"
+    ARDUINO_NICLA_VISION = "arduino_nicla_vision"
 
     @classmethod
     def create_literal(cls):
         return Literal[
             "RaspberryPi5",
             "RaspberryPi4B",
             "RaspberryPi3BPlus",
@@ -40,15 +41,16 @@
             "Jetson-AGX-Orin",
             "Jetson-Orin-Nano",
             "AWS-T4",
             "Intel-Xeon",
             "Ensemble-E7-DevKit-Gen2",
             "Renesas-RA8D1",
             "Arm Virtual Hardware Ethos-U Series",
-            "nxp_imx93_ethos_u65"
+            "nxp_imx93_ethos_u65",
+            "arduino_nicla_vision"
         ]
 
     JETSON_DEVICES = [
         JETSON_NANO,
         JETSON_TX2,
         JETSON_XAVIER,
         JETSON_NX,
@@ -70,17 +72,18 @@
         RENESAS_RA8D1,
         RASPBERRY_PI_5,
         RASPBERRY_PI_4B,
         RASPBERRY_PI_3B_PLUS,
         RASPBERRY_PI_ZERO_W,
         RASPBERRY_PI_ZERO_2W,
         ARM_ETHOS_U_SERIES,
-        NXP_iMX93
+        NXP_iMX93,
+        ARDUINO_NICLA_VISION
     ]
-    ONLY_INT8_DEVICES = [ALIF_ENSEMBLE_E7_DEVKIT_GEN2, RENESAS_RA8D1, ARM_ETHOS_U_SERIES, NXP_iMX93]
+    ONLY_INT8_DEVICES = [ALIF_ENSEMBLE_E7_DEVKIT_GEN2, RENESAS_RA8D1, ARM_ETHOS_U_SERIES, NXP_iMX93, ARDUINO_NICLA_VISION]
 
 
 class SoftwareVersion(str, Enum):
     JETPACK_4_4_1 = "4.4.1-b50"
     JETPACK_4_6 = "4.6-b199"
     JETPACK_5_0_1 = "5.0.1-b118"
     JETPACK_5_0_2 = "5.0.2-b231"
```

### Comparing `netspresso-1.5.0/netspresso/enums/model.py` & `netspresso-1.6.0/netspresso/enums/model.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/enums/tao/experiment.py` & `netspresso-1.6.0/netspresso/enums/tao/experiment.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/netspresso.py` & `netspresso-1.6.0/netspresso/netspresso.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/tao/dataset.py` & `netspresso-1.6.0/netspresso/tao/dataset.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/tao/tao.py` & `netspresso-1.6.0/netspresso/tao/tao.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/tao/utils/file.py` & `netspresso-1.6.0/netspresso/tao/utils/file.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/trainer/optimizers/optimizers.py` & `netspresso-1.6.0/netspresso/trainer/optimizers/optimizers.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/trainer/registries/model.py` & `netspresso-1.6.0/netspresso/trainer/registries/model.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/trainer/schedulers/schedulers.py` & `netspresso-1.6.0/netspresso/trainer/schedulers/schedulers.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/trainer/trainer.py` & `netspresso-1.6.0/netspresso/trainer/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,19 +362,19 @@
 
         Returns:
             Dict: A dictionary containing information about the training.
         """
 
         self._validate_config()
         self._apply_img_size()
-        self.logging.project_id = project_name
 
-        destination_folder = Path(self.logging.output_dir) / self.logging.project_id
-        FileHandler.create_unique_folder(folder_path=destination_folder)
+        destination_folder = Path(self.logging.output_dir) / project_name
+        destination_folder = FileHandler.create_unique_folder(folder_path=destination_folder)
         metadata = MetadataHandler.init_metadata(folder_path=destination_folder, task_type=TaskType.TRAIN)
+        self.logging.project_id = Path(destination_folder).name
 
         configs = TrainerConfigs(
             self.data,
             self.augmentation,
             self.model,
             self.training,
             self.logging,
```

### Comparing `netspresso-1.5.0/netspresso/trainer/trainer_configs.py` & `netspresso-1.6.0/netspresso/trainer/trainer_configs.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/utils/file.py` & `netspresso-1.6.0/netspresso/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,27 +67,30 @@
         """
         if is_folder_check and not FileHandler.check_exists(folder_path=folder_path):
             Path(folder_path).mkdir(parents=parents, exist_ok=exist_ok)
         elif is_folder_check:
             sys.exit(f"This folder already exists. Local Path: {Path(folder_path)}")
 
     @staticmethod
-    def create_unique_folder(folder_path: str) -> None:
+    def create_unique_folder(folder_path: str) -> str:
         folder_path = Path(folder_path)
         if not folder_path.exists():
             folder_path.mkdir(parents=True)
         else:
             count = 1
             while True:
                 new_folder_path = folder_path.with_name(f"{folder_path.name} ({count})")
                 if not new_folder_path.exists():
                     new_folder_path.mkdir(parents=True)
+                    folder_path = new_folder_path
                     break
                 count += 1
 
+        return str(folder_path)
+
     @staticmethod
     def create_file_path(folder_path: str, name: str, extension: str) -> Union[str, Path]:
         """Create a file path.
 
         Args:
             folder_path (str): The path to the folder where the file will be located.
             name (str): The name of the file.
```

### Comparing `netspresso-1.5.0/netspresso/utils/metadata/default/benchmarker.py` & `netspresso-1.6.0/netspresso/utils/metadata/default/benchmarker.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/utils/metadata/default/compressor.py` & `netspresso-1.6.0/netspresso/utils/metadata/default/compressor.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/utils/metadata/default/converter.py` & `netspresso-1.6.0/netspresso/utils/metadata/default/converter.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/utils/metadata/default/trainer.py` & `netspresso-1.6.0/netspresso/utils/metadata/default/trainer.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/utils/metadata/handler.py` & `netspresso-1.6.0/netspresso/utils/metadata/handler.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso/utils/plotter.py` & `netspresso-1.6.0/netspresso/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/netspresso.egg-info/PKG-INFO` & `netspresso-1.6.0/netspresso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netspresso
-Version: 1.5.0
+Version: 1.6.0
 Summary: PyNetsPresso
 Home-page: https://github.com/Nota-NetsPresso/PyNetsPresso
 Author: NetsPresso
 Author-email: netspresso@nota.ai
 License: UNKNOWN
 Description: <div align=right>
           <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FNota-NetsPresso%2Fnetspresso-python&count_bg=%2323E7E7E7&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
@@ -371,14 +371,15 @@
           | RASPBERRY_PI_3B_PLUS         |  ✔️  |          |       ✔️        |       |          |
           | RASPBERRY_PI_ZERO_W          |  ✔️  |          |       ✔️        |       |          |
           | RASPBERRY_PI_ZERO_2W         |  ✔️  |          |       ✔️        |       |          |
           | ARM_ETHOS_U_SERIES           |      |          |  ✔️(only INT8)  |       |          |
           | ALIF_ENSEMBLE_E7_DEVKIT_GEN2 |      |          |  ✔️(only INT8)  |       |          |
           | RENESAS_RA8D1                |      |          |  ✔️(only INT8)  |       |          |
           | NXP_iMX93                    |      |          |  ✔️(only INT8)  |       |          |
+          | ARDUINO_NICLA_VISION         |      |          |  ✔️(only INT8)  |       |          |
           | RENESAS_RZ_V2L               |  ✔️  |          |                 |  ✔️   |          |
           | RENESAS_RZ_V2M               |  ✔️  |          |                 |  ✔️   |          |
           | JETSON_NANO                  |  ✔️  |    ✔️    |                 |       |          |
           | JETSON_TX2                   |  ✔️  |    ✔️    |                 |       |          |
           | JETSON_XAVIER                |  ✔️  |    ✔️    |                 |       |          |
           | JETSON_NX                    |  ✔️  |    ✔️    |                 |       |          |
           | JETSON_AGX_ORIN              |  ✔️  |    ✔️    |                 |       |          |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netspresso Version: 1.5.0 Summary: PyNetsPresso
+Metadata-Version: 2.1 Name: netspresso Version: 1.6.0 Summary: PyNetsPresso
 Home-page: https://github.com/Nota-NetsPresso/PyNetsPresso Author: NetsPresso
 Author-email: netspresso@nota.ai License: UNKNOWN Description:
                                    _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
          _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_N_o_t_a_-_N_e_t_s_P_r_e_s_s_o_%_2_F_n_e_t_s_p_r_e_s_s_o_-
 _p_y_t_h_o_n_&_c_o_u_n_t___b_g_=_%_2_3_2_3_E_7_E_7_E_7_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_h_i_t_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
   _[_h_t_t_p_s_:_/_/_n_e_t_s_p_r_e_s_s_o_-_d_o_c_s_-_i_m_g_s_._s_3_._a_p_-_n_o_r_t_h_e_a_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_i_m_g_s_/_b_a_n_n_e_r_/
                            _N_e_t_s_P_r_e_s_s_o_2_._0___b_a_n_n_e_r_._p_n_g_]
@@ -136,30 +136,31 @@
 Framework | ONNX | TENSORRT | TENSORFLOW_LITE | DRPAI | OPENVINO | |:----------
 -------------------|:----:|:--------:|:---------------:|:-----:|:--------:| |
 RASPBERRY_PI_5 | âï¸ | | âï¸ | | | | RASPBERRY_PI_4B | âï¸ | | âï¸
 | | | | RASPBERRY_PI_3B_PLUS | âï¸ | | âï¸ | | | | RASPBERRY_PI_ZERO_W |
 âï¸ | | âï¸ | | | | RASPBERRY_PI_ZERO_2W | âï¸ | | âï¸ | | | |
 ARM_ETHOS_U_SERIES | | | âï¸(only INT8) | | | | ALIF_ENSEMBLE_E7_DEVKIT_GEN2
 | | | âï¸(only INT8) | | | | RENESAS_RA8D1 | | | âï¸(only INT8) | | | |
-NXP_iMX93 | | | âï¸(only INT8) | | | | RENESAS_RZ_V2L | âï¸ | | | âï¸
-| | | RENESAS_RZ_V2M | âï¸ | | | âï¸ | | | JETSON_NANO | âï¸ | âï¸
-| | | | | JETSON_TX2 | âï¸ | âï¸ | | | | | JETSON_XAVIER | âï¸ |
-âï¸ | | | | | JETSON_NX | âï¸ | âï¸ | | | | | JETSON_AGX_ORIN | âï¸
-| âï¸ | | | | | JETSON_ORIN_NANO | âï¸ | âï¸ | | | | | AWS_T4 | âï¸
-| âï¸ | | | | | INTEL_XEON_W_2233 | | | | | âï¸ | ### Software versions
-that support conversions and benchmarks for specific devices Software Versions
-requires only Jetson Device. If you are using a different device, you do not
-need to enter it. | Software Version / Device | JETSON_NANO | JETSON_TX2 |
-JETSON_XAVIER | JETSON_NX | JETSON_AGX_ORIN | JETSON_ORIN_NANO | |:------------
---------------|:-----------:|:----------:|:-------------:|:---------:|:--------
--------:|:----------------:| | JETPACK_4_4_1 | âï¸ | | | | | | | JETPACK_4_6
-| âï¸ | âï¸ | âï¸ | âï¸ | | | | JETPACK_5_0_1 | | | | | âï¸ | |
-| JETPACK_5_0_2 | | | | âï¸ | | | | JETPACK_6_0 | | | | | | âï¸ | The
-code below is an example of using software version. ```python conversion_result
-= converter.convert_model( input_model_path=INPUT_MODEL_PATH,
+NXP_iMX93 | | | âï¸(only INT8) | | | | ARDUINO_NICLA_VISION | | | âï¸
+(only INT8) | | | | RENESAS_RZ_V2L | âï¸ | | | âï¸ | | | RENESAS_RZ_V2M |
+âï¸ | | | âï¸ | | | JETSON_NANO | âï¸ | âï¸ | | | | | JETSON_TX2 |
+âï¸ | âï¸ | | | | | JETSON_XAVIER | âï¸ | âï¸ | | | | | JETSON_NX |
+âï¸ | âï¸ | | | | | JETSON_AGX_ORIN | âï¸ | âï¸ | | | | |
+JETSON_ORIN_NANO | âï¸ | âï¸ | | | | | AWS_T4 | âï¸ | âï¸ | | | | |
+INTEL_XEON_W_2233 | | | | | âï¸ | ### Software versions that support
+conversions and benchmarks for specific devices Software Versions requires only
+Jetson Device. If you are using a different device, you do not need to enter
+it. | Software Version / Device | JETSON_NANO | JETSON_TX2 | JETSON_XAVIER |
+JETSON_NX | JETSON_AGX_ORIN | JETSON_ORIN_NANO | |:--------------------------|:
+-----------:|:----------:|:-------------:|:---------:|:---------------:|:------
+----------:| | JETPACK_4_4_1 | âï¸ | | | | | | | JETPACK_4_6 | âï¸ |
+âï¸ | âï¸ | âï¸ | | | | JETPACK_5_0_1 | | | | | âï¸ | | |
+JETPACK_5_0_2 | | | | âï¸ | | | | JETPACK_6_0 | | | | | | âï¸ | The code
+below is an example of using software version. ```python conversion_result =
+converter.convert_model( input_model_path=INPUT_MODEL_PATH,
 output_dir=OUTPUT_DIR, target_framework=Framework.TENSORRT,
 target_device_name=DeviceName.JETSON_AGX_ORIN,
 target_software_version=SoftwareVersion.JETPACK_5_0_1, ) benchmark_result =
 benchmarker.benchmark_model( input_model_path=CONVERTED_MODEL_PATH,
 target_device_name=DeviceName.JETSON_AGX_ORIN,
 target_software_version=SoftwareVersion.JETPACK_5_0_1, ) ``` ### Hardware type
 that support benchmarks for specific devices Benchmark and compare models with
```

### Comparing `netspresso-1.5.0/netspresso.egg-info/SOURCES.txt` & `netspresso-1.6.0/netspresso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netspresso-1.5.0/setup.py` & `netspresso-1.6.0/setup.py`

 * *Files identical despite different names*

