# Comparing `tmp/polars_ols-0.2.3.tar.gz` & `tmp/polars_ols-0.2.4.tar.gz`

## Comparing `polars_ols-0.2.3.tar` & `polars_ols-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 polars_ols-0.2.3/Cargo.toml
--rw-r--r--   0     1001      127      116 2024-04-04 18:39:35.000000 polars_ols-0.2.3/.cargo/config.toml
--rw-r--r--   0     1001      127     3908 2024-04-04 18:39:35.000000 polars_ols-0.2.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      139 2024-04-04 18:39:35.000000 polars_ols-0.2.3/.gitignore
--rw-r--r--   0     1001      127      912 2024-04-04 18:39:35.000000 polars_ols-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1067 2024-04-04 18:39:35.000000 polars_ols-0.2.3/LICENSE
--rw-r--r--   0     1001      127      671 2024-04-04 18:39:35.000000 polars_ols-0.2.3/Makefile
--rw-r--r--   0     1001      127    13745 2024-04-04 18:39:35.000000 polars_ols-0.2.3/README.md
--rw-r--r--   0     1001      127    44513 2024-04-04 18:39:35.000000 polars_ols-0.2.3/notebooks/polars_ols_demo.ipynb
--rw-r--r--   0     1001      127     4327 2024-04-04 18:39:35.000000 polars_ols-0.2.3/polars_ols/__init__.py
--rw-r--r--   0     1001      127    15159 2024-04-04 18:39:35.000000 polars_ols-0.2.3/polars_ols/least_squares.py
--rw-r--r--   0     1001      127     3464 2024-04-04 18:39:35.000000 polars_ols-0.2.3/polars_ols/utils.py
--rw-r--r--   0     1001      127       63 2024-04-04 18:39:35.000000 polars_ols-0.2.3/requirements.txt
--rw-r--r--   0     1001      127     9320 2024-04-04 18:39:35.000000 polars_ols-0.2.3/src/expressions.rs
--rw-r--r--   0     1001      127    16506 2024-04-04 18:39:35.000000 polars_ols-0.2.3/src/least_squares.rs
--rw-r--r--   0     1001      127     5331 2024-04-04 18:39:35.000000 polars_ols-0.2.3/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-04 18:39:35.000000 polars_ols-0.2.3/tests/__init__.py
--rw-r--r--   0     1001      127     6257 2024-04-04 18:39:35.000000 polars_ols-0.2.3/tests/benchmark.py
--rw-r--r--   0     1001      127       87 2024-04-04 18:39:35.000000 polars_ols-0.2.3/tests/requirements-test.txt
--rw-r--r--   0     1001      127    16848 2024-04-04 18:39:35.000000 polars_ols-0.2.3/tests/test_ols.py
--rw-r--r--   0     1001      127    61832 2024-04-04 18:39:35.000000 polars_ols-0.2.3/Cargo.lock
--rw-r--r--   0     1001      127     1864 2024-04-04 18:39:35.000000 polars_ols-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    14452 1970-01-01 00:00:00.000000 polars_ols-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 polars_ols-0.2.4/Cargo.toml
+-rw-r--r--   0     1001      127      116 2024-04-05 21:12:56.000000 polars_ols-0.2.4/.cargo/config.toml
+-rw-r--r--   0     1001      127     3908 2024-04-05 21:12:56.000000 polars_ols-0.2.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      139 2024-04-05 21:12:56.000000 polars_ols-0.2.4/.gitignore
+-rw-r--r--   0     1001      127      912 2024-04-05 21:12:56.000000 polars_ols-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1067 2024-04-05 21:12:56.000000 polars_ols-0.2.4/LICENSE
+-rw-r--r--   0     1001      127      671 2024-04-05 21:12:56.000000 polars_ols-0.2.4/Makefile
+-rw-r--r--   0     1001      127    13832 2024-04-05 21:12:56.000000 polars_ols-0.2.4/README.md
+-rw-r--r--   0     1001      127    44513 2024-04-05 21:12:56.000000 polars_ols-0.2.4/notebooks/polars_ols_demo.ipynb
+-rw-r--r--   0     1001      127     4479 2024-04-05 21:12:56.000000 polars_ols-0.2.4/polars_ols/__init__.py
+-rw-r--r--   0     1001      127    17412 2024-04-05 21:12:56.000000 polars_ols-0.2.4/polars_ols/least_squares.py
+-rw-r--r--   0     1001      127     3464 2024-04-05 21:12:56.000000 polars_ols-0.2.4/polars_ols/utils.py
+-rw-r--r--   0     1001      127       63 2024-04-05 21:12:56.000000 polars_ols-0.2.4/requirements.txt
+-rw-r--r--   0     1001      127     9320 2024-04-05 21:12:56.000000 polars_ols-0.2.4/src/expressions.rs
+-rw-r--r--   0     1001      127    16506 2024-04-05 21:12:56.000000 polars_ols-0.2.4/src/least_squares.rs
+-rw-r--r--   0     1001      127     5331 2024-04-05 21:12:56.000000 polars_ols-0.2.4/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-05 21:12:56.000000 polars_ols-0.2.4/tests/__init__.py
+-rw-r--r--   0     1001      127     6245 2024-04-05 21:12:56.000000 polars_ols-0.2.4/tests/benchmark.py
+-rw-r--r--   0     1001      127       87 2024-04-05 21:12:56.000000 polars_ols-0.2.4/tests/requirements-test.txt
+-rw-r--r--   0     1001      127    17899 2024-04-05 21:12:56.000000 polars_ols-0.2.4/tests/test_ols.py
+-rw-r--r--   0     1001      127    61832 2024-04-05 21:12:56.000000 polars_ols-0.2.4/Cargo.lock
+-rw-r--r--   0     1001      127     1864 2024-04-05 21:12:56.000000 polars_ols-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    14539 1970-01-01 00:00:00.000000 polars_ols-0.2.4/PKG-INFO
```

### Comparing `polars_ols-0.2.3/Cargo.toml` & `polars_ols-0.2.4/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [package]
 name = "polars_ols"
