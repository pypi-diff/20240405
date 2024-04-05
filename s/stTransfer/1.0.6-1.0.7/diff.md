# Comparing `tmp/stTransfer-1.0.6.tar.gz` & `tmp/stTransfer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stTransfer-1.0.6.tar", last modified: Thu Feb 29 09:54:31 2024, max compression
+gzip compressed data, was "stTransfer-1.0.7.tar", last modified: Wed Apr  3 04:58:18 2024, max compression
```

## Comparing `stTransfer-1.0.6.tar` & `stTransfer-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-02-29 09:53:52.468556 stTransfer-1.0.6/
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1065 2024-02-28 07:25:00.000000 stTransfer-1.0.6/LICENSE
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     2321 2024-02-29 09:54:31.389678 stTransfer-1.0.6/PKG-INFO
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1813 2024-02-29 09:53:54.000000 stTransfer-1.0.6/README.md
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      160 2024-02-29 09:54:31.404859 stTransfer-1.0.6/setup.cfg
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1167 2024-02-29 08:43:00.000000 stTransfer-1.0.6/setup.py
-drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-02-29 09:53:52.384299 stTransfer-1.0.6/stTransfer/
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       80 2024-02-28 08:07:48.000000 stTransfer-1.0.6/stTransfer/__init__.py
-drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-02-29 09:53:52.452029 stTransfer-1.0.6/stTransfer/stTransfer/
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     6990 2024-02-29 09:22:50.000000 stTransfer-1.0.6/stTransfer/stTransfer/Transfer_entry.py
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      179 2024-02-23 04:34:51.000000 stTransfer-1.0.6/stTransfer/stTransfer/__init__.py
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)    10552 2024-02-29 09:12:43.000000 stTransfer-1.0.6/stTransfer/stTransfer/cell_type_ann_model.py
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1046 2024-02-23 03:03:45.000000 stTransfer-1.0.6/stTransfer/stTransfer/focal_loss.py
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     8348 2024-02-29 09:48:50.000000 stTransfer-1.0.6/stTransfer/stTransfer/scTrain_entry.py
-drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-02-29 09:53:52.419295 stTransfer-1.0.6/stTransfer.egg-info/
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     2321 2024-02-29 09:54:30.000000 stTransfer-1.0.6/stTransfer.egg-info/PKG-INFO
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      422 2024-02-29 09:54:30.000000 stTransfer-1.0.6/stTransfer.egg-info/SOURCES.txt
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)        1 2024-02-29 09:54:30.000000 stTransfer-1.0.6/stTransfer.egg-info/dependency_links.txt
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       15 2024-02-29 09:54:30.000000 stTransfer-1.0.6/stTransfer.egg-info/requires.txt
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       11 2024-02-29 09:54:30.000000 stTransfer-1.0.6/stTransfer.egg-info/top_level.txt
+drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-03 04:57:08.530777 stTransfer-1.0.7/
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1065 2024-02-28 07:25:00.000000 stTransfer-1.0.7/LICENSE
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     2291 2024-04-03 04:58:18.964668 stTransfer-1.0.7/PKG-INFO
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1813 2024-02-29 10:01:56.000000 stTransfer-1.0.7/README.md
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      160 2024-04-03 04:58:18.974107 stTransfer-1.0.7/setup.cfg
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1165 2024-03-12 02:55:46.000000 stTransfer-1.0.7/setup.py
+drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-03 04:57:08.449456 stTransfer-1.0.7/stTransfer/
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       80 2024-02-28 08:07:48.000000 stTransfer-1.0.7/stTransfer/__init__.py
+drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-03 04:57:08.519986 stTransfer-1.0.7/stTransfer/stTransfer/
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     7748 2024-03-14 05:57:47.000000 stTransfer-1.0.7/stTransfer/stTransfer/Transfer_entry.py
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      179 2024-02-23 04:34:51.000000 stTransfer-1.0.7/stTransfer/stTransfer/__init__.py
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     8994 2024-04-03 04:55:08.000000 stTransfer-1.0.7/stTransfer/stTransfer/cell_type_ann_model.py
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     8599 2024-03-28 06:20:45.000000 stTransfer-1.0.7/stTransfer/stTransfer/scTrain_entry.py
+drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-03 04:57:08.483876 stTransfer-1.0.7/stTransfer.egg-info/
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     2291 2024-04-03 04:58:18.000000 stTransfer-1.0.7/stTransfer.egg-info/PKG-INFO
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      353 2024-04-03 04:58:18.000000 stTransfer-1.0.7/stTransfer.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)        1 2024-04-03 04:58:18.000000 stTransfer-1.0.7/stTransfer.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       11 2024-04-03 04:58:18.000000 stTransfer-1.0.7/stTransfer.egg-info/top_level.txt
```

### Comparing `stTransfer-1.0.6/LICENSE` & `stTransfer-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stTransfer-1.0.6/PKG-INFO` & `stTransfer-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: stTransfer
-Version: 1.0.6
+Version: 1.0.7
 Summary: Transfer learning for spatial transcriptomics data and single-cell RNA-seq data.
 Home-page: https://github.com/zepoch/stTransfer.git
 Author: zhoutao
 Author-email: zhotoa@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp>=3.9.3
 
 # stTransfer
 
 [![python >= 3.8](https://img.shields.io/badge/python-3.8-brightgreen)](https://www.python.org/) 
 
 ### Installation      
 ```python
@@ -47,14 +46,14 @@
                                                  dnn_path = '/data/model/dnn.bgi', # dnn model path
                                                  gpu="0")
 
 st.distribution_fine_tune(st_adata_with_pslabel, 
                           pca_dim=0, 
                           k_graph=30, 
                           edge_weight=True, 
-                          epochs=200, 
+                          epochs=100, 
                           w_cls=50, 
                           w_dae=1., 
                           w_gae=1.,
                           gpu="0", 
                           save_path="/data/output") # output path
 ```
```

### Comparing `stTransfer-1.0.6/README.md` & `stTransfer-1.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,14 @@
                                                  dnn_path = '/data/model/dnn.bgi', # dnn model path
                                                  gpu="0")
 
 st.distribution_fine_tune(st_adata_with_pslabel, 
                           pca_dim=0, 
                           k_graph=30, 
                           edge_weight=True, 
-                          epochs=200, 
+                          epochs=100, 
                           w_cls=50, 
                           w_dae=1., 
                           w_gae=1.,
                           gpu="0", 
                           save_path="/data/output") # output path
 ```
```

### Comparing `stTransfer-1.0.6/setup.py` & `stTransfer-1.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Time    : 2024/2/28 16:09
 # @Author  : zhoutao
 # @File    : setup.py.py
 # @Software: VScode
-# @Email   : zhoutao3@genomics.cn
+# @Email   : zhotoa@foxmail.com
 
 import setuptools
 from wheel.bdist_wheel import bdist_wheel
 
-__version__ = "1.0.4"
+__version__ = "1.0.7"
 
 
 class BDistWheel(bdist_wheel):
     def get_tag(self):
         return (self.python_tag, "none", "any")
 
 
@@ -25,15 +25,15 @@
     long_description = fh.read()
 
 
 requirements = open("requirements.txt").readline()
 
 setuptools.setup(
     name = "stTransfer",
-    version = "1.0.6",
+    version = "1.0.7",
     description = "Transfer learning for spatial transcriptomics data and single-cell RNA-seq data.",
     author = "zhoutao",
     author_email = "zhotoa@foxmail.com",
     url = "https://github.com/zepoch/stTransfer.git",
     python_requires=">=3.8",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

### Comparing `stTransfer-1.0.6/stTransfer/stTransfer/Transfer_entry.py` & `stTransfer-1.0.7/stTransfer/stTransfer/Transfer_entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Time    : 25/2/24 21:54 PM
 # @Author  : zhoutao3
 # @File    : dnn_entry.py
 # @Email   : zhoutao3@genomics.cn
+'''
 import os.path as osp
 import pandas as pd
 import scanpy as sc # type: ignore
 import numpy as np
 import scipy.sparse as sp
 import random
 import torch
@@ -54,48 +55,60 @@
     # adata_X_sparse_backup = adata.X.copy()
     print('  After Preprocessing Data Info: %d cells × %d genes.' % (adata.shape[0], adata.shape[1]))
     if sp.issparse(adata.X):
         adata.X = adata.X.toarray() # type: ignore
     return adata
 
 
-def transfer_from_sc_data(adata, dnn_path, gpu="0"):
+def transfer_from_sc_data(adata, model_choice, model_path, gpu="0"):
     """
     :param adata:
     :param dnn_path: Pre-trained DNN model save path
     :param gpu: gpu number
     :return:
     """
     print("========> Transfering from sc-dataset...")
     if gpu is not None and torch.cuda.is_available():
         device = torch.device("cuda:{}".format(gpu))
     else:
         device = torch.device("cpu")
-
-    checkpoint = torch.load(dnn_path)
-    dnn_model = checkpoint["model"].to(device)
-    dnn_model.eval()
-
-    marker_genes = checkpoint["marker_genes"]
-    gene_indices = adata.var_names.get_indexer(marker_genes)
-    adata_X = np.pad(adata.X, ((0, 0), (0, 1)))[:, gene_indices].copy()
-    norm_factor = np.linalg.norm(adata_X, axis=1, keepdims=True)
-    norm_factor[norm_factor == 0] = 1
-    dnn_inputs = torch.Tensor(adata_X / norm_factor).split(checkpoint["batch_size"])
-    # Inference with DNN model.
-    dnn_predictions = []
-    with torch.no_grad():
-        for batch_idx, inputs in enumerate(dnn_inputs):
-            inputs = inputs.to(device)
-            outputs = dnn_model(inputs)
-            dnn_predictions.append(outputs.detach().cpu().numpy())
-    label_names = checkpoint['label_names']
-    adata.obsm['psuedo_label'] = np.concatenate(dnn_predictions)
-    adata.obs['psuedo_class'] = pd.Categorical([label_names[i] for i in adata.obsm['psuedo_label'].argmax(1)])
-    adata.uns['psuedo_classes'] = label_names
+    if model_choice == "dnn":
+        checkpoint = torch.load(model_path)
+        dnn_model = checkpoint["model"].to(device)
+        dnn_model.eval()
+
+        marker_genes = checkpoint["marker_genes"]
+        gene_indices = adata.var_names.get_indexer(marker_genes)
+        adata_X = np.pad(adata.X, ((0, 0), (0, 1)))[:, gene_indices].copy()
+        norm_factor = np.linalg.norm(adata_X, axis=1, keepdims=True)
+        norm_factor[norm_factor == 0] = 1
+        dnn_inputs = torch.Tensor(adata_X / norm_factor).split(checkpoint["batch_size"])
+        # Inference with DNN model.
+        dnn_predictions = []
+        with torch.no_grad():
+            for batch_idx, inputs in enumerate(dnn_inputs):
+                inputs = inputs.to(device)
+                outputs = dnn_model(inputs)
+                dnn_predictions.append(outputs.detach().cpu().numpy())
+        label_names = checkpoint['label_names']
+        adata.obsm['psuedo_label'] = np.concatenate(dnn_predictions)
+        adata.obs['psuedo_class'] = pd.Categorical([label_names[i] for i in adata.obsm['psuedo_label'].argmax(1)])
+        adata.uns['psuedo_classes'] = label_names
+        return adata
+    elif model_choice == "xgboost":
+        import pickle
+        with open(model_path, 'rb') as f:
+            model, dic, marker_genes = pickle.load(f)
+        gene_indices = adata.var_names.get_indexer(marker_genes)
+        adata_X = np.pad(adata.X, ((0, 0), (0, 1)))[:, gene_indices].copy()
+        xgboost_predictions = model.predict_proba(adata_X)
+        adata.obsm['psuedo_label'] = xgboost_predictions
+        adata.obs['psuedo_class'] = pd.Categorical([dic[i] for i in adata.obsm['psuedo_label'].argmax(1)])
+        adata.uns['psuedo_classes'] = dic
+        return adata
     return adata
 
 
 def distribution_fine_tune(adata, pca_dim=200, k_graph=30, edge_weight=True, epochs=200, w_cls=20, w_dae=1., w_gae=1.,
                            gpu="0", save_path="./output"):
     """
     :param adata:
@@ -153,20 +166,22 @@
     result = pd.DataFrame({'cell': adata.obs_names.tolist(), 'celltype_pred': celltype_pred})
     result.to_csv(osp.join(save_path, "model.csv"), index=False)
     adata.obs['celltype_pred'] = pd.Categorical(celltype_pred) # type: ignore
     # adata.X = adata_X_sparse_backup
 
     # --------------------------------------------------
     adata.obsm["X_pca"] = gene_mat.detach().cpu().numpy()
+    adata.uns = None
     adata.write(osp.join(save_path, "adata.h5ad"))
 
     # Save visualization.
     spot_size = 30
     psuedo_top100 = adata.obs['psuedo_class'].to_numpy()
     other_classes = list(pd.value_counts(adata.obs['psuedo_class'])[100:].index)
     psuedo_top100[adata.obs['psuedo_class'].isin(other_classes)] = 'Others'
     adata.obs['psuedo_top100'] = pd.Categorical(psuedo_top100)
     sc.pl.spatial(adata, img_key=None, color=['psuedo_top100'], spot_size=spot_size, show=False)
     plt.savefig(osp.join(save_path, "psuedo_top100.pdf"), bbox_inches='tight', dpi=150)
     sc.pl.spatial(adata, img_key=None, color=['celltype_pred'], spot_size=spot_size, show=False)
     plt.savefig(osp.join(save_path, "celltype_pred.pdf"), bbox_inches='tight', dpi=150)
-    print("Done!")
+    print("Done!")
+'''
```

### Comparing `stTransfer-1.0.6/stTransfer/stTransfer/cell_type_ann_model.py` & `stTransfer-1.0.7/stTransfer/stTransfer/cell_type_ann_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,126 +7,80 @@
 # @Email   : zhoutao3@genomics.cn
 
 import time
 import warnings
 import torch.nn.functional as F
 import torch
 import torch.nn as nn
-from torch_geometric.nn import GCNConv, VGAE, GATConv # type: ignore
+from torch_geometric.nn import GCNConv, VGAE, GATConv,GATv2Conv,GraphConv,GINConv, SAGEConv # type: ignore
 from torch_geometric.utils import remove_self_loops, add_self_loops, negative_sampling # type: ignore
-
+import xgboost as xgb # type: ignore
+from xgboost import XGBClassifier # type: ignore
 warnings.filterwarnings("ignore")
 
-class DNNModel(nn.Module):
-    def __init__(self, input_dim, hidden_dim, output_dim, drop_rate=0.5):
-        super(DNNModel, self).__init__()
-        self.net = nn.Sequential(
-            nn.Linear(input_dim, hidden_dim),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            nn.Linear(hidden_dim, int(hidden_dim / 2)),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            nn.Linear(int(hidden_dim / 2), int(hidden_dim / 4)),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            nn.Linear(int(hidden_dim / 4), output_dim),
-            nn.Dropout(p=drop_rate)
-        )
-    def forward(self, x):
-        return self.net(x)
-
-class SelfAttention(nn.Module):
-    def __init__(self, input_dim):
-        super(SelfAttention, self).__init__()
-        self.input_dim = input_dim
-        self.query = nn.Linear(input_dim, input_dim)
-        self.key = nn.Linear(input_dim, input_dim)
-        self.value = nn.Linear(input_dim, input_dim)
-    def forward(self, x):
-        q = self.query(x)
-        k = self.key(x)
-        v = self.value(x)
-        attention_weights = torch.softmax(q @ k.transpose(-2, -1) / (self.input_dim ** 0.5), dim=-1)
-        return attention_weights @ v
-
-class DNNModelWithAttention(nn.Module):
-    def __init__(self, input_dim, hidden_dim, output_dim, drop_rate=0.5):
-        super(DNNModelWithAttention, self).__init__()
-        self.net = nn.Sequential(
-            nn.Linear(input_dim, hidden_dim),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            SelfAttention(hidden_dim),
-            nn.Linear(hidden_dim, int(hidden_dim / 2)),
-            # SelfAttention(int(hidden_dim / 2)),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            nn.Linear(int(hidden_dim / 2), int(hidden_dim / 4)),
-            # SelfAttention(int(hidden_dim / 4)),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            nn.Linear(int(hidden_dim / 4), output_dim),
-            nn.Dropout(p=drop_rate)
-            
-        )
-    def forward(self, x):
-        return self.net(x)
-
-class MultiHeadAttention(nn.Module):
-    def __init__(self, input_dim, num_heads):
-        super(MultiHeadAttention, self).__init__()
-        self.num_heads = num_heads
-        self.input_dim = input_dim
-        self.attention = nn.MultiheadAttention(input_dim, num_heads)
-    def forward(self, x):
-        x = x.transpose(0, 1)  # MultiheadAttention需要(batch_size, seq_len, input_dim)的输入
-        attn_output, _ = self.attention(x, x, x)
-        return attn_output.transpose(0, 1)
-
-class DNNModelWithMultiHeadAttention(nn.Module):
-    def __init__(self, input_dim, hidden_dim, output_dim, num_heads, drop_rate=0.5):
-        super(DNNModelWithMultiHeadAttention, self).__init__()
-        self.net = nn.Sequential(
-            nn.Linear(input_dim, hidden_dim),
-            MultiHeadAttention(hidden_dim, num_heads),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            nn.Linear(hidden_dim, int(hidden_dim / 2)),
-            MultiHeadAttention(int(hidden_dim / 2), num_heads),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            nn.Linear(int(hidden_dim / 2), int(hidden_dim / 4)),
-            MultiHeadAttention(int(hidden_dim / 4), num_heads),
-            nn.GELU(),
-            nn.Dropout(p=drop_rate),
-            nn.Linear(int(hidden_dim / 4), output_dim),
-            nn.Dropout(p=drop_rate)
-        )
-    def forward(self, x):
-        return self.net(x)
+'''
+PyTorch Geometric (PyG) 提供了许多图神经网络层，其中一些可以直接替换 GCNConv 而不需要更改参数。以下是一些例子：
+
+ChebConv: ChebNet 卷积层，需要额外的参数 K，表示使用的切比雪夫多项式的阶数。
+
+SAGEConv: GraphSAGE 卷积层。
+
+GATConv: 图注意力网络 (GAT) 卷积层。发现很容易 聚合 临近节点的信息
+
+GINConv: 图同构网络 (GIN) 卷积层。无法正确调用
+
+GraphConv: 图卷积网络层，这是一个更一般的图卷积操作。发现 Psuedo-Acc 非常的低
+
+ARMAConv: 自回归移动平均 (ARMA) 卷积层。
 
+'''
 
 class GraphEncoder(nn.Module):
     def __init__(self, in_channels, hidden_channels, out_channels):
         super(GraphEncoder, self).__init__()
         # self.gc_feat = GCNConv(in_channels, hidden_channels)
         # self.gc_mean = GCNConv(hidden_channels, out_channels)
         # self.gc_logstd = GCNConv(hidden_channels, out_channels)
+        # self.gc_feat = GATConv(in_channels, hidden_channels)
+        # self.gc_mean = GATConv(hidden_channels, out_channels)
+        # self.gc_logstd = GATConv(hidden_channels, out_channels)
+        self.gc_feat = GCNConv(in_channels, hidden_channels,)
+        self.gc_mean = GATConv(hidden_channels, out_channels, heads=8, dropout=0.4)
+        self.gc_logstd = GCNConv(hidden_channels, out_channels)
         
-        self.gc_feat = GATConv(in_channels, hidden_channels)
-        self.gc_mean = GATConv(hidden_channels, out_channels)
-        self.gc_logstd = GATConv(hidden_channels, out_channels)
-
     def forward(self, x, edge_index, edge_weight):
         x = self.gc_feat(x, edge_index, edge_weight).relu()
         mean = self.gc_mean(x, edge_index, edge_weight)
         logstd = self.gc_logstd(x, edge_index, edge_weight)
         return mean, logstd
+'''
+from torch.nn import Sequential, Linear, ReLU
+
+class GraphEncoder(nn.Module):
+    def __init__(self, in_channels, hidden_channels, out_channels):
+        super(GraphEncoder, self).__init__()
 
+        nn1 = Sequential(Linear(in_channels, hidden_channels), ReLU(), Linear(hidden_channels, hidden_channels))
+        self.gc_feat = GINConv(nn1)
+        # x = self.gc_feat(x, edge_index)
+
+        nn2 = Sequential(Linear(hidden_channels, out_channels), ReLU(), Linear(out_channels, out_channels))
+        self.gc_mean = GINConv(nn2)
+        # mean = self.gc_mean(x, edge_index)
+
+        nn3 = Sequential(Linear(hidden_channels, out_channels), ReLU(), Linear(out_channels, out_channels))
+        self.gc_logstd = GINConv(nn3)
+        # logstd = self.gc_logstd(x, edge_index)
+
+    def forward(self, x, edge_index):
+        x = self.gc_feat(x, edge_index).relu()
+        mean = self.gc_mean(x, edge_index)
+        logstd = self.gc_logstd(x, edge_index)
+        return mean, logstd
+'''
 
 def full_block(in_features, out_features, drop_rate=0.2):
     return nn.Sequential(
         nn.Linear(in_features, out_features),
         nn.BatchNorm1d(out_features, momentum=0.01, eps=0.001),
         nn.ELU(),
         nn.Dropout(p=drop_rate)
```

### Comparing `stTransfer-1.0.6/stTransfer.egg-info/PKG-INFO` & `stTransfer-1.0.7/stTransfer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: stTransfer
-Version: 1.0.6
+Version: 1.0.7
 Summary: Transfer learning for spatial transcriptomics data and single-cell RNA-seq data.
 Home-page: https://github.com/zepoch/stTransfer.git
 Author: zhoutao
 Author-email: zhotoa@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp>=3.9.3
 
 # stTransfer
 
 [![python >= 3.8](https://img.shields.io/badge/python-3.8-brightgreen)](https://www.python.org/) 
 
 ### Installation      
 ```python
@@ -47,14 +46,14 @@
                                                  dnn_path = '/data/model/dnn.bgi', # dnn model path
                                                  gpu="0")
 
 st.distribution_fine_tune(st_adata_with_pslabel, 
                           pca_dim=0, 
                           k_graph=30, 
                           edge_weight=True, 
-                          epochs=200, 
+                          epochs=100, 
                           w_cls=50, 
                           w_dae=1., 
                           w_gae=1.,
                           gpu="0", 
                           save_path="/data/output") # output path
 ```
```

