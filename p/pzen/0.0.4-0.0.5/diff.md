# Comparing `tmp/pzen-0.0.4.tar.gz` & `tmp/pzen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzen-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pzen-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pzen-0.0.4.tar` & `pzen-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      114 2024-04-04 20:19:03.018407 pzen-0.0.4/.flake8
--rw-r--r--   0        0        0     2014 2024-04-04 20:19:03.018407 pzen-0.0.4/.github/workflows/ci.yaml
--rw-r--r--   0        0        0       26 2024-04-04 20:19:03.018407 pzen-0.0.4/.gitignore
--rw-r--r--   0        0        0     1080 2024-04-04 20:19:03.018407 pzen-0.0.4/LICENSE
--rw-r--r--   0        0        0       29 2024-04-04 20:19:03.018407 pzen-0.0.4/README.md
--rw-r--r--   0        0        0       22 2024-04-04 20:19:03.018407 pzen-0.0.4/env.sh
--rw-r--r--   0        0        0      343 2024-04-04 20:19:03.018407 pzen-0.0.4/mypy.ini
--rw-r--r--   0        0        0      317 2024-04-04 20:19:03.018407 pzen-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/__init__.py
--rw-r--r--   0        0        0     1062 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/cache_utils.py
--rw-r--r--   0        0        0       47 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/core_types.py
--rw-r--r--   0        0        0     1988 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/numpy_utils.py
--rw-r--r--   0        0        0        0 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/py.typed
--rw-r--r--   0        0        0     2072 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/soundfile_utils.py
--rw-r--r--   0        0        0       43 2024-04-04 20:19:03.018407 pzen-0.0.4/requirements_dev.txt
--rw-r--r--   0        0        0       60 2024-04-04 20:19:03.018407 pzen-0.0.4/requirements_opt.txt
--rwxr-xr-x   0        0        0      112 2024-04-04 20:19:03.018407 pzen-0.0.4/scripts/ci_all
--rwxr-xr-x   0        0        0       99 2024-04-04 20:19:03.018407 pzen-0.0.4/scripts/setup_dependencies.sh
--rwxr-xr-x   0        0        0      105 2024-04-04 20:19:03.018407 pzen-0.0.4/scripts/setup_venv.sh
--rw-r--r--   0        0        0        0 2024-04-04 20:19:03.018407 pzen-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-04 20:19:03.018407 pzen-0.0.4/tests/pzen/test_cache_utils.py
--rw-r--r--   0        0        0      911 2024-04-04 20:19:03.018407 pzen-0.0.4/tests/pzen/test_numpy_utils.py
--rw-r--r--   0        0        0      871 2024-04-04 20:19:03.018407 pzen-0.0.4/tests/pzen/test_soundfile_utils.py
--rw-r--r--   0        0        0      236 1970-01-01 00:00:00.000000 pzen-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      114 2024-04-05 21:32:54.056188 pzen-0.0.5/.flake8
+-rw-r--r--   0        0        0     2008 2024-04-05 21:32:54.060188 pzen-0.0.5/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0       26 2024-04-05 21:32:54.060188 pzen-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1080 2024-04-05 21:32:54.060188 pzen-0.0.5/LICENSE
+-rw-r--r--   0        0        0       29 2024-04-05 21:32:54.060188 pzen-0.0.5/README.md
+-rw-r--r--   0        0        0       22 2024-04-05 21:32:54.060188 pzen-0.0.5/env.sh
+-rw-r--r--   0        0        0      343 2024-04-05 21:32:54.060188 pzen-0.0.5/mypy.ini
+-rw-r--r--   0        0        0      317 2024-04-05 21:32:54.060188 pzen-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-05 21:32:54.060188 pzen-0.0.5/pzen/__init__.py
+-rw-r--r--   0        0        0     2162 2024-04-05 21:32:54.060188 pzen-0.0.5/pzen/audiofile_utils.py
+-rw-r--r--   0        0        0     1062 2024-04-05 21:32:54.060188 pzen-0.0.5/pzen/cache_utils.py
+-rw-r--r--   0        0        0       47 2024-04-05 21:32:54.060188 pzen-0.0.5/pzen/core_types.py
+-rw-r--r--   0        0        0     1988 2024-04-05 21:32:54.060188 pzen-0.0.5/pzen/numpy_utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:32:54.060188 pzen-0.0.5/pzen/py.typed
+-rw-r--r--   0        0        0      934 2024-04-05 21:32:54.060188 pzen-0.0.5/pzen/signal_utils.py
+-rw-r--r--   0        0        0       43 2024-04-05 21:32:54.060188 pzen-0.0.5/requirements_dev.txt
+-rw-r--r--   0        0        0       68 2024-04-05 21:32:54.060188 pzen-0.0.5/requirements_opt.txt
+-rwxr-xr-x   0        0        0      112 2024-04-05 21:32:54.060188 pzen-0.0.5/scripts/ci_all
+-rwxr-xr-x   0        0        0       99 2024-04-05 21:32:54.060188 pzen-0.0.5/scripts/setup_dependencies.sh
+-rwxr-xr-x   0        0        0      105 2024-04-05 21:32:54.060188 pzen-0.0.5/scripts/setup_venv.sh
+-rw-r--r--   0        0        0        0 2024-04-05 21:32:54.060188 pzen-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-05 21:32:54.060188 pzen-0.0.5/tests/pzen/test_cache_utils.py
+-rw-r--r--   0        0        0      911 2024-04-05 21:32:54.060188 pzen-0.0.5/tests/pzen/test_numpy_utils.py
+-rw-r--r--   0        0        0     1431 2024-04-05 21:32:54.060188 pzen-0.0.5/tests/pzen/test_signal_utils.py
+-rw-r--r--   0        0        0      236 1970-01-01 00:00:00.000000 pzen-0.0.5/PKG-INFO
```

### Comparing `pzen-0.0.4/.github/workflows/ci.yaml` & `pzen-0.0.5/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,17 @@
           flake8
 
       - name: Check format
         run: |
           black --check .
           isort --check .
 
