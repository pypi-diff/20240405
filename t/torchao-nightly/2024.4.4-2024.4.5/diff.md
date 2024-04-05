# Comparing `tmp/torchao-nightly-2024.4.4.tar.gz` & `tmp/torchao-nightly-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchao-nightly-2024.4.4.tar", last modified: Thu Apr  4 00:26:59 2024, max compression
+gzip compressed data, was "torchao-nightly-2024.4.5.tar", last modified: Fri Apr  5 00:19:11 2024, max compression
```

## Comparing `torchao-nightly-2024.4.4.tar` & `torchao-nightly-2024.4.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:26:59.955481 torchao-nightly-2024.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-04 00:26:59.955481 torchao-nightly-2024.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:26:59.955481 torchao-nightly-2024.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:26:59.947481 torchao-nightly-2024.4.4/torchao/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:26:59.951480 torchao-nightly-2024.4.4/torchao/dtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/dtypes/nf4tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/dtypes/uint4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:26:59.951480 torchao-nightly-2024.4.4/torchao/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/kernel/autotuner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/kernel/intmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/kernel/intmm_triton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:26:59.951480 torchao-nightly-2024.4.4/torchao/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)    48840 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/GPTQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/dynamic_quant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/quant_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/quant_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/smoothquant.py
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/subclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/unified.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/quantization/weight_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:26:59.951480 torchao-nightly-2024.4.4/torchao/sparsity/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/sparsity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/sparsity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-04 00:26:48.000000 torchao-nightly-2024.4.4/torchao/sparsity/wanda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:26:59.951480 torchao-nightly-2024.4.4/torchao_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-04 00:26:59.000000 torchao-nightly-2024.4.4/torchao_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-04 00:26:59.000000 torchao-nightly-2024.4.4/torchao_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:26:59.000000 torchao-nightly-2024.4.4/torchao_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 00:26:59.000000 torchao-nightly-2024.4.4/torchao_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 00:26:59.000000 torchao-nightly-2024.4.4/torchao_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.347684 torchao-nightly-2024.4.5/torchao/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.347684 torchao-nightly-2024.4.5/torchao/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/dtypes/nf4tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/dtypes/uint4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.347684 torchao-nightly-2024.4.5/torchao/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/kernel/autotuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/kernel/intmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/kernel/intmm_triton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/torchao/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)    52411 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/GPTQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/dynamic_quant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/quant_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/quant_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/smoothquant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/subclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/unified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/weight_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/torchao/sparsity/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/sparsity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/sparsity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/sparsity/wanda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/torchao_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/top_level.txt
```

### Comparing `torchao-nightly-2024.4.4/LICENSE` & `torchao-nightly-2024.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/PKG-INFO` & `torchao-nightly-2024.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.4.4
+Version: 2024.4.5
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
```

### Comparing `torchao-nightly-2024.4.4/README.md` & `torchao-nightly-2024.4.5/README.md`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/setup.py` & `torchao-nightly-2024.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return file.read().splitlines()
 
 
 # Determine the package name based on the presence of an environment variable
 package_name = "torchao-nightly" if os.environ.get("TORCHAO_NIGHTLY") else "torchao"
 
 # Version is year.month.date if using nightlies
-version = current_date if package_name == "torchao-nightly" else "0.0.3"
+version = current_date if package_name == "torchao-nightly" else "0.1"
 
 
 setup(
     name=package_name,
     version=version,
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `torchao-nightly-2024.4.4/torchao/dtypes/nf4tensor.py` & `torchao-nightly-2024.4.5/torchao/dtypes/nf4tensor.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/dtypes/uint4.py` & `torchao-nightly-2024.4.5/torchao/dtypes/uint4.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/kernel/autotuner.py` & `torchao-nightly-2024.4.5/torchao/kernel/autotuner.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/kernel/intmm.py` & `torchao-nightly-2024.4.5/torchao/kernel/intmm.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/kernel/intmm_triton.py` & `torchao-nightly-2024.4.5/torchao/kernel/intmm_triton.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/GPTQ.py` & `torchao-nightly-2024.4.5/torchao/quantization/GPTQ.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .unified import Quantizer
 
 from .quant_primitives import (
     get_groupwise_affine_qparams,
     groupwise_affine_quantize_tensor_from_qparams,
     groupwise_affine_dequantize_tensor_from_qparams,
     pack_tinygemm_scales_and_zeros,
+    groupwise_affine_quantize_tensor,
 )
 aten = torch.ops.aten
 
 ## eval.py ##
 
 try:
     import lm_eval  # pyre-ignore[21]  # noqa: F401
