# Comparing `tmp/fpsample-0.3.1.tar.gz` & `tmp/fpsample-0.3.2.tar.gz`

## Comparing `fpsample-0.3.1.tar` & `fpsample-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 fpsample-0.3.1/Cargo.toml
--rw-r--r--   0     1001      127     2767 2023-09-19 08:01:06.000000 fpsample-0.3.1/.github/workflows/release.yml
--rw-r--r--   0     1001      127     2189 2023-09-19 08:01:06.000000 fpsample-0.3.1/.github/workflows/test.yml
--rw-r--r--   0     1001      127      740 2023-09-19 08:01:06.000000 fpsample-0.3.1/.gitignore
--rw-r--r--   0     1001      127      508 2023-09-19 08:01:06.000000 fpsample-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1065 2023-09-19 08:01:06.000000 fpsample-0.3.1/LICENSE
--rw-r--r--   0     1001      127     7469 2023-09-19 08:01:06.000000 fpsample-0.3.1/README.md
--rw-r--r--   0     1001      127     6515 2023-09-19 08:01:06.000000 fpsample-0.3.1/bench/test_bench.py
--rw-r--r--   0     1001      127      515 2023-09-19 08:01:06.000000 fpsample-0.3.1/build.rs
--rw-r--r--   0     1001      127       41 2023-09-19 08:01:06.000000 fpsample-0.3.1/build_info.rs
--rw-r--r--   0     1001      127      934 2023-09-19 08:01:06.000000 fpsample-0.3.1/pyproject.toml
--rw-r--r--   0     1001      127       23 2023-09-19 08:01:06.000000 fpsample-0.3.1/python/fpsample/__init__.py
--rw-r--r--   0     1001      127     5052 2023-09-19 08:01:06.000000 fpsample-0.3.1/python/fpsample/wrapper.py
--rw-r--r--   0     1001      127       59 2023-09-19 08:01:06.000000 fpsample-0.3.1/requirements.txt
--rw-r--r--   0     1001      127      529 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/_ext/Interval.h
--rw-r--r--   0     1001      127     2600 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/_ext/KDLineTree.h
--rw-r--r--   0     1001      127     6063 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/_ext/KDNode.h
--rw-r--r--   0     1001      127     1547 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/_ext/KDTree.h
--rw-r--r--   0     1001      127     6614 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/_ext/KDTreeBase.h
--rw-r--r--   0     1001      127     2820 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/_ext/Point.h
--rw-r--r--   0     1001      127      474 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/_ext/utils.h
--rw-r--r--   0     1001      127     4712 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/c_wrapper.cpp
--rw-r--r--   0     1001      127      589 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/ffi.rs
--rw-r--r--   0     1001      127     1478 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/bucket_fps/mod.rs
--rw-r--r--   0     1001      127    11347 2023-09-19 08:01:06.000000 fpsample-0.3.1/src/lib.rs
--rw-r--r--   0     1001      127    10779 2023-09-19 08:01:06.000000 fpsample-0.3.1/Cargo.lock
--rw-r--r--   0        0        0     8135 1970-01-01 00:00:00.000000 fpsample-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 fpsample-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      127     2767 2024-04-05 13:06:34.000000 fpsample-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     2189 2024-04-05 13:06:34.000000 fpsample-0.3.2/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      740 2024-04-05 13:06:34.000000 fpsample-0.3.2/.gitignore
+-rw-r--r--   0     1001      127      508 2024-04-05 13:06:34.000000 fpsample-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1065 2024-04-05 13:06:34.000000 fpsample-0.3.2/LICENSE
+-rw-r--r--   0     1001      127     7781 2024-04-05 13:06:34.000000 fpsample-0.3.2/README.md
+-rw-r--r--   0     1001      127     6515 2024-04-05 13:06:34.000000 fpsample-0.3.2/bench/test_bench.py
+-rw-r--r--   0     1001      127      515 2024-04-05 13:06:34.000000 fpsample-0.3.2/build.rs
+-rw-r--r--   0     1001      127       41 2024-04-05 13:06:34.000000 fpsample-0.3.2/build_info.rs
+-rw-r--r--   0     1001      127       23 2024-04-05 13:06:34.000000 fpsample-0.3.2/python/fpsample/__init__.py
+-rw-r--r--   0     1001      127     6621 2024-04-05 13:06:34.000000 fpsample-0.3.2/python/fpsample/wrapper.py
+-rw-r--r--   0     1001      127       59 2024-04-05 13:06:34.000000 fpsample-0.3.2/requirements.txt
+-rw-r--r--   0     1001      127      529 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/_ext/Interval.h
+-rw-r--r--   0     1001      127     2600 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/_ext/KDLineTree.h
+-rw-r--r--   0     1001      127     6063 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/_ext/KDNode.h
+-rw-r--r--   0     1001      127     1547 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/_ext/KDTree.h
+-rw-r--r--   0     1001      127     6614 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/_ext/KDTreeBase.h
+-rw-r--r--   0     1001      127     2820 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/_ext/Point.h
+-rw-r--r--   0     1001      127      474 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/_ext/utils.h
+-rw-r--r--   0     1001      127     4712 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/c_wrapper.cpp
+-rw-r--r--   0     1001      127      589 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/ffi.rs
+-rw-r--r--   0     1001      127     1478 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/bucket_fps/mod.rs
+-rw-r--r--   0     1001      127    11347 2024-04-05 13:06:34.000000 fpsample-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      127    10779 2024-04-05 13:06:34.000000 fpsample-0.3.2/Cargo.lock
+-rw-r--r--   0     1001      127      934 2024-04-05 13:06:34.000000 fpsample-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8447 1970-01-01 00:00:00.000000 fpsample-0.3.2/PKG-INFO
```

### Comparing `fpsample-0.3.1/.github/workflows/release.yml` & `fpsample-0.3.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/.github/workflows/test.yml` & `fpsample-0.3.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/.gitignore` & `fpsample-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/LICENSE` & `fpsample-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/README.md` & `fpsample-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,27 @@
 
 * `FPS`: Vanilla farthest point sampling. Implemented in Rust. Achieve the same performance as `numpy`.
 * `FPS + NPDU`: Farthest point sampling with nearest-point-distance-updating (NPDU) heuristic strategy. 5x~10x faster than vanilla FPS. **Require dimensional locality and give sub-optimal answers**.
 * `FPS + NPDU + KDTree`: Farthest point sampling with NPDU heuristic strategy and KDTree. 3x~8x faster than vanilla FPS. Slightly slower than `FPS + NPDU`. But **DOES NOT** require dimensional locality.
 * `KDTree-based FPS`: A farthest point sampling algorithm based on KDTree. About 40~50x faster than vanilla FPS.
 * `Bucket-based FPS` or `QuickFPS`: A bucket-based farthest point sampling algorithm. About 80~100x faster than vanilla FPS. Require an additional hyperparameter for the height of the KDTree. In practice, `h=3` or `h=5` is recommended for small data, `h=7` is recommended for medium data, and `h=9` for extremely large data.
 
