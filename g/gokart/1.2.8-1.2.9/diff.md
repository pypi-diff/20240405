# Comparing `tmp/gokart-1.2.8.tar.gz` & `tmp/gokart-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokart-1.2.8.tar", max compression
+gzip compressed data, was "gokart-1.2.9.tar", max compression
```

## Comparing `gokart-1.2.8.tar` & `gokart-1.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1065 2024-03-25 00:48:25.491246 gokart-1.2.8/LICENSE
--rw-r--r--   0        0        0     3657 2024-03-25 00:48:25.491246 gokart-1.2.8/README.md
--rw-r--r--   0        0        0      635 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/__init__.py
--rw-r--r--   0        0        0     3388 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/build.py
--rw-r--r--   0        0        0     1534 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/config_params.py
--rw-r--r--   0        0        0     4426 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/conflict_prevention_lock/task_lock.py
--rw-r--r--   0        0        0     3962 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/conflict_prevention_lock/task_lock_wrappers.py
--rw-r--r--   0        0        0     8832 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/file_processor.py
--rw-r--r--   0        0        0     1004 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/gcs_config.py
--rw-r--r--   0        0        0     1380 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/gcs_zip_client.py
--rw-r--r--   0        0        0     1555 2024-03-25 00:48:25.491246 gokart-1.2.8/gokart/info.py
--rw-r--r--   0        0        0     2389 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/object_storage.py
--rw-r--r--   0        0        0     1754 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/pandas_type_config.py
--rw-r--r--   0        0        0     3266 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/parameter.py
--rw-r--r--   0        0        0        0 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/py.typed
--rw-r--r--   0        0        0     3899 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/run.py
--rw-r--r--   0        0        0      834 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/s3_config.py
--rw-r--r--   0        0        0     1657 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/s3_zip_client.py
--rw-r--r--   0        0        0      191 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/slack/__init__.py
--rw-r--r--   0        0        0     1693 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/slack/event_aggregator.py
--rw-r--r--   0        0        0     1819 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/slack/slack_api.py
--rw-r--r--   0        0        0      685 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/slack/slack_config.py
--rw-r--r--   0        0        0     8322 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/target.py
--rw-r--r--   0        0        0    24299 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/task.py
--rw-r--r--   0        0        0      471 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/task_complete_check.py
--rw-r--r--   0        0        0      204 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/testing/__init__.py
--rw-r--r--   0        0        0     3045 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/testing/check_if_run_with_empty_data_frame.py
--rw-r--r--   0        0        0     1289 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/testing/pandas_assert.py
--rw-r--r--   0        0        0     3918 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/tree/task_info.py
--rw-r--r--   0        0        0     4792 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/tree/task_info_formatter.py
--rw-r--r--   0        0        0      199 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/utils.py
--rw-r--r--   0        0        0     1177 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/workspace_management.py
--rw-r--r--   0        0        0     1402 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/zip_client.py
--rw-r--r--   0        0        0      432 2024-03-25 00:48:25.495246 gokart-1.2.8/gokart/zip_client_util.py
--rw-r--r--   0        0        0     1972 2024-03-25 00:48:36.971195 gokart-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 gokart-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-05 02:41:37.673605 gokart-1.2.9/LICENSE
+-rw-r--r--   0        0        0     3657 2024-04-05 02:41:37.673605 gokart-1.2.9/README.md
+-rw-r--r--   0        0        0      635 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/__init__.py
+-rw-r--r--   0        0        0     3388 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/build.py
+-rw-r--r--   0        0        0     1534 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/config_params.py
+-rw-r--r--   0        0        0     4426 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/conflict_prevention_lock/task_lock.py
+-rw-r--r--   0        0        0     3962 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/conflict_prevention_lock/task_lock_wrappers.py
+-rw-r--r--   0        0        0     9582 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/file_processor.py
+-rw-r--r--   0        0        0     1004 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/gcs_config.py
+-rw-r--r--   0        0        0     1380 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/gcs_zip_client.py
+-rw-r--r--   0        0        0     1555 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/info.py
+-rw-r--r--   0        0        0     2389 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/object_storage.py
+-rw-r--r--   0        0        0     1754 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/pandas_type_config.py
+-rw-r--r--   0        0        0     3266 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/parameter.py
+-rw-r--r--   0        0        0        0 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/py.typed
+-rw-r--r--   0        0        0     3899 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/run.py
+-rw-r--r--   0        0        0      834 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/s3_config.py
+-rw-r--r--   0        0        0     1657 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/s3_zip_client.py
+-rw-r--r--   0        0        0      191 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/slack/__init__.py
+-rw-r--r--   0        0        0     1693 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/slack/event_aggregator.py
+-rw-r--r--   0        0        0     1819 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/slack/slack_api.py
+-rw-r--r--   0        0        0      685 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/slack/slack_config.py
+-rw-r--r--   0        0        0     8322 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/target.py
+-rw-r--r--   0        0        0    24299 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/task.py
+-rw-r--r--   0        0        0      471 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/task_complete_check.py
+-rw-r--r--   0        0        0      204 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/testing/__init__.py
+-rw-r--r--   0        0        0     3045 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/testing/check_if_run_with_empty_data_frame.py
+-rw-r--r--   0        0        0     1289 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/testing/pandas_assert.py
+-rw-r--r--   0        0        0     3918 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/tree/task_info.py
+-rw-r--r--   0        0        0     4792 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/tree/task_info_formatter.py
+-rw-r--r--   0        0        0      199 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/utils.py
+-rw-r--r--   0        0        0     1177 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/workspace_management.py
+-rw-r--r--   0        0        0     1402 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/zip_client.py
+-rw-r--r--   0        0        0      432 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/zip_client_util.py
+-rw-r--r--   0        0        0     1972 2024-04-05 02:41:49.521626 gokart-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 gokart-1.2.9/PKG-INFO
```

### Comparing `gokart-1.2.8/LICENSE` & `gokart-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/README.md` & `gokart-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/__init__.py` & `gokart-1.2.9/gokart/__init__.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/build.py` & `gokart-1.2.9/gokart/build.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/config_params.py` & `gokart-1.2.9/gokart/config_params.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/conflict_prevention_lock/task_lock.py` & `gokart-1.2.9/gokart/conflict_prevention_lock/task_lock.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/conflict_prevention_lock/task_lock_wrappers.py` & `gokart-1.2.9/gokart/conflict_prevention_lock/task_lock_wrappers.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/file_processor.py` & `gokart-1.2.9/gokart/file_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import pickle
 import xml.etree.ElementTree as ET
 from abc import abstractmethod
