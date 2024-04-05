# Comparing `tmp/jaxonloader-0.3.0.tar.gz` & `tmp/jaxonloader-0.3.1.tar.gz`

## Comparing `jaxonloader-0.3.0.tar` & `jaxonloader-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/jaxonloader/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/jaxonloader/config.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/jaxonloader/dataset.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/jaxonloader/datasets/raw.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/tests/test_mnist.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/LICENSE
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/README.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 jaxonloader-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/config.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/datasets/raw.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/tests/test_mnist.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/README.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/PKG-INFO
```

### Comparing `jaxonloader-0.3.0/.github/workflows/nox.yaml` & `jaxonloader-0.3.1/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/docs/getting-started.md` & `jaxonloader-0.3.1/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/docs/index.md` & `jaxonloader-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/docs/images/performance.png` & `jaxonloader-0.3.1/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/jaxonloader/dataloader.py` & `jaxonloader-0.3.1/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/jaxonloader/dataset.py` & `jaxonloader-0.3.1/jaxonloader/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 class JaxonDataset(ABC):
     @abstractmethod
     def __len__(self) -> int:
         raise NotImplementedError()
 
     @abstractmethod
     def __getitem__(
-        self, idx: Int[NDArray, " batch_size"]
+        self, idx: Int[NDArray, " batch_size"] | slice
     ) -> NDArray | tuple[NDArray, ...]:
         raise NotImplementedError()
 
 
 class SingleArrayDataset(JaxonDataset):
     def __init__(self, data: NDArray):
         self.data = data
 
     def __len__(self) -> int:
         return len(self.data)
 
-    def __getitem__(self, idx: Int[NDArray, " batch_size"]) -> NDArray:
+    def __getitem__(self, idx) -> NDArray:
         return self.data[idx]
 
 
 class DataTargetDataset(JaxonDataset):
     def __init__(self, data: NDArray, target: NDArray):
         self.data = data
         self.target = target
         if len(data) != len(target):
             raise ValueError("data and target must have the same length")
 
     def __len__(self) -> int:
         return len(self.data)
 
-    def __getitem__(self, idx: Int[NDArray, " batch_size"]) -> tuple[NDArray, NDArray]:
+    def __getitem__(self, idx) -> tuple[NDArray, NDArray]:
         return self.data[idx], self.target[idx]
```

### Comparing `jaxonloader-0.3.0/jaxonloader/utils.py` & `jaxonloader-0.3.1/jaxonloader/utils.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.3.1/jaxonloader/datasets/_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             self.data = data
             self.fine_labels = np.array(fine_labels)
             self.coarse_labels = np.array(coarse_labels)
 
         def __len__(self) -> int:
             return len(self.data)
 
-        def __getitem__(self, idx: NDArray) -> tuple[NDArray, NDArray, NDArray]:
+        def __getitem__(self, idx) -> tuple[NDArray, NDArray, NDArray]:
             return self.data[idx], self.fine_labels[idx], self.coarse_labels[idx]
 
     train_dataset = CiFar100Dataset(
         train_data[b"data"], train_data[b"fine_labels"], train_data[b"coarse_labels"]
     )
     test_dataset = CiFar100Dataset(
         test_data[b"data"], test_data[b"fine_labels"], test_data[b"coarse_labels"]
```

### Comparing `jaxonloader-0.3.0/jaxonloader/datasets/raw.py` & `jaxonloader-0.3.1/jaxonloader/datasets/raw.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/tests/test_tinyshakespeare.py` & `jaxonloader-0.3.1/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/.gitignore` & `jaxonloader-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/LICENSE` & `jaxonloader-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/README.md` & `jaxonloader-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.0/pyproject.toml` & `jaxonloader-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonloader"
-version = "0.3.0"
+version = "0.3.1"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
```

### Comparing `jaxonloader-0.3.0/PKG-INFO` & `jaxonloader-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.0
+Version: 0.3.1
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

