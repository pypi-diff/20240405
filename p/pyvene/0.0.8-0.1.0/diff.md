# Comparing `tmp/pyvene-0.0.8.tar.gz` & `tmp/pyvene-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvene-0.0.8.tar", last modified: Tue Mar 26 07:52:26 2024, max compression
+gzip compressed data, was "pyvene-0.1.0.tar", last modified: Fri Apr  5 00:18:40 2024, max compression
```

## Comparing `pyvene-0.0.8.tar` & `pyvene-0.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.794264 pyvene-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-26 07:52:22.000000 pyvene-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 07:52:22.000000 pyvene-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-03-26 07:52:26.794264 pyvene-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-26 07:52:22.000000 pyvene-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.786264 pyvene-0.0.8/pyvene/
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.786264 pyvene-0.0.8/pyvene/data_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/data_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/data_generators/causal_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.790264 pyvene-0.0.8/pyvene/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.790264 pyvene-0.0.8/pyvene/models/backpack_gpt2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/backpack_gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/backpack_gpt2/modelings_backpack_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/backpack_gpt2/modelings_intervenable_backpack_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/basic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.790264 pyvene-0.0.8/pyvene/models/blip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/blip/modelings_blip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/blip/modelings_blip_itm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/blip/modelings_intervenable_blip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/blip/modelings_intervenable_blip_itm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/configuration_intervenable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.790264 pyvene-0.0.8/pyvene/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gpt2/modelings_intervenable_gpt2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.790264 pyvene-0.0.8/pyvene/models/gpt_neo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gpt_neo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gpt_neo/modelings_intervenable_gpt_neo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.790264 pyvene-0.0.8/pyvene/models/gpt_neox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gpt_neox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gpt_neox/modelings_intervenable_gpt_neox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.794264 pyvene-0.0.8/pyvene/models/gru/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gru/modelings_gru.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/gru/modelings_intervenable_gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    74237 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/intervenable_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/intervenable_modelcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/intervention_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19473 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/interventions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.794264 pyvene-0.0.8/pyvene/models/llama/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/llama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/llama/modelings_intervenable_llama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.794264 pyvene-0.0.8/pyvene/models/mistral/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/mistral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/mistral/modellings_intervenable_mistral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.794264 pyvene-0.0.8/pyvene/models/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/mlp/modelings_intervenable_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/mlp/modelings_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-03-26 07:52:22.000000 pyvene-0.0.8/pyvene/models/modeling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:52:26.794264 pyvene-0.0.8/pyvene.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-03-26 07:52:26.000000 pyvene-0.0.8/pyvene.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-26 07:52:26.000000 pyvene-0.0.8/pyvene.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 07:52:26.000000 pyvene-0.0.8/pyvene.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-26 07:52:26.000000 pyvene-0.0.8/pyvene.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 07:52:26.000000 pyvene-0.0.8/pyvene.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-03-26 07:52:22.000000 pyvene-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 07:52:26.794264 pyvene-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-26 07:52:22.000000 pyvene-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 00:18:36.000000 pyvene-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:18:36.000000 pyvene-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-04-05 00:18:40.549513 pyvene-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-05 00:18:36.000000 pyvene-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.545513 pyvene-0.1.0/pyvene/
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.545513 pyvene-0.1.0/pyvene/data_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/data_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16588 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/data_generators/causal_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.545513 pyvene-0.1.0/pyvene/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.545513 pyvene-0.1.0/pyvene/models/backpack_gpt2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/backpack_gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/backpack_gpt2/modelings_backpack_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/backpack_gpt2/modelings_intervenable_backpack_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/basic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/blip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/modelings_blip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/modelings_blip_itm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/modelings_intervenable_blip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/modelings_intervenable_blip_itm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/configuration_intervenable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt2/modelings_intervenable_gpt2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/gpt_neo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt_neo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt_neo/modelings_intervenable_gpt_neo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/gpt_neox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt_neox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt_neox/modelings_intervenable_gpt_neox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/gru/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gru/modelings_gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gru/modelings_intervenable_gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74237 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/intervenable_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/intervenable_modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/intervention_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19473 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/interventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/llama/modelings_intervenable_llama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/mistral/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mistral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mistral/modellings_intervenable_mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mlp/modelings_intervenable_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mlp/modelings_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/modeling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-04-05 00:18:36.000000 pyvene-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:18:40.553513 pyvene-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-05 00:18:36.000000 pyvene-0.1.0/setup.py
```

### Comparing `pyvene-0.0.8/LICENSE` & `pyvene-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/PKG-INFO` & `pyvene-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvene
-Version: 0.0.8
+Version: 0.1.0
 Summary: Use Activation Intervention to Interpret Causal Mechanism of Model
 Home-page: https://github.com/stanfordnlp/pyvene
 Author: Zhengxuan Wu
 Author-email: wuzhengx@stanford.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -13,26 +13,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