-version = "0.2.3"
+version = "0.2.4"
 edition = "2021"
 
 [lib]
 name = "polars_ols"
 crate-type= ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "*", features = ["extension-module", "abi3-py310"] }
+pyo3 = { version = "*", features = ["extension-module", "abi3-py38"] }  # set > py38 supported version
 pyo3-polars = { version = "*", features = ["derive"] }
 serde = { version = "*", features = ["derive"] }
 polars = { version = "*", features = ["performant", "lazy", "ndarray", "dtype-struct"]}
 ndarray-rand = {version = "*"}
 faer = {version = "*"}
 faer-ext = {version = "*", features = ["ndarray"]}
 num-traits = { version = "*" }
```

### Comparing `polars_ols-0.2.3/.github/workflows/publish_to_pypi.yml` & `polars_ols-0.2.4/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/.pre-commit-config.yaml` & `polars_ols-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/LICENSE` & `polars_ols-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/Makefile` & `polars_ols-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/README.md` & `polars_ols-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 API & Examples
 ------------
 
 Importing `polars_ols` will register the namespace `least_squares` provided by this package.
 You can build models either by either specifying polars expressions (e.g. `pl.col(...)`) for your targets and features or using
 the formula api (patsy syntax). All models support the following general (optional) arguments:
 - `mode` - a literal which determines the type of output produced by the model
+- `null_policy` - a literal which determines how to deal with missing data
 - `add_intercept` - a boolean specifying if an intercept feature should be added to the features
 - `sample_weights` - a column or expression providing non-negative weights applied to the samples
 
 Remaining parameters are model specific, for example `alpha` penalty parameter used by regularized least squares models.
 
 See below for basic usage examples.
 Please refer to the [tests](./tests/test_ols.py) or [demo notebook](./notebooks/polars_ols_demo.ipynb) for detailed examples.
@@ -175,25 +176,25 @@
 
 | Model                   | polars_ols       | Python Benchmark  | Benchmark Type | Speed-up vs Python Benchmark |
 |-------------------------|------------------|-------------------|----------------|------------------------------|
 | Least Squares           | 283 ± 4 us       | 509 ± 313 us      | Numpy          | 1.8x                         |
 | Ridge                   | 262 ± 3 us       | 369 ± 231 us      | Numpy          | 1.4x                         |
 | Weighted Least Squares  | 493 ± 7 us       | 2.13 ms ± 0.22 ms | Statsmodels    | 4.3x                         |
 | Elastic Net             | 326 ± 3 us       | 87.3 ms ± 9.0 ms  | Sklearn        | 268.2x                       |
-| Recursive Least Squares | 1.39 ms ± 0.01 ms| 22.3 ms ± 0.2 ms  | Statsmodels    | 16.0x                        |
+| Recursive Least Squares | 1.39 ms ± 0.01 ms| 18.7 ms ± 1.4 ms  | Statsmodels    | 13.5x                        |
 | Rolling Least Squares   | 2.72 ms ± 0.03 ms| 22.3 ms ± 0.2 ms  | Statsmodels    | 8.2x                         |
 
 ### n_samples=10_000, n_features=100