+from io import BytesIO
 from logging import getLogger
 
 import luigi
 import luigi.contrib.s3
 import luigi.format
 import numpy as np
 import pandas as pd
@@ -199,37 +200,50 @@
 class ParquetFileProcessor(FileProcessor):
     def __init__(self, engine='pyarrow', compression=None):
         self._engine = engine
         self._compression = compression
         super(ParquetFileProcessor, self).__init__()
 
     def format(self):
-        return None
+        return luigi.format.Nop
 
     def load(self, file):
-        # MEMO: read_parquet only supports a filepath as string (not a file handle)
-        return pd.read_parquet(file.name)
+        # FIXME(mamo3gr): enable streaming (chunked) read with S3.
+        # pandas.read_parquet accepts file-like object
+        # but file (luigi.contrib.s3.ReadableS3File) should have 'tell' method,
+        # which is needed for pandas to read a file in chunks.
+        if ObjectStorage.is_buffered_reader(file):
+            return pd.read_parquet(file.name)
+        else:
+            return pd.read_parquet(BytesIO(file.read()))
 
     def dump(self, obj, file):
         assert isinstance(obj, (pd.DataFrame)), f'requires pd.DataFrame, but {type(obj)} is passed.'
         # MEMO: to_parquet only supports a filepath as string (not a file handle)
         obj.to_parquet(file.name, index=False, compression=self._compression)
 
 
 class FeatherFileProcessor(FileProcessor):
     def __init__(self, store_index_in_feather: bool):
         super(FeatherFileProcessor, self).__init__()
         self._store_index_in_feather = store_index_in_feather
         self.INDEX_COLUMN_PREFIX = '__feather_gokart_index__'
 
     def format(self):
-        return None
+        return luigi.format.Nop
 
     def load(self, file):