-Requires-Dist: transformers==4.38.1
-Requires-Dist: datasets==2.16.1
-Requires-Dist: protobuf==3.20.*
-Requires-Dist: matplotlib==3.7.4
-Requires-Dist: seaborn==0.13.1
-Requires-Dist: ipywidgets==8.1.1
-Requires-Dist: plotnine==0.12.4
+Requires-Dist: transformers>=4.38.1
+Requires-Dist: datasets>=2.16.1
+Requires-Dist: protobuf>=3.20.0
+Requires-Dist: matplotlib>=3.7.4
+Requires-Dist: seaborn>=0.13.1
+Requires-Dist: ipywidgets>=8.1.1
+Requires-Dist: plotnine>=0.12.4
 Requires-Dist: huggingface-hub==0.20.3
-Requires-Dist: numpy==1.23.5
-Requires-Dist: fsspec==2023.6.0
+Requires-Dist: numpy>=1.23.5
+Requires-Dist: fsspec>=2023.6.0
 Requires-Dist: accelerate>=0.26.1
-Requires-Dist: sentencepiece==0.1.96
+Requires-Dist: sentencepiece>=0.1.96
 
 <br />
 <div align="center">
   <h1 align="center"><img src="https://i.ibb.co/BNkhQH3/pyvene-logo.png"></h1>
   <a href="https://arxiv.org/abs/2403.07809"><strong>Read Our Paper »</strong></a>
 </div>
```

### Comparing `pyvene-0.0.8/README.md` & `pyvene-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/__init__.py` & `pyvene-0.1.0/pyvene/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/data_generators/causal_model.py` & `pyvene-0.1.0/pyvene/data_generators/causal_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,28 +305,35 @@
 
     def generate_factual_dataset(
         self,
         size,
         sampler=None,
         filter=None,
         device="cpu",
+        input_function=None,
+        output_function=None,
         return_tensors=True,
     ):
         if sampler is None:
             sampler = self.sample_input
+        
+        if input_function is None:
+            input_function = self.input_to_tensor
+        if output_function is None:
+            output_function = self.output_to_tensor
 
         examples = []
         while len(examples) < size:
             example = dict()
             input = sampler()
             if filter is None or filter(input):
                 output = self.run_forward(input)
                 if return_tensors:
-                    example['input_ids'] = self.input_to_tensor(input).to(device)
-                    example['labels'] = self.output_to_tensor(output).to(device)
+                    example['input_ids'] = input_function(input).to(device)
+                    example['labels'] = output_function(output).to(device)
                 else:
                     example['input_ids'] = input
                     example['labels'] = output
                 examples.append(example)
 
         return examples
 
@@ -335,16 +342,23 @@
         size,
         intervention_id,
         batch_size,
         sampler=None,
         intervention_sampler=None,
         filter=None,
         device="cpu",
+        input_function=None,
+        output_function=None,
         return_tensors=True,
     ):