-**NOTE**: In most cases, `Bucket-based FPS` is the best choice, with proper hyperparameter setting.
+> **NOTE**: In most cases, `Bucket-based FPS` is the best choice, with proper hyperparameter setting.
+
+### Determinism
+
+For deterministic results, fix the first sampled point index by passing the `start_idx` parameter.
+```python
+kdline_fps_samples_idx = fpsample.bucket_fps_kdline_sampling(pc, 1024, h=3, start_idx=0)
+```
+
+**OR** set the random seed before calling the function.
+```python
+np.random.seed(42)
+```
 
 ## Performance
 Setup:
   - CPU: Intel(R) Core(TM) i9-10940X CPU @ 3.30GHz
   - RAM: 128 GiB
   - SYSTEM: Ubuntu 22.04.3 LTS
```

### Comparing `fpsample-0.3.1/bench/test_bench.py` & `fpsample-0.3.2/bench/test_bench.py`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/build.rs` & `fpsample-0.3.2/build.rs`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/pyproject.toml` & `fpsample-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.2,<2.0", "patchelf>=0.17"]
 build-backend = "maturin"
 
 [project]
 name = "fpsample"
-version = "0.3.1"
+version = "0.3.2"
 authors = [{ name = "Leonard Lin", email = "leonard.keilin@gmail.com" }]
 keyword = [
     "sampling",
     "farthest point sampling",
     "furthest point sampling",
     "point cloud",
 ]
