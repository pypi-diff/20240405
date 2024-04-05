# Comparing `tmp/tllab_common-2024.3.4.tar.gz` & `tmp/tllab_common-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2024.3.4.tar", max compression
+gzip compressed data, was "tllab_common-2024.4.0.tar", max compression
```

## Comparing `tllab_common-2024.3.4.tar` & `tllab_common-2024.4.0.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2024.3.4/LICENSE
--rw-r--r--   0        0        0      706 2023-08-24 13:53:49.878008 tllab_common-2024.3.4/README.md
--rw-r--r--   0        0        0      927 2024-03-27 16:10:08.109317 tllab_common-2024.3.4/pyproject.toml
--rw-r--r--   0        0        0      462 2024-02-27 12:16:59.090201 tllab_common-2024.3.4/tllab_common/__init__.py
--rwxr-xr-x   0        0        0     9595 2024-03-26 10:33:49.874564 tllab_common-2024.3.4/tllab_common/findcells.py
--rw-r--r--   0        0        0    10180 2024-03-22 12:40:55.230154 tllab_common-2024.3.4/tllab_common/fit.py
--rw-r--r--   0        0        0    13331 2024-03-22 13:12:06.294711 tllab_common-2024.3.4/tllab_common/io.py
--rw-r--r--   0        0        0    15669 2024-03-20 17:08:28.373032 tllab_common-2024.3.4/tllab_common/misc.py
--rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2024.3.4/tllab_common/transform.txt
--rw-r--r--   0        0        0     9245 2024-03-08 16:27:32.146103 tllab_common-2024.3.4/tllab_common/transforms.py
--rwxr-xr-x   0        0        0    70766 2024-03-08 16:27:31.926103 tllab_common-2024.3.4/tllab_common/wimread.py
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 tllab_common-2024.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2024.4.0/LICENSE
+-rw-r--r--   0        0        0      706 2023-08-24 13:53:49.878008 tllab_common-2024.4.0/README.md
+-rw-r--r--   0        0        0      953 2024-04-05 09:50:18.499420 tllab_common-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-02-27 12:16:59.090201 tllab_common-2024.4.0/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0     9595 2024-03-26 10:33:49.874564 tllab_common-2024.4.0/tllab_common/findcells.py
+-rw-r--r--   0        0        0    10664 2024-04-05 09:44:33.967664 tllab_common-2024.4.0/tllab_common/fit.py
+-rw-r--r--   0        0        0    13331 2024-04-05 09:50:19.667419 tllab_common-2024.4.0/tllab_common/io.py
+-rw-r--r--   0        0        0    15988 2024-04-05 09:48:59.307476 tllab_common-2024.4.0/tllab_common/misc.py
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 tllab_common-2024.4.0/PKG-INFO
```

### Comparing `tllab_common-2024.3.4/LICENSE` & `tllab_common-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.3.4/README.md` & `tllab_common-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.3.4/pyproject.toml` & `tllab_common-2024.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2024.3.4"
+version = "2024.4.0"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
@@ -26,17 +26,20 @@
 roifile = "*"
 ipython = "*"
 regex = "*"
 bidict = "*"
 pytest-xdist = { version = "*", optional = true }
 
 [tool.poetry.extras]
-test = ["pytest-xdist"]
+test = ["pytest"]
 transforms = ["SimpleITK-SimpleElastix"]
 bioformats = ["python-javabridge", "python-bioformats"]
 
 [tool.poetry.scripts]
 wimread = "tllab_common.wimread:main"
 
+[tool.isort]
+line_length = 119
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tllab_common-2024.3.4/tllab_common/findcells.py` & `tllab_common-2024.4.0/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.3.4/tllab_common/fit.py` & `tllab_common-2024.4.0/tllab_common/fit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,135 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
 from functools import cached_property
-from numbers import Number
-from typing import Callable, Optional, Sequence, Tuple
+from typing import Any, Callable, Sequence
 
 import numpy as np
-from numpy import typing as npt
+from numpy.typing import ArrayLike
 from scipy import special, stats
 from scipy.optimize import OptimizeResult, minimize
 
+Number = int | float | complex
+
 
 class Fit(metaclass=ABCMeta):
     bounds = None
 
-    def __init__(self, x: npt.ArrayLike, y: npt.ArrayLike,
-                 w: [npt.ArrayLike, None] = None, s: [npt.ArrayLike, None] = None,
-                 fit_window: Optional[Sequence[float]] = None, log_scale: bool = False):
+    def __init__(self, x: ArrayLike, y: ArrayLike,
+                 w: [ArrayLike, None] = None, s: [ArrayLike, None] = None,
+                 fit_window: Sequence[float] = None, log_scale: bool = False) -> None:
         x = np.asarray(x)
         y = np.asarray(y)
         w = np.ones_like(x) if w is None else np.asarray(w)
