# Comparing `tmp/geometricalgebra-0.1.1.tar.gz` & `tmp/geometricalgebra-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometricalgebra-0.1.1.tar", max compression
+gzip compressed data, was "geometricalgebra-0.1.2.tar", max compression
```

## Comparing `geometricalgebra-0.1.1.tar` & `geometricalgebra-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2024-03-08 12:07:58.199031 geometricalgebra-0.1.1/LICENSE
--rw-r--r--   0        0        0      837 2024-03-08 12:07:58.199031 geometricalgebra-0.1.1/README.md
--rw-r--r--   0        0        0       84 2024-03-08 12:07:58.199031 geometricalgebra-0.1.1/geometricalgebra/__init__.py
--rw-r--r--   0        0        0     8605 2024-03-08 12:07:58.199031 geometricalgebra-0.1.1/geometricalgebra/algebra.py
--rw-r--r--   0        0        0     3110 2024-03-08 12:07:58.199031 geometricalgebra-0.1.1/geometricalgebra/cayley.py
--rw-r--r--   0        0        0    39904 2024-03-08 12:07:58.199031 geometricalgebra-0.1.1/geometricalgebra/cga.py
--rw-r--r--   0        0        0      982 2024-03-08 12:07:58.199031 geometricalgebra-0.1.1/geometricalgebra/cga2d.py
--rw-r--r--   0        0        0     6061 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/cga3d.py
--rw-r--r--   0        0        0     1347 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/cga4d.py
--rw-r--r--   0        0        0     1914 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/coherent_point_drift.py
--rw-r--r--   0        0        0      450 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/tests/test_algebra.py
--rw-r--r--   0        0        0    16229 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/tests/test_cayley.py
--rw-r--r--   0        0        0     1476 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/tests/test_coherent_point_drift.py
--rw-r--r--   0        0        0      533 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/tests/test_gradient.py
--rw-r--r--   0        0        0     1378 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/tests/test_quaterion_interpolation.py
--rw-r--r--   0        0        0     2189 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/tests/test_tensorflow.py
--rw-r--r--   0        0        0     7162 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/tests/test_vector.py
--rw-r--r--   0        0        0    11381 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/tests/test_versor.py
--rw-r--r--   0        0        0      280 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/utils.py
--rw-r--r--   0        0        0    27779 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/vector.py
--rw-r--r--   0        0        0     8002 2024-03-08 12:07:58.203031 geometricalgebra-0.1.1/geometricalgebra/viewer.py
--rw-r--r--   0        0        0     1758 2024-03-08 12:07:58.207031 geometricalgebra-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 geometricalgebra-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/LICENSE
+-rw-r--r--   0        0        0      837 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/README.md
+-rw-r--r--   0        0        0       84 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/__init__.py
+-rw-r--r--   0        0        0     8605 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/algebra.py
+-rw-r--r--   0        0        0     3110 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cayley.py
+-rw-r--r--   0        0        0    39904 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cga.py
+-rw-r--r--   0        0        0      982 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cga2d.py
+-rw-r--r--   0        0        0     6061 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cga3d.py
+-rw-r--r--   0        0        0     1347 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cga4d.py
+-rw-r--r--   0        0        0     2853 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/coherent_point_drift.py
+-rw-r--r--   0        0        0      450 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_algebra.py
+-rw-r--r--   0        0        0    16229 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_cayley.py
+-rw-r--r--   0        0        0     1476 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_coherent_point_drift.py
+-rw-r--r--   0        0        0      533 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_gradient.py
+-rw-r--r--   0        0        0     1378 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_quaterion_interpolation.py
+-rw-r--r--   0        0        0     2189 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_tensorflow.py
+-rw-r--r--   0        0        0     7162 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_vector.py
+-rw-r--r--   0        0        0    11381 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_versor.py
+-rw-r--r--   0        0        0      280 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/utils.py
+-rw-r--r--   0        0        0    28069 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/vector.py
+-rw-r--r--   0        0        0     8139 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/viewer.py
+-rw-r--r--   0        0        0     1777 2024-04-05 09:55:07.354896 geometricalgebra-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 geometricalgebra-0.1.2/PKG-INFO
```

### Comparing `geometricalgebra-0.1.1/LICENSE` & `geometricalgebra-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/README.md` & `geometricalgebra-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/algebra.py` & `geometricalgebra-0.1.2/geometricalgebra/algebra.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/cayley.py` & `geometricalgebra-0.1.2/geometricalgebra/cayley.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/cga.py` & `geometricalgebra-0.1.2/geometricalgebra/cga.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/cga2d.py` & `geometricalgebra-0.1.2/geometricalgebra/cga2d.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/cga3d.py` & `geometricalgebra-0.1.2/geometricalgebra/cga3d.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/cga4d.py` & `geometricalgebra-0.1.2/geometricalgebra/cga4d.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/coherent_point_drift.py` & `geometricalgebra-0.1.2/geometricalgebra/coherent_point_drift.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,43 +2,69 @@
 
 from geometricalgebra.cga import CGAVector
 
 
 def e_step(p: CGAVector, q: CGAVector, v: CGAVector):
     """The E-step estimate the correspondences, i.e., the probabilities
 
-
     Args:
         p: tensor of shape (..., N) of vectors
         q: tensor of shape (..., M) of vectors
         v: tensor of shape (...,) of poses
 
     Returns:
         probabilities p of shape (..., N, M) where p[i, j] indicated whether the p[i] correspond to q[j]
     """
     logits = v[..., None].apply(p)[..., None].scalar_product(q[..., None, :])
     return p.framework().softmax(logits, axis=-1)
 
 
 def m_step(p, q, prob, only_2d=False):