-| Model                   | polars_ols       | Python Benchmark  | Benchmark Type | Speed-up vs Python Benchmark |
-|-------------------------|------------------|-------------------|----------------|------------------------------|
-| Least Squares           | 15.6 ms ± 0.2 ms| 29.9 ms ± 8.6 ms  | Numpy          | 1.9x                         |
-| Ridge                   | 5.81 ms ± 0.05 ms| 5.21 ms ± 0.94 ms | Numpy          | 0.9x                         |
-| Weighted Least Squares  | 16.8 ms ± 0.2 ms| 82.4 ms ± 9.1 ms  | Statsmodels    | 4.9x                         |
-| Elastic Net             | 20.9 ms ± 0.3 ms| 134 ms ± 21 ms    | Sklearn        | 6.4x                         |
-| Recursive Least Squares | 163 ms ± 28 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 24.5x                        |
+| Model                   | polars_ols       | Python Benchmark    | Benchmark Type | Speed-up vs Python Benchmark |
+|-------------------------|------------------|---------------------|----------------|------------------------------|
+| Least Squares           | 15.6 ms ± 0.2 ms| 29.9 ms ± 8.6 ms    | Numpy          | 1.9x                         |
+| Ridge                   | 5.81 ms ± 0.05 ms| 5.21 ms ± 0.94 ms   | Numpy          | 0.9x                         |
+| Weighted Least Squares  | 16.8 ms ± 0.2 ms| 82.4 ms ± 9.1 ms    | Statsmodels    | 4.9x                         |
+| Elastic Net             | 20.9 ms ± 0.3 ms| 134 ms ± 21 ms      | Sklearn        | 6.4x                         |
+| Recursive Least Squares | 163 ms ± 28 ms  | 65.7 sec ± 28.2 sec | Statsmodels    | 403.1x                       |
 | Rolling Least Squares   | 390 ms ± 10 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 10.2x                        |
 
 Numpy's `lstsq` is already a highly optimized call into LAPACK and so the scope for speed-up is limited.
 However, we can achieve substantial speed-ups for the more complex models by working entirely in rust
 and avoiding overhead from back and forth into python.
 
 Expect an additional relative order-of-magnitude speed up to your workflow if it involved repeated re-estimation of models in
```

### Comparing `polars_ols-0.2.3/notebooks/polars_ols_demo.ipynb` & `polars_ols-0.2.4/notebooks/polars_ols_demo.ipynb`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/polars_ols/__init__.py` & `polars_ols-0.2.4/polars_ols/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Literal, Optional
 
 import polars as pl
 
 from polars_ols.least_squares import (
+    NullPolicy,
     OLSKwargs,
+    OutputMode,
     RLSKwargs,
     RollingKwargs,
     compute_least_squares,
     compute_recursive_least_squares,
     compute_rolling_least_squares,
     least_squares_from_formula,
     predict,
@@ -29,23 +31,25 @@
         self._expr = expr
 
     def least_squares(
         self,
         *features: pl.Expr,
         sample_weights: Optional[pl.Expr] = None,
         add_intercept: bool = False,
-        mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+        mode: OutputMode = "predictions",
+        null_policy: NullPolicy = "ignore",
         **ols_kwargs,
     ) -> pl.Expr:
         return compute_least_squares(
             self._expr,
             *features,
             sample_weights=sample_weights,
             add_intercept=add_intercept,
             mode=mode,
+            null_policy=null_policy,
             ols_kwargs=OLSKwargs(**ols_kwargs),
         )
 
     def ols(self, *features: pl.Expr, **kwargs) -> pl.Expr:
         return self.least_squares(*features, **kwargs)
 
     def wls(self, *features: pl.Expr, sample_weights: pl.Expr, **kwargs) -> pl.Expr:
@@ -61,40 +65,44 @@
         return self.least_squares(*features, alpha=alpha, l1_ratio=l1_ratio, **kwargs)
 
     def rls(
         self,
         *features: pl.Expr,
         sample_weights: Optional[pl.Expr] = None,
         add_intercept: bool = False,
-        mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+        mode: OutputMode = "predictions",
+        null_policy: NullPolicy = "ignore",
         **rls_kwargs,
     ):
         return compute_recursive_least_squares(
             self._expr,
             *features,
             sample_weights=sample_weights,
             add_intercept=add_intercept,
             mode=mode,
+            null_policy=null_policy,
             rls_kwargs=RLSKwargs(**rls_kwargs),
         )
 
     def rolling_ols(
         self,
         *features: pl.Expr,
         sample_weights: Optional[pl.Expr] = None,
         add_intercept: bool = False,
-        mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+        mode: OutputMode = "predictions",
+        null_policy: NullPolicy = "ignore",
         **rolling_kwargs,
     ):
         return compute_rolling_least_squares(
             self._expr,
             *features,
             sample_weights=sample_weights,
             add_intercept=add_intercept,
             mode=mode,
+            null_policy=null_policy,
             rolling_kwargs=RollingKwargs(**rolling_kwargs),
         )
 
     def expanding_ols(self, *features: pl.Expr, **kwargs):
         return self.rls(*features, half_life=None, **kwargs)
 
     def from_formula(self, formula: str, **kwargs) -> pl.Expr:
@@ -107,16 +115,16 @@
             return self.rolling_ols(*features, add_intercept=add_intercept, **kwargs)
         else:
             return self.least_squares(*features, add_intercept=add_intercept, **kwargs)
 
     def predict(
         self, *features: pl.Expr, name: Optional[str] = None, add_intercept: bool = False
     ) -> pl.Expr:
-        return predict(self._expr, *features, name=name, add_intercept=add_intercept)
+        return predict(self._expr, *features, add_intercept=add_intercept, name=name)
 
     def predict_from_formula(self, formula: str, name: Optional[str] = None) -> pl.Expr:
         features, add_intercept = build_expressions_from_patsy_formula(
             formula, include_dependent_variable=False
         )
         has_const = any(f.meta.output_name == "const" for f in features)
         add_intercept &= not has_const
-        return self.predict(*features, add_intercept=add_intercept, name=name)
+        return self.predict(*features, name=name, add_intercept=add_intercept)
```