-        s = np.ones_like(x) if s is None else np.asarray(s)
+        if log_scale:
+            s = np.ones_like(x) if s is None else np.asarray(s) / np.abs(y)
+        else:
+            s = np.ones_like(x) if s is None else np.asarray(s)
 
         if fit_window:
             idx = (fit_window[0] <= x) & (x < fit_window[1])
             x, y, w, s = x[idx], y[idx], w[idx], s[idx]
 
-        if log_scale:
-            s[s == 0] = 1e-16
         self.x, self.y, self.w, self.s = nonnan(x, y, w, s)
         self.log_scale = log_scale
         self.n = np.sum(self.w)
         self.p_ci95 = None
         self.r_squared = None
         self.chi_squared = None
         self.r_squared_adjusted = None
 
     @property
     @abstractmethod
-    def n_p(self) -> Number:
+    def n_p(self) -> int:
         pass
 
     @property
     @abstractmethod
-    def p0(self) -> npt.ArrayLike:
+    def p0(self) -> ArrayLike:
         pass
 
     @staticmethod
     @abstractmethod
-    def fun(p: npt.ArrayLike, x: npt.ArrayLike) -> npt.ArrayLike:
+    def fun(p: ArrayLike, x: Number | ArrayLike) -> ArrayLike:
         pass
 
-    def dfun(self, p: npt.ArrayLike, x: npt.ArrayLike, diffstep: float = 1e-6) -> np.ndarray:
+    def dfun(self, p: ArrayLike, x: ArrayLike, diffstep: float = 1e-6) -> np.ndarray:
         """ d fun / dp_i for each p_i in p, this default function will calculate it numerically """
         eps = np.spacing(1)
         deriv = np.zeros((len(p), len(x)))
         f0 = np.asarray(self.fun(p, x))
         p = np.asarray(p)
         for i in range(len(p)):
             ph = p.copy()
             ph[i] = p[i] * (1 + diffstep) + eps
             f = np.asarray(self.fun(ph, x))
             deriv[i] = (f - f0) / (ph[i] - p[i])
         return deriv
 
-    def evaluate(self, x: [Number, npt.ArrayLike, None] = None) -> Tuple[npt.ArrayLike, npt.ArrayLike]:
+    def evaluate(self, x: Number | ArrayLike = None) -> tuple[ArrayLike, ArrayLike]:
         if x is None:
             x = np.linspace(np.nanmin(self.x), np.nanmax(self.x))
         else:
             x = np.asarray(x)
         return x.real, self.fun(self.p, x)
 
-    def evaluate_ci(self, x: [Number, npt.ArrayLike, None] = None) \
-            -> Tuple[npt.ArrayLike, npt.ArrayLike, npt.ArrayLike]:
+    def evaluate_ci(self, x: Number | ArrayLike = None) -> tuple[ArrayLike, ArrayLike, ArrayLike]:
         if x is None:
             x = np.linspace(np.nanmin(self.x), np.nanmax(self.x))
         else:
             x = np.asarray(x)
         f = self.fun(self.p, x)
         df = np.sqrt(np.sum((self.dfun(self.p, x).T * self.p_ci95).T ** 2, 0))
         return x.real, f - df, f + df
 
-    def get_cost_fun(self) -> Callable:
+    def get_cost_fun(self) -> Callable[[ArrayLike], float]:
         if self.log_scale:
-            def cost(p: npt.ArrayLike) -> npt.ArrayLike:
-                return np.nansum(np.abs(self.w / np.log(self.s) * np.log(self.y / self.fun(p, self.x)) ** 2))
+            def cost(p: ArrayLike) -> float:
+                return np.nansum(np.abs(self.w / self.s * np.log(self.y / self.fun(p, self.x)) ** 2))
         else:
-            def cost(p: npt.ArrayLike) -> npt.ArrayLike:
+            def cost(p: ArrayLike) -> float:
                 return np.nansum(np.abs(self.w / self.s * (self.y - self.fun(p, self.x)) ** 2))
         return cost
 
-    def fit(self):
+    def fit(self) -> Fit:
         _ = self.r
         return self
 
     @cached_property
     def r(self) -> OptimizeResult:
         if len(self.x):