-        loaded_df = pd.read_feather(file.name)
+        # FIXME(mamo3gr): enable streaming (chunked) read with S3.
+        # pandas.read_feather accepts file-like object
+        # but file (luigi.contrib.s3.ReadableS3File) should have 'tell' method,
+        # which is needed for pandas to read a file in chunks.
+        if ObjectStorage.is_buffered_reader(file):
+            loaded_df = pd.read_feather(file.name)
+        else:
+            loaded_df = pd.read_feather(BytesIO(file.read()))
 
         if self._store_index_in_feather:
             if any(col.startswith(self.INDEX_COLUMN_PREFIX) for col in loaded_df.columns):
                 index_columns = [col_name for col_name in loaded_df.columns[::-1] if col_name[: len(self.INDEX_COLUMN_PREFIX)] == self.INDEX_COLUMN_PREFIX]
                 index_column = index_columns[0]
                 index_name = index_column[len(self.INDEX_COLUMN_PREFIX) :]
                 if index_name == 'None':
```

### Comparing `gokart-1.2.8/gokart/gcs_config.py` & `gokart-1.2.9/gokart/gcs_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/gcs_zip_client.py` & `gokart-1.2.9/gokart/gcs_zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/info.py` & `gokart-1.2.9/gokart/info.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/object_storage.py` & `gokart-1.2.9/gokart/object_storage.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/pandas_type_config.py` & `gokart-1.2.9/gokart/pandas_type_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/parameter.py` & `gokart-1.2.9/gokart/parameter.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/run.py` & `gokart-1.2.9/gokart/run.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/s3_config.py` & `gokart-1.2.9/gokart/s3_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/s3_zip_client.py` & `gokart-1.2.9/gokart/s3_zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/slack/event_aggregator.py` & `gokart-1.2.9/gokart/slack/event_aggregator.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/slack/slack_api.py` & `gokart-1.2.9/gokart/slack/slack_api.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/slack/slack_config.py` & `gokart-1.2.9/gokart/slack/slack_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/target.py` & `gokart-1.2.9/gokart/target.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/task.py` & `gokart-1.2.9/gokart/task.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/testing/check_if_run_with_empty_data_frame.py` & `gokart-1.2.9/gokart/testing/check_if_run_with_empty_data_frame.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/testing/pandas_assert.py` & `gokart-1.2.9/gokart/testing/pandas_assert.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/tree/task_info.py` & `gokart-1.2.9/gokart/tree/task_info.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/tree/task_info_formatter.py` & `gokart-1.2.9/gokart/tree/task_info_formatter.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/workspace_management.py` & `gokart-1.2.9/gokart/workspace_management.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/gokart/zip_client.py` & `gokart-1.2.9/gokart/zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.8/pyproject.toml` & `gokart-1.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gokart"
-version = "1.2.8"  # using poetry-dynamic-versioning
+version = "1.2.9"  # using poetry-dynamic-versioning
 description="Gokart solves reproducibility, task dependencies, constraints of good code, and ease of use for Machine Learning Pipeline. [Documentation](https://gokart.readthedocs.io/en/latest/)"
 authors = ["M3, inc."]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/m3dev/gokart"
 repository = "https://github.com/m3dev/gokart"
 documentation = "https://gokart.readthedocs.io/en/latest/"
@@ -25,28 +25,28 @@
 tqdm = "*"
 google-auth = "*"
 pyarrow = "*"
 uritemplate = "*"
 google-api-python-client = "*"
 APScheduler = "*"
 redis = "*"
-matplotlib = "*"
 backoff = "^2.2.1"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "*"
 tox = "*"
 moto = "*"
 testfixtures = "*"
 coverage = "*"
 toml = "*"
 lupa = "*"
 fakeredis = "*"
 mypy = "*"
 types-redis = "*"
+matplotlib = "*"
 
 [tool.ruff]
 # All the rules are listed on https://docs.astral.sh/ruff/rules/
 extend-select = [
   "B", # bugbear
   "I" # isort
 ]
```

### Comparing `gokart-1.2.8/PKG-INFO` & `gokart-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokart
-Version: 1.2.8
+Version: 1.2.9
 Summary: Gokart solves reproducibility, task dependencies, constraints of good code, and ease of use for Machine Learning Pipeline. [Documentation](https://gokart.readthedocs.io/en/latest/)
 Home-page: https://github.com/m3dev/gokart
 License: MIT
 Author: M3, inc.
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: APScheduler
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: boto3
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth
 Requires-Dist: luigi
-Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: redis
 Requires-Dist: slack-sdk (>=3,<4)
 Requires-Dist: tqdm
 Requires-Dist: uritemplate
```