```

### Comparing `fpsample-0.3.1/python/fpsample/wrapper.py` & `fpsample-0.3.2/python/fpsample/wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,127 +8,155 @@
     _bucket_fps_kdtree_sampling,
     _fps_npdu_kdtree_sampling,
     _fps_npdu_sampling,
     _fps_sampling,
 )
 
 
-def fps_sampling(pc: np.ndarray, n_samples: int) -> np.ndarray:
+def fps_sampling(pc: np.ndarray, n_samples: int, start_idx: Optional[int] = None) -> np.ndarray:
     """
     Vanilla FPS sampling.
 
     Args:
         pc (np.ndarray): The input point cloud of shape (n_pts, D).
         n_samples (int): Number of samples.
+        start_idx (int, default=None): The starting index of sampling. If set to None, it will be randomly picked.
     Returns:
         np.ndarray: The selected indices of shape (n_samples,).
     """
     assert n_samples >= 1, "n_samples should be >= 1"
     assert pc.ndim == 2
     n_pts, _ = pc.shape
     assert n_pts >= n_samples, "n_pts should be >= n_samples"
+    assert (
+        start_idx is None or 0 <= start_idx < n_pts
+    ), "start_idx should be None or 0 <= start_idx < n_pts"
     pc = pc.astype(np.float32)
     # best performance with fortran array
     pc = np.asfortranarray(pc)
     # Random pick a start
-    start_idx = np.random.randint(low=0, high=n_pts)
+    start_idx = np.random.randint(low=0, high=n_pts) if start_idx is None else start_idx
     return _fps_sampling(pc, n_samples, start_idx)
 
 
-def fps_npdu_sampling(pc: np.ndarray, n_samples: int, w: Optional[int] = None) -> np.ndarray:
+def fps_npdu_sampling(
+    pc: np.ndarray, n_samples: int, w: Optional[int] = None, start_idx: Optional[int] = None
+) -> np.ndarray:
     """
     FPS sampling with nearest-point-distance-updating (NPDU) heuristic strategy.
     **Requires dimensional locality for best samples**.
 
     Args:
         pc (np.ndarray): The input point cloud of shape (n_pts, D).
         n_samples (int): Number of samples.
         w (int, default=None): Windows size of local heuristic search. If set to None, it will be set to `n_pts / n_samples * 16`.
+        start_idx (int, default=None): The starting index of sampling. If set to None, it will be randomly picked.
     Returns:
         np.ndarray: The selected indices of shape (n_samples,).
     """
     assert n_samples >= 1, "n_samples should be >= 1"
     assert pc.ndim == 2
     n_pts, _ = pc.shape
     assert n_pts >= n_samples, "n_pts should be >= n_samples"
+    assert (
+        start_idx is None or 0 <= start_idx < n_pts
+    ), "start_idx should be None or 0 <= start_idx < n_pts"
     pc = pc.astype(np.float32)
     w = w or int(n_pts / n_samples * 16)
     if w >= n_pts - 1:
         warnings.warn(f"k is too large, set to {n_pts - 1}")
         w = n_pts - 1
     # Random pick a start
-    start_idx = np.random.randint(low=0, high=n_pts)
+    start_idx = np.random.randint(low=0, high=n_pts) if start_idx is None else start_idx
     return _fps_npdu_sampling(pc, n_samples, w, start_idx)
 
 
