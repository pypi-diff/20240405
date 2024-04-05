# Comparing `tmp/schedulefree-1.1.tar.gz` & `tmp/schedulefree-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedulefree-1.1.tar", last modified: Fri Apr  5 14:56:25 2024, max compression
+gzip compressed data, was "schedulefree-1.2.tar", last modified: Fri Apr  5 20:30:53 2024, max compression
```

## Comparing `schedulefree-1.1.tar` & `schedulefree-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:56:25.734014 schedulefree-1.1/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)    11356 2024-04-01 19:27:30.000000 schedulefree-1.1/LICENSE
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6626 2024-04-05 14:56:25.735133 schedulefree-1.1/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6170 2024-04-05 14:28:11.000000 schedulefree-1.1/README.md
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      303 2024-04-01 19:31:49.000000 schedulefree-1.1/pyproject.toml
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:56:25.713160 schedulefree-1.1/schedulefree/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      420 2024-04-05 14:54:15.000000 schedulefree-1.1/schedulefree/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5744 2024-04-04 15:51:08.000000 schedulefree-1.1/schedulefree/adamw_schedulefree.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5035 2024-04-04 15:52:02.000000 schedulefree-1.1/schedulefree/adamw_schedulefree_closure.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5325 2024-04-04 14:49:28.000000 schedulefree-1.1/schedulefree/sgd_schedulefree.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     4571 2024-04-04 15:54:19.000000 schedulefree-1.1/schedulefree/sgd_schedulefree_closure.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3617 2024-04-04 17:59:14.000000 schedulefree-1.1/schedulefree/test_schedulefree.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:56:25.729130 schedulefree-1.1/schedulefree.egg-info/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6626 2024-04-05 14:56:25.000000 schedulefree-1.1/schedulefree.egg-info/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      406 2024-04-05 14:56:25.000000 schedulefree-1.1/schedulefree.egg-info/SOURCES.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2024-04-05 14:56:25.000000 schedulefree-1.1/schedulefree.egg-info/dependency_links.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       13 2024-04-05 14:56:25.000000 schedulefree-1.1/schedulefree.egg-info/top_level.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       79 2024-04-05 14:56:25.738262 schedulefree-1.1/setup.cfg
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      889 2024-04-05 14:55:56.000000 schedulefree-1.1/setup.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 20:30:53.113978 schedulefree-1.2/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)    11356 2024-04-01 19:27:30.000000 schedulefree-1.2/LICENSE
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7043 2024-04-05 20:30:53.115059 schedulefree-1.2/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6587 2024-04-05 20:29:15.000000 schedulefree-1.2/README.md
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      303 2024-04-01 19:31:49.000000 schedulefree-1.2/pyproject.toml
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 20:30:53.095954 schedulefree-1.2/schedulefree/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      420 2024-04-05 14:54:15.000000 schedulefree-1.2/schedulefree/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5746 2024-04-05 20:30:05.000000 schedulefree-1.2/schedulefree/adamw_schedulefree.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5035 2024-04-04 15:52:02.000000 schedulefree-1.2/schedulefree/adamw_schedulefree_closure.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5329 2024-04-05 20:29:53.000000 schedulefree-1.2/schedulefree/sgd_schedulefree.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     4575 2024-04-05 20:29:48.000000 schedulefree-1.2/schedulefree/sgd_schedulefree_closure.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3617 2024-04-04 17:59:14.000000 schedulefree-1.2/schedulefree/test_schedulefree.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 20:30:53.110207 schedulefree-1.2/schedulefree.egg-info/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7043 2024-04-05 20:30:52.000000 schedulefree-1.2/schedulefree.egg-info/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      406 2024-04-05 20:30:53.000000 schedulefree-1.2/schedulefree.egg-info/SOURCES.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2024-04-05 20:30:52.000000 schedulefree-1.2/schedulefree.egg-info/dependency_links.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       13 2024-04-05 20:30:52.000000 schedulefree-1.2/schedulefree.egg-info/top_level.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       79 2024-04-05 20:30:53.118150 schedulefree-1.2/setup.cfg
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      889 2024-04-05 20:30:33.000000 schedulefree-1.2/setup.py
```

### Comparing `schedulefree-1.1/LICENSE` & `schedulefree-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schedulefree-1.1/PKG-INFO` & `schedulefree-1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schedulefree
-Version: 1.1
+Version: 1.2
 Summary: Schedule Free Learning in PyTorch
 Home-page: https://github.com/facebookresearch/schedule_free
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -15,47 +15,59 @@
 # Schedule-Free Learning - A New Way to Train
 Schedule-Free Optimizers in PyTorch.
 
 Authors: Aaron Defazio, Xingyu Yang, Konstantin Mishchenko, Ashok Cutkosky, Harsh Mehta, Ahmed Khaled
 
 **TLDR** Faster training without schedules - no need to specify the stopping time/steps in advance!
 
