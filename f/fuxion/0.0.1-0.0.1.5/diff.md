# Comparing `tmp/fuxion-0.0.1.tar.gz` & `tmp/fuxion-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuxion-0.0.1.tar", max compression
+gzip compressed data, was "fuxion-0.0.1.5.tar", max compression
```

## Comparing `fuxion-0.0.1.tar` & `fuxion-0.0.1.5.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1063 2024-03-11 13:10:04.932423 fuxion-0.0.1/LICENSE
--rw-r--r--   0        0        0 27123712 2024-04-05 07:57:06.745409 fuxion-0.0.1/fuxion/.langchain.db
--rw-r--r--   0        0        0      253 2024-03-11 13:10:04.936423 fuxion-0.0.1/fuxion/__init__.py
--rw-r--r--   0        0        0     3061 2024-04-05 09:54:33.820724 fuxion-0.0.1/fuxion/base.py
--rw-r--r--   0        0        0    32768 2024-03-17 13:10:34.357183 fuxion-0.0.1/fuxion/examples/.langchain.db
--rw-r--r--   0        0        0    32768 2024-03-17 13:11:29.469407 fuxion-0.0.1/fuxion/examples/name_generator/.langchain.db
--rw-r--r--   0        0        0        0 2024-03-17 13:19:42.327470 fuxion-0.0.1/fuxion/examples/name_generator/README.md
--rw-r--r--   0        0        0      500 2024-03-11 13:10:04.936423 fuxion-0.0.1/fuxion/examples/name_generator/few_shot.json
--rw-r--r--   0        0        0      352 2024-03-11 13:10:04.936423 fuxion-0.0.1/fuxion/examples/name_generator/generator.template
--rw-r--r--   0        0        0      387 2024-04-05 09:32:49.325212 fuxion-0.0.1/fuxion/examples/name_generator/name_generator.py
--rw-r--r--   0        0        0      364 2024-04-05 09:41:21.878178 fuxion-0.0.1/fuxion/examples/name_generator/name_normalizer.py
--rw-r--r--   0        0        0      516 2024-04-04 17:58:20.475726 fuxion-0.0.1/fuxion/examples/name_generator/name_pipeline.py
--rw-r--r--   0        0        0      365 2024-03-11 13:10:04.936423 fuxion-0.0.1/fuxion/examples/name_generator/normalizer.template
--rw-r--r--   0        0        0     1563 2024-04-05 09:54:33.820724 fuxion-0.0.1/fuxion/few_shot.py
--rw-r--r--   0        0        0     1797 2024-04-04 17:58:20.475726 fuxion-0.0.1/fuxion/finetuning/dataset.py
--rw-r--r--   0        0        0     2598 2024-04-04 17:58:20.475726 fuxion-0.0.1/fuxion/finetuning/predict.py
--rw-r--r--   0        0        0     3431 2024-04-04 17:58:20.479726 fuxion-0.0.1/fuxion/finetuning/train.py
--rw-r--r--   0        0        0     3179 2024-04-05 09:54:33.820724 fuxion-0.0.1/fuxion/generators.py
--rw-r--r--   0        0        0     1226 2024-03-12 15:24:18.989467 fuxion-0.0.1/fuxion/irp/generator.template
--rw-r--r--   0        0        0     3187 2024-03-11 14:16:38.619010 fuxion-0.0.1/fuxion/irp/irp.json
--rw-r--r--   0        0        0      460 2024-04-05 07:57:54.265699 fuxion-0.0.1/fuxion/irp/irp_pipeline.py
--rw-r--r--   0        0        0      371 2024-03-11 13:58:41.237539 fuxion-0.0.1/fuxion/irp/normalizer.template
--rw-r--r--   0        0        0     1712 2024-04-05 09:58:46.354880 fuxion-0.0.1/fuxion/models.py
--rw-r--r--   0        0        0     3117 2024-04-05 09:54:33.820724 fuxion-0.0.1/fuxion/normalizers.py
--rw-r--r--   0        0        0     9525 2024-04-05 09:54:33.820724 fuxion-0.0.1/fuxion/pipelines.py
--rw-r--r--   0        0        0       21 2024-04-05 09:54:33.820724 fuxion-0.0.1/fuxion/settings.py
--rw-r--r--   0        0        0      553 2024-04-05 09:54:33.820724 fuxion-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 fuxion-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-11 13:10:04.932423 fuxion-0.0.1.5/LICENSE
+-rw-r--r--   0        0        0       72 2024-04-05 10:03:53.743494 fuxion-0.0.1.5/fuxion/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0 27123712 2024-04-05 07:57:06.745409 fuxion-0.0.1.5/fuxion/.langchain.db
+-rw-r--r--   0        0        0    43968 2024-04-05 10:05:54.412011 fuxion-0.0.1.5/fuxion/Untitled.ipynb
+-rw-r--r--   0        0        0      253 2024-03-11 13:10:04.936423 fuxion-0.0.1.5/fuxion/__init__.py
+-rw-r--r--   0        0        0     3061 2024-04-05 09:54:33.820724 fuxion-0.0.1.5/fuxion/base.py
+-rw-r--r--   0        0        0    32768 2024-03-17 13:10:34.357183 fuxion-0.0.1.5/fuxion/examples/.langchain.db
+-rw-r--r--   0        0        0    32768 2024-03-17 13:11:29.469407 fuxion-0.0.1.5/fuxion/examples/name_generator/.langchain.db
+-rw-r--r--   0        0        0        0 2024-03-17 13:19:42.327470 fuxion-0.0.1.5/fuxion/examples/name_generator/README.md
+-rw-r--r--   0        0        0      500 2024-03-11 13:10:04.936423 fuxion-0.0.1.5/fuxion/examples/name_generator/few_shot.json
+-rw-r--r--   0        0        0      352 2024-03-11 13:10:04.936423 fuxion-0.0.1.5/fuxion/examples/name_generator/generator.template
+-rw-r--r--   0        0        0      387 2024-04-05 09:32:49.325212 fuxion-0.0.1.5/fuxion/examples/name_generator/name_generator.py
+-rw-r--r--   0        0        0      364 2024-04-05 09:41:21.878178 fuxion-0.0.1.5/fuxion/examples/name_generator/name_normalizer.py
+-rw-r--r--   0        0        0      516 2024-04-04 17:58:20.475726 fuxion-0.0.1.5/fuxion/examples/name_generator/name_pipeline.py
+-rw-r--r--   0        0        0      365 2024-03-11 13:10:04.936423 fuxion-0.0.1.5/fuxion/examples/name_generator/normalizer.template
+-rw-r--r--   0        0        0     1563 2024-04-05 09:54:33.820724 fuxion-0.0.1.5/fuxion/few_shot.py
+-rw-r--r--   0        0        0     1797 2024-04-04 17:58:20.475726 fuxion-0.0.1.5/fuxion/finetuning/dataset.py
+-rw-r--r--   0        0        0     2598 2024-04-04 17:58:20.475726 fuxion-0.0.1.5/fuxion/finetuning/predict.py
+-rw-r--r--   0        0        0     3431 2024-04-04 17:58:20.479726 fuxion-0.0.1.5/fuxion/finetuning/train.py
+-rw-r--r--   0        0        0     3179 2024-04-05 09:54:33.820724 fuxion-0.0.1.5/fuxion/generators.py
+-rw-r--r--   0        0        0     1226 2024-03-12 15:24:18.989467 fuxion-0.0.1.5/fuxion/irp/generator.template
+-rw-r--r--   0        0        0     3187 2024-03-11 14:16:38.619010 fuxion-0.0.1.5/fuxion/irp/irp.json
+-rw-r--r--   0        0        0      460 2024-04-05 07:57:54.265699 fuxion-0.0.1.5/fuxion/irp/irp_pipeline.py
+-rw-r--r--   0        0        0      371 2024-03-11 13:58:41.237539 fuxion-0.0.1.5/fuxion/irp/normalizer.template
+-rw-r--r--   0        0        0     1712 2024-04-05 09:58:46.354880 fuxion-0.0.1.5/fuxion/models.py
+-rw-r--r--   0        0        0     3117 2024-04-05 09:54:33.820724 fuxion-0.0.1.5/fuxion/normalizers.py
+-rw-r--r--   0        0        0     9592 2024-04-05 13:42:15.107830 fuxion-0.0.1.5/fuxion/pipelines.py
+-rw-r--r--   0        0        0       21 2024-04-05 09:54:33.820724 fuxion-0.0.1.5/fuxion/settings.py
+-rw-r--r--   0        0        0      555 2024-04-05 14:15:59.139866 fuxion-0.0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 fuxion-0.0.1.5/PKG-INFO
```

### Comparing `fuxion-0.0.1/LICENSE` & `fuxion-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/.langchain.db` & `fuxion-0.0.1.5/fuxion/.langchain.db`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/base.py` & `fuxion-0.0.1.5/fuxion/base.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/examples/.langchain.db` & `fuxion-0.0.1.5/fuxion/examples/.langchain.db`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/examples/name_generator/.langchain.db` & `fuxion-0.0.1.5/fuxion/examples/name_generator/.langchain.db`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/examples/name_generator/name_pipeline.py` & `fuxion-0.0.1.5/fuxion/examples/name_generator/name_pipeline.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/few_shot.py` & `fuxion-0.0.1.5/fuxion/few_shot.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/finetuning/dataset.py` & `fuxion-0.0.1.5/fuxion/finetuning/dataset.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/finetuning/predict.py` & `fuxion-0.0.1.5/fuxion/finetuning/predict.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/finetuning/train.py` & `fuxion-0.0.1.5/fuxion/finetuning/train.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/generators.py` & `fuxion-0.0.1.5/fuxion/generators.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/irp/generator.template` & `fuxion-0.0.1.5/fuxion/irp/generator.template`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/irp/irp.json` & `fuxion-0.0.1.5/fuxion/irp/irp.json`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/models.py` & `fuxion-0.0.1.5/fuxion/models.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/normalizers.py` & `fuxion-0.0.1.5/fuxion/normalizers.py`

 * *Files identical despite different names*