+        if input_function is None:
+            input_function = self.input_to_tensor
+        if output_function is None:
+            output_function = self.output_to_tensor
+
         maxlength = len(
             [
                 var
                 for var in self.variables
                 if var not in self.inputs and var not in self.outputs
             ]
         )
```

### Comparing `pyvene-0.0.8/pyvene/models/backpack_gpt2/modelings_backpack_gpt2.py` & `pyvene-0.1.0/pyvene/models/backpack_gpt2/modelings_backpack_gpt2.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/backpack_gpt2/modelings_intervenable_backpack_gpt2.py` & `pyvene-0.1.0/pyvene/models/backpack_gpt2/modelings_intervenable_backpack_gpt2.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/basic_utils.py` & `pyvene-0.1.0/pyvene/models/basic_utils.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/blip/modelings_blip.py` & `pyvene-0.1.0/pyvene/models/blip/modelings_blip.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/blip/modelings_blip_itm.py` & `pyvene-0.1.0/pyvene/models/blip/modelings_blip_itm.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/blip/modelings_intervenable_blip.py` & `pyvene-0.1.0/pyvene/models/blip/modelings_intervenable_blip.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/blip/modelings_intervenable_blip_itm.py` & `pyvene-0.1.0/pyvene/models/blip/modelings_intervenable_blip_itm.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/configuration_intervenable_model.py` & `pyvene-0.1.0/pyvene/models/configuration_intervenable_model.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/constants.py` & `pyvene-0.1.0/pyvene/models/constants.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/gpt2/modelings_intervenable_gpt2.py` & `pyvene-0.1.0/pyvene/models/gpt2/modelings_intervenable_gpt2.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/gpt_neo/modelings_intervenable_gpt_neo.py` & `pyvene-0.1.0/pyvene/models/gpt_neo/modelings_intervenable_gpt_neo.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/gpt_neox/modelings_intervenable_gpt_neox.py` & `pyvene-0.1.0/pyvene/models/gpt_neox/modelings_intervenable_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/gru/modelings_gru.py` & `pyvene-0.1.0/pyvene/models/gru/modelings_gru.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/gru/modelings_intervenable_gru.py` & `pyvene-0.1.0/pyvene/models/gru/modelings_intervenable_gru.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/intervenable_base.py` & `pyvene-0.1.0/pyvene/models/intervenable_base.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/intervenable_modelcard.py` & `pyvene-0.1.0/pyvene/models/intervenable_modelcard.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,74 +3,82 @@
 from .mistral.modellings_intervenable_mistral import *
 from .gpt2.modelings_intervenable_gpt2 import *
 from .gpt_neo.modelings_intervenable_gpt_neo import *
 from .gpt_neox.modelings_intervenable_gpt_neox import *
 from .mlp.modelings_intervenable_mlp import *
 from .gru.modelings_intervenable_gru import *
 from .blip.modelings_intervenable_blip import *
+from .blip.modelings_intervenable_blip_itm import *
 from .backpack_gpt2.modelings_intervenable_backpack_gpt2 import *
 
 
 #########################################################################
 """
 Below are functions that you need to modify if you add
 a new model arch type in this library.
 
 We put them in front so it is easier to keep track of
 things that need to be changed.
 """
 
 import transformers.models as hf_models
 from .blip.modelings_blip import BlipWrapper