-def fps_npdu_kdtree_sampling(pc: np.ndarray, n_samples: int, w: Optional[int] = None) -> np.ndarray:
+def fps_npdu_kdtree_sampling(
+    pc: np.ndarray, n_samples: int, w: Optional[int] = None, start_idx: Optional[int] = None
+) -> np.ndarray:
     """
     FPS sampling with nearest-point-distance-updating (NPDU) heuristic strategy.
     Using KDTree to eliminate the need of dimensional locality.
     Slower than `fps_npdu_sampling` but more robust.
 
     Args:
         pc (np.ndarray): The input point cloud of shape (n_pts, D).
         n_samples (int): Number of samples.
         w (int, default=None): Windows size of local heuristic search. If set to None, it will be set to `n_pts / n_samples * 16`.
+        start_idx (int, default=None): The starting index of sampling. If set to None, it will be randomly picked.
     Returns:
         np.ndarray: The selected indices of shape (n_samples,).
     """
     assert n_samples >= 1, "n_samples should be >= 1"
     assert pc.ndim == 2
     n_pts, _ = pc.shape
     assert n_pts >= n_samples, "n_pts should be >= n_samples"
+    assert (
+        start_idx is None or 0 <= start_idx < n_pts
+    ), "start_idx should be None or 0 <= start_idx < n_pts"
     pc = pc.astype(np.float32)
     w = w or int(n_pts / n_samples * 16)
     if w >= n_pts:
         warnings.warn(f"k is too large, set to {n_pts}")
         w = n_pts
     # Random pick a start
-    start_idx = np.random.randint(low=0, high=n_pts)
+    start_idx = np.random.randint(low=0, high=n_pts) if start_idx is None else start_idx
     return _fps_npdu_kdtree_sampling(pc, n_samples, w, start_idx)
 
 
-def bucket_fps_kdtree_sampling(pc: np.ndarray, n_samples: int) -> np.ndarray:
+def bucket_fps_kdtree_sampling(
+    pc: np.ndarray, n_samples: int, start_idx: Optional[int] = None
+) -> np.ndarray:
     """
     Bucket-based FPS sampling using KDTree. Also called "QuickFPS" in the paper.
 
     Args:
         pc (np.ndarray): The input point cloud of shape (n_pts, D).
         n_samples (int): Number of samples.
         k (int, default=None): Windows size of local heuristic search. If set to None, it will be set to `n_pts / n_samples * 16`.
+        start_idx (int, default=None): The starting index of sampling. If set to None, it will be randomly picked.
     Returns:
         np.ndarray: The selected indices of shape (n_samples,).
     """
     assert n_samples >= 1, "n_samples should be >= 1"
     assert pc.ndim == 2
     n_pts, _ = pc.shape
     assert n_pts >= n_samples, "n_pts should be >= n_samples"
+    assert (
+        start_idx is None or 0 <= start_idx < n_pts
+    ), "start_idx should be None or 0 <= start_idx < n_pts"
     pc = pc.astype(np.float32)
     # Random pick a start
-    start_idx = np.random.randint(low=0, high=n_pts)
+    start_idx = np.random.randint(low=0, high=n_pts) if start_idx is None else start_idx
     return _bucket_fps_kdtree_sampling(pc, n_samples, start_idx)
 
 
-def bucket_fps_kdline_sampling(pc: np.ndarray, n_samples: int, h: int) -> np.ndarray:
+def bucket_fps_kdline_sampling(
+    pc: np.ndarray, n_samples: int, h: int, start_idx: Optional[int] = None
+) -> np.ndarray:
     """
     Bucket-based FPS sampling using KDTree, with multiple points in each bucket. Also called "QuickFPS" in the paper.
 
     Args:
         pc (np.ndarray): The input point cloud of shape (n_pts, D).
         n_samples (int): Number of samples.
         h (int, default=None): Height of KDTree. The bucket size is `2**h`.
             According to the paper, for small workload, h=3 is enough;
             for medium workload, h=7 is enough; for large workload, h=9 is enough.
+        start_idx (int, default=None): The starting index of sampling. If set to None, it will be randomly picked.
 
     Returns:
         np.ndarray: The selected indices of shape (n_samples,).
     """
     assert n_samples >= 1, "n_samples should be >= 1"
     assert pc.ndim == 2
     n_pts, _ = pc.shape
     assert n_pts >= n_samples, "n_pts should be >= n_samples"
     assert h >= 1, "h should be >= 1"
     assert 2**h <= n_pts, "2**h should be <= n_pts"