-            r = minimize(self.get_cost_fun(), self.p0, method='Nelder-Mead', bounds=self.bounds)
+            r = minimize(self.get_cost_fun(), np.asarray(self.p0), method='Nelder-Mead', bounds=self.bounds)
         else:
             r = OptimizeResult(fun=np.nan, message='Empty data', nfev=0, nit=0, status=1, success=False,
                                x=np.full(self.n_p, np.nan))
         if self.log_scale:
             self.chi_squared, self.p_ci95, self.r_squared = fminerr(lambda p, x: np.log(self.fun(p, x)), r.x,
                                                                     np.log(self.y), (self.x,),
                                                                     self.w, np.log(self.s))
         else:
             self.chi_squared, self.p_ci95, self.r_squared = fminerr(self.fun, r.x,
                                                                     self.y, (self.x,), self.w, self.s)
         self.r_squared_adjusted = 1 - (1 - self.r_squared) * (self.n - 1) / (len(r.x) - 1)
         return r
 
     @property
-    def p(self) -> npt.ArrayLike:
+    def p(self) -> np.ndarray:
         return np.full(self.n_p, np.nan) if self.r is None else self.r.x
 
     @property
-    def log_likelihood(self) -> Number:
+    def log_likelihood(self) -> float:
         return -self.n * np.log(2 * np.pi * self.r.fun / (self.n - 1)) / 2 - (self.n - 1) / 2
 
     @property
-    def bic(self) -> Number:
+    def bic(self) -> float:
         """ Bayesian Information Criterion: the fit with the smallest bic should be the best fit """
         return self.n_p * np.log(self.n) - 2 * self.log_likelihood
 
-    def ftest(self, fit2) -> Number:
+    def ftest(self, fit2) -> float:
         """ returns the p-value for the hypothesis that fit2 is the better fit,
             assuming fit2 is the fit with more free parameters
             if the fits are swapped the p-value will be negative """
         if not np.all(self.x == fit2.x):
             raise ValueError('Only two fits on the same data can be compared.')
         if self.n_p == fit2.n_p:
             raise ValueError('The two fits cannot have the same number of parameters.')
@@ -146,104 +149,106 @@
 
 
 class Exponential1(Fit):
     n_p = 2
     bounds = ((0, None), (0, None))
 
     @property
-    def p0(self):
+    def p0(self) -> ArrayLike:
         """ y = a*exp(-t/tau)
             return a, tau
         """
         x, y = finite(self.x.astype('complex'), np.log(self.y.astype('complex')))
         if len(x) < 2:
             return [1, 1]
         else:
             q = np.polyfit(x, y, 1)
             return [np.clip(value.real, *bound) for value, bound in zip((np.exp(q[1]), -1 / q[0]), self.bounds)]
 
     @staticmethod
-    def fun(p, x):
+    def fun(p: ArrayLike, x: Number | ArrayLike) -> ArrayLike:
         return p[0] * np.exp(-x / p[1])
 
     # def dfun(self, p, x, diffstep=None):
     #     e = np.exp(-x / p[1])
     #     return np.vstack((e, p[0] * x * e / p[1] ** 2))
 
 
 class Exponential2(Fit):
     n_p = 4
     bounds = ((0, None), (0, 1), (0, None), (0, None))
 
     @property
-    def p0(self):
+    def p0(self) -> ArrayLike:
         """ y = A(a*exp(-t/tau_0) + (1-a)*exp(-t/tau_1)
             return A, a, tau_0, tau_1
         """
         n = len(self.x) // 2
         y0 = np.nanmax(self.y)
         q = Exponential1(self.x[n:], self.y[n:] / y0).p0
         return [np.clip(value, *bound)
                 for value, bound in zip((y0, 1 - q[0], q[1] / 3, q[1]), self.bounds)]
 
     @staticmethod
-    def fun(p, x):
+    def fun(p: ArrayLike, x: Number | ArrayLike) -> ArrayLike:
         return p[0] * (p[1] * np.exp(-x / p[2]) + (1 - p[1]) * np.exp(-x / p[3]))
 
     # def dfun(self, p, x, diffstep=None):
     #     e0 = np.exp(-x / p[2])
     #     e1 = np.exp(-x / p[3])
     #     return np.vstack((p[1] * e0 + (1 - p[1]) * e1, p[0] * (e0 - e1),
     #                       p[0] * p[1] * e0 / p[2] ** 2, p[0] * (1 - p[1]) * e1 / p[3] ** 2))
 
 
 class Powerlaw(Fit):
     n_p = 2
 
     @property
-    def p0(self):
+    def p0(self) -> ArrayLike:
         """ y = (x/tau)^alpha
             return alpha, tau
         """
         q = np.polyfit(*finite(np.log(self.x.astype('complex')), np.log(self.y.astype('complex'))), 1)
         return q[0].real, np.exp(-q[1] / q[0]).real
 
     @staticmethod
-    def fun(p, x):
+    def fun(p: ArrayLike, x: Number | ArrayLike) -> ArrayLike:
         return ((np.asarray(x).astype('complex') / p[1]) ** p[0]).real
 
 
 class GammaCDF(Fit):
     n_p = 2
 
     @property