### Comparing `polars_ols-0.2.3/polars_ols/least_squares.py` & `polars_ols-0.2.4/polars_ols/least_squares.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from dataclasses import asdict, dataclass
-from functools import partial
+from functools import partial, reduce
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional, Set, get_args
 
 import polars as pl
 from polars.plugins import register_plugin_function
 from polars.type_aliases import IntoExpr
 
 from polars_ols.utils import build_expressions_from_patsy_formula, parse_into_expr
 
@@ -17,16 +17,24 @@
     "compute_recursive_least_squares",
     "compute_rolling_least_squares",
     "least_squares_from_formula",
     "predict",
     "OLSKwargs",
     "RLSKwargs",
     "RollingKwargs",
+    "NullPolicy",
+    "OutputMode",
 ]
 
+NullPolicy = Literal["zero", "drop", "drop_y_zero_x", "ignore"]
+OutputMode = Literal["predictions", "residuals", "coefficients"]
+
+_VALID_NULL_POLICIES: Set[NullPolicy] = set(get_args(NullPolicy))
+_VALID_OUTPUT_MODES: Set[OutputMode] = set(get_args(OutputMode))
+
 
 @dataclass
 class OLSKwargs:
     """Specifies parameters relevant for regularized linear models: LASSO / Ridge / ElasticNet.
 
     Attributes:
         alpha: Regularization strength. Defaults to 0.0.
@@ -70,63 +78,100 @@
     alpha: Optional[float] = None  # optional ridge alpha
 
     def to_dict(self) -> Dict[str, Any]:
         return asdict(self)
 
 
 def _pre_process_data(
-    target: pl.Expr, *features: pl.Expr, sample_weights: Optional[pl.Expr], add_intercept: bool
+    target: pl.Expr,
+    *features: pl.Expr,
+    sample_weights: Optional[pl.Expr],
+    add_intercept: bool,
+    null_policy: NullPolicy,
 ):
     """Pre-processes the input data by casting it to float32 and scaling it with sample weights if
      provided.
 
     Args:
         target: The target expression.
         *features: Variable number of feature expressions.
         sample_weights: Optional expression representing sample weights.
         add_intercept: Whether to add an intercept column.
+        null_policy: literal defining a strategy for handling missing data.
 
     Returns:
         Tuple containing the pre-processed target, features, and sample weights.
     """
     target = parse_into_expr(target).cast(pl.Float32)
     features = [f.cast(pl.Float32) for f in features]
+
+    # handle nulls
+    match null_policy:
+        case "zero":
+            target = target.fill_null(0.0)
+            features = [f.fill_null(0.0) for f in features]
+        case "drop_y_zero_x":
+            # drops rows based on missing targets, and otherwise zero's out any
+            # remaining missing features
+            is_valid = target.is_not_null()
+            target = target.filter(is_valid)
+            features = [f.filter(is_valid).fill_null(0.0) for f in features]
+        case "drop":
+            # drops rows if either target or any feature is missing
+            is_valid_y = target.is_not_null()
+            is_valid_x = reduce(lambda x, y: x.is_not_null() & y.is_not_null(), features)
+            is_valid = is_valid_y & is_valid_x
+            features = [f.filter(is_valid) for f in features]
+            target = target.filter(is_valid)
+        case "ignore":
+            # only choose this if nulls are already handled upstream
+            pass
+        case _:
+            raise NotImplementedError(
+                f"null_policy: '{null_policy}' is not supported. "
+                f"It must be one of '{_VALID_NULL_POLICIES}'"
+            )
+
+    # handle intercept
     if add_intercept:
         if any(f.meta.output_name == "const" for f in features):
             logger.info("feature named 'const' already detected, assuming it is an intercept")
         else:
             features += [target.mul(0.0).add(1.0).alias("const")]
+    # handle sample weights
     sqrt_w = 1.0
     if sample_weights is not None:
         sqrt_w = sample_weights.cast(pl.Float32).sqrt()
         target *= sqrt_w
         features = [expr * sqrt_w for expr in features]
     return target, features, sqrt_w
 
 
 def compute_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
-    mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+    mode: OutputMode = "predictions",
+    null_policy: NullPolicy = "ignore",
     ols_kwargs: Optional[OLSKwargs] = None,
 ) -> pl.Expr:
     """Performs least squares regression.
 
     Depending on parameters provided this method supports a combination of sample weighting (WLS),
      L1/L2 regularization,
      and/or non-negativity constraint on coefficients.
 
     Args:
         target: The target expression.
         *features: Variable number of feature expressions.
         sample_weights: Optional expression representing sample weights.
         add_intercept: Whether to add an intercept column.
         mode: Mode of operation ("predictions", "residuals", "coefficients").
