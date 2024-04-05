# Comparing `tmp/loss-balancer-tf-0.0.2.tar.gz` & `tmp/loss-balancer-tf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loss-balancer-tf-0.0.2.tar", last modified: Fri Mar 29 09:05:35 2024, max compression
+gzip compressed data, was "loss-balancer-tf-0.0.3.tar", last modified: Fri Apr  5 09:30:26 2024, max compression
```

## Comparing `loss-balancer-tf-0.0.2.tar` & `loss-balancer-tf-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 09:05:35.428232 loss-balancer-tf-0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-03-02 07:42:11.000000 loss-balancer-tf-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      192 2024-03-29 09:05:35.427730 loss-balancer-tf-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1992 2024-03-29 08:28:46.000000 loss-balancer-tf-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 09:05:35.404730 loss-balancer-tf-0.0.2/loss_balancer_tf/
--rw-rw-rw-   0        0        0       58 2024-03-02 07:44:33.000000 loss-balancer-tf-0.0.2/loss_balancer_tf/__init__.py
--rw-rw-rw-   0        0        0     4061 2024-03-29 08:01:08.000000 loss-balancer-tf-0.0.2/loss_balancer_tf/loss_balancer_tf.py
-drwxrwxrwx   0        0        0        0 2024-03-29 09:05:35.426233 loss-balancer-tf-0.0.2/loss_balancer_tf.egg-info/
--rw-rw-rw-   0        0        0      192 2024-03-29 09:05:35.000000 loss-balancer-tf-0.0.2/loss_balancer_tf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-03-29 09:05:35.000000 loss-balancer-tf-0.0.2/loss_balancer_tf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 09:05:35.000000 loss-balancer-tf-0.0.2/loss_balancer_tf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-29 09:05:35.000000 loss-balancer-tf-0.0.2/loss_balancer_tf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-29 09:05:35.000000 loss-balancer-tf-0.0.2/loss_balancer_tf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 09:05:35.428730 loss-balancer-tf-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      323 2024-03-29 07:50:08.000000 loss-balancer-tf-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:30:26.243614 loss-balancer-tf-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-03-02 07:42:11.000000 loss-balancer-tf-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      192 2024-04-05 09:30:26.243614 loss-balancer-tf-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1992 2024-03-29 08:28:46.000000 loss-balancer-tf-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 09:30:26.227113 loss-balancer-tf-0.0.3/loss_balancer_tf/
+-rw-rw-rw-   0        0        0       58 2024-03-02 07:44:33.000000 loss-balancer-tf-0.0.3/loss_balancer_tf/__init__.py
+-rw-rw-rw-   0        0        0     4141 2024-04-05 09:28:15.000000 loss-balancer-tf-0.0.3/loss_balancer_tf/loss_balancer_tf.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:30:26.242613 loss-balancer-tf-0.0.3/loss_balancer_tf.egg-info/
+-rw-rw-rw-   0        0        0      192 2024-04-05 09:30:26.000000 loss-balancer-tf-0.0.3/loss_balancer_tf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-05 09:30:26.000000 loss-balancer-tf-0.0.3/loss_balancer_tf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 09:30:26.000000 loss-balancer-tf-0.0.3/loss_balancer_tf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 09:30:26.000000 loss-balancer-tf-0.0.3/loss_balancer_tf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-05 09:30:26.000000 loss-balancer-tf-0.0.3/loss_balancer_tf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 09:30:26.244113 loss-balancer-tf-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      323 2024-04-05 09:28:43.000000 loss-balancer-tf-0.0.3/setup.py
```

### Comparing `loss-balancer-tf-0.0.2/LICENSE` & `loss-balancer-tf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loss-balancer-tf-0.0.2/README.md` & `loss-balancer-tf-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `loss-balancer-tf-0.0.2/loss_balancer_tf/loss_balancer_tf.py` & `loss-balancer-tf-0.0.3/loss_balancer_tf/loss_balancer_tf.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
         self.total = tf.Variable(tf.zeros(len(self.loss_weights)), trainable=False)
         self.fix = tf.Variable(tf.zeros(len(self.loss_weights)), trainable=False)
         self.keys_to_indices = {k: i for i, k in enumerate(self.loss_weights)}
 
     def _update(self, metrics: tp.Dict[str, tp.Any], weight: float = 1) -> tp.Dict[str, float]:
         for key, value in metrics.items():
+            if tf.reduce_any(tf.math.is_nan(value)):
+                continue
             idx = self.keys_to_indices[key]
             self.total[idx].assign(self.total[idx] * self.ema_decay + weight * value)
             self.fix[idx].assign(self.fix[idx] * self.ema_decay + weight)
         return {key: self.total[self.keys_to_indices[key]] / self.fix[self.keys_to_indices[key]]
                     for key in metrics.keys()}
 
     def gradient(self, loss_dict: tp.Dict[str, tf.Tensor], tape: tf.GradientTape, output: tf.Tensor, trainable_variables):
```

