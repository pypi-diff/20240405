# Comparing `tmp/torchseal-0.1.1.tar.gz` & `tmp/torchseal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchseal-0.1.1.tar", last modified: Fri Mar  8 04:08:08 2024, max compression
+gzip compressed data, was "torchseal-0.1.2.tar", last modified: Fri Apr  5 06:53:58 2024, max compression
```

## Comparing `torchseal-0.1.1.tar` & `torchseal-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,43 @@
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-03-08 04:08:08.838352 torchseal-0.1.1/
--rw-r--r--   0 rayhankinan   (501) staff       (20)     1112 2024-02-27 12:01:08.000000 torchseal-0.1.1/LICENSE
--rw-r--r--   0 rayhankinan   (501) staff       (20)      758 2024-03-08 04:08:08.838105 torchseal-0.1.1/PKG-INFO
--rw-r--r--   0 rayhankinan   (501) staff       (20)      100 2024-02-27 12:01:08.000000 torchseal-0.1.1/README.md
--rw-r--r--   0 rayhankinan   (501) staff       (20)      717 2024-03-08 04:07:25.000000 torchseal-0.1.1/pyproject.toml
--rw-r--r--   0 rayhankinan   (501) staff       (20)       38 2024-03-08 04:08:08.838399 torchseal-0.1.1/setup.cfg
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-03-08 04:08:08.833392 torchseal-0.1.1/src/
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-03-08 04:08:08.834554 torchseal-0.1.1/src/torchseal/
--rw-r--r--   0 rayhankinan   (501) staff       (20)       86 2024-03-04 07:35:25.000000 torchseal-0.1.1/src/torchseal/__init__.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-03-08 04:08:08.835988 torchseal-0.1.1/src/torchseal/function/
--rw-r--r--   0 rayhankinan   (501) staff       (20)      142 2024-03-03 10:51:25.000000 torchseal-0.1.1/src/torchseal/function/__init__.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     2870 2024-03-07 09:48:06.000000 torchseal-0.1.1/src/torchseal/function/conv2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     1797 2024-03-05 16:12:11.000000 torchseal-0.1.1/src/torchseal/function/linear.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      871 2024-03-05 06:24:44.000000 torchseal-0.1.1/src/torchseal/function/sigmoid.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      863 2024-03-05 06:24:44.000000 torchseal-0.1.1/src/torchseal/function/square.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-03-08 04:08:08.836508 torchseal-0.1.1/src/torchseal/nn/
--rw-r--r--   0 rayhankinan   (501) staff       (20)       54 2024-03-03 05:18:47.000000 torchseal-0.1.1/src/torchseal/nn/__init__.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     1431 2024-03-07 09:32:23.000000 torchseal-0.1.1/src/torchseal/nn/conv2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      822 2024-03-05 04:26:56.000000 torchseal-0.1.1/src/torchseal/nn/linear.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-03-08 04:08:08.837113 torchseal-0.1.1/src/torchseal/utils/
--rw-r--r--   0 rayhankinan   (501) staff       (20)      131 2024-03-07 07:32:49.000000 torchseal-0.1.1/src/torchseal/utils/__init__.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      310 2024-03-07 08:41:23.000000 torchseal-0.1.1/src/torchseal/utils/im2col_conv2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     1246 2024-03-08 03:56:54.000000 torchseal-0.1.1/src/torchseal/utils/im2col_decoding.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      734 2024-03-08 03:56:57.000000 torchseal-0.1.1/src/torchseal/utils/im2col_encoding.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-03-08 04:08:08.837666 torchseal-0.1.1/src/torchseal/wrapper/
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-04 07:34:56.000000 torchseal-0.1.1/src/torchseal/wrapper/__init__.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     5521 2024-03-07 08:36:33.000000 torchseal-0.1.1/src/torchseal/wrapper/ckks.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      402 2024-03-07 08:09:02.000000 torchseal-0.1.1/src/torchseal/wrapper/function.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-03-08 04:08:08.837877 torchseal-0.1.1/src/torchseal.egg-info/
--rw-r--r--   0 rayhankinan   (501) staff       (20)      758 2024-03-08 04:08:08.000000 torchseal-0.1.1/src/torchseal.egg-info/PKG-INFO
--rw-r--r--   0 rayhankinan   (501) staff       (20)      738 2024-03-08 04:08:08.000000 torchseal-0.1.1/src/torchseal.egg-info/SOURCES.txt
--rw-r--r--   0 rayhankinan   (501) staff       (20)        1 2024-03-08 04:08:08.000000 torchseal-0.1.1/src/torchseal.egg-info/dependency_links.txt
--rw-r--r--   0 rayhankinan   (501) staff       (20)       20 2024-03-08 04:08:08.000000 torchseal-0.1.1/src/torchseal.egg-info/requires.txt
--rw-r--r--   0 rayhankinan   (501) staff       (20)       10 2024-03-08 04:08:08.000000 torchseal-0.1.1/src/torchseal.egg-info/top_level.txt
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.362795 torchseal-0.1.2/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1112 2024-02-27 12:01:08.000000 torchseal-0.1.2/LICENSE
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      758 2024-04-05 06:53:58.362575 torchseal-0.1.2/PKG-INFO
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      100 2024-02-27 12:01:08.000000 torchseal-0.1.2/README.md
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      717 2024-04-05 06:53:54.000000 torchseal-0.1.2/pyproject.toml
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       38 2024-04-05 06:53:58.362845 torchseal-0.1.2/setup.cfg
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.356893 torchseal-0.1.2/src/
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.358044 torchseal-0.1.2/src/torchseal/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       86 2024-03-04 07:35:25.000000 torchseal-0.1.2/src/torchseal/__init__.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.360126 torchseal-0.1.2/src/torchseal/function/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      183 2024-04-04 20:12:15.000000 torchseal-0.1.2/src/torchseal/function/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     2579 2024-04-04 19:13:37.000000 torchseal-0.1.2/src/torchseal/function/average2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     3272 2024-04-04 19:13:40.000000 torchseal-0.1.2/src/torchseal/function/conv2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1767 2024-04-04 16:28:22.000000 torchseal-0.1.2/src/torchseal/function/linear.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-04-04 16:47:44.000000 torchseal-0.1.2/src/torchseal/function/max2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-25 17:29:39.000000 torchseal-0.1.2/src/torchseal/function/relu.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      851 2024-04-04 16:28:35.000000 torchseal-0.1.2/src/torchseal/function/sigmoid.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      843 2024-04-04 16:28:47.000000 torchseal-0.1.2/src/torchseal/function/square.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-25 18:45:58.000000 torchseal-0.1.2/src/torchseal/function/tanh.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.361499 torchseal-0.1.2/src/torchseal/nn/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      143 2024-04-04 16:52:01.000000 torchseal-0.1.2/src/torchseal/nn/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1293 2024-04-04 20:12:26.000000 torchseal-0.1.2/src/torchseal/nn/average2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1247 2024-04-04 20:12:29.000000 torchseal-0.1.2/src/torchseal/nn/conv2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      790 2024-04-04 20:12:33.000000 torchseal-0.1.2/src/torchseal/nn/linear.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-04-04 16:47:50.000000 torchseal-0.1.2/src/torchseal/nn/max2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-25 17:29:34.000000 torchseal-0.1.2/src/torchseal/nn/relu.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      391 2024-04-04 16:12:14.000000 torchseal-0.1.2/src/torchseal/nn/sigmoid.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-26 15:51:49.000000 torchseal-0.1.2/src/torchseal/nn/softmax.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      387 2024-04-04 16:12:37.000000 torchseal-0.1.2/src/torchseal/nn/square.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-25 18:46:04.000000 torchseal-0.1.2/src/torchseal/nn/tanh.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.361751 torchseal-0.1.2/src/torchseal/utils/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       49 2024-04-04 05:05:15.000000 torchseal-0.1.2/src/torchseal/utils/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     4028 2024-04-04 18:46:35.000000 torchseal-0.1.2/src/torchseal/utils/toeplitz.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.362155 torchseal-0.1.2/src/torchseal/wrapper/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-04 07:34:56.000000 torchseal-0.1.2/src/torchseal/wrapper/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     5015 2024-04-04 18:32:05.000000 torchseal-0.1.2/src/torchseal/wrapper/ckks.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      319 2024-04-04 12:28:23.000000 torchseal-0.1.2/src/torchseal/wrapper/function.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.362341 torchseal-0.1.2/src/torchseal.egg-info/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      758 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/PKG-INFO
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      974 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        1 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       20 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/requires.txt
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       10 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/top_level.txt
```

### Comparing `torchseal-0.1.1/LICENSE` & `torchseal-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchseal-0.1.1/PKG-INFO` & `torchseal-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchseal
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyTorch extension to enable training and testing using homomorphic encryption
 Author-email: Rayhan Kinan Muhannad <rayhankinan@gmail.com>
 Project-URL: Homepage, https://github.com/cnn-for-ckks/pytorch-for-tenseal
 Project-URL: Issues, https://github.com/cnn-for-ckks/pytorch-for-tenseal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `torchseal-0.1.1/pyproject.toml` & `torchseal-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torchseal"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Rayhan Kinan Muhannad", email="rayhankinan@gmail.com" },
 ]
 description = "PyTorch extension to enable training and testing using homomorphic encryption"
 readme = "README.md"
 requires-python = ">=3.6, <3.10"
 dependencies = [
```

### Comparing `torchseal-0.1.1/src/torchseal/function/conv2d.py` & `torchseal-0.1.2/src/torchseal/function/conv2d.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,86 @@
 from typing import Tuple, Optional
-from torch import Tensor
-from torch.autograd import Function
 from torch.nn.grad import conv2d_input, conv2d_weight
 from torchseal.wrapper.ckks import CKKSWrapper
 from torchseal.wrapper.function import CKKSConvFunctionWrapper
+from torchseal.utils import toeplitz_multiple_channels
 
+import torch
 
-class Conv2dFunction(Function):
+
+class Conv2dFunction(torch.autograd.Function):
     @staticmethod
-    def forward(ctx: CKKSConvFunctionWrapper, enc_x: CKKSWrapper, weight: Tensor, bias: Tensor, num_row: int, num_col: int, output_size: Tuple[int, int], kernel_size: Tuple[int, int], stride: int, padding: int) -> CKKSWrapper:
+    def forward(ctx: CKKSConvFunctionWrapper, enc_x: CKKSWrapper, weight: torch.Tensor, bias: torch.Tensor, output_size: torch.Size, stride: int, padding: int) -> CKKSWrapper:
         # Save the ctx for the backward method
         ctx.save_for_backward(weight)
         ctx.enc_x = enc_x.clone()
-        ctx.num_row = num_row
-        ctx.num_col = num_col
         ctx.output_size = output_size
-        ctx.kernel_size = kernel_size
         ctx.stride = stride
         ctx.padding = padding
 
+        # Get the toeplitz weight
+        toeplitz_weight = toeplitz_multiple_channels(
+            weight, output_size, stride=stride, padding=padding
+        )
+
+        # Get the bias
+        toeplitz_output_length, _ = toeplitz_weight.shape
+        bias_length, = bias.shape
+        toeplitz_bias = torch.cat(
+            [bias for _ in range(toeplitz_output_length // bias_length)]
+        )
+
         # Apply the convolution to the encrypted input
-        out_x = enc_x.do_conv2d(weight, bias, num_col)
+        out_x = enc_x.do_linear(toeplitz_weight, toeplitz_bias)
 
         return out_x
 
-    # NOTE: This method requires private key access
     @staticmethod
-    def backward(ctx: CKKSConvFunctionWrapper, grad_output: Tensor) -> Tuple[Optional[Tensor], Optional[Tensor], Optional[Tensor], Optional[Tensor], Optional[Tensor], Optional[Tensor], Optional[Tensor], Optional[Tensor], Optional[Tensor]]:
+    def backward(ctx: CKKSConvFunctionWrapper, grad_output: torch.Tensor) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]:
         # Get the saved tensors
-        saved_tensors: Tuple[Tensor] = ctx.saved_tensors  # type: ignore
+        saved_tensors: Tuple[torch.Tensor] = ctx.saved_tensors  # type: ignore
         enc_x = ctx.enc_x
-        num_row = ctx.num_row
-        num_col = ctx.num_col
         output_size = ctx.output_size
-        kernel_size = ctx.kernel_size
         stride = ctx.stride
         padding = ctx.padding
 
         # Unpack the saved tensors
         weight, = saved_tensors
 
-        # Get the needs_input_grad
-        result: Tuple[bool, bool, bool] = ctx.needs_input_grad  # type: ignore
+        # Unpack the tensor shapes
+        output_channel, output_height, output_width = output_size
+        kernel_out_channel, _, kernel_height, kernel_width = weight.shape
 
         # Calculate feature dimension
         feature_h = (
-            output_size[0] - kernel_size[0] + 2 * padding
+            output_height - kernel_height + 2 * padding
         ) // stride + 1
         feature_w = (
-            output_size[1] - kernel_size[1] + 2 * padding
+            output_width - kernel_width + 2 * padding
         ) // stride + 1
 
         # Decrypt the input
-        x = enc_x.do_image_decryption(
-            num_row, num_col, output_size, kernel_size, stride, padding
-        ).unsqueeze(0)
-        reshaped_grad_output = grad_output.reshape(
-            1, 1, feature_h, feature_w
+        reshaped_x = enc_x.do_decryption().view(
+            1, output_channel, output_height, output_width  # TODO: Handle larger batch sizes
+        )
+        reshaped_grad_output = grad_output.view(
+            1, kernel_out_channel, feature_h, feature_w  # TODO: Handle larger batch sizes
         )
 
+        # Get the needs_input_grad
+        result: Tuple[bool, bool, bool] = ctx.needs_input_grad  # type: ignore
+
         # Initialize the gradients
         grad_input = grad_weight = grad_bias = None
 
         if result[0]:
             grad_input = conv2d_input(
-                x.shape, weight, reshaped_grad_output, stride=stride
+                reshaped_x.shape, weight, reshaped_grad_output, stride=stride, padding=padding
             ).view(-1)
         if result[1]:
             grad_weight = conv2d_weight(
-                x, weight.shape, reshaped_grad_output, stride=stride
-            ).reshape(weight.shape)
+                reshaped_x, weight.shape, reshaped_grad_output, stride=stride, padding=padding
+            )
         if result[2]:
-            grad_bias = grad_output
+            grad_bias = reshaped_grad_output.sum(dim=(0, 2, 3))
 
-        return grad_input, grad_weight, grad_bias, None, None, None, None, None, None
+        return grad_input, grad_weight, grad_bias, None, None, None
```

### Comparing `torchseal-0.1.1/src/torchseal/function/linear.py` & `torchseal-0.1.2/src/torchseal/function/linear.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from typing import Optional, Tuple
-from torch import Tensor
-from torch.autograd import Function
 from torchseal.wrapper.ckks import CKKSWrapper
 from torchseal.wrapper.function import CKKSFunctionWrapper
 
+import torch
 
-class LinearFunction(Function):
+
+class LinearFunction(torch.autograd.Function):
     @staticmethod
-    def forward(ctx: CKKSFunctionWrapper, enc_x: CKKSWrapper, weight: Tensor, bias: Tensor) -> CKKSWrapper:
+    def forward(ctx: CKKSFunctionWrapper, enc_x: CKKSWrapper, weight: torch.Tensor, bias: torch.Tensor) -> CKKSWrapper:
         # Save the ctx for the backward method
         ctx.save_for_backward(weight)
         ctx.enc_x = enc_x.clone()
 
         # Apply the linear transformation to the encrypted input
         out_x = enc_x.do_linear(weight, bias)
 
         return out_x
 
-    # NOTE: This method requires private key access
     @staticmethod
-    def backward(ctx: CKKSFunctionWrapper, grad_output: Tensor) -> Tuple[Optional[Tensor], Optional[Tensor], Optional[Tensor]]:
+    def backward(ctx: CKKSFunctionWrapper, grad_output: torch.Tensor) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]:
         # Get the saved tensors
-        saved_tensors: Tuple[Tensor] = ctx.saved_tensors  # type: ignore
+        saved_tensors: Tuple[torch.Tensor] = ctx.saved_tensors  # type: ignore
         x = ctx.enc_x.do_decryption()
 
         # Unpack the saved tensors
         weight, = saved_tensors
 
         # Get the needs_input_grad
         result: Tuple[bool, bool, bool] = ctx.needs_input_grad  # type: ignore
@@ -40,13 +39,13 @@
             grad_weight = grad_output.unsqueeze(0).t().matmul(x.unsqueeze(0))
         if result[2]:
             grad_bias = grad_output
 
         return grad_input, grad_weight, grad_bias
 
     @staticmethod
-    def apply(enc_x: CKKSWrapper, weight: Tensor, bias: Tensor) -> CKKSWrapper:
+    def apply(enc_x: CKKSWrapper, weight: torch.Tensor, bias: torch.Tensor) -> CKKSWrapper:
         out_x: CKKSWrapper = super(LinearFunction, LinearFunction).apply(
             enc_x, weight, bias
         )  # type: ignore
 
         return out_x
```

### Comparing `torchseal-0.1.1/src/torchseal/function/sigmoid.py` & `torchseal-0.1.2/src/torchseal/function/sigmoid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Tuple
-from torch import Tensor
-from torch.autograd import Function
 from torchseal.wrapper.ckks import CKKSWrapper
 from torchseal.wrapper.function import CKKSFunctionWrapper
 
+import torch
 
-class SigmoidFunction(Function):
+
+class SigmoidFunction(torch.autograd.Function):
     @staticmethod
     def forward(ctx: CKKSFunctionWrapper, enc_x: CKKSWrapper) -> CKKSWrapper:
         # Save the ctx for the backward method
         ctx.enc_x = enc_x.clone()
 
         # Apply the sigmoid function to the encrypted input
         out_x = enc_x.do_sigmoid()
 
         return out_x
 
     @staticmethod
-    def backward(ctx: CKKSFunctionWrapper, grad_output: Tensor) -> Tuple[Tensor]:
+    def backward(ctx: CKKSFunctionWrapper, grad_output: torch.Tensor) -> Tuple[torch.Tensor]:
         # Get the saved tensors
         x = ctx.enc_x.do_decryption()
 
         # Do the backward operation
         out = x.do_sigmoid_backward()
 
         # Compute the gradients
```

### Comparing `torchseal-0.1.1/src/torchseal/nn/conv2d.py` & `torchseal-0.1.2/src/torchseal/nn/conv2d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from typing import Tuple, Optional
-from torch import Tensor
-from torch.nn import Module, Parameter
 from torchseal.wrapper.ckks import CKKSWrapper
-from torchseal.function.conv2d import Conv2dFunction
+from torchseal.function import Conv2dFunction
 
 import torch
 
 
-class Conv2d(Module):  # TODO: Add support for in_channels and out_channels (this enables the use of multiple convolutions in a row)
-    def __init__(self, output_size: Tuple[int, int], kernel_size: Tuple[int, int], stride: int, padding: int, weight: Optional[Tensor] = None, bias: Optional[Tensor] = None) -> None:
+class Conv2d(torch.nn.Module):
+    def __init__(self, in_channel: int, out_channel: int, kernel_size: Tuple[int, int], output_size: torch.Size, stride: int = 1, padding: int = 0, weight: Optional[torch.Tensor] = None, bias: Optional[torch.Tensor] = None) -> None:
         super(Conv2d, self).__init__()
 
         # Save the parameters
         self.output_size = output_size
-        self.kernel_size = kernel_size
         self.stride = stride
         self.padding = padding
 
         # Unpack the kernel size
-        kernel_n_rows, kernel_n_cols = self.kernel_size
+        kernel_n_rows, kernel_n_cols = kernel_size
 
         # Create the weight and bias
-        self.weight = Parameter(
+        self.weight = torch.nn.Parameter(
             torch.rand(
-                1, 1, kernel_n_rows, kernel_n_cols
+                out_channel, in_channel, kernel_n_rows, kernel_n_cols
             ) if weight is None else weight
         )
-        self.bias = Parameter(
-            torch.rand(1) if bias is None else bias
+        self.bias = torch.nn.Parameter(
+            torch.rand(out_channel) if bias is None else bias
         )
 
-    def forward(self, enc_x: CKKSWrapper, num_row: int, num_col: int) -> CKKSWrapper:
+    def forward(self, enc_x: CKKSWrapper) -> CKKSWrapper:
         out_x: CKKSWrapper = Conv2dFunction.apply(
-            enc_x, self.weight, self.bias, num_row, num_col, self.output_size, self.kernel_size, self.stride, self.padding
+            enc_x, self.weight, self.bias, self.output_size, self.stride, self.padding
         )  # type: ignore
 
         return out_x
```

### Comparing `torchseal-0.1.1/src/torchseal/nn/linear.py` & `torchseal-0.1.2/src/torchseal/nn/linear.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from typing import Optional
-from torch import Tensor
-from torch.nn import Module, Parameter
 from torchseal.wrapper.ckks import CKKSWrapper
-from torchseal.function.linear import LinearFunction
+from torchseal.function import LinearFunction
 
 import torch
 
 
-class Linear(Module):
-    def __init__(self, in_features: int, out_features: int, weight: Optional[Tensor] = None, bias: Optional[Tensor] = None):
+class Linear(torch.nn.Module):
+    def __init__(self, in_features: int, out_features: int, weight: Optional[torch.Tensor] = None, bias: Optional[torch.Tensor] = None):
         super(Linear, self).__init__()
 
-        self.weight = Parameter(
+        self.weight = torch.nn.Parameter(
             torch.rand(in_features, out_features) if weight is None else weight
         )
-        self.bias = Parameter(
+        self.bias = torch.nn.Parameter(
             torch.rand(out_features) if bias is None else bias
         )
 
     def forward(self, enc_x: CKKSWrapper) -> CKKSWrapper:
         out_x: CKKSWrapper = LinearFunction.apply(
             enc_x, self.weight, self.bias
         )  # type: ignore
```

### Comparing `torchseal-0.1.1/src/torchseal/wrapper/ckks.py` & `torchseal-0.1.2/src/torchseal/wrapper/ckks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from typing import Tuple
-from torch import Tensor
 from tenseal import CKKSVector
-from torchseal.utils import im2col_conv2d, im2col_decoding
 
 import torch
 import tenseal as ts
 
 
-class CKKSWrapper(Tensor):
+class CKKSWrapper(torch.Tensor):
     __ckks_data: CKKSVector
 
     @property
     def ckks_data(self) -> CKKSVector:
         return self.__ckks_data
 
     @ckks_data.setter
@@ -23,74 +20,69 @@
     # def __torch_function__(cls, func, types, *args, **kwargs):
     #     # Print the function and the types
     #     print(f"Function: {func}")
 
     #     return super(CKKSWrapper, cls).__torch_function__(func, types, *args, **kwargs)
 
     # Overridden methods
-    def __new__(cls, _data: Tensor, _ckks_data: CKKSVector, *args, **kwargs) -> "CKKSWrapper":
+    def __new__(cls, _data: torch.Tensor, _ckks_data: CKKSVector, *args, **kwargs) -> "CKKSWrapper":
         # Create the tensor
         data = super(CKKSWrapper, cls).__new__(cls, *args, **kwargs)
 
         # Create the instance
         instance = torch.Tensor._make_subclass(cls, data)
 
         return instance
 
     # Overridden methods
-    def __init__(self, data: Tensor, ckks_data: CKKSVector, *args, **kwargs) -> None:
+    def __init__(self, data: torch.Tensor, ckks_data: CKKSVector, *args, **kwargs) -> None:
         # Call the super constructor
-        super(Tensor, self).__init__(*args, **kwargs)
+        super(torch.Tensor, self).__init__(*args, **kwargs)
 
         # Set the data
         self.data = data
         self.ckks_data = ckks_data
 
     # Overridden methods
     def clone(self, *args, **kwargs) -> "CKKSWrapper":
         # Clone the data
-        data = super(Tensor, self).clone(*args, **kwargs)
+        data = super(torch.Tensor, self).clone(*args, **kwargs)
         ckks_data: CKKSVector = self.ckks_data.copy()  # type: ignore
 
         # Create the new instance
         instance = CKKSWrapper(data, ckks_data)
 
         return instance
 
     # Overridden methods
 
     def view_as(self, other: "CKKSWrapper") -> "CKKSWrapper":
-        self.data = super(Tensor, self).view_as(other)
+        self.data = super(torch.Tensor, self).view_as(other)
 
         return self
 
-    # CKKS Operation
-    def do_conv2d(self, weight: Tensor, bias: Tensor, num_col: int) -> "CKKSWrapper":
-        # TODO: Add support for multiple input and output channels
-        out_weight = weight.view(-1)
-        out_bias = bias.item()
-
-        # Apply the convolution to the encrypted input
-        new_ckks_vector = im2col_conv2d(
-            self.ckks_data, out_weight, num_col
-        ).add(out_bias)
+    def do_multiplication(self, matrix: torch.Tensor) -> "CKKSWrapper":
+        # Apply the multiplication to the encrypted input
+        new_ckks_vector: CKKSVector = self.ckks_data.matmul(
+            matrix.t().tolist()
+        )
 
         # Change the shape of the data
         tensor = torch.rand(new_ckks_vector.size())
 
-        # Update the CKKS data
+        # Update the data
         self.ckks_data = new_ckks_vector
 
         # Update the data
         self.data = tensor.data
 
         return self
 
     # CKKS Operation
-    def do_linear(self, weight: Tensor, bias: Tensor) -> "CKKSWrapper":
+    def do_linear(self, weight: torch.Tensor, bias: torch.Tensor) -> "CKKSWrapper":
         # Apply the linear transformation to the encrypted input
         new_ckks_vector = self.ckks_data.matmul(
             weight.t().tolist()
         ).add(
             bias.tolist()
         )
 
@@ -103,14 +95,15 @@
         # Update the data
         self.data = tensor.data
 
         return self
 
     # CKKS Operation
     def do_sigmoid(self) -> "CKKSWrapper":
+        # TODO: Create an adjustable approximation to calculate the sigmoid function
         new_ckks_vector: CKKSVector = self.ckks_data.polyval(
             [0.5, 0.197, 0, -0.004]
         )  # type: ignore
 
         # Update the data
         self.ckks_data = new_ckks_vector
 
@@ -135,14 +128,15 @@
         self.ckks_data = new_ckks_vector
 
         return self
 
     # Data Operation
     def do_sigmoid_backward(self) -> "CKKSWrapper":
         # Apply the sigmoid backward function to the data
+        # TODO: Create an adjustable approximation to calculate the sigmoid backward function
         new_tensor = torch.tensor(
             list(map(lambda x: 0.197 - 0.008 * x, self.data))
         )
 
         # Update the data
         self.data = new_tensor.data
 
@@ -167,26 +161,14 @@
 
         # Update the data
         self.data = new_tensor.data
 
         return self
 
     # Data Operation
-    def do_image_decryption(self, num_row: int, num_col: int, output_size: Tuple[int, int], kernel_size: Tuple[int, int], stride: int, padding: int) -> "CKKSWrapper":
-        # Define the new tensor
-        new_tensor = im2col_decoding(
-            self.ckks_data, num_row, num_col, output_size, kernel_size, stride, padding
-        )
-
-        # Update the data
-        self.data = new_tensor.data
-
-        return self
-
-    # Data Operation
     def do_decryption(self) -> "CKKSWrapper":
         # Define the new tensor
         new_tensor = torch.tensor(
             self.ckks_data.decrypt(), requires_grad=True
         )
 
         # Update the data
```

### Comparing `torchseal-0.1.1/src/torchseal.egg-info/PKG-INFO` & `torchseal-0.1.2/src/torchseal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchseal
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyTorch extension to enable training and testing using homomorphic encryption
 Author-email: Rayhan Kinan Muhannad <rayhankinan@gmail.com>
 Project-URL: Homepage, https://github.com/cnn-for-ckks/pytorch-for-tenseal
 Project-URL: Issues, https://github.com/cnn-for-ckks/pytorch-for-tenseal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