@@ -61,16 +62,16 @@
 
 if TORCH_VERSION_AFTER_2_3:
     add_ons += ["Int8DynActInt4WeightQuantizer", "Int8DynActInt4WeightGPTQQuantizer"]
 
 
 __all__ = [
     "MultiInput",
-    "WeightOnlyInt4Linear",
     "Int4WeightOnlyGPTQQuantizer",
+    "Int4WeightOnlyQuantizer",
 ] + add_ons
 
 if lm_eval_available:
     class InputRecorder(eval_wrapper):
         """
         This is a fake evaluation wrapper from the lm_eval library that just records the inputs
         so that they can be used in calibration.
@@ -113,15 +114,18 @@
             self.pad_calibration_inputs = pad_calibration_inputs
             self.pad_token = pad_token
 
             self.inputs = None
 
         @property
         def eot_token_id(self):
-            return self._tokenizer.eos_id()
+            try:
+                return self._tokenizer.eos_id()
+            except:
+                return self._tokenizer.eos_id
 
         @property
         def max_length(self):
             return self._max_seq_length
 
         @property
         def max_gen_toks(self):
@@ -135,15 +139,18 @@
         def device(self):
             return self._device
 
         def tok_encode(self, string: str, **kwargs):
             # TODO: verify this for multi-batch as well
             tokens = self._tokenizer.encode(string)
             if hasattr(self._tokenizer, "bos_id"):
-                tokens = [self._tokenizer.bos_id()] + tokens
+                try:
+                    tokens = [self._tokenizer.bos_id()] + tokens
+                except:
+                    tokens = [self._tokenizer.bos_id] + tokens
             return tokens
 
         def tok_decode(self, tokens):
             decoded = self._tokenizer.decode(tokens)
             return decoded
 
         def add_input(self, args):
@@ -743,14 +750,20 @@
     def _convert_for_runtime(self, model: torch.nn.Module) -> "nn.Module":
         raise NotImplementedError("_convert_for_runtime not implemented")
 
     @torch.no_grad()
     def quantize(self, model: torch.nn.Module, inputs: List[MultiInput], **kwargs: Any) -> torch.nn.Module:
         pass
 
+def _check_linear_int4_k(k, groupsize = 1, inner_k_tiles = None):
+    k_divisible_by_groupsize = k % groupsize == 0
+    if inner_k_tiles is not None:
+        k_divisible_by_16_times_inner_k_tiles = k % (inner_k_tiles * 16) == 0
+        return k_divisible_by_groupsize and k_divisible_by_16_times_inner_k_tiles
+    return k_divisible_by_groupsize
 
 def linear_forward_int4(x, weight_int4pack, scales_and_zeros, out_features, groupsize):
     origin_x_size = x.size()
     x = x.reshape(-1, origin_x_size[-1])
     c = torch.ops.aten._weight_int4pack_mm(x, weight_int4pack, groupsize, scales_and_zeros)
     new_shape = origin_x_size[:-1] + (out_features,)
     c = c.reshape(new_shape)
@@ -763,15 +776,15 @@
     weight: torch.Tensor
 
     def __init__(
             self, in_features: int, out_features: int,
             bias=False, device=None, dtype=None, groupsize: int = 128, inner_k_tiles: int = 8, use_cuda=True,
     ) -> None:
         super().__init__()
-        self.padding = _check_linear_int4_k(in_features, groupsize, inner_k_tiles)
+        self.padding = not _check_linear_int4_k(in_features, groupsize, inner_k_tiles)
         if self.padding:
             from model import find_multiple
             self.origin_in_features = in_features
             in_features = find_multiple(in_features, 1024)
 
         self.in_features = in_features
         self.out_features = out_features
@@ -802,34 +815,103 @@
             import torch.nn.functional as F
             input = F.pad(input, pad=(0, self.in_features - self.origin_in_features))
         return linear_forward_int4(
             input,
             self.weight, self.scales_and_zeros, self.out_features, self.groupsize
         )
 
-
-def _check_linear_int4_k(k, groupsize = 1, inner_k_tiles = None):
-    k_divisible_by_groupsize = k % groupsize == 0
-    if inner_k_tiles is not None:
-        k_divisible_by_16_times_inner_k_tiles = k % (inner_k_tiles * 16) == 0
-        return k_divisible_by_groupsize and k_divisible_by_16_times_inner_k_tiles
-    return k_divisible_by_groupsize
-
 def replace_linear_int4(module, groupsize, inner_k_tiles, padding_allowed, use_cuda=True, skip_layer_func = None):
 
     for name, child in module.named_children():
         if isinstance(child, nn.Linear) and (skip_layer_func is None or not skip_layer_func(child.weight)):
             if _check_linear_int4_k(child.in_features, groupsize, inner_k_tiles) or padding_allowed:
                 setattr(module, name, WeightOnlyInt4Linear(
                     child.in_features, child.out_features, bias=False,
                     groupsize=groupsize, inner_k_tiles=inner_k_tiles, use_cuda=use_cuda
                 ))
         else:
             replace_linear_int4(child, groupsize, inner_k_tiles, padding_allowed, use_cuda, skip_layer_func)
 
+class Int4WeightOnlyQuantizer(Quantizer):
+    def __init__(
+        self,
+        groupsize: int = 256,
+        padding_allowed: bool = True,
+        inner_k_tiles: Optional[int] = 8,
+    ) -> None:
+        super().__init__()
+        assert inner_k_tiles in [2, 4, 8]
+        assert groupsize in [32, 64, 128, 256]
+
+        self.inner_k_tiles = inner_k_tiles
+        self.groupsize: int = groupsize
+        self.padding_allowed: bool = padding_allowed
+
+    @torch.no_grad()
+    def _create_quantized_state_dict(
+        self, model: torch.nn.Module
+    ) -> Dict[str, torch.Tensor]:
+        cur_state_dict = model.state_dict()
+        for fqn, mod in model.named_modules():
+            if isinstance(mod, torch.nn.Linear):
+                assert not mod.bias
+                out_features = mod.out_features
+                in_features = mod.in_features
+                # assert out_features % 8 == 0, "require out_features % 8 == 0"
+                print(f"linear: {fqn}, in={in_features}, out={out_features}")
+
+                assert (
+                    in_features % self.groupsize == 0
+                ), f"require in_features:{in_features} % self.groupsize:{self.groupsize} == 0"
+
+                weight = mod.weight.data
+                if not _check_linear_int4_k(
+                    in_features, self.groupsize, self.inner_k_tiles
+                ):
+                    if self.padding_allowed:
+                        from .utils import find_multiple
+                        import torch.nn.functional as F
+                        print(f"warning: {fqn} is padded to satisfy in_features % 1024 == 0")
+                        padded_in_features = find_multiple(in_features, 1024)
+                        weight = F.pad(weight, pad=(0, padded_in_features - in_features))
+                    else:
+                        print(f"warning: {fqn} is skipped, int4 requires that in_features is 32, 64, or is divisible by 1024, " +
+                                "and that groupsize and inner_k_tiles*16 evenly divide into it")
+                        continue
+                (
+                    w_int4x8,
+                    scales_and_zeros
+                ) = groupwise_affine_quantize_tensor(
+                    weight,
+                    4,  # n_bit
+                    self.groupsize,
+                )
+                weight_int4pack = torch.ops.aten._convert_weight_to_int4pack(w_int4x8.to("cuda"), self.inner_k_tiles)
+                cur_state_dict[f"{fqn}.weight"] = weight_int4pack.to("cuda")
+                cur_state_dict[f"{fqn}.scales_and_zeros"] = scales_and_zeros.to("cuda")
+        return cur_state_dict
+
+    def _convert_for_runtime(self, model: torch.nn.Module) -> torch.nn.Module:
+        replace_linear_int4(
+            model,
+            self.groupsize,
+            self.inner_k_tiles,
+            self.padding_allowed,
+        )
+        return model
+
+    def quantize(
+        self, model: torch.nn.Module, *args: Any, **kwargs: Any
+    ) -> torch.nn.Module:
+        state_dict = self._create_quantized_state_dict(model)
+        model = self._convert_for_runtime(model)
+        # TODO: make it strict
+        model.load_state_dict(state_dict, strict=False)
+        return model
+
 class Int4WeightOnlyGPTQQuantizer(GPTQQuantizer):
         def __init__(
             self,
             blocksize,
             percdamp,
             groupsize,
             inner_k_tiles=8,
@@ -864,15 +946,18 @@
             )
 
             # we need to do the padding here, both for q and the qparams if necessary
 
             # TODO: this is the gpt-fast version, merge with the main version later
             def make_names_and_values_dict_func(q, qparams):
                 k = q.shape[1]
-                new_k = find_multiple(k, 1024)
+                if not _check_linear_int4_k(k, groupsize):
+                    new_k = find_multiple(k, 1024)
+                else:
+                    new_k = k
                 # how much we need to pad the weight
                 delta_k = new_k - q.shape[1]
                 q = q.to(torch.int32)
                 final_q = torch.ops.aten._convert_weight_to_int4pack(F.pad(q, pad=(0, delta_k)), inner_k_tiles)
                 scales = qparams[0].to(torch.bfloat16)
                 zeros = qparams[1].to(torch.bfloat16)
                 scales_and_zeros = pack_tinygemm_scales_and_zeros(scales, zeros)
```

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/__init__.py` & `torchao-nightly-2024.4.5/torchao/quantization/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,8 +38,10 @@
     "set_smooth_fq_attribute",
     "Int8DynamicallyQuantizedLinearWeight",
     "Int8WeightOnlyQuantizedLinearWeight",
     "Int4WeightOnlyQuantizedLinearWeight",
     "compute_error",
     "get_model_size_in_bytes",
     "WeightOnlyInt8QuantLinear",
+    "Int4WeightOnlyGPTQQuantizer",
+    "Int4WeightOnlyQuantizer",
 ]
```

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/dynamic_quant.py` & `torchao-nightly-2024.4.5/torchao/quantization/dynamic_quant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/quant_api.py` & `torchao-nightly-2024.4.5/torchao/quantization/quant_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,29 @@
     Int8WeightOnlyQuantizedLinearWeight,
     QuantizedLinearWeightBase,
 )
 from .weight_only import WeightOnlyInt8QuantLinear
 from .unified import Quantizer, TwoStepQuantizer
 from .GPTQ import (
     Int4WeightOnlyGPTQQuantizer,
+    Int4WeightOnlyQuantizer,
 )
 
 
 __all__ = [
     "apply_weight_only_int8_quant",
     "apply_dynamic_quant",
     "change_linear_weights_to_int8_dqtensors",
     "change_linear_weights_to_int8_woqtensors",
     "change_linear_weights_to_int4_woqtensors",
     "swap_conv2d_1x1_to_linear",
     "Quantizer",
     "TwoStepQuantizer",
     "Int4WeightOnlyGPTQQuantizer",
+    "Int4WeightOnlyQuantizer"
 ]
 
 if TORCH_VERSION_AFTER_2_3:
     from .GPTQ import (
         Int8DynActInt4WeightQuantizer,
         Int8DynActInt4WeightGPTQQuantizer,
```

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/quant_primitives.py` & `torchao-nightly-2024.4.5/torchao/quantization/quant_primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,14 @@
         .transpose(0, 1)
         .contiguous()
     )
 
 
 def unpack_tinygemm_scales_and_zeros(scales_and_zeros):
     assert len(scales_and_zeros.shape) == 3 and scales_and_zeros.shape[2] == 2
-    assert scales_and_zeros.dtype == torch.float
     return torch.split(scales_and_zeros.transpose(0, 1), 1, 2)
 
 
 def groupwise_affine_quantize_tensor_from_qparams(
     w,
     scales,
     zeros,
```

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/smoothquant.py` & `torchao-nightly-2024.4.5/torchao/quantization/smoothquant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/subclass.py` & `torchao-nightly-2024.4.5/torchao/quantization/subclass.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/unified.py` & `torchao-nightly-2024.4.5/torchao/quantization/unified.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/utils.py` & `torchao-nightly-2024.4.5/torchao/quantization/utils.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/quantization/weight_only.py` & `torchao-nightly-2024.4.5/torchao/quantization/weight_only.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,16 @@
     """
 
     def __init__(self, *args, **kwargs):
         w_int8 = kwargs.pop("w_int8")
         scales = kwargs.pop("scales")
         super().__init__(*args, **kwargs)
 
-        self.w_int8 = w_int8
-
-        self.scales = scales
+        self.register_buffer("w_int8", w_int8)
+        self.register_buffer("scales", scales)
 
     def forward(self, x, *args, **kwargs):
         """
         Performs the forward pass of the quantized linear layer which consists
         ofmixed dtype matmul using int8 symmetric per-channel weight quantization
 
         Args:
```

### Comparing `torchao-nightly-2024.4.4/torchao/sparsity/utils.py` & `torchao-nightly-2024.4.5/torchao/sparsity/utils.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao/sparsity/wanda.py` & `torchao-nightly-2024.4.5/torchao/sparsity/wanda.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.4/torchao_nightly.egg-info/PKG-INFO` & `torchao-nightly-2024.4.5/torchao_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.4.4
+Version: 2024.4.5
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
```

### Comparing `torchao-nightly-2024.4.4/torchao_nightly.egg-info/SOURCES.txt` & `torchao-nightly-2024.4.5/torchao_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

