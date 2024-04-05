# Comparing `tmp/mamba_former-0.0.2.tar.gz` & `tmp/mamba_former-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamba_former-0.0.2.tar", max compression
+gzip compressed data, was "mamba_former-0.0.3.tar", max compression
```

## Comparing `mamba_former-0.0.2.tar` & `mamba_former-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-04-04 00:00:17.570890 mamba_former-0.0.2/LICENSE
--rw-r--r--   0        0        0      692 2024-04-04 00:27:33.859935 mamba_former-0.0.2/README.md
--rw-r--r--   0        0        0       74 2024-04-04 00:27:44.557905 mamba_former-0.0.2/mamba_former/__init__.py
--rw-r--r--   0        0        0     3067 2024-04-04 00:26:46.917210 mamba_former-0.0.2/mamba_former/main.py
--rw-r--r--   0        0        0     1356 2024-04-04 00:40:29.629889 mamba_former-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 mamba_former-0.0.2/setup.py
--rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 mamba_former-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-04 00:00:17.570890 mamba_former-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1228 2024-04-05 00:54:10.855766 mamba_former-0.0.3/README.md
+-rw-r--r--   0        0        0       69 2024-04-05 00:53:20.155753 mamba_former-0.0.3/mamba_former/__init__.py
+-rw-r--r--   0        0        0     3388 2024-04-05 00:53:20.754723 mamba_former-0.0.3/mamba_former/main.py
+-rw-r--r--   0        0        0     1356 2024-04-05 00:54:34.000883 mamba_former-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 mamba_former-0.0.3/setup.py
+-rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 mamba_former-0.0.3/PKG-INFO
```

### Comparing `mamba_former-0.0.2/LICENSE` & `mamba_former-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mamba_former-0.0.2/mamba_former/main.py` & `mamba_former-0.0.3/mamba_former/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,137 +1,143 @@
-import torch
 from torch import nn, Tensor
 from zeta.nn import MambaBlock, OutputHead
 from zeta.nn.attention.multiquery_attention import MultiQueryAttention
+import torch.nn.functional as F
+
 
 class MambaFormerBlock(nn.Module):
     def __init__(
         self,
         dim: int,
         d_state: int,
         d_conv: int,
         heads: int,
         dim_head: int,
         *args,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.dim = dim
         self.d_state = d_state
         self.d_conv = d_conv
         self.heads = heads
         self.dim_head = dim_head
-        
+
         # MambaBlock
         self.input_mamba = MambaBlock(
-            dim,
-            1,
-            d_state,
-            d_conv,
-            *args,
-            **kwargs
+            dim, 1, d_state, d_conv, *args, **kwargs
         )
-        
+
         # MultiQueryAttention
-        self.attn = MultiQueryAttention(
-            dim,
-            heads,
-            *args,
-            **kwargs   
-        )
-    
+        self.attn = MultiQueryAttention(dim, heads, *args, **kwargs)
+
     def forward(self, x: Tensor):
         # First step is Attention
         skip = x
-        
+
         # Attention
         attended, _, _ = self.attn(x)
-        
+
         # Add residual
         x = attended + skip
-        
+
         # Second step is MambaBlock
         skip_two = x
-        
+
         # Mamba
         x = self.input_mamba(x)
-        
+
         # Add residual and return
         return x + skip_two
-    
+
 
 class MambaFormer(nn.Module):
     def __init__(
         self,
         dim: int,
         num_tokens: int,
         depth: int,
         d_state: int,
         d_conv: int,
         heads: int,
         dim_head: int,
         return_tokens: bool = True,
+        cross_entropy_ignore_index=0,
         *args,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.dim = dim
         self.num_tokens = num_tokens
         self.depth = depth
         self.d_state = d_state
         self.d_conv = d_conv
         self.heads = heads
         self.dim_head = dim_head
         self.return_tokens = return_tokens
-        
+        self.cross_entropy_ignore_index = cross_entropy_ignore_index
+
         # Embedding
         self.embed = nn.Embedding(num_tokens, dim)
-        
+
         # Mamba as input
         self.input_mamba = MambaBlock(
-            dim,
-            1,
-            d_state,
-            d_conv,
-            *args,
-            **kwargs
+            dim, 1, d_state, d_conv, *args, **kwargs
         )
-        
+
         # Layers of Mamba Former Block
-        self.layers = nn.ModuleList([
-            MambaFormerBlock(
-                dim,
-                d_state,
-                d_conv,
-                heads,
-                dim_head,
-            )
-            for _ in range(depth)
-        ])
-        
-        
+        self.layers = nn.ModuleList(
+            [
+                MambaFormerBlock(
+                    dim,
+                    d_state,
+                    d_conv,
+                    heads,
+                    dim_head,
+                )
+                for _ in range(depth)
+            ]
+        )
+
         # Norm
         self.norm = nn.LayerNorm(dim)
-        
-    def forward(self, x):
+
+    def forward(
+        self,
+        x,
+        return_loss: bool = False,
+        return_embeddings: bool = False,
+    ):
+        if return_loss:
+            x, labels = x[:, -1], x[:, 1:]
+
+        mask = x >= 0
+        x = x.masked_fill(~mask, 0)
+
         # Embed tokens to get tensors
         x = self.embed(x)
-        
+
         # Normalize
         x = self.norm(x)
-        
+
         # Then skip
         skip = x
-        
+
         # Mamba
         x = self.input_mamba(x) + skip
-        
+
         # MambaFormer Blocks
         for layer in self.layers:
             x = layer(x) + x
-        
+
         if self.return_tokens:
             out = OutputHead(self.dim, -1)(x)
             return out
-        else: 
+        elif return_loss:
+            logits = OutputHead(self.dim, -1)(x)
+            out = F.cross_entropy(
+                logits,
+                labels,
+                ignore_index=self.cross_entropy_ignore_index,
+            )
+        elif return_embeddings:
             return x
-
```

### Comparing `mamba_former-0.0.2/pyproject.toml` & `mamba_former-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mamba-former"
-version = "0.0.2"
+version = "0.0.3"
 description = "Paper - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/MambaFormer"
 documentation = "https://github.com/kyegomez/MambaFormer"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/MambaFormer"
```