-      # - name: Tests
-      #   run: |
-      #     pytest
+      - name: Tests
+        run: |
+          pytest
 
 
   deploy-pypi:
 
     needs: tests
 
     runs-on: ubuntu-latest
```

### Comparing `pzen-0.0.4/LICENSE` & `pzen-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pzen-0.0.4/pzen/cache_utils.py` & `pzen-0.0.5/pzen/cache_utils.py`

 * *Files identical despite different names*

### Comparing `pzen-0.0.4/pzen/numpy_utils.py` & `pzen-0.0.5/pzen/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pzen-0.0.4/pzen/soundfile_utils.py` & `pzen-0.0.5/pzen/audiofile_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,40 @@
 from pathlib import Path
 from typing import Literal
 
+import librosa
 import numpy as np
 import soundfile
 import torch
 
+from .cache_utils import with_memory
 from .core_types import StrPath
+from .signal_utils import normalize, normalize_min_max
+
+
+@with_memory
+def load_resampled(
+    path: StrPath,
+    sr: int,
+    offset_sec: float = 0.0,
+    duration_sec: float | None = None,
+    duration_samples: int | None = None,
+) -> np.ndarray:
+    """
+    Wrapper around librosa.load (because resampling can be somewhat slow, and I prefer
+    the more explicit caching approach).
+    """
+    print(f"Loading audio from '{path}'...")
+    signal, sampling_rate_loaded = librosa.load(
+        path, sr=sr, offset=offset_sec, duration=duration_sec
+    )
+    assert sampling_rate_loaded == sr
+    if duration_samples is not None:
+        signal = signal[:duration_samples]
+    return signal
 
 
 def soundfile_write(
     path: StrPath,
     data: np.ndarray | torch.Tensor,
     sr: int,
     *,
@@ -45,34 +70,7 @@
             if clip == "error":
                 raise ValueError(msg)
             elif clip == "warn":
                 print(f"WARNING: {msg}")
 
     Path(path).parent.mkdir(exist_ok=True, parents=True)
     soundfile.write(str(path), data, sr)
-
-
-def normalize(array: np.ndarray) -> np.ndarray:
-    """
-    Normalize signal to stay within [-1, +1], but leave the zero point unmodified.
-    """
-    abs_max = np.abs(array).max()
-    if abs_max != 0:
-        return array / abs_max
-    else:
-        return array
-
-
-def normalize_min_max(array: np.ndarray) -> np.ndarray:
-    """
-    This function normalizes the min/max to [-1, +1].
-
-    Note that this can be a bit confusing, because it may look like the output has a constant
-    DC-offset.
-    """
-    max = array.max()
-    min = array.min()
-
-    if max > min:
-        return -1.0 + (array - min) / (max - min) * 2
-    else:
-        return array
```

### Comparing `pzen-0.0.4/tests/pzen/test_cache_utils.py` & `pzen-0.0.5/tests/pzen/test_cache_utils.py`

 * *Files identical despite different names*

### Comparing `pzen-0.0.4/tests/pzen/test_numpy_utils.py` & `pzen-0.0.5/tests/pzen/test_numpy_utils.py`

 * *Files identical despite different names*