+``` pip install schedulefree ```
+
+Primary implementations are `SGDScheduleFree` and `AdamWScheduleFree`.
+
 ## Approach
 Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-free update is:
 
 $$
 \begin{align*}
 y_{t} & = (1-\beta)z_{t} + \beta x_{t},\\
 z_{t+1} & =z_{t}-\gamma\nabla f(y_{t}),\\
 x_{t+1} & =\left(1-\frac{1}{t}\right)x_{t}+\frac{1}{t}z_{t+1},
 \end{align*}
 $$
 
 Here $x$ is the sequence that evaluations of test/val loss should occur at, which differs from the primary iterates $z$ and the gradient evaluation locations $y$. The updates to $z$ correspond to the underlying optimizer, in this case a simple gradient step.
 
-As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requires as the base optimizer (parameter buffer + momentum).
+As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
 
 We provide both AdamW and SGD versions in this repo.
 
 ## How to Use
 Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`.
 
 If your code supports PyTorch Optimizer step closures, you can use the closure forms of the optimizers, which do not require the `.train()` and `.eval()` calls.
 
+### Examples
+Examples of using the `schedulefree` package can be found in the `examples` folder. These include:
+- [Image classification (MNIST) using Convnets](./examples/mnist/README.md)*
+- More examples to be added
+
+*Example is modified from [Pytorch Examples Repo](https://github.com/pytorch/examples).
+
+
 ## Caveats 
 - If your model uses BatchNorm, additional modifications are required for test/val evaluations to work correctly. Right before eval, something like the following:
   
  ```python
   model.train()
   optimizer.eval()
   for batch in itertools.islice(train_loader, 50):
     _ = self.model(batch)
   model.eval()
 ```
-This will replace the `training_mean`/`training_var` cache (which is updated in each forward pass when in model.train() mode) with values calculated at $x$ instead of $y$. Using PreciseBN will also avoid this isssue.
+This will replace the `training_mean`/`training_var` cache (which is updated in each forward pass when in model.train() mode) with values calculated at $x$ instead of $y$. Using PreciseBN will also avoid this issue.
 
 
  - Many code bases use additional features that may not be compatible without additonal changes. For instance, if the parameters are cached in fp16, the cached versions will need to be updated manually to ensure the correct $x$ sequence is used for evaluation, not the $y$ sequence. Some GradScalers do this.
  - Training is more sensitive to the choice of $\beta$ than you may expect from standard momentum. Our default of $0.9$ works on most problems but it may be necessary to increase the value to $0.95$ or $0.98$ particually for very long training runs.
  - There is no need to use a learning rate scheduler, however the code is compatible with one.
  - Using learning rate warmup is recommended. This is supported through the `warmup_steps` parameter.
  - This method does require tuning - it won't necessarily out-perform a schedule approach without also tuning regularization and learning rate parameters.
```

### Comparing `schedulefree-1.1/README.md` & `schedulefree-1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 # Schedule-Free Learning - A New Way to Train
 Schedule-Free Optimizers in PyTorch.
 
 Authors: Aaron Defazio, Xingyu Yang, Konstantin Mishchenko, Ashok Cutkosky, Harsh Mehta, Ahmed Khaled
 
 **TLDR** Faster training without schedules - no need to specify the stopping time/steps in advance!
 
+``` pip install schedulefree ```
+
+Primary implementations are `SGDScheduleFree` and `AdamWScheduleFree`.
+
 ## Approach
 Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-free update is:
 
 $$
 \begin{align*}
 y_{t} & = (1-\beta)z_{t} + \beta x_{t},\\
 z_{t+1} & =z_{t}-\gamma\nabla f(y_{t}),\\
 x_{t+1} & =\left(1-\frac{1}{t}\right)x_{t}+\frac{1}{t}z_{t+1},
 \end{align*}
 $$
 
 Here $x$ is the sequence that evaluations of test/val loss should occur at, which differs from the primary iterates $z$ and the gradient evaluation locations $y$. The updates to $z$ correspond to the underlying optimizer, in this case a simple gradient step.
 