+        null_policy: Strategy for handling missing data ("zero", "drop", "ignore").
         ols_kwargs: Additional keyword arguments specific for regularized OLS models. These include:
             - "alpha": Regularization strength. Default is 0.0.
                       Expected dtype: float.
             - "l1_ratio": Mixing parameter for ElasticNet regularization (0 for Ridge, 1 for LASSO).
                           Default is None (equivalent to Ridge regression).
                           Expected dtype: float or None.
             - "max_iter": Maximum number of iterations. Defaults to 1000 iterations.
@@ -135,21 +180,21 @@
                      Expected dtype: float or None.
             - "positive": Whether to enforce non-negativity constraints on coefficients.
                           Default is None (equivalent to False, i.e. no constraint on coefficients).
                           Expected dtype: bool or None.
     Returns:
         Resulting expression based on the chosen mode.
     """
-    assert mode in {
-        "predictions",
-        "residuals",
-        "coefficients",
-    }, "'mode' must be one of {predictions, residuals, coefficients}"
+    assert mode in _VALID_OUTPUT_MODES, f"'mode' must be one of '{_VALID_OUTPUT_MODES}'"
     target, features, sqrt_w = _pre_process_data(
-        target, *features, sample_weights=sample_weights, add_intercept=add_intercept
+        target,
+        *features,
+        sample_weights=sample_weights,
+        add_intercept=add_intercept,
+        null_policy=null_policy,
     )
 
     ols_kwargs: OLSKwargs = ols_kwargs or OLSKwargs()
 
     # register either coefficient or prediction plugin functions
     if mode == "coefficients":
         return (
@@ -183,28 +228,30 @@
 
 
 def compute_recursive_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
-    mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+    mode: OutputMode = "predictions",
+    null_policy: NullPolicy = "ignore",
     rls_kwargs: Optional[RLSKwargs] = None,
 ) -> pl.Expr:
     """Performs an efficient recursive least squares regression (RLS).
 
     Defaults to RLS with forgetting factor of 1.0 and a high initial state variance: equivalent to
      efficient 'streaming' expanding window OLS.
 
     Args:
         target: The target expression.
         *features: Variable number of feature expressions.
         sample_weights: Optional expression representing sample weights.
         add_intercept: Whether to add an intercept column.
         mode: Mode of operation ("predictions", "residuals", "coefficients").
