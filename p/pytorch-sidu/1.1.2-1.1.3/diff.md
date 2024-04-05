# Comparing `tmp/pytorch-sidu-1.1.2.tar.gz` & `tmp/pytorch-sidu-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-sidu-1.1.2.tar", last modified: Wed Apr  3 11:07:39 2024, max compression
+gzip compressed data, was "pytorch-sidu-1.1.3.tar", last modified: Fri Apr  5 15:50:42 2024, max compression
```

## Comparing `pytorch-sidu-1.1.2.tar` & `pytorch-sidu-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:39.819689 pytorch-sidu-1.1.2/pytorch_sidu/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/pytorch_sidu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/pytorch_sidu/sidu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/pytorch_sidu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/pytorch_sidu/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:50:42.450675 pytorch-sidu-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-05 15:49:14.000000 pytorch-sidu-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 15:49:14.000000 pytorch-sidu-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-05 15:50:42.450675 pytorch-sidu-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-05 15:49:14.000000 pytorch-sidu-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:50:42.450675 pytorch-sidu-1.1.3/pytorch_sidu/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 15:49:14.000000 pytorch-sidu-1.1.3/pytorch_sidu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-05 15:49:14.000000 pytorch-sidu-1.1.3/pytorch_sidu/sidu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:50:42.450675 pytorch-sidu-1.1.3/pytorch_sidu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-05 15:49:14.000000 pytorch-sidu-1.1.3/pytorch_sidu/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:50:42.450675 pytorch-sidu-1.1.3/pytorch_sidu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-05 15:50:42.000000 pytorch-sidu-1.1.3/pytorch_sidu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-05 15:50:42.000000 pytorch-sidu-1.1.3/pytorch_sidu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:50:42.000000 pytorch-sidu-1.1.3/pytorch_sidu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 15:50:42.000000 pytorch-sidu-1.1.3/pytorch_sidu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 15:50:42.000000 pytorch-sidu-1.1.3/pytorch_sidu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 15:49:14.000000 pytorch-sidu-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 15:50:42.454675 pytorch-sidu-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-05 15:49:14.000000 pytorch-sidu-1.1.3/setup.py
```

### Comparing `pytorch-sidu-1.1.2/LICENSE` & `pytorch-sidu-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.1.2/PKG-INFO` & `pytorch-sidu-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-sidu
-Version: 1.1.2
+Version: 1.1.3
 Summary: SIDU: SImilarity Difference and Uniqueness method for explainable AI
 Home-page: https://github.com/MarcoParola/pytorch-sidu
 Author: Marco Parola
 Author-email: marcoparola96@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,14 @@
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: numpy
 
 # **pytorch-sidu**
 
-![example workflow](https://github.com/MarcoParola/pytorch-sidu/actions/workflows/python-publish.yml/badge.svg)
 [![size](https://img.shields.io/github/languages/code-size/MarcoParola/pytorch-sidu)]()
 
 SIDU: SImilarity Difference and Uniqueness method for explainable AI from the [original paper](https://arxiv.org/pdf/2006.03122.pdf)
 
 - Pytorch implementation of the SIDU method. 
 - Simple interface for loading pretrained models by specifying one of the following [string name](https://pytorch.org/vision/stable/models.html#table-of-all-available-classification-weights)
 - Clear interface for generating saliency maps
@@ -71,15 +70,15 @@
 
 transform = torchvision.transforms.Compose([torchvision.transforms.Resize((224, 224)), torchvision.transforms.ToTensor()])
 data_loader = torch.utils.data.DataLoader(
     torchvision.datasets.CIFAR10(root='./data', download=True, transform=transform), batch_size=2)
 
 target_layer = 'layer4.2.conv2'
 model_name = 'ResNet34_Weights.IMAGENET1K_V1'
-model = load_torch_model_by_string(model_name)
+model = sidu.load_torch_model_by_string(model_name)
 
 for image, _ in data_loader:
     saliency_maps = sidu.sidu(model, target_layer, image)
     image, saliency_maps = image.cpu(), saliency_maps.cpu()
 
     for j in range(len(image)):
         plt.figure(figsize=(5, 2.5))
```

### Comparing `pytorch-sidu-1.1.2/README.md` & `pytorch-sidu-1.1.3/pytorch_sidu.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,27 @@
+Metadata-Version: 2.1
+Name: pytorch-sidu
+Version: 1.1.3
+Summary: SIDU: SImilarity Difference and Uniqueness method for explainable AI
+Home-page: https://github.com/MarcoParola/pytorch-sidu
+Author: Marco Parola
+Author-email: marcoparola96@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: numpy
+
 # **pytorch-sidu**
 
-![example workflow](https://github.com/MarcoParola/pytorch-sidu/actions/workflows/python-publish.yml/badge.svg)
 [![size](https://img.shields.io/github/languages/code-size/MarcoParola/pytorch-sidu)]()
 
 SIDU: SImilarity Difference and Uniqueness method for explainable AI from the [original paper](https://arxiv.org/pdf/2006.03122.pdf)
 
 - Pytorch implementation of the SIDU method. 
 - Simple interface for loading pretrained models by specifying one of the following [string name](https://pytorch.org/vision/stable/models.html#table-of-all-available-classification-weights)
 - Clear interface for generating saliency maps
@@ -53,15 +70,15 @@
 
 transform = torchvision.transforms.Compose([torchvision.transforms.Resize((224, 224)), torchvision.transforms.ToTensor()])
 data_loader = torch.utils.data.DataLoader(
     torchvision.datasets.CIFAR10(root='./data', download=True, transform=transform), batch_size=2)
 
 target_layer = 'layer4.2.conv2'
 model_name = 'ResNet34_Weights.IMAGENET1K_V1'
-model = load_torch_model_by_string(model_name)
+model = sidu.load_torch_model_by_string(model_name)
 
 for image, _ in data_loader:
     saliency_maps = sidu.sidu(model, target_layer, image)
     image, saliency_maps = image.cpu(), saliency_maps.cpu()
 
     for j in range(len(image)):
         plt.figure(figsize=(5, 2.5))
```

### Comparing `pytorch-sidu-1.1.2/pytorch_sidu/sidu.py` & `pytorch-sidu-1.1.3/pytorch_sidu/sidu.py`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.1.2/pytorch_sidu/utils/utils.py` & `pytorch-sidu-1.1.3/pytorch_sidu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.1.2/setup.cfg` & `pytorch-sidu-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.1.2/setup.py` & `pytorch-sidu-1.1.3/setup.py`

 * *Files identical despite different names*