-As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requires as the base optimizer (parameter buffer + momentum).
+As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
 
 We provide both AdamW and SGD versions in this repo.
 
 ## How to Use
 Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`.
 
 If your code supports PyTorch Optimizer step closures, you can use the closure forms of the optimizers, which do not require the `.train()` and `.eval()` calls.
 
+### Examples
+Examples of using the `schedulefree` package can be found in the `examples` folder. These include:
+- [Image classification (MNIST) using Convnets](./examples/mnist/README.md)*
+- More examples to be added
+
+*Example is modified from [Pytorch Examples Repo](https://github.com/pytorch/examples).
+
+
 ## Caveats 
 - If your model uses BatchNorm, additional modifications are required for test/val evaluations to work correctly. Right before eval, something like the following:
   
  ```python
   model.train()
   optimizer.eval()
   for batch in itertools.islice(train_loader, 50):
     _ = self.model(batch)
   model.eval()
 ```
-This will replace the `training_mean`/`training_var` cache (which is updated in each forward pass when in model.train() mode) with values calculated at $x$ instead of $y$. Using PreciseBN will also avoid this isssue.
+This will replace the `training_mean`/`training_var` cache (which is updated in each forward pass when in model.train() mode) with values calculated at $x$ instead of $y$. Using PreciseBN will also avoid this issue.
 
 
  - Many code bases use additional features that may not be compatible without additonal changes. For instance, if the parameters are cached in fp16, the cached versions will need to be updated manually to ensure the correct $x$ sequence is used for evaluation, not the $y$ sequence. Some GradScalers do this.
  - Training is more sensitive to the choice of $\beta$ than you may expect from standard momentum. Our default of $0.9$ works on most problems but it may be necessary to increase the value to $0.95$ or $0.98$ particually for very long training runs.
  - There is no need to use a learning rate scheduler, however the code is compatible with one.
  - Using learning rate warmup is recommended. This is supported through the `warmup_steps` parameter.
  - This method does require tuning - it won't necessarily out-perform a schedule approach without also tuning regularization and learning rate parameters.
```

### Comparing `schedulefree-1.1/schedulefree/adamw_schedulefree.py` & `schedulefree-1.2/schedulefree/adamw_schedulefree.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             with power r (default 0).
         weight_lr_power (float): During warmup, the weights in the average will
             be equal to lr raised to this power. Set to 0 for no weighting
             (default 2.0).
     """
     def __init__(self,
                  params, 
-                 lr=1e-3, 
+                 lr=0.0025, 
                  betas=(0.9, 0.999), 
                  eps=1e-8,
                  weight_decay=0,
                  warmup_steps=0,
                  r=0.0,
                  weight_lr_power=2.0,
                  ):
```

### Comparing `schedulefree-1.1/schedulefree/adamw_schedulefree_closure.py` & `schedulefree-1.2/schedulefree/adamw_schedulefree_closure.py`

 * *Files identical despite different names*

### Comparing `schedulefree-1.1/schedulefree/sgd_schedulefree.py` & `schedulefree-1.2/schedulefree/sgd_schedulefree.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             with power r (default 0).
         weight_lr_power (float): During warmup, the weights in the average will
             be equal to lr raised to this power. Set to 0 for no weighting
             (default 2.0).
     """
     def __init__(self,
                  params, 
-                 lr, 
+                 lr=1.0, 
                  momentum=0.9, 
                  weight_decay=0,
                  warmup_steps=0,
                  r=0.0,
                  weight_lr_power=2,
                  ):
         if lr < 0.0:
```

### Comparing `schedulefree-1.1/schedulefree/sgd_schedulefree_closure.py` & `schedulefree-1.2/schedulefree/sgd_schedulefree_closure.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             with power r (default 0).
         weight_lr_power (float): During warmup, the weights in the average will
             be equal to lr raised to this power. Set to 0 for no weighting
             (default 2.0).
     """
     def __init__(self, 
                  params, 
-                 lr, 
+                 lr=1.0, 
                  weight_decay=0,
                  momentum=0.9, 
                  warmup_steps=0,
                  r=0.0,
                  weight_lr_power=2.0,
                  ):
         if lr < 0.0:
```

### Comparing `schedulefree-1.1/schedulefree/test_schedulefree.py` & `schedulefree-1.2/schedulefree/test_schedulefree.py`

 * *Files identical despite different names*

### Comparing `schedulefree-1.1/schedulefree.egg-info/PKG-INFO` & `schedulefree-1.2/schedulefree.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schedulefree
-Version: 1.1
+Version: 1.2
 Summary: Schedule Free Learning in PyTorch
 Home-page: https://github.com/facebookresearch/schedule_free
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -15,47 +15,59 @@
 # Schedule-Free Learning - A New Way to Train
 Schedule-Free Optimizers in PyTorch.
 
 Authors: Aaron Defazio, Xingyu Yang, Konstantin Mishchenko, Ashok Cutkosky, Harsh Mehta, Ahmed Khaled
 
 **TLDR** Faster training without schedules - no need to specify the stopping time/steps in advance!
 
+``` pip install schedulefree ```
+
+Primary implementations are `SGDScheduleFree` and `AdamWScheduleFree`.
+
 ## Approach
 Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-free update is:
 
 $$
 \begin{align*}
 y_{t} & = (1-\beta)z_{t} + \beta x_{t},\\
 z_{t+1} & =z_{t}-\gamma\nabla f(y_{t}),\\
 x_{t+1} & =\left(1-\frac{1}{t}\right)x_{t}+\frac{1}{t}z_{t+1},
 \end{align*}
 $$
 
 Here $x$ is the sequence that evaluations of test/val loss should occur at, which differs from the primary iterates $z$ and the gradient evaluation locations $y$. The updates to $z$ correspond to the underlying optimizer, in this case a simple gradient step.
 
-As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requires as the base optimizer (parameter buffer + momentum).
+As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
 
 We provide both AdamW and SGD versions in this repo.
 
 ## How to Use
 Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`.
 
 If your code supports PyTorch Optimizer step closures, you can use the closure forms of the optimizers, which do not require the `.train()` and `.eval()` calls.
 
+### Examples
+Examples of using the `schedulefree` package can be found in the `examples` folder. These include:
+- [Image classification (MNIST) using Convnets](./examples/mnist/README.md)*
+- More examples to be added
+
+*Example is modified from [Pytorch Examples Repo](https://github.com/pytorch/examples).
+
+
 ## Caveats 
 - If your model uses BatchNorm, additional modifications are required for test/val evaluations to work correctly. Right before eval, something like the following:
   
  ```python
   model.train()
   optimizer.eval()
   for batch in itertools.islice(train_loader, 50):
     _ = self.model(batch)
   model.eval()
 ```
-This will replace the `training_mean`/`training_var` cache (which is updated in each forward pass when in model.train() mode) with values calculated at $x$ instead of $y$. Using PreciseBN will also avoid this isssue.
+This will replace the `training_mean`/`training_var` cache (which is updated in each forward pass when in model.train() mode) with values calculated at $x$ instead of $y$. Using PreciseBN will also avoid this issue.
 
 
  - Many code bases use additional features that may not be compatible without additonal changes. For instance, if the parameters are cached in fp16, the cached versions will need to be updated manually to ensure the correct $x$ sequence is used for evaluation, not the $y$ sequence. Some GradScalers do this.
  - Training is more sensitive to the choice of $\beta$ than you may expect from standard momentum. Our default of $0.9$ works on most problems but it may be necessary to increase the value to $0.95$ or $0.98$ particually for very long training runs.
  - There is no need to use a learning rate scheduler, however the code is compatible with one.
  - Using learning rate warmup is recommended. This is supported through the `warmup_steps` parameter.
  - This method does require tuning - it won't necessarily out-perform a schedule approach without also tuning regularization and learning rate parameters.
```

### Comparing `schedulefree-1.1/setup.py` & `schedulefree-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="schedulefree",
-    version="1.1",
+    version="1.2",
     author="Aaron Defazio",
     author_email="adefazio@meta.com",
     description="Schedule Free Learning in PyTorch",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/schedule_free",
     packages=setuptools.find_packages(),
```