+    assert (
+        start_idx is None or 0 <= start_idx < n_pts
+    ), "start_idx should be None or 0 <= start_idx < n_pts"
     pc = pc.astype(np.float32)
     # Random pick a start
-    start_idx = np.random.randint(low=0, high=n_pts)
+    start_idx = np.random.randint(low=0, high=n_pts) if start_idx is None else start_idx
     return _bucket_fps_kdline_sampling(pc, n_samples, h, start_idx)
```

### Comparing `fpsample-0.3.1/src/bucket_fps/_ext/Interval.h` & `fpsample-0.3.2/src/bucket_fps/_ext/Interval.h`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/bucket_fps/_ext/KDLineTree.h` & `fpsample-0.3.2/src/bucket_fps/_ext/KDLineTree.h`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/bucket_fps/_ext/KDNode.h` & `fpsample-0.3.2/src/bucket_fps/_ext/KDNode.h`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/bucket_fps/_ext/KDTree.h` & `fpsample-0.3.2/src/bucket_fps/_ext/KDTree.h`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/bucket_fps/_ext/KDTreeBase.h` & `fpsample-0.3.2/src/bucket_fps/_ext/KDTreeBase.h`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/bucket_fps/_ext/Point.h` & `fpsample-0.3.2/src/bucket_fps/_ext/Point.h`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/bucket_fps/c_wrapper.cpp` & `fpsample-0.3.2/src/bucket_fps/c_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/bucket_fps/ffi.rs` & `fpsample-0.3.2/src/bucket_fps/ffi.rs`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/bucket_fps/mod.rs` & `fpsample-0.3.2/src/bucket_fps/mod.rs`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/src/lib.rs` & `fpsample-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fpsample-0.3.1/Cargo.lock` & `fpsample-0.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 name = "cty"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b365fabc795046672053e29c954733ec3b05e4be654ab130fe8f1f94d7051f35"
 
 [[package]]
 name = "fpsample"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "cc",
  "cty",
  "kdtree",
  "numpy",
  "pyo3",
 ]
```

### Comparing `fpsample-0.3.1/PKG-INFO` & `fpsample-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fpsample
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Summary: An efficient CPU implementation of farthest point sampling (FPS) for point clouds.
 Author-email: Leonard Lin <leonard.keilin@gmail.com>
@@ -96,15 +96,27 @@
 
 * `FPS`: Vanilla farthest point sampling. Implemented in Rust. Achieve the same performance as `numpy`.
 * `FPS + NPDU`: Farthest point sampling with nearest-point-distance-updating (NPDU) heuristic strategy. 5x~10x faster than vanilla FPS. **Require dimensional locality and give sub-optimal answers**.
 * `FPS + NPDU + KDTree`: Farthest point sampling with NPDU heuristic strategy and KDTree. 3x~8x faster than vanilla FPS. Slightly slower than `FPS + NPDU`. But **DOES NOT** require dimensional locality.
 * `KDTree-based FPS`: A farthest point sampling algorithm based on KDTree. About 40~50x faster than vanilla FPS.
 * `Bucket-based FPS` or `QuickFPS`: A bucket-based farthest point sampling algorithm. About 80~100x faster than vanilla FPS. Require an additional hyperparameter for the height of the KDTree. In practice, `h=3` or `h=5` is recommended for small data, `h=7` is recommended for medium data, and `h=9` for extremely large data.
 
-**NOTE**: In most cases, `Bucket-based FPS` is the best choice, with proper hyperparameter setting.
+> **NOTE**: In most cases, `Bucket-based FPS` is the best choice, with proper hyperparameter setting.
+
+### Determinism
+
+For deterministic results, fix the first sampled point index by passing the `start_idx` parameter.
+```python
+kdline_fps_samples_idx = fpsample.bucket_fps_kdline_sampling(pc, 1024, h=3, start_idx=0)
+```
+
+**OR** set the random seed before calling the function.
+```python
+np.random.seed(42)
+```
 
 ## Performance
 Setup:
   - CPU: Intel(R) Core(TM) i9-10940X CPU @ 3.30GHz
   - RAM: 128 GiB
   - SYSTEM: Ubuntu 22.04.3 LTS
```

