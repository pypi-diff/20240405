# Comparing `tmp/jaxonloader-0.3.1.tar.gz` & `tmp/jaxonloader-0.3.2.tar.gz`

## Comparing `jaxonloader-0.3.1.tar` & `jaxonloader-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/mkdocs.yml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/config.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/dataset.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/jaxonloader/datasets/raw.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/tests/test_mnist.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/LICENSE
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/README.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 jaxonloader-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/mkdocs.yml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/config.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/datasets/raw.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/tests/test_mnist.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/tests/test_slicing.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/README.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/PKG-INFO
```

### Comparing `jaxonloader-0.3.1/.github/workflows/nox.yaml` & `jaxonloader-0.3.2/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/docs/getting-started.md` & `jaxonloader-0.3.2/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/docs/index.md` & `jaxonloader-0.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/docs/images/performance.png` & `jaxonloader-0.3.2/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/jaxonloader/dataloader.py` & `jaxonloader-0.3.2/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/jaxonloader/dataset.py` & `jaxonloader-0.3.2/jaxonloader/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from abc import ABC, abstractmethod
+from typing import Union
 
 from jaxtyping import Int
 from numpy import ndarray as NDArray
 
 
 class JaxonDataset(ABC):
     @abstractmethod
     def __len__(self) -> int:
         raise NotImplementedError()
 
     @abstractmethod
     def __getitem__(
         self, idx: Int[NDArray, " batch_size"] | slice
-    ) -> NDArray | tuple[NDArray, ...]:
+    ) -> Union[NDArray, tuple[NDArray, ...], "JaxonDataset"]:
         raise NotImplementedError()
 
 
 class SingleArrayDataset(JaxonDataset):
     def __init__(self, data: NDArray):
         self.data = data
 
     def __len__(self) -> int:
         return len(self.data)
 
-    def __getitem__(self, idx) -> NDArray:
+    def __getitem__(self, idx):
         return self.data[idx]
 
 
 class DataTargetDataset(JaxonDataset):
     def __init__(self, data: NDArray, target: NDArray):
         self.data = data
         self.target = target
         if len(data) != len(target):
             raise ValueError("data and target must have the same length")
 
     def __len__(self) -> int:
         return len(self.data)
 
-    def __getitem__(self, idx) -> tuple[NDArray, NDArray]:
-        return self.data[idx], self.target[idx]
+    def __getitem__(self, idx):
+        if isinstance(idx, slice):
+            return DataTargetDataset(self.data[idx], self.target[idx])
+        else:
+            return self.data[idx], self.target[idx]
```

### Comparing `jaxonloader-0.3.1/jaxonloader/utils.py` & `jaxonloader-0.3.2/jaxonloader/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,9 +88,7 @@
         urllib.request.urlretrieve(url, data_path / "temp.zip", show_progress)
         with zipfile.ZipFile(data_path / "temp.zip", "r") as zip_ref:
             logger.info(f"Extracting the dataset to {data_path}")
             zip_ref.extractall(data_path)
         os.remove(data_path / "temp.zip")
         if os.path.exists(data_path / "__MACOSX"):
             shutil.rmtree(data_path / "__MACOSX")
-    else:
-        logger.info(f"Dataset already exists in {data_path}")
```

### Comparing `jaxonloader-0.3.1/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.3.2/jaxonloader/datasets/_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,15 @@
     data_url = "https://omnisium.eu-central-1.linodeobjects.com/titanic/titanic.zip"
     data_path = pathlib.Path(JAXONLOADER_PATH) / "titanic"
     download_and_extract_zip(data_url, data_path)
     train_df = pl.read_csv(data_path / "train.csv")
 
     def _gender_to_int(df: pl.DataFrame) -> pl.DataFrame:
         df = df.with_columns(
-            pl.col("Sex")
-            .apply(lambda gender: 0 if gender == "male" else 1)
-            .alias("Sex")
+            pl.when(pl.col("Sex") == "male").then(0).otherwise(1).alias("Sex")
         )
         return df
 
     train = _gender_to_int(train_df)
     train_data = train.select(pl.exclude("Survived")).to_numpy()
     train_target = train.select(pl.col("Survived")).to_numpy()
```

### Comparing `jaxonloader-0.3.1/jaxonloader/datasets/raw.py` & `jaxonloader-0.3.2/jaxonloader/datasets/raw.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/tests/test_tinyshakespeare.py` & `jaxonloader-0.3.2/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/.gitignore` & `jaxonloader-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/LICENSE` & `jaxonloader-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.1/README.md` & `jaxonloader-0.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Jaxonloader
 
 A dataloader that no one asked for, but here it is anyway.
 
+## Attention!
+
+This package is still in heavy development! There will be no backwards compatibility until version 1.0.0 is released and the API can/will change at any time without warning.
+
 ## Documentation
 
 Check out the docs [here](https://artur-galstyan.github.io/jaxonloader/)
 
 ## Installation
 
 Install this package using pip like so:
```

### Comparing `jaxonloader-0.3.1/pyproject.toml` & `jaxonloader-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonloader"
-version = "0.3.1"
+version = "0.3.2"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
```

### Comparing `jaxonloader-0.3.1/PKG-INFO` & `jaxonloader-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.1
+Version: 0.3.2
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,18 @@
 Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Jaxonloader
 
 A dataloader that no one asked for, but here it is anyway.
 
+## Attention!
+
+This package is still in heavy development! There will be no backwards compatibility until version 1.0.0 is released and the API can/will change at any time without warning.
+
 ## Documentation
 
 Check out the docs [here](https://artur-galstyan.github.io/jaxonloader/)
 
 ## Installation
 
 Install this package using pip like so:
```

