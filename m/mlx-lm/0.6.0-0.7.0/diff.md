# Comparing `tmp/mlx-lm-0.6.0.tar.gz` & `tmp/mlx-lm-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx-lm-0.6.0.tar", last modified: Tue Apr  2 20:54:33 2024, max compression
+gzip compressed data, was "mlx-lm-0.7.0.tar", last modified: Fri Apr  5 21:11:51 2024, max compression
```

## Comparing `mlx-lm-0.6.0.tar` & `mlx-lm-0.7.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.022838 mlx-lm-0.6.0/
--rw-r--r--   0 awnihannun   (501) staff       (20)       63 2024-01-19 21:42:37.000000 mlx-lm-0.6.0/MANIFEST.in
--rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-02 20:54:33.022664 mlx-lm-0.6.0/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)     4604 2024-03-03 19:16:48.000000 mlx-lm-0.6.0/README.md
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.015215 mlx-lm-0.6.0/mlx_lm/
--rw-r--r--   0 awnihannun   (501) staff       (20)      113 2024-02-28 03:35:15.000000 mlx-lm-0.6.0/mlx_lm/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1622 2024-03-21 17:35:13.000000 mlx-lm-0.6.0/mlx_lm/convert.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3542 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/fuse.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3887 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/generate.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    11364 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/gguf.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7852 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4770 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/merge.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.019754 mlx-lm-0.6.0/mlx_lm/models/
--rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-01-19 21:42:37.000000 mlx-lm-0.6.0/mlx_lm/models/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)      314 2024-01-19 21:42:37.000000 mlx-lm-0.6.0/mlx_lm/models/base.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5409 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/cohere.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     8281 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/dbrx.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5548 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/gemma.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6307 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/llama.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7869 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/mixtral.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5092 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/olmo.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5961 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/phi.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6599 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/phixtral.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7101 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/plamo.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4990 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/qwen.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6523 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/qwen2.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     8479 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/models/qwen2_moe.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5931 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/stablelm.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5416 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/starcoder2.py
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-02-28 03:35:15.000000 mlx-lm-0.6.0/mlx_lm/py.typed
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/requirements.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)     1354 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/sample_utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    15877 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/server.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.020707 mlx-lm-0.6.0/mlx_lm/tuner/
--rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-02-28 03:35:15.000000 mlx-lm-0.6.0/mlx_lm/tuner/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3258 2024-03-20 13:42:49.000000 mlx-lm-0.6.0/mlx_lm/tuner/datasets.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     2875 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/tuner/lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     9439 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/tuner/trainer.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5354 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/tuner/utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    19526 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/version.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.022412 mlx-lm-0.6.0/mlx_lm.egg-info/
--rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)     1038 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/SOURCES.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/dependency_links.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/requires.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        7 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/top_level.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-04-02 20:54:33.022889 mlx-lm-0.6.0/setup.cfg
--rw-r--r--   0 awnihannun   (501) staff       (20)      824 2024-02-28 03:35:15.000000 mlx-lm-0.6.0/setup.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.021976 mlx-lm-0.6.0/tests/
--rw-r--r--   0 awnihannun   (501) staff       (20)     2892 2024-03-20 13:42:49.000000 mlx-lm-0.6.0/tests/test_datsets.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1844 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/tests/test_gguf.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6052 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/tests/test_lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     9705 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/tests/test_models.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1446 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/tests/test_sample_utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     2955 2024-03-15 14:22:39.000000 mlx-lm-0.6.0/tests/test_utils.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.286661 mlx-lm-0.7.0/
+-rw-r--r--   0 awnihannun   (501) staff       (20)       63 2024-01-19 21:42:37.000000 mlx-lm-0.7.0/MANIFEST.in
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-05 21:11:51.286462 mlx-lm-0.7.0/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4604 2024-03-03 19:16:48.000000 mlx-lm-0.7.0/README.md
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.277913 mlx-lm-0.7.0/mlx_lm/
+-rw-r--r--   0 awnihannun   (501) staff       (20)      113 2024-02-28 03:35:15.000000 mlx-lm-0.7.0/mlx_lm/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1622 2024-03-21 17:35:13.000000 mlx-lm-0.7.0/mlx_lm/convert.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3542 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/fuse.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3887 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/generate.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    11364 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/gguf.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7852 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4770 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/merge.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.283101 mlx-lm-0.7.0/mlx_lm/models/
+-rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-01-19 21:42:37.000000 mlx-lm-0.7.0/mlx_lm/models/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)      314 2024-01-19 21:42:37.000000 mlx-lm-0.7.0/mlx_lm/models/base.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6061 2024-04-05 21:11:41.000000 mlx-lm-0.7.0/mlx_lm/models/cohere.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8281 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/dbrx.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5548 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/gemma.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6307 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/llama.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7869 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/mixtral.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5092 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/olmo.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5961 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/phi.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6599 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/phixtral.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7101 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/models/plamo.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4990 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/qwen.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6523 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/qwen2.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8479 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/models/qwen2_moe.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5931 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/stablelm.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5416 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/models/starcoder2.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-02-28 03:35:15.000000 mlx-lm-0.7.0/mlx_lm/py.typed
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/requirements.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1354 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/mlx_lm/sample_utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    15877 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/server.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.284256 mlx-lm-0.7.0/mlx_lm/tuner/
+-rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-02-28 03:35:15.000000 mlx-lm-0.7.0/mlx_lm/tuner/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3258 2024-03-20 13:42:49.000000 mlx-lm-0.7.0/mlx_lm/tuner/datasets.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2875 2024-03-25 13:08:25.000000 mlx-lm-0.7.0/mlx_lm/tuner/lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     9439 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/tuner/trainer.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5354 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/tuner/utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    19526 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/mlx_lm/utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-05 21:11:41.000000 mlx-lm-0.7.0/mlx_lm/version.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.286205 mlx-lm-0.7.0/mlx_lm.egg-info/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1038 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/requires.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        7 2024-04-05 21:11:51.000000 mlx-lm-0.7.0/mlx_lm.egg-info/top_level.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-04-05 21:11:51.286703 mlx-lm-0.7.0/setup.cfg
+-rw-r--r--   0 awnihannun   (501) staff       (20)      824 2024-02-28 03:35:15.000000 mlx-lm-0.7.0/setup.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-05 21:11:51.285894 mlx-lm-0.7.0/tests/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2892 2024-03-20 13:42:49.000000 mlx-lm-0.7.0/tests/test_datsets.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1844 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/tests/test_gguf.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6052 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/tests/test_lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     9705 2024-04-02 20:54:21.000000 mlx-lm-0.7.0/tests/test_models.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1446 2024-04-01 16:35:43.000000 mlx-lm-0.7.0/tests/test_sample_utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2955 2024-03-15 14:22:39.000000 mlx-lm-0.7.0/tests/test_utils.py
```

### Comparing `mlx-lm-0.6.0/PKG-INFO` & `mlx-lm-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-lm
-Version: 0.6.0
+Version: 0.7.0
 Summary: LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx-lm-0.6.0/README.md` & `mlx-lm-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/convert.py` & `mlx-lm-0.7.0/mlx_lm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/fuse.py` & `mlx-lm-0.7.0/mlx_lm/fuse.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/generate.py` & `mlx-lm-0.7.0/mlx_lm/generate.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/gguf.py` & `mlx-lm-0.7.0/mlx_lm/gguf.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/lora.py` & `mlx-lm-0.7.0/mlx_lm/lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/merge.py` & `mlx-lm-0.7.0/mlx_lm/merge.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/cohere.py` & `mlx-lm-0.7.0/mlx_lm/models/starcoder2.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,47 +6,42 @@
 
 from .base import BaseModelArgs
 
 
 @dataclass
 class ModelArgs(BaseModelArgs):
     model_type: str
