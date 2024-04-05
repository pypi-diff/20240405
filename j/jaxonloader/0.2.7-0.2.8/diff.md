# Comparing `tmp/jaxonloader-0.2.7.tar.gz` & `tmp/jaxonloader-0.2.8.tar.gz`

## Comparing `jaxonloader-0.2.7.tar` & `jaxonloader-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/mkdocs.yml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/images/performance.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/__init__.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/dataset.py
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/datasets.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/utils.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/tests/test_mnist.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/LICENSE
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/README.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/mkdocs.yml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/docs/images/performance.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/__init__.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/utils.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/jaxonloader/datasets/raw.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/tests/test_mnist.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/README.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 jaxonloader-0.2.8/PKG-INFO
```

### Comparing `jaxonloader-0.2.7/.github/workflows/nox.yaml` & `jaxonloader-0.2.8/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/docs/getting-started.md` & `jaxonloader-0.2.8/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/docs/index.md` & `jaxonloader-0.2.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/docs/images/performance.png` & `jaxonloader-0.2.8/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/jaxonloader/dataloader.py` & `jaxonloader-0.2.8/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/jaxonloader/dataset.py` & `jaxonloader-0.2.8/jaxonloader/dataset.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/jaxonloader/datasets.py` & `jaxonloader-0.2.8/jaxonloader/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/jaxonloader/utils.py` & `jaxonloader-0.2.8/jaxonloader/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,24 @@
     if downloaded < total_size:
         pbar.update(downloaded)
     else:
         pbar.finish()
         pbar = None
 
 
+def download(url: str, data_path: pathlib.Path) -> None:
+    if not os.path.exists(data_path):
+        os.makedirs(data_path)
+    file_name = url.split("/")[-1]
+    logger.info(f"Downloading from {url}")
+    urllib.request.urlretrieve(url, data_path / file_name, show_progress)
+    if os.path.exists(data_path / "__MACOSX"):
+        shutil.rmtree(data_path / "__MACOSX")
+
+
 def download_and_extract_zip(url: str, data_path: pathlib.Path) -> None:
     if os.path.exists(data_path / ".DS_Store"):
         os.remove(data_path / ".DS_Store")
     if not os.path.exists(data_path) or len(os.listdir(data_path)) == 0:
         logger.info(f"Downloading the dataset from {url}")
         urllib.request.urlretrieve(url, data_path / "temp.zip", show_progress)
         with zipfile.ZipFile(data_path / "temp.zip", "r") as zip_ref:
```

### Comparing `jaxonloader-0.2.7/tests/test_tinyshakespeare.py` & `jaxonloader-0.2.8/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/.gitignore` & `jaxonloader-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/LICENSE` & `jaxonloader-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/README.md` & `jaxonloader-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.7/pyproject.toml` & `jaxonloader-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonloader"
-version = "0.2.7"
+version = "0.2.8"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
```

### Comparing `jaxonloader-0.2.7/PKG-INFO` & `jaxonloader-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.2.7
+Version: 0.2.8
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