+from .blip.modelings_blip_itm import BlipITMWrapper
 from .mlp.modelings_mlp import MLPModel, MLPForClassification
 from .gru.modelings_gru import GRUModel, GRULMHeadModel, GRUForClassification
 from .backpack_gpt2.modelings_backpack_gpt2 import BackpackGPT2LMHeadModel
 
 global type_to_module_mapping
 global type_to_dimension_mapping
 global output_to_subcomponent_fn_mapping
 global scatter_intervention_output_fn_mapping
 
 
 type_to_module_mapping = {
     hf_models.gpt2.modeling_gpt2.GPT2Model: gpt2_type_to_module_mapping,
     hf_models.gpt2.modeling_gpt2.GPT2LMHeadModel: gpt2_lm_type_to_module_mapping,
+    hf_models.gpt2.modeling_gpt2.GPT2ForSequenceClassification: gpt2_classifier_type_to_module_mapping,
     hf_models.llama.modeling_llama.LlamaModel: llama_type_to_module_mapping,
     hf_models.llama.modeling_llama.LlamaForCausalLM: llama_lm_type_to_module_mapping,
     hf_models.gpt_neo.modeling_gpt_neo.GPTNeoModel: gpt_neo_type_to_module_mapping,
     hf_models.gpt_neo.modeling_gpt_neo.GPTNeoForCausalLM: gpt_neo_lm_type_to_module_mapping,
     hf_models.gpt_neox.modeling_gpt_neox.GPTNeoXModel: gpt_neox_type_to_module_mapping,
     hf_models.gpt_neox.modeling_gpt_neox.GPTNeoXForCausalLM: gpt_neox_lm_type_to_module_mapping,
     hf_models.mistral.modeling_mistral.MistralModel: mistral_type_to_module_mapping,
     hf_models.mistral.modeling_mistral.MistralForCausalLM: mistral_lm_type_to_module_mapping,
     hf_models.blip.modeling_blip.BlipForQuestionAnswering: blip_type_to_module_mapping,
+    hf_models.blip.modeling_blip.BlipForImageTextRetrieval: blip_itm_type_to_module_mapping,
     BlipWrapper: blip_wrapper_type_to_module_mapping,
+    BlipITMWrapper: blip_itm_wrapper_type_to_module_mapping,
     MLPModel: mlp_type_to_module_mapping,
     MLPForClassification: mlp_classifier_type_to_module_mapping,
     GRUModel: gru_type_to_module_mapping,
     GRULMHeadModel: gru_lm_type_to_module_mapping,
     GRUForClassification: gru_classifier_type_to_module_mapping,
     BackpackGPT2LMHeadModel: backpack_gpt2_lm_type_to_module_mapping,
     # new model type goes here after defining the model files
 }
 
 
 type_to_dimension_mapping = {
     hf_models.gpt2.modeling_gpt2.GPT2Model: gpt2_type_to_dimension_mapping,
     hf_models.gpt2.modeling_gpt2.GPT2LMHeadModel: gpt2_lm_type_to_dimension_mapping,
+    hf_models.gpt2.modeling_gpt2.GPT2ForSequenceClassification: gpt2_classifier_type_to_dimension_mapping,
     hf_models.llama.modeling_llama.LlamaModel: llama_type_to_dimension_mapping,
     hf_models.llama.modeling_llama.LlamaForCausalLM: llama_lm_type_to_dimension_mapping,
     hf_models.gpt_neo.modeling_gpt_neo.GPTNeoModel: gpt_neo_type_to_dimension_mapping,
     hf_models.gpt_neo.modeling_gpt_neo.GPTNeoForCausalLM: gpt_neo_lm_type_to_dimension_mapping,
     hf_models.gpt_neox.modeling_gpt_neox.GPTNeoXModel: gpt_neox_type_to_dimension_mapping,
     hf_models.gpt_neox.modeling_gpt_neox.GPTNeoXForCausalLM: gpt_neox_lm_type_to_dimension_mapping,
     hf_models.mistral.modeling_mistral.MistralModel: mistral_type_to_dimension_mapping,
     hf_models.mistral.modeling_mistral.MistralForCausalLM: mistral_lm_type_to_dimension_mapping,
     hf_models.blip.modeling_blip.BlipForQuestionAnswering: blip_type_to_dimension_mapping,
+    hf_models.blip.modeling_blip.BlipForImageTextRetrieval: blip_itm_type_to_dimension_mapping,
     BlipWrapper: blip_wrapper_type_to_dimension_mapping,
+    BlipITMWrapper: blip_itm_wrapper_type_to_dimension_mapping,
     MLPModel: mlp_type_to_dimension_mapping,
     MLPForClassification: mlp_classifier_type_to_dimension_mapping,
     GRUModel: gru_type_to_dimension_mapping,
     GRULMHeadModel: gru_lm_type_to_dimension_mapping,
     GRUForClassification: gru_classifier_type_to_dimension_mapping,
     BackpackGPT2LMHeadModel: backpack_gpt2_lm_type_to_dimension_mapping,
     # new model type goes here after defining the model files
```

### Comparing `pyvene-0.0.8/pyvene/models/intervention_utils.py` & `pyvene-0.1.0/pyvene/models/intervention_utils.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/interventions.py` & `pyvene-0.1.0/pyvene/models/interventions.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/layers.py` & `pyvene-0.1.0/pyvene/models/layers.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/llama/modelings_intervenable_llama.py` & `pyvene-0.1.0/pyvene/models/llama/modelings_intervenable_llama.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/mistral/modellings_intervenable_mistral.py` & `pyvene-0.1.0/pyvene/models/mistral/modellings_intervenable_mistral.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/mlp/modelings_intervenable_mlp.py` & `pyvene-0.1.0/pyvene/models/mlp/modelings_intervenable_mlp.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/mlp/modelings_mlp.py` & `pyvene-0.1.0/pyvene/models/mlp/modelings_mlp.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene/models/modeling_utils.py` & `pyvene-0.1.0/pyvene/models/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/pyvene.egg-info/PKG-INFO` & `pyvene-0.1.0/pyvene.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvene
-Version: 0.0.8
+Version: 0.1.0
 Summary: Use Activation Intervention to Interpret Causal Mechanism of Model
 Home-page: https://github.com/stanfordnlp/pyvene
 Author: Zhengxuan Wu
 Author-email: wuzhengx@stanford.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -13,26 +13,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
-Requires-Dist: transformers==4.38.1
-Requires-Dist: datasets==2.16.1
-Requires-Dist: protobuf==3.20.*
-Requires-Dist: matplotlib==3.7.4
-Requires-Dist: seaborn==0.13.1
-Requires-Dist: ipywidgets==8.1.1
-Requires-Dist: plotnine==0.12.4
+Requires-Dist: transformers>=4.38.1
+Requires-Dist: datasets>=2.16.1
+Requires-Dist: protobuf>=3.20.0
+Requires-Dist: matplotlib>=3.7.4
+Requires-Dist: seaborn>=0.13.1
+Requires-Dist: ipywidgets>=8.1.1
+Requires-Dist: plotnine>=0.12.4
 Requires-Dist: huggingface-hub==0.20.3
-Requires-Dist: numpy==1.23.5
-Requires-Dist: fsspec==2023.6.0
+Requires-Dist: numpy>=1.23.5
+Requires-Dist: fsspec>=2023.6.0
 Requires-Dist: accelerate>=0.26.1
-Requires-Dist: sentencepiece==0.1.96
+Requires-Dist: sentencepiece>=0.1.96
 
 <br />
 <div align="center">
   <h1 align="center"><img src="https://i.ibb.co/BNkhQH3/pyvene-logo.png"></h1>
   <a href="https://arxiv.org/abs/2403.07809"><strong>Read Our Paper »</strong></a>
 </div>
```

### Comparing `pyvene-0.0.8/pyvene.egg-info/SOURCES.txt` & `pyvene-0.1.0/pyvene.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvene-0.0.8/setup.py` & `pyvene-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="pyvene",
-    version="0.0.8",
+    version="0.1.0",
     description="Use Activation Intervention to Interpret Causal Mechanism of Model",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/stanfordnlp/pyvene",
     author="Zhengxuan Wu",
     author_email="wuzhengx@stanford.edu",
     license="Apache License 2.0",
```