-    hidden_size: int = 8192
-    num_hidden_layers: int = 40
-    intermediate_size: int = 22528
-    num_attention_heads: int = 64
-    num_key_value_heads: int = 64
-    rope_theta: float = 8000000.0
-    vocab_size: int = 256000
-    layer_norm_eps: float = 1e-05
-    logit_scale: float = 0.0625
-    attention_bias: bool = False
-    layer_norm_bias: bool = False
+    hidden_size: int
+    num_hidden_layers: int
+    intermediate_size: int
+    num_attention_heads: int
+    num_key_value_heads: int
+    norm_epsilon: float = 1e-5
+    vocab_size: int = 49152
+    rope_theta: float = 100000
+    tie_word_embeddings: bool = True
 
 
 class Attention(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.args = args
 
         dim = args.hidden_size
         self.n_heads = n_heads = args.num_attention_heads
         self.n_kv_heads = n_kv_heads = args.num_key_value_heads
 
         head_dim = args.hidden_size // args.num_attention_heads
         self.scale = head_dim**-0.5
 
-        attetion_bias = args.attention_bias
-
-        self.q_proj = nn.Linear(dim, n_heads * head_dim, bias=attetion_bias)
-        self.k_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=attetion_bias)
-        self.v_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=attetion_bias)
-        self.o_proj = nn.Linear(n_heads * head_dim, dim, bias=attetion_bias)
-
-        self.rope = nn.RoPE(head_dim, traditional=True, base=args.rope_theta)
+        self.q_proj = nn.Linear(dim, n_heads * head_dim, bias=True)
+        self.k_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=True)
+        self.v_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=True)
+        self.o_proj = nn.Linear(n_heads * head_dim, dim, bias=True)
+        self.rope = nn.RoPE(head_dim, traditional=False, base=args.rope_theta)
 
     def __call__(
         self,
         x: mx.array,
         mask: Optional[mx.array] = None,
         cache: Optional[Tuple[mx.array, mx.array]] = None,
     ) -> mx.array:
@@ -76,61 +71,60 @@
         output = output.transpose(0, 2, 1, 3).reshape(B, L, -1)
         return self.o_proj(output), (keys, values)
 
 
 class MLP(nn.Module):
     def __init__(self, dim, hidden_dim):
         super().__init__()
-        self.gate_proj = nn.Linear(dim, hidden_dim, bias=False)
-        self.up_proj = nn.Linear(dim, hidden_dim, bias=False)
-        self.down_proj = nn.Linear(hidden_dim, dim, bias=False)
+        self.c_fc = nn.Linear(dim, hidden_dim, bias=True)
+        self.c_proj = nn.Linear(hidden_dim, dim, bias=True)
 
     def __call__(self, x):
-        return self.down_proj(nn.silu(self.gate_proj(x)) * self.up_proj(x))
+        return self.c_proj(nn.gelu(self.c_fc(x)))
 
 
 class TransformerBlock(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.hidden_size = args.hidden_size
         self.n_heads = args.num_attention_heads
 
         self.self_attn = Attention(args)
         self.mlp = MLP(args.hidden_size, args.intermediate_size)
-        self.input_layernorm = nn.LayerNorm(
-            args.hidden_size, eps=args.layer_norm_eps, bias=args.layer_norm_bias
+        self.input_layernorm = nn.LayerNorm(args.hidden_size, eps=args.norm_epsilon)
+        self.post_attention_layernorm = nn.LayerNorm(
+            args.hidden_size, eps=args.norm_epsilon
         )
         self.args = args
 
     def __call__(
         self,
         x: mx.array,
         mask: Optional[mx.array] = None,
         cache: Optional[Tuple[mx.array, mx.array]] = None,
     ) -> mx.array:
-        h = self.input_layernorm(x)
-        attn_h, cache = self.self_attn(h, mask, cache)
-        ff_h = self.mlp(h)
-        return attn_h + ff_h + x, cache
+        r, cache = self.self_attn(self.input_layernorm(x), mask, cache)
+        h = x + r
+        r = self.mlp(self.post_attention_layernorm(h))
+        out = h + r
+        return out, cache
 
 
-class CohereModel(nn.Module):
+class Starcoder2Model(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.args = args
         self.vocab_size = args.vocab_size
         self.num_hidden_layers = args.num_hidden_layers
         assert self.vocab_size > 0
         self.embed_tokens = nn.Embedding(args.vocab_size, args.hidden_size)
         self.layers = [
             TransformerBlock(args=args) for _ in range(args.num_hidden_layers)
         ]
-        self.norm = nn.LayerNorm(
-            args.hidden_size, eps=args.layer_norm_eps, bias=args.layer_norm_bias
-        )
+        self.norm = nn.LayerNorm(args.hidden_size, eps=args.norm_epsilon)
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
     ):
         h = self.embed_tokens(inputs)
@@ -148,23 +142,28 @@
 
         return self.norm(h), cache
 
 
 class Model(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
+        self.args = args
         self.model_type = args.model_type
-        self.model = CohereModel(args)
+        self.model = Starcoder2Model(args)
+        self.lm_head = nn.Linear(args.hidden_size, args.vocab_size, bias=False)
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
     ):
         out, cache = self.model(inputs, cache)
-        out = out @ self.model.embed_tokens.weight.T
-        out = out * self.model.args.logit_scale
-        return out, cache
+        return self.lm_head(out), cache
+
+    def sanitize(self, weights):
+        if self.args.tie_word_embeddings and "lm_head.weight" not in weights:
+            weights["lm_head.weight"] = weights["model.embed_tokens.weight"]
+        return weights
 
     @property
     def layers(self):
         return self.model.layers
```

### Comparing `mlx-lm-0.6.0/mlx_lm/models/dbrx.py` & `mlx-lm-0.7.0/mlx_lm/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/gemma.py` & `mlx-lm-0.7.0/mlx_lm/models/gemma.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/llama.py` & `mlx-lm-0.7.0/mlx_lm/models/llama.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/mixtral.py` & `mlx-lm-0.7.0/mlx_lm/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/olmo.py` & `mlx-lm-0.7.0/mlx_lm/models/olmo.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/phi.py` & `mlx-lm-0.7.0/mlx_lm/models/phi.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/phixtral.py` & `mlx-lm-0.7.0/mlx_lm/models/phixtral.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/plamo.py` & `mlx-lm-0.7.0/mlx_lm/models/plamo.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/qwen.py` & `mlx-lm-0.7.0/mlx_lm/models/qwen.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/qwen2.py` & `mlx-lm-0.7.0/mlx_lm/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/qwen2_moe.py` & `mlx-lm-0.7.0/mlx_lm/models/qwen2_moe.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/stablelm.py` & `mlx-lm-0.7.0/mlx_lm/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/models/starcoder2.py` & `mlx-lm-0.7.0/mlx_lm/models/cohere.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,56 +6,85 @@
 
 from .base import BaseModelArgs
 
 
 @dataclass
 class ModelArgs(BaseModelArgs):
     model_type: str
-    hidden_size: int
-    num_hidden_layers: int
-    intermediate_size: int
-    num_attention_heads: int
-    num_key_value_heads: int
-    norm_epsilon: float = 1e-5
-    vocab_size: int = 49152
-    rope_theta: float = 100000
-    tie_word_embeddings: bool = True
+    hidden_size: int = 8192
+    num_hidden_layers: int = 40
+    intermediate_size: int = 22528
+    num_attention_heads: int = 64
+    num_key_value_heads: int = 64
+    rope_theta: float = 8000000.0
+    vocab_size: int = 256000
+    layer_norm_eps: float = 1e-05
+    logit_scale: float = 0.0625
+    attention_bias: bool = False
+    layer_norm_bias: bool = False
+    use_qk_norm: bool = False
+
+
+class LayerNorm2D(nn.Module):
+
+    def __init__(self, d1, d2, eps):
+        super().__init__()
+        self.weight = mx.zeros((d1, d2))
+        self.eps = eps
+
+    def __call__(self, x):
+        return self.weight * mx.fast.layer_norm(x, None, None, self.eps)
 
 
 class Attention(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.args = args
 
         dim = args.hidden_size
         self.n_heads = n_heads = args.num_attention_heads
         self.n_kv_heads = n_kv_heads = args.num_key_value_heads
 
         head_dim = args.hidden_size // args.num_attention_heads
         self.scale = head_dim**-0.5
 
-        self.q_proj = nn.Linear(dim, n_heads * head_dim, bias=True)
-        self.k_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=True)
-        self.v_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=True)
-        self.o_proj = nn.Linear(n_heads * head_dim, dim, bias=True)
-        self.rope = nn.RoPE(head_dim, traditional=False, base=args.rope_theta)
+        attetion_bias = args.attention_bias
+
+        self.q_proj = nn.Linear(dim, n_heads * head_dim, bias=attetion_bias)
+        self.k_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=attetion_bias)
+        self.v_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=attetion_bias)
+        self.o_proj = nn.Linear(n_heads * head_dim, dim, bias=attetion_bias)
+
+        self.use_qk_norm = args.use_qk_norm
+        if self.use_qk_norm:
+            self.q_norm = LayerNorm2D(self.n_heads, head_dim, eps=args.layer_norm_eps)
+            self.k_norm = LayerNorm2D(
+                self.n_kv_heads, head_dim, eps=args.layer_norm_eps
+            )
+
+        self.rope = nn.RoPE(head_dim, traditional=True, base=args.rope_theta)
 
     def __call__(
         self,
         x: mx.array,
         mask: Optional[mx.array] = None,
         cache: Optional[Tuple[mx.array, mx.array]] = None,
     ) -> mx.array:
         B, L, D = x.shape
 
         queries, keys, values = self.q_proj(x), self.k_proj(x), self.v_proj(x)
 