-    """The M-step maximizes the likelihood by finding the optimal motor"""
+    """The M-step maximizes the likelihood by finding the optimal motor
+
+    Args:
+        p: tensor of shape (..., N) of vectors
+        q: tensor of shape (..., M) of vectors
+        prob: tensor of shape (..., N, M) of probabilities
+        only_2d: if True, the motor is only estimated in 2d
+
+    Returns:
+        motor: the estimated motor given the correspondence probabilities
+        (variance, variance_dir): the estimated variances
+    """
     q_weighted = q[..., None, :] * prob
     motor = type(p).from_motor_estimation(p, q_weighted.sum(-1), only_2d=only_2d)
     variance = -2 * (motor[..., None].apply(p)[..., None].scalar_product(q_weighted(1))).sum(-1).mean(-1)
     variance_dir = -2 * ((motor[..., None].apply(p)[..., None].scalar_product(q_weighted(3))).sum(-1) - 1).mean(-1)
     variance = p.xnp().maximum(1e-6, variance)
     variance_dir = p.xnp().maximum(1e-6, variance_dir)
     return motor, (variance, variance_dir)
 
 
 def pose_and_correspondence_registration(p: CGAVector, q: CGAVector, threshold=1e-3, max_iteration=50, only_2d=False):
-    """A simultaneous pose and correspondence registration via the covariant point drift"""
-    v = type(p).from_identity()
+    """A simultaneous pose and correspondence registration via the covariant point drift
+
+    Args:
+        p: tensor of shape (..., N) of vectors
+        q: tensor of shape (..., M) of vectors
+        threshold: the threshold for convergence
+        max_iteration: the maximum number of iterations
+        only_2d: if True, the motor is only estimated in 2d
+
+    Returns:
+        motor: the estimated motor
+        prob: tensor of shape (..., N, M) of the estimated correspondence probabilities that q[i] corresponds to p[j]
+        variance: the estimated variance
+    """
+    motor = type(p).from_identity()
     variance = variance_dir = q.xnp().array(1e-6)
     last = variance
     for i in range(max_iteration):
-        prob = e_step(p, (q(1) / variance[..., None] + 0.5 * q(3) / variance_dir[..., None]) * 2, v)
-        v, (variance, variance_dir) = m_step(p, q, prob, only_2d)
+        # E-step
+        prob = e_step(p, 2 * (q(1) / variance[..., None] + 0.5 * q(3) / variance_dir[..., None]), motor)
+        # M-step
+        motor, (variance, variance_dir) = m_step(p, q, prob, only_2d)
+        # Check for convergence
         if variance * (1 + threshold) > last and i > 4:
             break
         last = variance
-    return v, prob, variance
+    return motor, prob, variance
```

### Comparing `geometricalgebra-0.1.1/geometricalgebra/tests/test_cayley.py` & `geometricalgebra-0.1.2/geometricalgebra/tests/test_cayley.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/tests/test_coherent_point_drift.py` & `geometricalgebra-0.1.2/geometricalgebra/tests/test_coherent_point_drift.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/tests/test_gradient.py` & `geometricalgebra-0.1.2/geometricalgebra/tests/test_gradient.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/tests/test_quaterion_interpolation.py` & `geometricalgebra-0.1.2/geometricalgebra/tests/test_quaterion_interpolation.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/tests/test_tensorflow.py` & `geometricalgebra-0.1.2/geometricalgebra/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/tests/test_vector.py` & `geometricalgebra-0.1.2/geometricalgebra/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/tests/test_versor.py` & `geometricalgebra-0.1.2/geometricalgebra/tests/test_versor.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.1/geometricalgebra/vector.py` & `geometricalgebra-0.1.2/geometricalgebra/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,14 +483,22 @@
 
     def split(self: Subtype) -> List[Subtype]:
         length = self.shape[0]  # len(self) does not work for symbolic tensors in tf
         if length is None:
             raise TypeError("Can not split tensors of unknown dimension")
         return [self[i] for i in range(length)]
 