-    def p0(self):
+    def p0(self) -> ArrayLike:
         """ y = γ(k, x / θ) / Γ(k)
         """
         m = np.sum(-self.x[1:] * np.diff(self.y))
         v = np.sum(-(self.x[1:] - m) ** 2 * np.diff(self.y))
         return m ** 2 / v, v / m  # A, k, theta
 
     @staticmethod
-    def fun(p, x):
+    def fun(p: ArrayLike, x: Number | ArrayLike) -> ArrayLike:
         """ p: k, theta """
         return 1 - special.gammainc(p[0], x / p[1])
 
 
-def finite(*args):
+def finite(*args: ArrayLike) -> list[np.ndarray]:
     idx = np.prod([np.isfinite(arg) for arg in args], 0).astype(bool)
-    return [arg[idx] for arg in args]
+    return [np.asarray(arg)[idx] for arg in args]
 
 
-def nonnan(*args):
+def nonnan(*args: ArrayLike) -> list[np.ndarray]:
     idx = np.prod([~np.isnan(arg) for arg in args], 0).astype(bool)
-    return [arg[idx] for arg in args]
+    return [np.asarray(arg)[idx] for arg in args]
 
 
-def fminerr(fun, a, y, args=(), w=None, s=None, diffstep=1e-6):
+def fminerr(fun: Callable[[ArrayLike, Any], float], a: ArrayLike, y: ArrayLike,
+            args: tuple[Any] = (), w: ArrayLike = None, s: ArrayLike = None,
+            diffstep: float = 1e-6) -> tuple[float, np.ndarray, float]:
     """ Error estimation of a fit
 
         Inputs:
         fun:  function which was fitted to data
         a:    function parameters
         y:    ydata
         args: extra arguments to fun
```

### Comparing `tllab_common-2024.3.4/tllab_common/io.py` & `tllab_common-2024.4.0/tllab_common/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pickle
+import shutil
 import zipfile
 from contextlib import ExitStack
 from functools import wraps
 from io import BytesIO, StringIO
 from pathlib import Path
-from typing import Any, Callable, Hashable, Iterator, IO, Optional, Sequence, Type
-import shutil
+from typing import IO, Any, Callable, Hashable, Iterator, Optional, Sequence, Type
 
 import dill
 import numpy as np
 import pandas
 import roifile
 from bidict import bidict
 from ruamel import yaml
```

### Comparing `tllab_common-2024.3.4/tllab_common/misc.py` & `tllab_common-2024.4.0/tllab_common/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import re
 import sys
 from abc import ABCMeta
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from glob import glob
-from numbers import Number
 from pathlib import Path
 from traceback import format_exc, print_exception
-from typing import Sequence
+from typing import Any, Hashable, Sequence
 
 import numpy as np
 import pandas
 import regex
-from ruamel import yaml
 from IPython import embed
+from ruamel import yaml
+
+from .io import get_params, pickle_dump, yaml_load
 
-from .io import pickle_dump, get_params, yaml_load
+Number = int | float | complex
 
 
 class Struct(dict):
     """ dict where the items are accessible as attributes """
     key_pattern = regex.compile(r'(^(?=\d)|\W)')
 
     def __init__(self, *args, **kwargs):
@@ -448,12 +449,20 @@
             return df.join(g.droplevel(0), lsuffix=f'_{j:.0f}', rsuffix=f'_{i:.0f}')
         else:
             df = df.join(g.droplevel(0), lsuffix=f'_{j:.0f}')
         j = i
     return df
 
 
+def add_extra_parameters(parameters: dict[Hashable, Any], extra_parameters: dict[Hashable, Any]) -> None:
+    for key, value in extra_parameters.items():
+        if isinstance(value, dict):
+            add_extra_parameters(parameters[key], value)
+        else:
+            parameters[key] = value
+
+
 color = Color()
 get_config = yaml_load
 getConfig = get_config
 getParams = get_params
 objFromDict = Struct
```

### Comparing `tllab_common-2024.3.4/PKG-INFO` & `tllab_common-2024.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab_common
-Version: 2024.3.4
+Version: 2024.4.0
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.10,<4.0
@@ -20,15 +20,15 @@
 Requires-Dist: colorcet
 Requires-Dist: czifile
 Requires-Dist: dill
 Requires-Dist: ipython
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: psutil
-Requires-Dist: pytest-xdist ; extra == "test"
+Requires-Dist: pytest-xdist
 Requires-Dist: regex
 Requires-Dist: roifile
 Requires-Dist: ruamel.yaml (>=0.17,<0.18)
 Requires-Dist: scipy
 Requires-Dist: tifffile
 Requires-Dist: tiffwrite
 Requires-Dist: tqdm
```

