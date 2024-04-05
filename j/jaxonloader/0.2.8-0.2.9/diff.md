# Comparing `tmp/jaxonloader-0.2.8.tar.gz` & `tmp/jaxonloader-0.2.9.tar.gz`

## Comparing `jaxonloader-0.2.8.tar` & `jaxonloader-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/mkdocs.yml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/images/performance.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/__init__.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/dataset.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/utils.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/datasets/raw.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/tests/test_mnist.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/LICENSE
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/README.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/mkdocs.yml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/docs/images/performance.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/jaxonloader/config.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/jaxonloader/utils.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/jaxonloader/datasets/raw.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/tests/test_mnist.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/README.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 jaxonloader-0.2.9/PKG-INFO
```

### Comparing `jaxonloader-0.2.8/.github/workflows/nox.yaml` & `jaxonloader-0.2.9/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/docs/getting-started.md` & `jaxonloader-0.2.9/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/docs/index.md` & `jaxonloader-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/docs/images/performance.png` & `jaxonloader-0.2.9/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/jaxonloader/dataloader.py` & `jaxonloader-0.2.9/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/jaxonloader/dataset.py` & `jaxonloader-0.2.9/jaxonloader/dataset.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/jaxonloader/utils.py` & `jaxonloader-0.2.9/jaxonloader/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from functools import wraps
 from typing import Any
 
 import progressbar
 from loguru import logger
 from numpy.random import default_rng
 
+from jaxonloader.config import JAXONLOADER_PATH
 
-JAXONLOADER_PATH = pathlib.Path.home() / ".jaxonloader"
 
 pbar = None
 
 
 def _make_jaxonloader_dir_if_not_exists():
     if not os.path.exists(JAXONLOADER_PATH):
         os.makedirs(JAXONLOADER_PATH)
```

### Comparing `jaxonloader-0.2.8/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.2.9/jaxonloader/datasets/_datasets.py`

 * *Files 9% similar despite different names*

```diff
@@ -181,14 +181,29 @@
     y_test = np.roll(x_test, -1)
     test_data = np.concatenate((x_test, y_test), axis=1)
     test_dataset = SingleArrayDataset(test_data)
 
     return train_dataset, test_dataset, vocab_size, encoder, decoder
 
 
+@jaxonloader_cache(dataset_name="titanic")
+def get_titanic():
+    data_url = "https://omnisium.eu-central-1.linodeobjects.com/titanic/titanic.zip"
+    data_path = pathlib.Path(JAXONLOADER_PATH) / "titanic"
+    download_and_extract_zip(data_url, data_path)
+
+    train = pd.read_csv(data_path / "train.csv").to_numpy()
+    test = pd.read_csv(data_path / "test.csv").to_numpy()
+
+    train_dataset = SingleArrayDataset(train)
+    test_dataset = SingleArrayDataset(test)
+
+    return train_dataset, test_dataset
+
+
 def from_dataframe(dataframe: pl.DataFrame | pd.DataFrame) -> JaxonDataset:
     """
     Convert a polars.DataFrame (or pandas.DataFrame) to a JaxonDataset.
 
     Args:
     dataframe: A polars.DataFrame (or pandas.DataFrame).
```

### Comparing `jaxonloader-0.2.8/jaxonloader/datasets/raw.py` & `jaxonloader-0.2.9/jaxonloader/datasets/raw.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/tests/test_tinyshakespeare.py` & `jaxonloader-0.2.9/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/.gitignore` & `jaxonloader-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/LICENSE` & `jaxonloader-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/README.md` & `jaxonloader-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.8/pyproject.toml` & `jaxonloader-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonloader"
-version = "0.2.8"
+version = "0.2.9"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
```

### Comparing `jaxonloader-0.2.8/PKG-INFO` & `jaxonloader-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.2.8
+Version: 0.2.9
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