+    def sparsified(self):
+        """Keep only the grades with non-zero elements"""
+        new_grades = set()
+        for grade in self.grades:
+            if self.xnp().count_nonzero(abs(self(grade)._values) > 1e-9):
+                new_grades.add(grade)
+        return self(new_grades)
+
     @classmethod
     def from_scalar(cls: Type[Subtype], scalar: ArrayLike, pseudo: bool = False) -> Subtype:
         """Create a multivector (tensor) representing scalar(s)
 
         Args:
             scalar: tensor of scalar inputs of shape (no copy is made)
             pseudo: if True returns a pseudo-scalar
```

### Comparing `geometricalgebra-0.1.1/geometricalgebra/viewer.py` & `geometricalgebra-0.1.2/geometricalgebra/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Classes:
     PathViewer: Show path in cartesian space
     OrientationViewer: Show orientation space on unit sphere
 """
 
 from itertools import count
+from typing import Union
 
 import numpy as np
 from matplotlib.patches import FancyArrowPatch
 from mpl_toolkits.mplot3d.proj3d import proj_transform
 from scipy import linalg
 
 from geometricalgebra import cga3d
@@ -76,15 +77,17 @@
 
     def __getattr__(self, key):
         return getattr(self._axes, key)
 
     def __dir__(self):
         return dir(self) + dir(self._axes)
 
-    def trace_point(self, tensor: cga3d.Vector, linestyle="None", marker="o", **kwargs):
+    def trace_point(self, tensor: Union[list[cga3d.Vector], cga3d.Vector], linestyle="None", marker="o", **kwargs):
+        if isinstance(tensor, list):
+            tensor = cga3d.Vector.stack(tensor)
         return self._axes.plot(*tensor.ravel().to_euclid().T, linestyle=linestyle, marker=marker, **kwargs)
 
     def trace_point_pair(self, tensor: cga3d.Vector, linestyle="-", startmarker="o", endmarker=">", **kwargs):
         for pair in tensor.ravel():
             end_points = pair.point_pair_to_end_points()
             (object_,) = self.trace_point(
                 end_points, linestyle=linestyle, marker="", label=kwargs.pop("label", None), **kwargs
```

### Comparing `geometricalgebra-0.1.1/pyproject.toml` & `geometricalgebra-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "geometricalgebra"
-version = '0.1.1'
+version = '0.1.2'
 description = "A package for conformal geometric algebra"
 authors = [
     "Daniel Vorberg <daniel.vorberg@wandelbots.com>",
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 numpy = ">=1.19.0"
 scipy = ">=1.8.0"
 tensorflow = { version = "2.14.0", optional = true, platform = "linux" }
-tensorflow-macos = { version = "^2.10.0", optional = true, platform = "darwin"}
+tensorflow-macos = { version = "2.14.1", optional = true, platform = "darwin"}
 matplotlib = { version = ">=3.4.2", optional = true }
 jax = { version = "0.4.10", optional = true }
 jaxlib = { version = "0.4.10", optional = true }
 
 
 [tool.poetry.extras]
-all = ["matplotlib", "tensorflow", "jax", "jaxlib"]
+all = ["matplotlib", "tensorflow", "tensorflow-macos", "jax", "jaxlib"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.4.4"
 pylint = "2.15.4"
 mypy = "^1.8.0"
 isort = "5.10.1"
 darglint = "1.8.1"
```

### Comparing `geometricalgebra-0.1.1/PKG-INFO` & `geometricalgebra-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: geometricalgebra
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for conformal geometric algebra
 Author: Daniel Vorberg
 Author-email: daniel.vorberg@wandelbots.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: all
 Requires-Dist: jax (==0.4.10) ; extra == "all"
 Requires-Dist: jaxlib (==0.4.10) ; extra == "all"
 Requires-Dist: matplotlib (>=3.4.2) ; extra == "all"
 Requires-Dist: numpy (>=1.19.0)
 Requires-Dist: scipy (>=1.8.0)
 Requires-Dist: tensorflow (==2.14.0) ; (sys_platform == "linux") and (extra == "all")
-Requires-Dist: tensorflow-macos (>=2.10.0,<3.0.0) ; sys_platform == "darwin"
+Requires-Dist: tensorflow-macos (==2.14.1) ; (sys_platform == "darwin") and (extra == "all")
 Description-Content-Type: text/markdown
 
 # geometricalgebra
 
 ![badge](https://github.com/wandelbotsgmbh/geometricalgebra/actions/workflows/python-app.yml/badge.svg)
 
 Library implementing conformal geometric algebra.
```