### Comparing `fuxion-0.0.1/fuxion/pipelines.py` & `fuxion-0.0.1.5/fuxion/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
     def save_batch(self, batch: list[dict[str, Any]], batch_index: int):
         """Save a batch of outputs to a file, with each batch saved in a separate file."""
 
         if self.dataset_name is None:
             self.dataset_name = str(int(time.time()))
 
         batch_name = f"{self.dataset_name}_batch_{batch_index}.json"
-        batch_dir = os.path.join(os.path.dirname(__file__), "datasets")
+        # batch_dir = os.path.join(os.path.dirname(__file__), "datasets")
+        batch_dir = "datasets"
         if not os.path.exists(batch_dir):
             os.makedirs(batch_dir, exist_ok=True)
 
         batch_path = os.path.join(batch_dir, batch_name)
         batch_outputs: dict[str, dict[str, list[dict[str, Any | str]] | str]] = {
             "dataset": {
                 "outputs": batch,
@@ -100,16 +101,16 @@
     ) -> None:
         """Save the complete dataset to a file."""
         if self.dataset_name is None:
             self.dataset_name = f"{str(int(time.time()))}.json"
         else:
             self.dataset_name = f"{self.dataset_name}.json"
 
-        dataset_dir = os.path.join(os.path.dirname(__file__), "datasets")
-
+        # dataset_dir = os.path.join(os.path.dirname(__file__), "datasets")
+        dataset_dir = "datasets"
         if not os.path.exists(dataset_dir):
             os.makedirs(dataset_dir, exist_ok=True)
 
         dataset_path = os.path.join(dataset_dir, self.dataset_name)
 
         with open(dataset_path, "w") as fd:
             json.dump(results, fd)
```

### Comparing `fuxion-0.0.1/pyproject.toml` & `fuxion-0.0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name ="fuxion"
-version = "0.0.1"
+version = "0.0.1.5"
 description = "Synthetic dataset generation and normalization functions powered by LLMs"
 authors = ["Oluwatobi Adefami <tobiadefami@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 openai = "^1.0.0"
```

### Comparing `fuxion-0.0.1/PKG-INFO` & `fuxion-0.0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxion
-Version: 0.0.1
+Version: 0.0.1.5
 Summary: Synthetic dataset generation and normalization functions powered by LLMs
 License: MIT
 Author: Oluwatobi Adefami
 Author-email: tobiadefami@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

