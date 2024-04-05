# Comparing `tmp/transformer_smaller_training_vocab-0.3.2.tar.gz` & `tmp/transformer_smaller_training_vocab-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_smaller_training_vocab-0.3.2.tar", max compression
+gzip compressed data, was "transformer_smaller_training_vocab-0.3.3.tar", max compression
```

## Comparing `transformer_smaller_training_vocab-0.3.2.tar` & `transformer_smaller_training_vocab-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-09-18 13:46:32.615023 transformer_smaller_training_vocab-0.3.2/LICENSE
--rw-r--r--   0        0        0     7019 2023-09-18 13:46:32.615023 transformer_smaller_training_vocab-0.3.2/README.md
--rw-r--r--   0        0        0     2876 2023-09-18 13:47:23.951622 transformer_smaller_training_vocab-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      337 2023-09-18 13:46:32.615023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/__init__.py
--rw-r--r--   0        0        0     7713 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/contextual_reduce.py
--rw-r--r--   0        0        0      154 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/logging_utils.py
--rw-r--r--   0        0        0     2444 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/modify_model.py
--rw-r--r--   0        0        0      719 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/modify_tokenizer.py
--rw-r--r--   0        0        0        0 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/py.typed
--rw-r--r--   0        0        0      756 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/token_stats.py
--rw-r--r--   0        0        0      716 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/__init__.py
--rw-r--r--   0        0        0     1520 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/auto_set_vocab.py
--rw-r--r--   0        0        0      566 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_bert.py
--rw-r--r--   0        0        0     3444 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_fast_tokenizer.py
--rw-r--r--   0        0        0      472 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_roberta.py
--rw-r--r--   0        0        0      539 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_xlm_roberta.py
--rw-r--r--   0        0        0     1414 2023-09-18 13:46:32.619023 transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/utils.py
--rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 transformer_smaller_training_vocab-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-12-04 17:40:11.300613 transformer_smaller_training_vocab-0.3.3/LICENSE
+-rw-r--r--   0        0        0     7019 2023-12-04 17:40:11.300613 transformer_smaller_training_vocab-0.3.3/README.md
+-rw-r--r--   0        0        0     2876 2023-12-04 17:40:51.036089 transformer_smaller_training_vocab-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      337 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/__init__.py
+-rw-r--r--   0        0        0     7713 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/contextual_reduce.py
+-rw-r--r--   0        0        0      154 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/logging_utils.py
+-rw-r--r--   0        0        0     2499 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/modify_model.py
+-rw-r--r--   0        0        0      719 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/modify_tokenizer.py
+-rw-r--r--   0        0        0        0 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/py.typed
+-rw-r--r--   0        0        0      756 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/token_stats.py
+-rw-r--r--   0        0        0      716 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/__init__.py
+-rw-r--r--   0        0        0     1520 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/auto_set_vocab.py
+-rw-r--r--   0        0        0      566 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_bert.py
+-rw-r--r--   0        0        0     3444 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_fast_tokenizer.py
+-rw-r--r--   0        0        0      472 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_roberta.py
+-rw-r--r--   0        0        0      539 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_xlm_roberta.py
+-rw-r--r--   0        0        0     1414 2023-12-04 17:40:11.304613 transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/utils.py
+-rw-r--r--   0        0        0     7997 1970-01-01 00:00:00.000000 transformer_smaller_training_vocab-0.3.3/PKG-INFO
```

### Comparing `transformer_smaller_training_vocab-0.3.2/LICENSE` & `transformer_smaller_training_vocab-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/README.md` & `transformer_smaller_training_vocab-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/pyproject.toml` & `transformer_smaller_training_vocab-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformer-smaller-training-vocab"
-version = "0.3.2"
+version = "0.3.3"
 description = "Temporary remove unused tokens during training to save ram and speed."
 authors = ["Benedikt Fuchs <benedikt.fuchs.staw@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "transformer_smaller_training_vocab" }]
 repository = "https://github.com/helpmefindaname/transformer-smaller-training-vocab"
```

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/contextual_reduce.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/contextual_reduce.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/modify_model.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/modify_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,9 +50,10 @@
     embedding_weights: torch.Tensor = model.get_input_embeddings().cpu().weight.detach()
     model.get_input_embeddings().__delattr__("weight")
     if empty_cuda_cache:
         torch.cuda.empty_cache()  # pragma: no cover  # no need to test this line
     for reduced_id, full_id in enumerate(keep_token_ids):
         saved_embeddings[full_id] = embedding_weights[reduced_id]
     new_input_embedding = nn.Embedding(saved_embeddings.size(0), saved_embeddings.size(1), _weight=saved_embeddings)
+    model.config.vocab_size = saved_embeddings.size(0)
     model.set_input_embeddings(new_input_embedding)
     model.get_input_embeddings().to(model_device)
```

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/modify_tokenizer.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/modify_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/token_stats.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/token_stats.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/__init__.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/__init__.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/auto_set_vocab.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/auto_set_vocab.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_bert.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_bert.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_fast_tokenizer.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_fast_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_xlm_roberta.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/transformer_smaller_training_vocab/utils.py` & `transformer_smaller_training_vocab-0.3.3/transformer_smaller_training_vocab/utils.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.3.2/PKG-INFO` & `transformer_smaller_training_vocab-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: transformer-smaller-training-vocab
-Version: 0.3.2
+Version: 0.3.3
 Summary: Temporary remove unused tokens during training to save ram and speed.
 Home-page: https://github.com/helpmefindaname/transformer-smaller-training-vocab
 License: MIT
 Author: Benedikt Fuchs
 Author-email: benedikt.fuchs.staw@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: sentencepiece (>=0.1.97,<0.2.0)
 Requires-Dist: torch (>=1.8.0,<3.0.0,!=2.0.1)
 Requires-Dist: transformers[torch] (>=4.1,<5.0)
 Project-URL: Repository, https://github.com/helpmefindaname/transformer-smaller-training-vocab
 Description-Content-Type: text/markdown
 
 # transformer-smaller-training-vocab
```