-        # Prepare the queries, keys and values for the attention computation
-        queries = queries.reshape(B, L, self.n_heads, -1).transpose(0, 2, 1, 3)
-        keys = keys.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
+        queries = queries.reshape(B, L, self.n_heads, -1)
+        keys = keys.reshape(B, L, self.n_kv_heads, -1)
+        if self.use_qk_norm:
+            queries = self.q_norm(queries)
+            keys = self.k_norm(keys)
+
+        queries = queries.transpose(0, 2, 1, 3)
+        keys = keys.transpose(0, 2, 1, 3)
         values = values.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
 
         if cache is not None:
             key_cache, value_cache = cache
             queries = self.rope(queries, offset=key_cache.shape[2])
             keys = self.rope(keys, offset=key_cache.shape[2])
             keys = mx.concatenate([key_cache, keys], axis=2)
@@ -71,60 +100,61 @@
         output = output.transpose(0, 2, 1, 3).reshape(B, L, -1)
         return self.o_proj(output), (keys, values)
 
 
 class MLP(nn.Module):
     def __init__(self, dim, hidden_dim):
         super().__init__()
-        self.c_fc = nn.Linear(dim, hidden_dim, bias=True)
-        self.c_proj = nn.Linear(hidden_dim, dim, bias=True)
+        self.gate_proj = nn.Linear(dim, hidden_dim, bias=False)
+        self.up_proj = nn.Linear(dim, hidden_dim, bias=False)
+        self.down_proj = nn.Linear(hidden_dim, dim, bias=False)
 
     def __call__(self, x):