+        null_policy: Strategy for handling missing data ("zero", "drop", "ignore").
         rls_kwargs: Additional keyword arguments for the recursive least squares model.
             - "half_life": Half-life parameter for exponential forgetting. Default is None
             (no forgetting).
             Expected dtype: float or None.
             - "initial_state_covariance":
             Scalar representing which behaves like an L2 regularization parameter. Larger values
              correspond to larger prior uncertainty around mean vector of state (inversely
@@ -214,21 +261,21 @@
             - "initial_state_mean": Initial mean vector of the state.
                                     Default is zero vector.
                                     Expected dtype: List[float] or None.
 
     Returns:
         Resulting expression based on the chosen mode.
     """
-    assert mode in {
-        "predictions",
-        "residuals",
-        "coefficients",
-    }, "'mode' must be one of {predictions, residuals, coefficients}"
+    assert mode in _VALID_OUTPUT_MODES, f"'mode' must be one of '{_VALID_OUTPUT_MODES}'"
     target, features, sqrt_w = _pre_process_data(
-        target, *features, sample_weights=sample_weights, add_intercept=add_intercept
+        target,
+        *features,
+        sample_weights=sample_weights,
+        add_intercept=add_intercept,
+        null_policy=null_policy,
     )
     rls_kwargs: RLSKwargs = rls_kwargs or RLSKwargs()
 
     # register either coefficient or prediction plugin functions
     if mode == "coefficients":
         return (
             register_plugin_function(
@@ -259,43 +306,45 @@
 
 
 def compute_rolling_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
-    mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+    mode: OutputMode = "predictions",
+    null_policy: NullPolicy = "ignore",
     rolling_kwargs: Optional[RollingKwargs] = None,
 ) -> pl.Expr:
     """Performs least squares regression in a rolling window fashion.
 
     Args:
         target: The target expression.
         *features: Variable number of feature expressions.
         sample_weights: Optional expression representing sample weights.
         add_intercept: Whether to add an intercept column.
         mode: Mode of operation ("predictions", "residuals", "coefficients").
+        null_policy: Strategy for handling missing data ("zero", "drop", "ignore").
         rolling_kwargs: Additional keyword arguments for the rolling least squares model.
             - "window_size": The size of the rolling window.
             - "min_periods": The minimum number of observations required to produce estimates.
             - "use_woodbury": Whether to use Woodbury matrix identity for faster computation.
                               Defaults to True if num_features > 10.
             - "alpha": L2 Regularization strength. Default is 0.0.
                       Expected dtype: float.
 
     Returns:
         Resulting expression based on the chosen mode.
     """
-    assert mode in {
-        "predictions",
-        "residuals",
-        "coefficients",
-    }, "'mode' must be one of {predictions, residuals, coefficients}"
+    assert mode in _VALID_OUTPUT_MODES, f"'mode' must be one of '{_VALID_OUTPUT_MODES}'"
     target, features, sqrt_w = _pre_process_data(
-        target, *features, sample_weights=sample_weights, add_intercept=add_intercept
+        target,
+        *features,
+        sample_weights=sample_weights,
+        add_intercept=add_intercept,
+        null_policy=null_policy,
     )
     rolling_kwargs: RollingKwargs = rolling_kwargs or RollingKwargs()
 
     # register either coefficient or prediction plugin functions
     if mode == "coefficients":
         return (
             register_plugin_function(
@@ -324,24 +373,28 @@
         else:
             return target - predictions
 
 
 def least_squares_from_formula(
     formula: str,
     sample_weights: Optional[pl.Expr] = None,
-    mode: Literal["predictions", "residuals", "coefficients"] = "predictions",
+    mode: OutputMode = "predictions",
+    null_policy: NullPolicy = "ignore",
     **kwargs,
 ) -> pl.Expr:
     """Performs least squares regression using a formula.
 
     Depending on choice of additional kwargs dispatches either rolling, recursive,
     on static least squares compute functions.
 
     Args:
         formula: Patsy-style formula string.
+        sample_weights: Optional expression representing sample weights.
+        mode: Mode of operation ("predictions", "residuals", "coefficients").
+        null_policy: Strategy for handling missing data ("zero", "drop", "ignore").
         **kwargs: Additional keyword arguments for the least squares function.
 
     Returns:
         Resulting expression based on the formula.
     """
     expressions, add_intercept = build_expressions_from_patsy_formula(
         formula, include_dependent_variable=True
@@ -359,39 +412,41 @@
         func = partial(compute_least_squares, ols_kwargs=ols_kwargs)
 
     return func(
         expressions[0],
         *expressions[1:],
         add_intercept=add_intercept,
         sample_weights=sample_weights,
+        null_policy=null_policy,
         mode=mode,
     )
 
 
 def predict(
     coefficients: IntoExpr,
     *features: pl.Expr,
-    name: Optional[str] = None,
     add_intercept: bool = False,
+    name: Optional[str] = None,
 ) -> pl.Expr:
     """Helper which computes predictions as a product of (aligned) coefficients with features.
 
     Args:
         coefficients: Polars expression returning a coefficients struct.
         *features: variable number of feature expressions.
         add_intercept: boolean indicating if a constant should be added to features.
+        name: optional str defining an alias for computed predictions expression.
 
     Returns:
         polars expression denoting computed predictions.
     """
     if add_intercept:
         if any(f.meta.output_name == "const" for f in features):
             logger.warning("feature named 'const' already detected, assuming it is the intercept")
         else:
-            features += (features[-1].mul(0.0).add(1.0).alias("const"),)
+            features += (features[-1].fill_null(0.0).mul(0.0).add(1.0).alias("const"),)
 
     return register_plugin_function(
         plugin_path=Path(__file__).parent,
         function_name="predict",
-        args=[coefficients, *(f.cast(pl.Float32) for f in features)],
+        args=[coefficients, *(f.fill_null(0.0).cast(pl.Float32) for f in features)],
         is_elementwise=False,
     ).alias(name or "predictions")
```

### Comparing `polars_ols-0.2.3/polars_ols/utils.py` & `polars_ols-0.2.4/polars_ols/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/src/expressions.rs` & `polars_ols-0.2.4/src/expressions.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/src/least_squares.rs` & `polars_ols-0.2.4/src/least_squares.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/src/lib.rs` & `polars_ols-0.2.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/tests/benchmark.py` & `polars_ols-0.2.4/tests/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,22 +144,22 @@
 
 
 def benchmark_recursive_least_squares_statsmodels(data: pl.DataFrame):
     x = data.select(pl.all().exclude("y")).to_numpy()
     res = RecursiveLS(
         df["y"].to_numpy(),
         x,
-    ).fit(params_only=True)
+    ).fit()
     return data.lazy().with_columns(predictions=pl.lit((res.params * x).sum(1))).collect()
 
 
 if __name__ == "__main__":
     # example: python tests/benchmark.py --quiet --fast
     # we run the benchmarks in python (as opposed to rust) so that overhead of pyO3 is included
-    df = _make_data(n_features=10, n_samples=2_000)
+    df = _make_data(n_features=100, n_samples=10_000)
     runner = pyperf.Runner()
     runner.bench_func("benchmark_least_squares", benchmark_least_squares, df)
     runner.bench_func("benchmark_ridge", benchmark_ridge, df)
     runner.bench_func("benchmark_wls_from_formula", benchmark_wls_from_formula, df)
     runner.bench_func("benchmark_elastic_net", benchmark_elastic_net, df)
     runner.bench_func("benchmark_recursive_least_squares", benchmark_recursive_least_squares, df)
     runner.bench_func("benchmark_rolling_least_squares", benchmark_rolling_least_squares, df)
@@ -168,15 +168,15 @@
     # runner.bench_func("benchmark_ridge_numpy", benchmark_ridge_numpy, df)
     # runner.bench_func(
     #     "benchmark_wls_from_formula_statsmodels", benchmark_wls_from_formula_statsmodels, df
     # )
     # runner.bench_func("benchmark_elastic_net_sklearn", benchmark_elastic_net_sklearn, df)
     # runner.bench_func(
     #     "benchmark_recursive_least_squares_statsmodels",
-    #     benchmark_rolling_least_squares_statsmodels,
+    #     benchmark_recursive_least_squares_statsmodels,
     #     df,
     # )
     # runner.bench_func(
     #     "benchmark_rolling_least_squares_statsmodels",
     #     benchmark_rolling_least_squares_statsmodels,
     #     df,
     # )
```

### Comparing `polars_ols-0.2.3/tests/test_ols.py` & `polars_ols-0.2.4/tests/test_ols.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 from contextlib import contextmanager
 
 import numpy as np
 import polars as pl
+import pytest
 import statsmodels.formula.api as smf
 from sklearn.linear_model import ElasticNet
 from statsmodels.regression.rolling import RollingOLS
 
 from polars_ols import OLSKwargs, compute_least_squares, least_squares_from_formula
 
 
@@ -49,14 +50,45 @@
             x, y = df.select("x1", "x2").to_numpy(), df.select("y").to_numpy().flatten()
             coef = np.linalg.lstsq(x, y, rcond=None)[0]
             df = df.with_columns(predictions2=pl.lit(x @ coef).flatten())
 
     assert np.allclose(df["predictions"], df["predictions2"], atol=1.0e-4, rtol=1.0e-4)
 
 
+def test_fit_missing_data():
+    df = _make_data()
+    rng = np.random.default_rng(0)
+
+    def insert_nulls(val):
+        return None if rng.random() < 0.1 else val
+
+    df = df.with_columns(
+        *(pl.col(c).map_elements(insert_nulls, return_dtype=pl.Float32) for c in df.columns)
+    )
+
+    with pytest.raises(pl.exceptions.ComputeError):
+        df.select(pl.col("y").least_squares.ols(pl.col("x1"), pl.col("x2"), null_policy="ignore"))
+
+    # test zero policy is sane
+    assert np.allclose(
+        df.select(pl.col("y").least_squares.ols(pl.col("x1"), pl.col("x2"), null_policy="zero")),
+        df.fill_null(0.0).select(
+            pl.col("y").least_squares.ols(pl.col("x1"), pl.col("x2"), null_policy="ignore")
+        ),
+    )
+
+    # test drop policy is sane
+    assert np.allclose(
+        df.select(pl.col("y").least_squares.ols(pl.col("x1"), pl.col("x2"), null_policy="drop")),
+        df.drop_nulls().select(
+            pl.col("y").least_squares.ols(pl.col("x1"), pl.col("x2"), null_policy="ignore")
+        ),
+    )
+
+
 def test_coefficients_ols():
     df = _make_data()
     coef = (
         df.select(
             pl.col("y")
             .least_squares.from_formula("x1 + x2 -1", mode="coefficients")
             .alias("coefficients")
```

### Comparing `polars_ols-0.2.3/Cargo.lock` & `polars_ols-0.2.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1586,15 +1586,15 @@
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_ols"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "approx",
  "faer",
  "faer-ext",
  "jemallocator",
  "ndarray",
  "ndarray-linalg",
```

### Comparing `polars_ols-0.2.3/pyproject.toml` & `polars_ols-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.3/PKG-INFO` & `polars_ols-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-ols
-Version: 0.2.3
+Version: 0.2.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.6
 Requires-Dist: numpy ; extra == 'dev'
 Requires-Dist: pytest >=7.4.1 ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
@@ -49,14 +49,15 @@
 API & Examples
 ------------
 
 Importing `polars_ols` will register the namespace `least_squares` provided by this package.
 You can build models either by either specifying polars expressions (e.g. `pl.col(...)`) for your targets and features or using
 the formula api (patsy syntax). All models support the following general (optional) arguments:
 - `mode` - a literal which determines the type of output produced by the model
+- `null_policy` - a literal which determines how to deal with missing data
 - `add_intercept` - a boolean specifying if an intercept feature should be added to the features
 - `sample_weights` - a column or expression providing non-negative weights applied to the samples
 
 Remaining parameters are model specific, for example `alpha` penalty parameter used by regularized least squares models.
 
 See below for basic usage examples.
 Please refer to the [tests](./tests/test_ols.py) or [demo notebook](./notebooks/polars_ols_demo.ipynb) for detailed examples.
@@ -194,25 +195,25 @@
 
 | Model                   | polars_ols       | Python Benchmark  | Benchmark Type | Speed-up vs Python Benchmark |
 |-------------------------|------------------|-------------------|----------------|------------------------------|
 | Least Squares           | 283 ± 4 us       | 509 ± 313 us      | Numpy          | 1.8x                         |
 | Ridge                   | 262 ± 3 us       | 369 ± 231 us      | Numpy          | 1.4x                         |
 | Weighted Least Squares  | 493 ± 7 us       | 2.13 ms ± 0.22 ms | Statsmodels    | 4.3x                         |
 | Elastic Net             | 326 ± 3 us       | 87.3 ms ± 9.0 ms  | Sklearn        | 268.2x                       |
-| Recursive Least Squares | 1.39 ms ± 0.01 ms| 22.3 ms ± 0.2 ms  | Statsmodels    | 16.0x                        |
+| Recursive Least Squares | 1.39 ms ± 0.01 ms| 18.7 ms ± 1.4 ms  | Statsmodels    | 13.5x                        |
 | Rolling Least Squares   | 2.72 ms ± 0.03 ms| 22.3 ms ± 0.2 ms  | Statsmodels    | 8.2x                         |
 
 ### n_samples=10_000, n_features=100
-| Model                   | polars_ols       | Python Benchmark  | Benchmark Type | Speed-up vs Python Benchmark |
-|-------------------------|------------------|-------------------|----------------|------------------------------|
-| Least Squares           | 15.6 ms ± 0.2 ms| 29.9 ms ± 8.6 ms  | Numpy          | 1.9x                         |
-| Ridge                   | 5.81 ms ± 0.05 ms| 5.21 ms ± 0.94 ms | Numpy          | 0.9x                         |
-| Weighted Least Squares  | 16.8 ms ± 0.2 ms| 82.4 ms ± 9.1 ms  | Statsmodels    | 4.9x                         |
-| Elastic Net             | 20.9 ms ± 0.3 ms| 134 ms ± 21 ms    | Sklearn        | 6.4x                         |
-| Recursive Least Squares | 163 ms ± 28 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 24.5x                        |
+| Model                   | polars_ols       | Python Benchmark    | Benchmark Type | Speed-up vs Python Benchmark |
+|-------------------------|------------------|---------------------|----------------|------------------------------|
+| Least Squares           | 15.6 ms ± 0.2 ms| 29.9 ms ± 8.6 ms    | Numpy          | 1.9x                         |
+| Ridge                   | 5.81 ms ± 0.05 ms| 5.21 ms ± 0.94 ms   | Numpy          | 0.9x                         |
+| Weighted Least Squares  | 16.8 ms ± 0.2 ms| 82.4 ms ± 9.1 ms    | Statsmodels    | 4.9x                         |
+| Elastic Net             | 20.9 ms ± 0.3 ms| 134 ms ± 21 ms      | Sklearn        | 6.4x                         |
+| Recursive Least Squares | 163 ms ± 28 ms  | 65.7 sec ± 28.2 sec | Statsmodels    | 403.1x                       |
 | Rolling Least Squares   | 390 ms ± 10 ms  | 3.99 sec ± 0.54 sec | Statsmodels    | 10.2x                        |
 
 Numpy's `lstsq` is already a highly optimized call into LAPACK and so the scope for speed-up is limited.
 However, we can achieve substantial speed-ups for the more complex models by working entirely in rust
 and avoiding overhead from back and forth into python.
 
 Expect an additional relative order-of-magnitude speed up to your workflow if it involved repeated re-estimation of models in
```

