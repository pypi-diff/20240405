# Comparing `tmp/jaxonloader-0.3.2.tar.gz` & `tmp/jaxonloader-0.3.3.tar.gz`

## Comparing `jaxonloader-0.3.2.tar` & `jaxonloader-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/mkdocs.yml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/config.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/dataset.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/jaxonloader/datasets/raw.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/tests/test_mnist.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/tests/test_slicing.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/README.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 jaxonloader-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/mkdocs.yml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/jaxonloader/config.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/jaxonloader/datasets/raw.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/tests/test_mnist.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/tests/test_slicing.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/README.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 jaxonloader-0.3.3/PKG-INFO
```

### Comparing `jaxonloader-0.3.2/.github/workflows/nox.yaml` & `jaxonloader-0.3.3/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/docs/getting-started.md` & `jaxonloader-0.3.3/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/docs/index.md` & `jaxonloader-0.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/docs/images/performance.png` & `jaxonloader-0.3.3/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/jaxonloader/dataloader.py` & `jaxonloader-0.3.3/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/jaxonloader/dataset.py` & `jaxonloader-0.3.3/jaxonloader/dataset.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/jaxonloader/utils.py` & `jaxonloader-0.3.3/jaxonloader/utils.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.3.3/jaxonloader/datasets/_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,27 @@
 
     def _gender_to_int(df: pl.DataFrame) -> pl.DataFrame:
         df = df.with_columns(
             pl.when(pl.col("Sex") == "male").then(0).otherwise(1).alias("Sex")
         )
         return df
 
+    def _embarked_to_int(df: pl.DataFrame) -> pl.DataFrame:
+        df = df.with_columns(
+            pl.when(pl.col("Embarked") == "S")
+            .then(0)
+            .when(pl.col("Embarked") == "C")
+            .then(1)
+            .otherwise(2)
+            .alias("Embarked")
+        )
+        return df
+
     train = _gender_to_int(train_df)
+    train = _embarked_to_int(train)
     train_data = train.select(pl.exclude("Survived")).to_numpy()
     train_target = train.select(pl.col("Survived")).to_numpy()
 
     train_dataset = DataTargetDataset(train_data, train_target)
 
     return train_dataset
```

### Comparing `jaxonloader-0.3.2/jaxonloader/datasets/raw.py` & `jaxonloader-0.3.3/jaxonloader/datasets/raw.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/tests/test_slicing.py` & `jaxonloader-0.3.3/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/tests/test_tinyshakespeare.py` & `jaxonloader-0.3.3/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/.gitignore` & `jaxonloader-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/LICENSE` & `jaxonloader-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/README.md` & `jaxonloader-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.2/pyproject.toml` & `jaxonloader-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonloader"
-version = "0.3.2"
+version = "0.3.3"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
```

### Comparing `jaxonloader-0.3.2/PKG-INFO` & `jaxonloader-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.2
+Version: 0.3.3
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