-        return self.c_proj(nn.gelu(self.c_fc(x)))
+        return self.down_proj(nn.silu(self.gate_proj(x)) * self.up_proj(x))
 
 
 class TransformerBlock(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.hidden_size = args.hidden_size
         self.n_heads = args.num_attention_heads
 
         self.self_attn = Attention(args)
         self.mlp = MLP(args.hidden_size, args.intermediate_size)
-        self.input_layernorm = nn.LayerNorm(args.hidden_size, eps=args.norm_epsilon)
-        self.post_attention_layernorm = nn.LayerNorm(
-            args.hidden_size, eps=args.norm_epsilon
+        self.input_layernorm = nn.LayerNorm(
+            args.hidden_size, eps=args.layer_norm_eps, bias=args.layer_norm_bias
         )
         self.args = args
 
     def __call__(
         self,
         x: mx.array,
         mask: Optional[mx.array] = None,
         cache: Optional[Tuple[mx.array, mx.array]] = None,
     ) -> mx.array:
-        r, cache = self.self_attn(self.input_layernorm(x), mask, cache)
-        h = x + r
-        r = self.mlp(self.post_attention_layernorm(h))
-        out = h + r
-        return out, cache
+        h = self.input_layernorm(x)
+        attn_h, cache = self.self_attn(h, mask, cache)
+        ff_h = self.mlp(h)
+        return attn_h + ff_h + x, cache
 
 
-class Starcoder2Model(nn.Module):
+class CohereModel(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.args = args
         self.vocab_size = args.vocab_size
         self.num_hidden_layers = args.num_hidden_layers
         assert self.vocab_size > 0
         self.embed_tokens = nn.Embedding(args.vocab_size, args.hidden_size)
         self.layers = [
             TransformerBlock(args=args) for _ in range(args.num_hidden_layers)
         ]
-        self.norm = nn.LayerNorm(args.hidden_size, eps=args.norm_epsilon)
+        self.norm = nn.LayerNorm(
+            args.hidden_size, eps=args.layer_norm_eps, bias=args.layer_norm_bias
+        )
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
     ):
         h = self.embed_tokens(inputs)
@@ -142,28 +172,23 @@
 
         return self.norm(h), cache
 
 
 class Model(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
-        self.args = args
         self.model_type = args.model_type
-        self.model = Starcoder2Model(args)
-        self.lm_head = nn.Linear(args.hidden_size, args.vocab_size, bias=False)
+        self.model = CohereModel(args)
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
     ):
         out, cache = self.model(inputs, cache)
-        return self.lm_head(out), cache
-
-    def sanitize(self, weights):
-        if self.args.tie_word_embeddings and "lm_head.weight" not in weights:
-            weights["lm_head.weight"] = weights["model.embed_tokens.weight"]
-        return weights
+        out = out @ self.model.embed_tokens.weight.T
+        out = out * self.model.args.logit_scale
+        return out, cache
 
     @property
     def layers(self):
         return self.model.layers
```

### Comparing `mlx-lm-0.6.0/mlx_lm/sample_utils.py` & `mlx-lm-0.7.0/mlx_lm/sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/server.py` & `mlx-lm-0.7.0/mlx_lm/server.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/tuner/datasets.py` & `mlx-lm-0.7.0/mlx_lm/tuner/datasets.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/tuner/lora.py` & `mlx-lm-0.7.0/mlx_lm/tuner/lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/tuner/trainer.py` & `mlx-lm-0.7.0/mlx_lm/tuner/trainer.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/tuner/utils.py` & `mlx-lm-0.7.0/mlx_lm/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm/utils.py` & `mlx-lm-0.7.0/mlx_lm/utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/mlx_lm.egg-info/PKG-INFO` & `mlx-lm-0.7.0/mlx_lm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-lm
-Version: 0.6.0
+Version: 0.7.0
 Summary: LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx-lm-0.6.0/mlx_lm.egg-info/SOURCES.txt` & `mlx-lm-0.7.0/mlx_lm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/setup.py` & `mlx-lm-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/tests/test_datsets.py` & `mlx-lm-0.7.0/tests/test_datsets.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/tests/test_gguf.py` & `mlx-lm-0.7.0/tests/test_gguf.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/tests/test_lora.py` & `mlx-lm-0.7.0/tests/test_lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/tests/test_models.py` & `mlx-lm-0.7.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/tests/test_sample_utils.py` & `mlx-lm-0.7.0/tests/test_sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.6.0/tests/test_utils.py` & `mlx-lm-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

